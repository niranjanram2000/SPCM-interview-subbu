https://itonlinehub.com/v2/oracle-project-implementation-support-process/

Implementation types
Types of Implementation:
1. Fresh Implementation
2. Rollout projects
3. Up gradation Projects
4. Supporting Projects
5. Enhancement Project (Adding Modules)
Implementation steps
1. Project Management Plan
2. Kick off Meeting
3. As Is Analysis
4. As Is Document
5. To be document
6. Mapping
7. Gap Analysis
8. Configuration/ Setup
9. Testing of Configuration
10. CRP – Conference Room Pilot
11. UAT – User Acceptance Test
12. Production Configuration
13. Data Migration
14. End User Training
15. Go Live
16. Parallel Run
17. Post implementation Support
##Implementation steps
### 1. Project Management Plan:
In this phase, Project Manager will create document called “PMP Document” with the details of project time frame, required resources and the total cost of the project.
This document will be shared with client side steering committee members to get sign off that document.
Manager will be shared this document with team members.
## 2. Kick off Meeting:
In this phase introduction will be happen between the implementation team and the steering committee members nand super users of client side.
## 3. As Is Analysis:
In this phase implementation team will study and analyze the current process of the client business.
## 4. As Is Document: 
This will be created with the current process analysis.
## 5. To Be Document:
In this document we will capture all the information how would be the future process of client on Oracle Apps.
This document will be reviewed by steering committee of client and get signed off.
## 6. Mapping:
Process of verify the customer requirement with Oracle Standard functionality is called “Mapping”.
## 7. Gap:
If any requirement is not available in the Oracle Standard functionality is called Gap.
To fix the gap we have to do the following Gap Analysis to find out the best solution.
Customization
Form Personalization
Work Around
Re engineering
Enhancements
Implementation steps
Customization: Developing new forms or Reports in Oracle Apps
Form Personalization: Without writing any programs and coding we can modify some forms.
Work around: Some process may not be required to do by customer, but he has to follow the process to complete the activity. For example: Zero payments and Petty cash.
Re engineering: Changing the current process followed by customer to fit with oracle.
## 8. Configuration & Setup:
In this stage we will configure the setup for client systems.
We have 3 types of instances:
1. Test instances (CRP Instance) – Only for testing
2. Development Instance (Dev Instance) – To develop custom components
3. Production Instance (Prod Instance) – Real time instance.
## 9. Testing of Configuration:
We will verify the accuracy of the configuration before showing to client.
## Implementation steps
### 10. CRP: Conference room pilot:
We will show the configuration to client and will get signoff. In general there are 2 CRP’s is enough to get sign off.
### 11. UAT: User Acceptance Test:
In this phase test instance will be provided to key users of client to test the application.
### 12. Production Configuration:
Once UAT signed off we will configure the production instance. Through “cloning” test instance will be copied to Dev instance for the purpose of technical people usage.
### 13. Data Migration:
Data moving from Legacy System to Production instance is called “Data Migration” or “data Conversion”.
Functional Consultant responsibility in data migration:
Template preparation for Suppliers, Customers, Purchase Invoice, Sales invoices, Assets, Bank accounts, Payment terms.
Implementation steps
Templates will be filled up by client and implementation team will validate the completed templates.
These templates with data will be shared to technical consultants.
Technical people will be developing some staging tables by using some tools like “SQL Loader”. They will be writing some custom programs to store the data in directories. They will be writing the programs in such a way that, system will pick up the data from the staging tables.
If you run the program then data will flow into Oracle Apps.
Before that Functional consultant has to set up the pre requisites like Customer and Supplier Accounts.
To upload the assets data we use “Web ADI” process. For this we do not need to create staging tables for data storing. Validation also not required.
There will be cut off date for data migration.
Information which we migrate: Supplier header, Supplier site, Supplier contact information. Customer header, Open transactions.
Implementation steps
### 14. End user training:
Training to end users
### 15. Go live:
After migrating data into production instance, customer start using the Oracle apps, this activity is called as Go Live. This instance is called Prod instance.
### 16. Parallel Run:
Customer will enter the data in the both the applications in Legacy and Oracle Apps. This process is required until the Oracle instance get stabilized.
### 17. Post implementation Support :
Once the implementation completed, after go live, customer may request to provide support for some time.
<img width="892" height="2881" alt="image" src="https://github.com/user-attachments/assets/76256ded-9227-4c42-942b-d324629bd10e" />
