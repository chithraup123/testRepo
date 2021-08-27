# Resupply PO
Screen to show the list of products with the quantity to be purchased from the manufacturer to avoid the shortage/overage of stock. The screen has two tabs, 'Total' and 'Region' where Total is to view the products based on Manufacturer and Region tab allows the user to view the products based on the market region and the manufacturer.
The screen has the following fields in addition to the model, product, and title
1. Total Avg/Day 
   The average number of products that are sold each day.
   ```sh   
    We need to find avg sales over 7 days of the last 7 consecutive days where inventory > 0. If not found, it is zero. If the product doesn't have any sales history(If the product is new) then it will be 'N/A'
    ```
2. Inv Left
   Inventory Left in the fulfillment center. The value is available on Administration-->Fulfillment center-->Market Region
3. Days To Expire Curr Inv
   To find the no of days taken to expire the current inventory available in the fulfillment center. 
   ```sh
   Inv Left / (Total Avg/Day)
   ```
4. Days To Next Delivery
   To find the no of days taken to reach the OTW quantity in the fulfillment center. The value will be getting as follows
    ```sh
   a) Go to the Purchase Orders page and select the appropriate manufacturer and open the details by clicking on the down arrow button
   b) Check Order Quantity and Quantity Shipped are equal, If it is equal then no need of taking PO and go  to Import shipment page and apply below equation, 
   IS.ETA + IS.Warehouse\3PL.AverageProcessingTime
   c) If it is not equal, apply below equation
      PO.ETA + MarketRegion.OceanDeliveryTime + IS.Warehouse/3PL.AverageProcessingTime. 
      If there is no Warehouse\3PL is assigned for an IS, apply below Eqn,
      PO.ETA + MarketRegion.OceanDeliveryTime + MarketRegion.AveragePrepCenterProcessingTime
      ```
5. Days Out Of Stock
    To find within how many days the product will take to get out of stock
    ```sh
    (Days To Next Deliver) - (Days To Expire)
    ```
6. OTW(On the way count)
    The total quantity of the product on the way to the fulfillment center.
    PO.Unshipped qty+IS.Unallocated qty+SIG.Current qty+FC.totally where FC is not delivered
    ```sh
    Total Qty from PO - Total Qty from FC
    ```
7. Days To Exp Incl Next Ship 
    To find the no of days taken to expire the current qty and the on the way (OTW) qty of the product
    ```sh
    (OTW/(Total Avg/Day)) + Days To Next Deliver
    ```
8. Order Now
    To find the quantity of product to be purchased from manufacturer as per the current sale of the prouduct
    ```sh
    Check DeliverTime and LeadTime(Since LeadTime is manufacturer specific, find it from Administration-->Manufacturer)
    TotTime = DeliverTime + LeadTime
    If (TotTime *2) < Days To Exp Incl Next Ship,
    OrderNow = 0
    Else If (TotTime)< Days To Exp Incl Next Ship then,
    OrderNow = (TotTime - (Days To Exp Incl Next Ship - TotTime)) *(avg sale) 
    Else, 
    OrderNow = TotTime * Avg sale
    Need to round the value based on Packs/Carton as follows
    OrderNow + (PacksPerCarton - (OrderNow MOD PacksPerCarton))
    ```
9. Units per Each
    The no of units available in a pack when the product is purchased from the manufacturer
    ```sh
    Units/ Pack from Product-->Basic-->Manufacturer Specific Fields
    ```
10. No Of Units
    Total no of products to be purchased from the manufacturer
    ```sh
    Order Now *  Units per Each
    ```
11. Eaches p Carton
    No of units in a single carton when the product is shipped by the manufacturer
    ```sh
    Master Carton Qty from Product-->Basic-->Master Carton
    ```
12. Cartons US
    To find the no of cartons required to ship the total qty of product
    ```sh
     (No Of Units) / (Eaches P Carton)  
    ```
13. CBM/Carton
    To find the cubic meters while shipping the product by Manufacturer thus it is easy to calculate how many products will fit in a carton
    ```sh
    Master Carton Height(meters) * Master Carton Length(meters) * Master Carton Width(meters)
    ```
14. Total CBM
    CBM of total no of Product
    (Cartons US)*(CBM/Carton)
15. Weight/Carton (kg)
    To find the weight of the product in one carton
    ```sh
    Weight from Product-->Basic-->Master Carton
    ```
16. Total Weight
    Total weight of a product at the shipping time
    ```sh
    (Cartons US)*(Weight/Carton (kg))
    ```
17. Days To Reorder
    Within how many days the product has to be reordered
    ```sh
    (Days To Exp Incl Next Ship) - (DeliverTime +LeadTime)
    ```
18. Mfctr Cost Per Pack
    The unit price of the manufacturer for a product
    ```sh
    Manufacturer Price from Product--->Profit and Loss
    ```
19. Tot Cost
    The total manufacturer cost of the ordered product
    ```sh
    Mfctr Cost Per Pack * Order Now
    ```
- Deliver Time
    Time taken by the manufacturer to deliver the product
- Lead Time
    The total time taken to manufacture the product and then deliver it to the seller
- Order Qty Rounded by Carton Size
    Order now quantity can be rounded as per the Carton size by selecting the check box provided at the top of the grid as given in the below image.
    [Product](./content/product.md)
    When checking the option to view the rounded value, the new value will be equal to Cartons US * Eaches P Carton
- Show only SKUs needing re-order
    To view only the products which have to be purchased again ie products with 'Order Now' >0
- Download
    The grid data can be exported in an excel file if the products are selected in the model column
- Create PO
    A new purchase order can be created directly from the resupply PO screen by selecting the list of products to be purchased. This button navigates the user to the PO screen with the selected product and order now value to create the new order
![My image](product.md " ")
