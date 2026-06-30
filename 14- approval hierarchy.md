approval hierarchy

1. employee supervisor hierarchy
   
2.job level hierarchy

3.position hierarchy

4. approval group
   
5.single approver

6. automatic approval
 
employee supervisor hierarchy works on employee and manager relationship
in supervisor hierarchy, configuration wise, we dont need to create any job, position
or anything .we directly create a employee and attach the manager to that employee
and create an supervisor hierarchy approval by providing the hierarchy details and deploying it
"after that we create respective documents 
like requsition or po or bpa or cpa"
"and verify the approvals is working andthen check 
whether approval notifications working and approve it"


job level hierarchy works on the job of the employee  and its level of job.
system will identify the next job based on the level
you have to create the job and enter the job level also
after that assign the job to the employee. the configure your approvals
then create the reapective document(requsitiion,po,bpa or cpa)
and verify the approvals are working or not
and verfying the approval notofications and approving the document


position based hierarchy

position hierarchy works on the position , not based on the job.
departments and jobs are mandatory to create positions
assign job and position to the respective employees
then create  a position tree, then create tree version
in the tree version add the positions reporting wise who is reporting to whom

then make it active and then do the row or column flattening
difference between row flattening and column flattening is
 whatever the positions that you have created. those positions data
will sit in the table is decicded by  flattening
ex- if you do row flattening then the positions data will sit  row wise in the table
if  you do column flattening then positions data will sit column wise in the table

approval group

approval group has to be created in bpm 
in that you need to add the approvers that you need to approve the documnent
and then save it

then you need to create approval hierarchy by calling the respective approval group 
in the approvals.

then create the reapective document(requsitiion,po,bpa or cpa)
and verify the approvals are working or not
and verfying the approval notofications and approving the document

incase of single approver then the approval goes for a single person for approvals


Project modules
we need to select the condition that the project and task selected then we will create a approval rules 
like where we mention the project manager and next level

if the requiisition is non project enabled then 

we need to use the HCM in shared mode to create employees and assign jobs and positions
TAD
yes


Parallel Approval: All at once
Serial Approval: One after the other
1. Parallel Approval – Consensus:
"The client requires every PO with Procurement Business Unit
 as “Business Unit” to be routed to 3 approvers."
 The PO status should become “Open” only after all the 3 approvers approve the PO

(OR)
Consensus: All the relevant approvers need to approve or else the approval will be rejected
2. Parallel Approval – First Responder Wins:
"The client requires every PO with Procurement 
Business Unit as “US1 Business Unit” to be routed to 3 approvers. "
The PO status should become “Open” after any one of the 3 approvers approve the PO

(OR)
First Responder Wins: Decision (whether approve or reject) of the first responder will be final

"Select “Setup:” as Procurement. Select the functional area as “Approval Management”. 
Select “Show” as All tasks. Go to task Manage Approval Groups. "
This will take you to the “BPM (Business Process Management) Worklist

Approval Group.
"An Approval Group is a Sequence / Collection of Users / Approval Groups /
 a combination of Users and Approval Groups. Sequence in approval groups "
"is relevant for sequential approval. 
For a parallel approval scenario all the members of the approval group will receive the approval notification simultaneously"

Approval Rules - Components
1. Rules: Determines name and priority (precedence) of the rule.
2. Conditions: Determines the trigger for the rules
3. Actions: Determines the actions to be taken after the rules are triggered



we need to setup the user defined attribute like currency where we can add the curreny type like USD
then we have match that condition we can send to the approvals



