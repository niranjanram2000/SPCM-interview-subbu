Dropship sales order

"Drop Shipment is a process where the Sales Orders are fulfilled using third party suppliers
 who ship the products/items directly to the customer, 
without physically receiving the material into the organization."
"Order Management sends a purchase request to Oracle Procurement, 
which places a purchase order with third party supplier, then 
the supplier ships directly to your customer.
 The process helps to reduce total inventory management and reduce overall fulfillment cost."


"In this we don’t have inventory. Drop shipments occur when 
your customer orders product from you, "
you order the product from your supplier
"and your supplier ships the product directly to your customer. 
It means you can receive orders for items"
"that you do not stock or for which you lack sufficient inventory, and
 have a supplier who provide the items"
"directly to your customer. We process to suppliers as purchase order,
sales order is converted as purchase order."

The sales organization wont deilever the product directly to the customer, 
sales organization uses third party supplier to directly deleiver the product to customer.

dropship status 
header status - Header : Draft -> Processing -> Close
"Line : Scheduled -> Requisition Created -> PO Created -> Awaiting Shipping -> 
Shipped(upon ASN or AP Invoice Match) -> Awaiting Billing -> Closed"

dropship configurations

Enable Profit center Business Unit under Business Functions
Add the Profit Center BU to the Inv Org
then do the dropship setups
Manage Supply Chain Financial Orchestration System Options
here we Linking our master organization with the supply chain order orchestration.

then you create drop ship qualifers
here you add the items or item categories  which qualifies for dropshipment

then you create drop ship financial flows
here we select the Supplier ownership change event
"If we select ASN from supplier option then 
advance shipment notice like delivering the product to the customer on so & so date"
AP Invoice Match means when our supplier is sending the product to the customer we need to pay to our supplier

"when the AP invoice is got created & matched with the purchase order then 
the financial events going to start creating like accounting"
you add your dropship qualifer here
then you define What is the selling BU to receiving BU relationships
 in order management parameters , you need to define the preparer for procurement name
Purchase requisition will be created under this person name

when you create a sales order by entering the item details and supplier information
 and submit it then system is going to pull the dropship orchestration and 
create a purchase  requisition under the preparer for procuerement name 

then you process the requistion into purchase order 
then we get asn from supplier, after that item is shipped from supplier to customer location



we have the dropship returns
usually we make the return by selecting the supplier location
otherwise we usually receive into our warehouse
and then we can do the RTV process
we will receive in the system by raising the RMA then we will make a credit memo to customer
we will do the RTV with suppliers and then we will raise debit or credit memo to suppliers


