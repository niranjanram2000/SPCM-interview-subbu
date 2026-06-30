Back to back sales order

"Back to back sales orders when 
we have a stock we basically ship from our warehouse but when we"
"don’t have a stock we process that sales order into 
purchase order & we will receive the stock from the supplier"
we ship that stock from our warehouse to customer. its called a back to back sales order

configurations

"For Configuration of back to back sourcing rule is required. 
We have to create a buy from sourcing rule"
"in the sourcing assignment,
 you need to define that  if this is the item and org, pick up this sourcing rule"

"in manage administration  porfile values,  
you need to select the msp default assignment set as your assignment set"
in sales order line level we have to select warehouse as a supply.
at the item level, back to back attribute has to be enabled.
and purchase price/ list price of the item should be defined.
in order management parameters, you need to define the preparer for procurment person
for automatic requsition creation

then when you create an sales order , it is going to pickup the back to back orchestration 
and  create a back to back supply order number
with automatic creation of requisition, if you have approved supplier and agreement 
for that item the it will automatically create purchase order

or else you have manually process the requistion into purchase order
and receive the materials against the purchase order into our inventory
then you have to create a pickwave and do the pick confirm 
then you do the ship confirm  against the ship method by providing  shipping qty

b2b header status - Draft -> Processing -> Close
b2b line status - Schedule -> Create Purchase Requisition -> PO ->  Receipt -> Pick -> Ship -> Invoice

back 2 back requirements
Sourcing Rule is Required, Buy - Buy from (Global/Local), Make - Make at (Local Sourcing Rule)
In the sales order screen select the warehouse

Sourcing Assignment Set condition should be Item & Organization
Item should be back 2 back enabled 
Requisition Preparer Preferences should be set to the sales order BU
Requisition business function options - Line type should be Goods
List Price/purchase price required

"for the same item if you dont provide warehouse in the sales order screen
 it identifies as a drophship becuase of the Buy from sourcing rule"
"Item can be back 2 back enabled but it could be used for dropship based on the supplier
 selection in the sales order screen or Buy from sourcing rule"
User Requisition preference should be set to Inventory

in the order management tab
in the item level we need to enable the back to back tick must be enabled
then we need to define sourcing rules
GOP only we are doing the sourcing rule
collection needed for all the cases
like standard SO, Dropship, back to back 
collection is need to be run
I am explain implementation point of view
yes

item must be back to back enabled
there is sourcing rule where we need to select the buy from option
so then it will give us the procureent process
let me exp;alin all setups
<img width="924" height="1676" alt="image" src="https://github.com/user-attachments/assets/bde37954-6e13-489b-b8cd-5ac16fb878f8" />
