# Purchase Order

- Purchase Order page showcases the detailed information of orders placed for various products. - It is represented in a tabular form.

   Below image shows the table representation

 ![](https://i.ibb.co/9ZzKQVm/purchase-home.jpg)

- In the top right of the page two search filters for Sku and the Model are given which will filter the table content.A hide completed check box is available on the  top right of the window and this will filter out the completed POs from the list.

    Below Image shows the above said fields

![](https://i.ibb.co/LrQCjzN/sku.jpg)

- Table fields includes a general Id along with the purchase order ID.For each purchase order the page will maintain a specific Id.

- Manufacturer field will keep the name of manufacturer.The purchase order created dates are listed in the table.The estimated product shipment completion dates are placed next to the date created field.The total cost for the purchase is given in the Total cost column.In the purchase if any initial payment is  done then that cost is given in the down payment sent field.

- To the extreme right end of the table an action column is given with edit,view and delete button for each purchase order entry.

- Below Image shows the above said fields



 ![](https://i.ibb.co/F3rCcY9/header.jpg)

- The Export button on top middle of the window will exports a file that comprises the details of already created purchase orders.

   Below Image shows the above said field

   ![](https://i.ibb.co/wBLHzBx/export.jpg)

-  The Plus button on the right corner will give the provision to create a new purchase order by entering relevant field values in the redirected page-Add new Purchase Order.

   Below Image shows the above said field

  ![](https://i.ibb.co/JKJ86m9/plus.jpg)

## Add new Purchase Order

- Add new Purchase Order window is segregated to mainly three regions where the top region collects the manufacturer and the purchase order id details.The middle region holds the cost details and the bottom region will accept the SKU related information.

   Below Image represents the Add new Purchase Order Window.

  ![](https://i.ibb.co/r0N1Q0H/addnewpurchase.jpg)

##### Top Region of the window Add new Purchase Order

- This region includes a text field which receives the purchase order id and this field value is unique for each purchase order.The next field is a manufacturer name selected from a drop down list.

- The purchase order created date is recorded in the date created field of the page.The estimated completion date for the shipment of the product is mentioned as the last text field of this region.All the fields in this region are mandatory.

  Below Image displays the top region of Add new Purchase Order Window

  ![](https://i.ibb.co/SRCs0Y3/topregionofpurchaseadd.jpg)

##### Middle Region of the window Add new Purchase Order

- It is having a pro forma invoice button that allows to choose or browse the bill of a respective transaction.

- Next comes the total cost resetable text field where the total cost of the purchase order is given and also this value is able to reset.

- The down payment sent and the down payment date fields gives the provision to enter the advance amount paid for the Purchase Order with the corresponding date.The balance payment due text field takes the balance amount to be paid for the purchase of the product.

- The due date field will take the deadline date for giving the balance due amount.The balance payment date field will receives the actual date on which the balance payment was done.

    Below Image shows the middle region of Add new Purchase Order Window with above said fields.

   ![](https://i.ibb.co/jLtW2s4/middleofadd.jpg)

- In the same window besides the middle region two highlighting buttons are given , one for downloading the newly created purchase order and the other button is used to upload  already created sku file to this page.

##### Bottom Region of the window Add new Purchase Order

- This section collects the Stock Keeping Unit(SKU) details.In the region the model text field will specify the model of the SKU from a drop down and the drop down is populated with various product models which is mentioned in the product page.

- The SKU mandatory field takes the sku value from the drop down which is populated with the values in the product page.The price per each field will records the price of the product for each unit and this is a text field which is able to reset its value.Order quantity text field receives the quantity of the product to be ordered in eaches or units rate.

- In this zone along with SKU Details header two buttons Download Template and Upload SKU file are placed.

- Download template button is used to download the excel template of the purchase order being created.Upload SKU file button allows to browse or choose the pre existed sku file to the Add new purchase order window.

- In the bottom border and the top border of this region one plus button and minus button  is placed in order to create new panel for entering SKU details further and removing already created sku details respectively.

   Below Image shows the bottom region of Add new Purchase Order Window with above said fields.

  ![](https://i.ibb.co/Y3Qv3Yr/bottomskudetailsfinal.jpg)

- In the bottom right corner of the page Add new Purchase Order two buttons are placed for saving the purchase order details and for resetting the entered details of the purchase order.

  Below Image shows the above said fields.

  ![](https://i.ibb.co/6srFtyc/savebutton.jpg)



## Purchase Order Details

- While clicking the view or edit  button on the purchase order page we can move on to the purchase order Details page.

- This window displays the details of the already created purchase order with relevant field values.The purchase order id is displayed on the top  right of the page.

   Below Image shows the above said fields.

  ![](https://i.ibb.co/pjLDJ8y/purcahseorderetails.jpg)

##### Top Region of the window Purchase Order Details

- In the top region the purchase order id field displays the purchase order id of the corresponding purchase order.

- The manufacturer field shows the manufacturer name which was selected at the time of order creation.

- In this region the manufacturer field is displayed as drop down from which we can change the name of manufacturer.

- The purchase order created date and the estimated completion date of the purchase which was inserted at the time of order creation is displayed in the corresponding fields on this region.

  Below Image shows the above said fields.

 ![](https://i.ibb.co/ncMtFtn/podetailstop.jpg)

##### Middle Region of the window Purchase Order Details

- In the middle region of the page the cost details are automatically displayed in the text fields as per the costs entered at the time of order creation.

- It is having a pro forma invoice button that allows to choose or browse the bill of a respective transaction.Total cost field displays the sum of SKU level cost, that is the sum of (per each cost of SKU * SKU level quantity) and this text field value is able to recalculate by the above said formula.

- The down payment sent and the down payment date fields displays the advance amount paid for the Purchase Order with the corresponding date.

- The balance payment due text field shows the balance amount to be paid for the purchase of the product.The due date field displays the deadline date for remitting the balance due amount.

- The balance payment date field will showcase the actual date on which the balance payment was done.

  Below Image shows the above said fields.

![](https://i.ibb.co/Dg9h0HB/middlepodetals.png)

##### Bottom Region of the window Purchase Order Details

- In this segment the sku details of the products which are purchased by a particular purchase order id.

- Sku details comprises of Model displaying text field and a product name displaying text field which is non resettable.

- Next to the product text field the price per each text field displays the current price of each unit according to the values entered at the time of order creation.Previous price is the price of the same SKU from the previous Purchase Order and it is getting displayed in the previous price field.

- By comparing the price per each unit and the previous price text field values a status icon is displayed on the previous price text field.

- The icon will be blue thumbs up if the price per each unit is less than the previous price.

- The icon will be green tick if the price per each unit is equal to  the previous price.The icon will be red cross symbol if the price per each unit is greater than the previous price.

 Images represents various icons shown on previous price text field

![](https://i.ibb.co/Y0G2j7D/pricecomparisonimage1.jpg)

![](https://i.ibb.co/YbT51tD/comparisontwo.jpg)

- Order quantity field will show the quantity of the SKU eaches ordered for a particular PO.Eaches shipped is a read only text field displays the eaches shipped to import shipment(IS) from manufacturer or eaches shipped to fulfillment channel shipment(FC) or eaches shipped to storage Inventory group(SIG).

- According to the shipment category like IS,FC,SIG of eaches shipped the corresponding details can be viewed in the region by clicking on view details.

- The more details will list a table which shows the source ie whether it is IS,FC or SIG shipment along with total cartons and total quantity fields which will say the total number of cartons required to ship total quantity value, and the number of cartons required field value depends on the eaches per carton value which is created in IS,FC or SIG.So in the detail table the different category of  shipment will be mentioned along with the total quantity and number of cartons.

- Next field in this region is per each WH receiving cost that shows the 3 PL(Third Party Logistics) invoices associated with the SKU entry.

- Last text field of this region is eaches remaining in FCs and this field will displays the eaches  remaining in the FC which is not being pulled to sales channel.

- In the bottom corner of the sku detail region one label named COMPLETED is placed diagonally which indicates that the shipment of that sku is completed for the entire quantity which is mentioned in the purchase order.

- The per each cost and Real P&L checkboxes of this region will be elaborated in the next bullet.

   Below Image shows the above said fields.  ![](https://i.ibb.co/FWxMj75/skudetailsonewith-table.jpg)

- The per each cost check box in the SKU details region displays a pop up form while selecting the checkbox.This Pop up displays different cost text fields like import and logistics cost,FC ship cost,WH storage cost.

- Import and logistics cost is the sum of per each import ship cost from IS.FC ship cost is the sum of Per Each Shipping Cost from FC.WH storage cost is the sum of  per each storage costs from SIG.

- Suppose in a purchase order a product is ordered for a quantity 150 and among those 100 was shipped through IS ,so while creating an IS, the per each cost for that sku is given.

- Similarly among 150 skus 50 products were  shipped through FC so while creating an FC the per each cost for that sku in FC is assigned, so the total per each cost for the sku in a particular purchase order is the summation of the per each cost in IS and the per each cost in FC shipment. 

   Below Image shows the above said fields. 

  ![](https://i.ibb.co/M2yvcjm/pereachcost.jpg)

- Real P&L checkbox opens a pop up with set of fields. The values of the corresponding fields are fetched from the profit and loss page .Revenue field keeps the amount of gross income produced through sales of the product in a particular purchase order.

- Amz Storage Cost is the cost incurred for the amazon storage if the product of a particular PO is selled through amazon fulfillment FBA.

- The WH Storage cost of a product is the cost created for the storage in SIG.Advertising Cost shows the cost given for the advertisement of the product in the respective purchase order for selling that product among customers.

- Return Fees field keeps the value of return on investment which is calculated on the basis of revenue of the product.Revenue can be calculated as product_price-(fulfillment cost+storage cost+advertisement cost).

- Reimbursements field displays the reimbursement cost of a product if  the product is getting damaged at any stage of the delivery.

- Net Amount is calculated as revenue(manufacturing cost+shipping cost+tariff cost). All the above said field values are automatically displayed on this page from the profit and loss window.

 Below Image shows the above said fields. 

![](https://i.ibb.co/fD63cX5/realp-l.jpg)

- In a particular purchase order if discontinued products exists then that information will be highlighted at the right top of the window.

- In the purchase order details page one button named Create FC Shipment is placed near to the SKU Details label.

- This button will create a pop up on the button click on which we can select the fulfillment service and the respective fulfillment service address for creating a new FC shipment for the product.

- While creating an FC shipment through the pop up two buttons are available , one button is to create FC for those SKUs which have been uploaded as file through the button.

- The next button is All open SKU and this will permits to create FC with the incompleted SKUs from the respective PO. The button click on the above said two buttons will results in the creation of new FC by redirecting the control to FC window.

![](https://i.ibb.co/JkQh6Zd/FCpopup.jpg)

-  Upload SKU button in the page  allows to upload the pre-existing SKU file to the window.The Download Template button in the window allows to download the file of generated purchase order in an appropriate template.

- Create Storage Inventory Group button in the window will give the provision to create SIG from the purchase order details page. 

- Generate PO button on the page will allows to generate an excel file that includes all the purchase orders created for all skus of  a particular manufacturer.

 Below Image shows the above said fields.

![](https://i.ibb.co/1ncxm52/createFC.jpg)

- Save and Reset button is given at the bottom of the page for saving the content on the page and resetting the text field values with an initial value.

  Below Image shows the above said fields.

  ![](https://i.ibb.co/7rB4v3g/finalrestandsave.png)

     

     

