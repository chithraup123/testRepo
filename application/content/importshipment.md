# Import Shipments

The page deals with the shipment of the inventory from the manufacturer. It covers all the intermediate stage details.

   Below image shows the table representation

  ![](https://i.ibb.co/qBtybhN/importhme.png)

- The  top region of the window comprises of drop down text field  for sku to hold the sku value and this drop down is repurposed with the sku values which have been entered in product window.

- Model text field takes the model number of the product from the drop down list which is repurposed with the product values which have been entered in product window.

- Invoice Number text field give the provision to enter the invoice number which represents the invoice created for recording the Import Shipment(IS) related expenses and Container Id text field will take the container Id of the product which is created in the import shipment window during the creation of a new Import Shipment(IS).

- These four text fields are filters which are used to filter out the contents of the table.To the extreme top right end one check box is placed to filter the completed ISs.

  The above said filter text fields and check box displayed below

  ![](https://i.ibb.co/CzrbJZ6/import-shipmentfilterfleds.png)



- Below to this text fields the import shipment table is displayed which  is listed with various import shipments related details. Table comprises the following fields.

- A general  Id and SIG Id indicates the starting attributes of the table uniquely identifies the storage inventory group of the warehouse to which the imported products stored.

- Forwarders field holds the name of the agency or company that organizes shipments for customers to get goods from the manufacturer to a market.

- Clearing agent field is a country dependent value which is introduced by the authorities relevant for the shipment of the goods.

- Warehouse/Third Party Logistics(3PL) column will keep the  name of warehouse or the name of third-party agency to which the goods are stored in storage inventory group window.

- Supplier/Manufacturer Name is the manufacturer of PO listed in the IS details page. If multiple manufactures comes in one IS then take the manufacturer of first PO

- HBL field holds the house bill of lading identifier and this field will helps to filter out the acknowledgment issued to the manufacturer once the cargo has been received at the customer side.

- Estimated Time of Arrival field will keep the estimated date of arrival of the goods to the customer.

- Released and the paid status column will displays the status of the shipment and payment status respectively. If Released flag is set, Paid status will be set automatically. Still the paid status can be edited manually.

- To the extreme right end of the table the last field represents various actions like view,edit,delete to be performed on the table values.

- Click on Edit button will redirect to the Import Shipment Details page that covers all the minute level details regarding the Import shipment of goods.

 The above said fields are pictorially shown here

![](https://i.ibb.co/sQVXxRj/IS-headers.jpg)

- The click on the plus button which have placed on the top right corner redirect to the Add new Import shipments window.

# Add New Import Shipments

- In the top region four drop down text fields are arranged.The Market region mandatory field will select the market region from which the products are imported.

- Warehouse drop down selects the name of warehouse in which the imported products are stored.

- Clearing agent and the Forwarders drop down selects intermediate agencies who take care the shipment procedures.

- Below to this top region one drop down list is given to select the document type of the file which is chosen from the browse button placed nearby the document type drop down.

- If more than one document to be uploaded then this segment can be replicated by making use of a plus button on the boundary of the region.

- The bottom region of the window includes a House Bill Lading(HBL) text field that takes a value that represents the  acknowledgment of the receipt of product that are to be shipped.

- Estimated time of Arrival field select a date on which the arrival of the product is expected.

- Total CBM no editable text field receives the total volume of the products which is to be shipped.
Total CBM calculation is,
SKU1's CBM = MasterCartonLength(meter) * MasterCartonHeight(meter) * MasterCartonWidth(meter)
SKU1's Total Carton CBM = SKU1's CBM * No of Cartons
Total CBM  = Sum of all SKUs Total Carton CBM

![](https://i.ibb.co/VMzf17X/IS-add-one.jpg)

- Add Invoice button generate an invoice details entering region.

- Invoice type can be selected from the drop down . Invoice number field keep the invoice number. The amount field collects the amount specified in the invoice for the shipment.

- Currency field is a country dependent drop down that selects the currency type.

- Invoice number, currency and amount fields are mandatory fields.

- Invoice date field keep the date on which the invoice is created.Due date field keep the deadline date on which the payment mentioned in the invoice to be done.

- In Payment date field the actual date on which the payment was done is given.

- If more than one invoice type details to be given then this invoice region can be replicated by clicking on the plus button on the boundary of the region.

![](https://i.ibb.co/g9W4Jdv/invoice.jpg)

- Import shipment details window gives the shipment details in appropriate text fields.

In the top right corner one label called ID is placed which indicates the identifier of a particular import shipment(IS).

#Create WH Import file 

- Helps to generate a warehouse import file as per the template that has been mentioned in the 'Import Template' icon of Warehouse/3PL page under Administration menu.

- The fields of the templates are flexible and it can be added as per the requirement.For a particular warehouse if template is not defined an error message will be raised while clicking on the create WH Import file button saying, Preparation Center Template is not available.

- 
























