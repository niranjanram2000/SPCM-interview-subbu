GOP(Global order promising)


GOP module is useful for two things

1) Derive the schedule ship date
2) Identifying the Fulfillment 

for these first we need to define the source system and the destination system 
in - Manage Planning source systems and we need to select  our inv orgs 
then we need to run the collections
"after the collections program is suceeded, 
the collected data is will get transferred to the source table to the planning tables "

then we can set up the atp rules

we have 3 types of ATP promising modes
1.supply chain availability
2. lead time based
3.infinite availability based

Lead time is the time taken to complete that activity
in that we can give the user defined leadtime or pre processing lead time etc
in supply chain availability, it is based on supply and demand criteria.
based on that the scheduled shipdate is  decided
if its infinite availability, we have infinite stock available.  ex- if the sales order is created today 

then the scheduled ship date  is today itself
and then we select the assignment basis, like item, category,organisation or item and organisation
and assign them

then we define the sourcing rule
sourcing rule purpose is to identify the fulfillment for the sales order
in sourcing rule ,we have  local sourcing and global sourcing rule
local sourcing rule means it is applicable a particular inventory org
global sorcing rule means it is appliclabe to all the inventory organizations

we have 3 sourcing types,
1. transfer from 2.buy from 3. make at
if you use transfer from, then the sourcing is done from a particular inv organization
if you use buy from, then sourcing is done from a particular supplier
you can give the ranking and allocation percentage  when you are creating the sourcing rule

then we define the sourcing assignment
by providing the assignment level like customer or customer and customer site or item
or item and org etc
here we attach our sourcing rule
 ex- if the assignment level is item and organisation, then  use this soucring rule like that

then we need to add our assignment set to the msp default assignmnet set in 
manage adminstrative profile options

then only the system is going to understand otherwise no
then we need to run the refrersh and start the order promising server program
what are all  new or changes you have created that need to be submitted through this program
this is how the sourcing rule setup
<img width="814" height="1482" alt="image" src="https://github.com/user-attachments/assets/60b153c8-c575-40e2-9520-a56e945b4d8b" />
