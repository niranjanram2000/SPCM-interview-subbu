Transfer Order
Transfer order is a transaction which provides the ability to transfer material from source organization to destination organization
transfer order can be done 3 ways
	1. from supply chain orchestration and selecting new supply request
	2. From requsition form by selecting source as Inventory organization
	3. From item on hand quantities form from inventory by selecting create supply request from action
	transfer order  represents demand and supply in a single document
	there are 3 types of transfer order
	1. Direct Organization transfer
	2. Intransit Organization transfer
	3. Intransit organization transfer with Transfer order enabled tick box
	on hand should be there in the source inventory. item must be linked to both the organisation
	
 setups for  transfer order 
	
   "then you need to create inter org parameters between source org and 
destination org by selecting transfer type as direct or intransit"
	"at the item level,transfer order attributes like transfer order enabled and 
internally transferable  must be enabled  "
		at the item level, planning method should be selected as non planned.
	for non planned items, source org is indenified  by interorg parameters
	if its a planned item , then  the source org is identified from sourcing rule and sourcing assignment through GOP
	transfer cost i.e item cost for the item should be there. create a cost scenario and add the item cost
	if there is no item cost defined then it would pick the purchase price from the item level. if defined yes
	
   transfer order process
   
 we  create an internal requistion,with item  and source as inventory and providing the source org details 
	in requsition business functions , if you have selected checkbox for supply availability for internal transfers 
	then when you create a internal requsition ,you can see the inv of the item in the source org
	according to inv available in the source  org ,you can create a internal requisition
	you can select from which inv that you want to source the item
	then you can add the requsition to the cart , then review and submit it
	
   then from tools > schedule process we run the process supply chain orchestration interface program
	"whenever  there is a data interface between two modules, 
we have to run process supply chain interface program"
	in the supply chain interface program , we select the source as self service procurement and submit it.
	after the program is sucessfully completed, when we go to inventory management
	and click on manage transfer orders and give the source org or destination org details and give it a search
	you can  see transfer order number got generated.
	"Click on transfer order number link. It will take us to the Transfer Order page.
"
	Now transfer order is in Open status.
	
create a pick wave using the transfer order number to release the item from the source sub inv
	this process will generate the pick release documents that is pickslip report
	then from the manage shipment lines, provide the transfer order number and give it a search
	it will show ur shipment details. then clicking on auto create shipment
	shipment number gets generated. when you click on that shipment number
	it will take you to the shipment screen, where you give the shipping method and shipment qty and submit
	this porcess will generate  the shipping documents like bill of lading and packing slip report
	
send shipment advice and manage shipment interface also runs in the background
	then To receive the material into the destination organization.
	if its a direct transfer, then when you click on the ship confirm automatically 
	the transaction is processed and destination org will receive the item
	for this u need to define the item transaction defaults like for a particular tranaction
	and particular item , use this sub inv as default to store it
	if its a intransit transfer order then u have to receive the materials against the receipt routing method  defined
	
   intransit without transfer order setups
	in inter org parameters, transfer type should be intransit and receipt routing should be  selected
	receiving parameters for the destination org has to be defined
	shipping parameters for the source org has to be defined
	during the inter org transfer ,it will generate a shipment number
	using that shipment number, you willl do the picking and shipping from the source org
	and you will receive against the destination org using the receipt routing method
	which you have selected in interorg parameters
	
   transfer order with inventory management
	
   "first u need to map ur destination inv to the destination location. 
this will make that location as local location"
	"then you need to create interorg parameters between source org and 
destination org by selecting transfer type as direct or intransit"
	"at the item level,transfer order attributes like transfer order enabled and 
internally transferable  must be enabled  "
	at the item level, planning method should be selected as non planned.
	
   purchase price should be given at the item level
	on hand should be there in the source org
	item should be associated with both the orgs
	in inventory management,click on manage item qty screen
	go to actions and select request  transfer order
	it will take you to the supply request creation page
	here give the item and requested qty and requested delivery date  and then select the source 
	and  submit it
  
this process will automatically create a transfer order number
	which you  can check by searching for the item in the manage transfer order page
	using that transfer order number,pick and ship from the source org
	and receive it against the destination org using the receipt routing method selected in the 
	inter org parameters
<img width="1073" height="2445" alt="image" src="https://github.com/user-attachments/assets/99d2123d-3236-4392-bb9c-53ed91637cdb" />
