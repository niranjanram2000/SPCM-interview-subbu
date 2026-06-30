## counting is also called as accuracy methods

in business we are going to count the stock on yearly basis, Quarterly or monthly basis.
we have to count what is the stock available in the warehouse & 
what is the stock showing in the systems. there could be the difference

there are 2 types of counting
physical counting
cycle counting

Physical counting we performed for entire stock 
we are going to count our entire stock once or twice in a year

Cycle Counting – It’s called as a frequent counting we can perform very frequently 
for the important items like daily, weekly for less important items monthly.
"In cycle counting we can classify the items which item is very important, 
less important based on that classification we make the counting.

physical  counting
here first we create a physical inventory
u need to select that if you want to count all sub inventory or 
a particular sub inventories that we need to count

Approvals there are three types
always, never, out of tolerance
Always means If there is a deviation or no deviation always approval required
 Never means No Approval required
"If out of tolerance  means we are excepting a deviation of +/- 5% 
it will auto approve if more than 5% we need to approve it

here in physical counting , tags are generated. 
you need to provide the starting default tag number 
in real time, item number is a 12 digit alphanumeric number
its not possible to remember all  those number 
so we generate 3 or 4 digit number tag number

after creating the physical inventory, we run a couple of programs
first we run the generate physical inventory  snapshot program
it will give us the snapshot of current on hand stock in the choosed  sub inventory
after this prgram is sucessfully completed
We have identified the current system stock for that stock we need to generate tag number

then run Generate Physical Inventory Tags for current system stock to generate the tag numbers 

then run the program print physical inventory tag listing report
by providing the organisation  and  physical inventory  details
this report  we send to the store keepers to count the stock in the warehouse and
 ask them to send it back to us."
after that we record the physical inventory tags in the system by the data provided by the storekeepers
all the tags information, we need to enter manually. there is no fbdi or adfdi option available

then if the adjustments are within the tolerence.
it is auto approved. if it is out of tolerence it goes for approvals"
if the snapshot qty and counted qty are within the adjustment tolerence you can approve
or else you can reject the particular item counted qty
then finally we post the physical inventory adjustments to the system


cycle counting
 cycle counting can be done very frequently
In cycle counting before counting we are going to classify our items like which item we are going to count very frequently
cycle counting can be done 2 ways
1. abc class
2. item category

if you use abc class then
. Before initiating the counting we need to classify the items like 
class A (More important items); Class B (Less important items); Class C (very less important items)

Steps of Cycle Counting

 we define the abc classification set, here you select the criteria like based on what you want to do the cycle count
ex- current on hand qty, current item cost, current on hand value etc

once the program is succeeded  then you can see the abc classification set items
then we define the abc classes based on the abc classification set items data
after that we create the abc assignment group by assigning the classes and assigning the item to the classes

procedure for cycle counting 
at the item level, we need to enable the cycle count attribute for the items we need to do the counting
then we create the cycle count  by entering the details like which sub inv we need to include in the cycle count
then you give your abc assignment group and then we define the schedules and approvals
here you can select the auto schedule option and define the scheduling frequency like period or daily or weekly etc
and give the tolerence percentage and you give your inv schedule

"then you define the parameters like start counting sequence and 
how many max days the counting process can be late"
and you select if manual count is allowed or not
"then you define the abc classes and abc items and 
you provide information about how many counts can be done in a year "

if you want to include a particular item like most important, 
you can include that in  counting always

then we run the program generate count schedules
this is for how many days the counting should happen
the next program is generate count sequences - It’s nothing but day wise which items has to be counted
last program  we run is print cycle count listing report, here we provide the org and cycle count details and submit
this cycle count listing report we send  it to the store kepper. 

he will enter what is the qty available physically  with comments"
"the items which we see is based on the scheduling, 
like today which items we need to be counted only those item will display here"
 then  we need to record the counted sequences,  i.e,recording the counted qty information in the application
if the counted qty is out of  tolerance, it goes for approvals
if the counted qty and system qty of an item is with in the tolerence  we approve it  or else we reject it

"or we can submit that particular item for counting again, 
whenever the new counting schedule starts this item will be counted again"
by doing this we submit the approve count sequences and post the adjustments 
you can  go to review complted transactions, there you can see the cycle count adjustments  details

cycle counting based on item categories  

at the item level, we need to enable the cycle count attribute for the items we need to do the counting
then we create the cycle count  by entering the details like which sub inv we need to include in the cycle count

if we deceide to do the cycle count based on category then you need to select that here in the first page itself

if you select item categories, then you dont get to use abc analysis
then you need to select the sub inv that you want to include in the cycle count

then you need to define schedule and  approvals
"here you can select the auto schedule option and 
define the scheduling frequency like period or daily weekly etc"
you  can select if approval is required andgive the approval type like always or if out of tolerence
and give the tolerence percentage and you give your inv schedule

"then you define the parameters like start counting sequence and 
how many max days the counting process can be late"
and you select if manual count is allowed or not

"then youcanselect the categories 
that you want to include in the cycle count or exclude in cycle count"
once you include  the item categories then you get the syncornization options 
if you select none , then sysyrm is not going to pull the items in the  categories automatically
you have to assign manually

if you want to pull the items from the categories then you have to select the complete option
whenever any changes happens to the category like when you have added one more item 
or you removed any existing items , if you want to suncronise and delete those items

then you can select the append changes option
then you give how many times the counting should happen in a year for that particular category
the system automatically pulls the items form that category  
if you want to include or exculde a particular items in that schedule always, you can do that

then you review and submit
then we run the program generate count schedules
this is for how many days the counting should happen
the next program is generate count sequences - It’s nothing but day wise which items has to be counted
last program  we run is print cycle count listing report, here we provide the org and cycle count details and submit

"this cycle count listing report we send  it to the store kepper. 
he will enter what is the qty available physically  with comments"
"the items which we see is based on the scheduling, 
like today which items we need to be counted only those item will display here"

" then  we need to record the counted sequences, 
 i.e,recording the counted qty information in the application"
if the counted qty is out of  tolerance, it goes for approvals
if the counted qty and system qty of an item is with in the tolerence  we approve it  or else we reject it

"or we can submit that particular item for counting again,
 whenever the new counting schedule starts this item will be counted again"
by doing this we submit the approve count sequences and post the adjustments 
you can  go to review complted transactions, there you can see the cycle count adjustments  details



For cycle count :if adjustment is positive then
Inventory valuation:db
Offset:cr

<img width="1397" height="496" alt="image" src="https://github.com/user-attachments/assets/299cf55f-9dcf-469f-a192-03d1081dc3a8" />

ABC classification set
ABC assignment group
Define the cycle count
link the ABC assignment group
schedule the cycle count
do the counting
at item level we need to enable the cycle count tick box
usually all raw material, finished goods we will tick box
then we group them into A, B, C classes
in A class we can count yearly 200 times
B classes we can 100
C class 50
then system will calculate and provide the list of items
there is formalua 
we have (A class * number of counts + B class * number counts + C class* Count) / number of working days
yes
to define the subinventory creations
we can also create the locators
we can also assignn the item to subinventories and locators

we have the FSM 
where we can download the configruation and then we can unzip the folder
manage subinventories and locators is the configuration
download the configuration 
if there is no setup then we need to setup at least one subivnentory and then we can download 
setups like manage subinevntory and lcoator setup  and then we can u


