Order to Cash (O2C)

Order to cash cycle starts with receiving orders from the customers
"so when we receive the order,  the customer service desk team  
will input the details about the customers and all"

"so when we input the customers , there is a pre transformation and 
post transformation rules to default the information on the sales order"
"when we go the line level and put the item, when we search for it. 
pricing engine in the background  will give you the selling price for the item"
which depends on the  pricing segment  and pricing strategy we have configured
and based on the GOP, scheduling and atp etc the stock availability will be coming into the line level

then we add the lines to the sales order, when we save it. It will be in draft mode
if all the information is ok, we  will initiate the submit process 
"then the orchestration process starts involving. 
so if there are no validation errors like credit check holds or any extensions etc"
if there are no validation errors, then the order will go for the next step 
if there are validation errors,we need to correct them and revaildate and we need to submit again
"then the movement we submit the header will be in processing status, 
line will start with scheduling status"


then we need to go to actions and switch to fulfillment view, there we can see the sub sequent status. 
"where it will give the orchestration number nothing but sort of work flow. 
it will have a sequence of steps"

for standard sales order, it will show like scheduled, reserved and then it will go for awaiting shipping
so it will take some time to complete that based on the sourcing rules, availability check etc
"material  will be allocated to the sales order lines. first it will go scheduled, then 
it will go to reserved  and then it will go to awaiting shipping"
so when it goes to awaiting shipping, we can initaite the release process
"release can be done in multiple ways, we can run the generate shipment advice program or 
we can go and run the pickwave release rule"
"or we can go to manage shipment forms, where we can do the release all  or 
add to shipment etc process we can do"
that means we can do the multiple ways of release

"so when we do the pick wave release,  material is moved from 
 source sub inventory to stage sub inventory"
 when we do the pick confirm,pick release documents  that is pickslip report gets generated
  so when  we do the ship confirm, during this process  ship confirm documents gets generated  
those are  packing slip report, bill of lading report etc gets generated


"in this process, manage shipment interface program does 2 things , 
1 is reducing the inventory and 
2nd is interfacing the record to AR module "
"after this process done, if you go and verify the sales order line level. 
we can see that shipped  then awaiting billing sort of status we can see"
"then we can go to schedule process and run the import auto invoice program by 
passing the source as a distributed order orchestration"

and we can enter the  sales order number to trigger the account receivable invioce .
"this invoice once completed, if you go to sales order line level  
under billing section you can see the invoice number"
"similarly you can go to the  account receivable offering, 
billing section you can able to see the transaction"
based on that we can create receipts to collect the money from the customers
once the payment is done, then we post all the transactions to the ledger

like this the O2C flow goes.
sales order header status - draft > processing > closed
"sales order line status - Not Started -> Created/Entered -> Scheduled ->
 Reserved -> Awaiting Shipping -> Shipped -> Awaiting Billing -> Closed"

o2c accounting enties

during sales order entry and submit - no account gets impact
during picking - stage subinventory account debited, source subinventory account  credited
during shipping -  COGS (cost of goods sold)  account debited, stage subinventory / material account account credited
during invoice - receivable  account  debited ,  revenue account credited
during receipt - cash account debited, cash clearing account credited

Order Tables
DOO_HEADERS_ALL
DOO_LINES_ALL
DOO_FULFILL_LINES_ALL
WSH_DELIVERY_DETAILS
Receivables tables
RA_INTERFACE_LINES
RA_CUSTOMER_TRX_ALL
 RA_CUSTOMER_TRX_LINES_ALL
RA_CUST_TRX_LINE_GL_DIST_ALL
AR_CASH_RECEIPTS_ALL
AR_RECEIVABLE_APPLICATIONS_AL
SLA Tables
XLA_EVENTS
XLA_AE_HEADERS
 XLA_AE_LINES 

GL Tables
 GL_INTERFACE
GL_JE_BATCHES
GL_JE_HEADERS
GL_JE_LINES

<img width="882" height="2431" alt="image" src="https://github.com/user-attachments/assets/dd79d6e2-9329-47e2-9590-f96423fdb760" />

