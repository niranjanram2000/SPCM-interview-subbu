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

### P2P సైకిల్

P2P సైకిల్ ప్రారంభం
P2P సైకిల్ requisition (అభ్యర్థన) సమర్పణతో ప్రారంభమవుతుంది. రెండు రకాల requisitionలు ఉంటాయి: Purchase Requisition మరియు Internal Requisition (Transfer Order). requisition సాధారణంగా వస్తువులు లేదా సేవలు కొనుగోలు చేయడానికి రైజ్ చేస్తారు. ఇది ఒక indent లేదా ఆ ఫార్మల్ రిక్వెస్ట్ లాంటిది. ఇంటర్నల్ స్టాక్ లేని సందర్భాల్లో Purchase Requisition రైజ్ చేస్తాం.

అప్రూవల్ మరియు సోర్సింగ్
Requisition రూపొందిన తర్వాత అది ఒక Approval Process ద్వారా వెళుతుంది (ఇది వివిధ రీతులుగా కాన్ఫిగర్ చేయవచ్చు). Requisition అప్రూవ్ అయిన తర్వాత, Approved Supplier List ఉంటే Standard Purchase Order (PO) నేరుగా క్రియేట్ చేయవచ్చు. Approved suppliers లేకపోతే negotiation ప్రారంభిస్తారు. ఈ కోసం Sourcing Module ఉపయోగిస్తారు — ఇక్కడ RFI (Request for Information), RFQ (Request for Quotation) లేదా auctions వంటి సెట్లు కాన్ఫిగర్ చేయవచ్చు.
- RFI: సమాచారం కోసం — ధరలు, availability మొదలైనవి తెలుసుకోవడానికి.
- RFQ: కోట్ కోసం రిక్వెస్ట్ — సరఫరాదారులు RFQని విశ్లేషించి ప్రతిస్పందిస్తారు; ప్రతిస్పందనను Quotation అంటారు.
- RFQలు రకాలు: Single-stage RFQ, Two-stage RFQ, Surrogate Quote.
Quotes (బహుళ సరఫరాదారుల నుండి వచ్చిన తర్వాత) sourcing టీమ్ వాటిని evaluate చేసి వ్యాపారానికి సరైనదాన్ని ఎంచుకుంటుంది — దీన్ని Quote Analysis అంటారు. Quote analysis తర్వాత Award ఇవ్వబడుతుంది, అంటే Purchase Order జారీ చేయబడుతుంది.

Purchase Order రకాలు (Cloud లో)
Cloudలో మూడు రకాల POలు ఉంటాయి: Standard Purchase Order, Blanket Purchase Agreement (BPA), Contract Purchase Agreement (CPA).
- Standard Purchase Order: ఐటెమ్, quantity, price, need-by-date, terms & conditions — ఈ 5 అంశాలు తెలిసి ఒకసారి కోసం వస్తువులు/సేవలు కోరినప్పుడు వాడతాం. POలు కమర్షియల్ డాక్యుమెంట్స్ — సరఫరాదారుతో కొన్ని terms & conditionsకి అంగీకారం. POలు కూడా approvalsకి వెళ్తాయి; అప్రూవ్ అయిన తర్వాత PO PDFని సరఫరాదారుకు ఇష్యూ చేస్తాం.
- Blanket Purchase Agreement (BPA): ఒక తేదీ పరిధి కోసం రేటు ఫిక్స్ చేయడం — rate contract award. అవసరమైనప్పుడు ఆ BPAకి releaseగా Standard PO చేయబడుతుంది. BPAలో line information ఉంటుంది. Negotiationలో Price Breaks (డిస్కౌంట్లు) కూడా సెట్ చేయవచ్చు — ఇవి రెండు రకాలుగా ఉంటాయి: Cumulative మరియు Non-cumulative.
- Cumulative: అనేక releases చేయవచ్చు; releases కలిపి ఒక quantityకి చేరినప్పుడు discount వర్తిస్తుంది.
- Non-cumulative: ప్రతి కొనుగోలు ఆ రేంజ్‌లో ఉంటేనే discount వర్తిస్తుంది.
- Contract Purchase Agreement (CPA): ఇక్కడ కేవలం terms & conditionsకి ఒప్పందం ఉంటుంది; line లేదా shipment సమాచారం ఉండదు. CPAకి ఆధారంగా కావలసినప్పుడు Standard POని releaseగా చేస్తాం.

Receiving (సరుకు స్వీకరణ) మరియు ASN
PO సరఫరాదారులకు షేర్ చేసిన తర్వాత, సరఫరాదారులు ASN (Advanced Shipping Notice) పంపవచ్చు లేదా సరుకు నేరుగా పంపవచ్చు. సరుకులను మూడు routing methods ద్వారా స్వీకరిస్తాం:
- Direct Delivery: సరుకు అందగానే sub-inventoryకి delivery transaction చేస్తాం.
- Standard Receipt: ముందుగా receiving locationకి స్వీకరిస్తాం; తర్వాత sub-inventoryకి delivery/putaway చేస్తాం.
- Inspection Required: receiving locationకి స్వీకరించి, QC (Quality Control) టీమ్ inspection చేస్తుంది. ఫలితం రెండు రకాలే: Accept లేదా Reject.
- Accepted వస్తువులు sub-inventoryకి పంపబడతాయి.
- Rejected వస్తువులు rejected sub-inventoryకి వెళ్తాయి లేదా Return to Vendor ప్రక్రియ ద్వారా తిరిగి పంపుతాం.

Invoice Matching (ఇన్వాయిస్ మ్యాచ్)
సరుకు స్వీకరించిన తర్వాత సరఫరాదారుని ఇన్వాయిస్ వస్తుంది. ఇన్వాయ్సులను వివిధ matching ఆప్షన్లతో మ్యాచ్ చేస్తాం:
- 2-way matching: Invoice మరియు Purchase Order మాత్రమే మ్యాచ్.
- 3-way matching: Purchase Order, Receipt (received quantity) మరియు Invoice quantity — మొత్తం 3 డాక్యుమెంట్లు మ్యాచ్.
- 4-way matching: PO, Receiving, Inspection results మరియు Invoice — ఈ రూటింగ్ కోసం receiving రూట్ Inspection Required ఉండాలి.
ఇన్వాయిస్ validate చేసి accounting చేసిన తర్వాత payment విడుదల చేస్తాం — single payment చేయవచ్చు లేదా payment process profile ద్వారా బల్క్‌గా రన్ చేయవచ్చు. చివరగా invoicing, payment process మరియు reconciliation జరుగుతాయి.

P2P లైన్ మరియు హెడ్డర్ స్టేటస్‌లు
Requisition Status: Incomplete → Pending Approval → Approved.
PO Header/Line Status: Incomplete → Pending for Approval → Open → Closed for Receiving → Closed for Invoicing → Closed.

P2P సైకిల్‌లో అకౌంటింగ్ ఎంట్రీస్
- Requisition: అకౌంటింగ్ ఇంపాక్ట్ లేదు; కేవలం charge accounts default అవుతాయి.
- Purchase Order: అకౌంటింగ్ ఇంపాక్ట్ లేదు; accounts default అవుతాయి.
- During Receiving: Receiving Inspection Account డెబిట్; Accrual Account క్రెడిట్.
- During Delivery / Putaway: Inventory Account డెబిట్; Receiving Inspection Account క్రెడిట్.
- During Invoice: Accrual Account డెబిట్; Supplier Liability Account క్రెడిట్.
- During Payment: Supplier Liability Account డెబిట్; Cash Account క్రెడిట్.

సంబంధిత టేబుల్స్ (Oracle/Cloud టేబుల్స్)
Requisition Tables: POR_REQUISITION_HEADERS_ALL; POR_REQUISITION_LINES_ALL; POR_REQ_DISTRIBUTIONS_ALL
PO Tables: PO_HEADERS_ALL; PO_LINES_ALL; PO_LINE_LOCATIONS_ALL; PO_DISTRIBUTIONS_ALL; POZ_SUPPLIERS
Receiving Tables: RCV_SHIPMENT_HEADERS; RCV_SHIPMENT_LINES
Invoice Tables: AP_INVOICES_ALL; IBY_PAYMENT_METHODS; AP_TERMS; AP_INVOICE_LINES_ALL

మీకు ఈ అనువాదం బాగా అర్థమైందా? అవసరమైతే ప్రతి స్టెప్‌కు సంబంధించిన ఫ్లోచార్ట్ లేదా చిన్న ఉదాహరణలతో మరింత సులభంగా వివరించగలను.


