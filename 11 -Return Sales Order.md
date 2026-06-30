When customer reqeusted to take the material or service back, then the sales team will raise the return sales orders


Return Sales Orders can created in two different ways
Referrenced Return and Un-Referrenced returns
when you create an order and add the item, in the sales order line undr actions
you can select add unreferenced return lines and create an return sales order

Or else we can create an return order on already shipped sales order also
when you go to the shipped sales order at the line level
 there you will have a return option  available

in that you can select the return type and return reason and create a return sales order
before submitting the salesorder,you need to provide the warehouse details
for which warehouse you  want to receive the returning item
after submitting the order, RMA number gets generated

when you go to receive expected shipments and search with the RMA order number
 you can  receive the item and create receipt
and then you can  perform inspection  and do the put away
after the put away , you need to run the program
send receipt confirmation

By giving the org and RMA number details and selecting
source as oracle fusion order orchestration and planning
and submit the program
up on sucessful completion of this program only
the status of return order changes to delivered from awaiting receiving
 for RMA orders the receipt routing is defaulted fromthe receiving parameters for return orders

 for return orders, you need to configure  return price list
return price list is used when the selling price and return price lists of the item are different
for return orders, we need to enable the returnable attribute at the item level against particular item


we usually need to add new line status
we need to include them in the orchestration
we need to move the steps from the seeded orchestration
like we need to add this step may be between scheduled and rserved
then we need to link the step number to new steps

we have update and close orders ESS jobs

we usually pass the order header id
we usually pass the order header ID in our project

this Is used to to idenfiy how long the time taken between shipping method and mode of transport
etc we usually set in the manage intransit time
where we can select the source and destination and mode of transport etc
these will give the actual arrival date etc

back to back buy we buy and recive the stock in our warehosue and then we will ship to customer
in the dropship we directly ask our supplier to customer to delivery the stock

we have to configure the SCFO also where we need to setup the dropship qualifiers


then we need to do the sandbox customization
