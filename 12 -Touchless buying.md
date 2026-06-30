Touchless buying(automatic po creation)

Creating a purchase order automatically from the requsition whether the requsition
got created manually or the requsition got imported manually in any case you want to create PO automatically
then we can touchless buying feature

automatic po creation can be done 2 ways

first one is  with negotiated check box 
other way is without enabling the negotiated check box (using BPA or CPA)

first one is  with negotiated check box 
for this when you are creating requsition , you need to enable the negotiated checkbox to yes
and you need to provide the supplier, buyer details then PO gets automatically created from requsition.
for automayically created po we need to  by-pass the approvals,
for that in procurement business functions, you need to enable auto generate orders from requester negotiated lines checkbox
and bypass approvals for automatically submitted orders checboxes  has to be enabled
if all these setups are done properly then when you create requistion by selecting the 
negotiated checkbox and give the supplier and buyer details then PO is automatically created from requsition
that po will be automatically approved and it will be in open status

other way is without enabling the negotiated check box
for this you should have an agreement(BPA or CPA) with the supplier
in requsition business functions, create orders automatically from requsition import should be selected to yes.
in procurement business functions, by pass approvals for automatically submitted  orders should be enabled.
it works for import requsitions for min max, dropship,back2back

after po gets auto created, if you want to auto submit for approval
then at the agreement level,you should enable auto submit for approval
checkbox in the control section
if you want to verify the po and then submit for approval then disable this checkbox
ASL is not mandatory for automatic po creation from requsition

 if one item is having 2 suppliers agreement, then the system will go to the ASL(approved supplier list)
if you have created one ASL then it will pickup that supplier for automatic po creation
for automatically created po's default buyer preference are
1st preference  will be item level
2nd preference is procurment business functions
3rd preference is buyer assignment rules
