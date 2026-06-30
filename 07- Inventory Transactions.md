Inventory Transactions or movements

By using inventory transactions we can increase or decrease the stock or we can move the stock different locations 
We have different types of inventory transactions
1. Miscellenouse transactions
Miscellenouse transactions include transactions like Miscellenouse receipt, Miscellenouse issue, account alias receipt, account alia issues, etc
Miscellenouse transactions are using for stock adjustment or initial stock load purpose
 issue  means decreasing the on hand
receipt means increasing the on hand
Miscellaneous transaction is the transaction which is used to receipt or issue the material without any documentation.
miscellaneous transaction use to Load all on-hand items during Inventory Management Implementation, 
Issue items to individuals, departments, or projects,Receive items that were acquired without purchase orders,
 to post Counting adjustment And to Issue damaged items to expense accounts, such as scrap .

2. Sub inventory transfer

"subinventory transfer is use to 
transfer material within your current organization between subinventories, "
"or between two locators within the same subinventory. 
in sub inv transfer, there is no documantation support"

3. movement request
"Movement requests are requests for the movement of material within an 
inventory organization with document support"
Document here is movement request pickslip report.

 there are 2 types of movement request
movement request transfer - you are transfering the item from source sub inv to destination sub inv
monement request issue - here you are issueing the item from  source sub inv to destination account
 for movement request, approvals can be configured
we have automatic,job level,single approver,approval group and supervisor hierarchy


there are 4 kinds of movement request
1. requistion movement request(manual)
2. pick wave movement request (comes in sales order)
3. replenishment movement request (min max planning)
4. job movement request(min max planning)

steps in creating the movement request

1. create movement request
2.  create picks i.e. generate pickslip report (based on the pickslip report, pickers will perform the transer of stock)
3. confirm the pick slip in the application
for  movement request approvals can be configured
approval types  are automatic,job level, single approver,supervisor and approval group

Movement request transfer transaction type is use to subinventory transfter.
Movement request issue transaction type is use to issue stock againt account.

4. inter organisation transfer
"Interorganization transfers enable you to transfer material between
 inventory organizations without creating any document."
The items that you transfer must exist in both the source and destination organizations.
on hand should be there in the source inventory to transfer to destination inventory
"for interorg transfer , you need to define the inter org parameters between 
source and destination organization"
in interorg transfer , there is no documentation support by default. 
if needed you need to enable the transfer order checkbox in interorg parameters

There are 3 types of inter org transfer
direct inter org transfer
intransit inter org transfer
transfer order
in direct inter org transfer -  movement of items happens directly between inventory organizations. 
The destination organization receives the material immediately when you submit the transaction.

In intransit interorg  transfer - 
movement of materials happens from the shipping organization to  the intransit inventory
then we have to move the  items from in transit inventory to the destination org through receipts

accounting entries
in interorg transfer (direct,intransit)
source org : issue
trade intransit  valuation  DR
inventory valuation CR

interorganisation receivables DR
trade intransit valuation  CR

destination org : receipt
inventory valuation DR
trade intransit valuation  CR

trade intransit valuatiion DR
trade clearing CR


movement request 
transfer order
these are the document number enabled
<img width="861" height="2130" alt="image" src="https://github.com/user-attachments/assets/78987138-46eb-4693-9061-9699d393f2f4" />
