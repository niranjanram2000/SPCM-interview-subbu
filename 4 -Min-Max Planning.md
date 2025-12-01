min max planning
Min Max Planning is one of the replenshiment planning method in Inventory. In Min Max planning the system re-order stock when the current stock goes down to the minimum quantity

min max planning is used to maintain inventory levels
min max planning can be done at 2 levels - 1. organisation 2. sub inventory
for an  item we can configure attributes like  min qty, max qty, min order qty, 
max order qty at the item level for maintaining the min & max qty of the stock

formulas for min max planning

Total Availability = Onhand + Incoming supply - demand
incoming supply or pipeline supply include open purchase order, open work order
"If Total availability <(less than) Min Qty, then 
the application try to order autumatically, if min max planning program is scheduled"
"Whenever this program is running its check for the item, 
item availability, min qty it will verify all this information"

based on the item attributes system will order the stock from different sources
for example: In case if item has enabled with make or buy attribute as buy and supply source as Supplier, then system will create the Purchase requisitions, when we run or schedule the jobs like print min max planning report and process supply chain orchestration jobs.

In case if item has enabled with make or buy attribute as buy and supply source as Inventory, then system will create the Transfer Order, when we run or schedule the jobs like print min max planning report and process supply chain orchestration jobs.

In case if item has enabled with make or buy attribute as buy and supply source as Sub Inventory, then system will create the Replenshiment movement request, when we run or schedule the jobs like print min max planning report and process supply chain orchestration jobs.

In case if item has enabled with make or buy attribute as make and supply source as Inventory, then system will create the  work order, when we run or schedule the jobs like print min max planning report and process supply chain orchestration jobs.
<img width="990" height="1244" alt="image" src="https://github.com/user-attachments/assets/e2f44b44-ecbe-4692-a2d5-e9e7628b3871" />
