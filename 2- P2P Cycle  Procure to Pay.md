P2P Cycle

"The P2P cycle start with the submission of a requisition. 
There are two types of requisitions: purchase requisitions and internal requisitions (or transfer orders). 
A requisition is typically raised for procuring materials or services. 
It essentially serves as an indent or formal request for these 
resources. We raise a purchase requisition when there are no materials or stock available internally. 
"

"Once the requisition is generated, it undergoes an approval process, which can be configured in various ways
. Upon approval of the requisition, 
if an approved supplier list is available, a standard purchase order can be created directly. 
In the absence of approved suppliers, the negotiation process can be initiated. 
The sourcing module can be utilized for this purpose, where different sets of RFI (Request for Information), 
RFQ (Request for Quotation), or auctions can be configured."

so these rfi are for information purpose , just to check pricing information availability
rfq are request for quotation, so basically we have multiple types of rfq
suppliers will analyse the rfq and they will respond back to that rfq. we an call it as quotation
here we have  single stage  RFQ, two stage RFQ and surrogate quote 
once the quotes has been received from multiple suppliers, the sourcing team will evaluate the quote
which is best suitable for their business that means they will do the quote analysis
after quote analysis they issue the award nothing but the purchase order
in cloud we have 3 types of purchase order 
standard purchase order, blanket purchase agreement and contract purchase agreement
so standard purchase order we will raise when we know all the information like

item, quantity,price, need by date, and terms and conditions
when you know all these 5  elements and that is for one time request for materials or service
all purchase orders are commercial documents that means we agreed certain terms and conditions with our suppliers
again the purchase orders can go for approvals.
once the purchase order is approved , we can issue the purchase order pdf to the  supplier.

blanket purchase agreement we will raise when we are freezing the rate for a date range
nothing but  its a rate contract award. 
rate is freezing for a date range. as and when we want material we do a standard PO as a release document
in BPA,we have line information
in BPA, we also initiate the negotiation in the form of price breaks , where we can set up the discounts
when between a certain date range you  purchase,you can get it discount
these are 2 types one is cumulative and another is non-cumulative
"cummulative- we can create multiple release, the release which reach the quatity then discount will get applied
non cummulative- we always purchase in that range for the discount"
then we have contract purchase agreement, here we only agree the terms and conditions
we don't have any line information,shipment information etc
so when ever we want any material against the cpa, we can do a standard po as a release document

so once the po has been shared with suppliers. suppliers can send the asn or they can send the materials directly to us
these materials we can receive  with 3 routing methods
direct delivery, standard receipt and inspection required
in the direct delivery, we receive the material and do the delivery transaction to sub inventory immediately
in standard receipt,  we recive to a reciving  location, and then we deliver to the sub inventory
in inspection required, we receive to a receiving location. 
quality control team will do the inspection. it will be 2 outcomes either accept or reject
accepted materials will be delivered to the sub inventory

rejected materials will be rejected to a rejected sub inventory or we can do the return to vendor process
so after we receive the material , we also receive the invoice from the supplier
these invoices we will match  with 3 match options
we have 2 way matching, 3  way matching, 4 way matching
that means we are matching 2 documents here, invoice and purchase order

in 3 way matching, we are matching purchase order with receipt quantity and invoice quantity
that means we are matching 3 documents here
when its a four way, the routing should be inspection required because
we are matching invoice  with purchase order, receiving and inspection results.
so once the invoice has been validated and accounted, then we will release the payment
we can make a single payment or we can run the payment process profile
and finally we can do the invoicing payment process and reconsilation process
this is how the procure to pay follows and in my project also followed similarly.
P2P Line and Header Statuses
requistion status -  Incomplete -> Pending Approval -> Approved
po header/ line status -  incomplete-> pending for approval -> open -> closed for receiving -> closed for invoicing -> closed
po header/ line status -  incomplete-> pending for approval -> open -> closed for receiving -> closed for invoicing -> closed

accounting  entries on p2p cycle

 requisition - no accounting impact, only charge accounts gets  defaulted 
purchase order - no accounting impact, only accounts gets defaulted 
 during receiving -  receiving inspection account debited, accural account credited
during   delivery or Putaway transaction - inventory account  debited, receiving inspection account  credited
during invoice - accural account debited, supplier liability account credited
during payment - Supplier liability account debited, cash account credited

Tables
Requisition tables
POR_REQUISITION_HEADERS_ALL
POR_REQUISITION_LINES_ALL
POR_REQ_DISTRIBUTIONS_ALL
PO TABLES
PO_HEADERS_ALL
PO_LINES_ALL
PO_LINE_LOCATIONS_ALL
PO_DISTRIBUTIONS_ALL
POZ_SUPPLIERS
RECEIVING TABLES
RCV_SHIPMENT_HEADERS
RCV_SHIPMENT_LINES

INVOICE TABLES
AP_INVOICES_ALL
IBY_PAYMENT_METHODS
AP_TERMS
AP_INVOICE_LINES_ALL

<img width="1075" height="2672" alt="image" src="https://github.com/user-attachments/assets/6b215b7a-80d8-4776-81b1-bfbfd1e4525e" />

