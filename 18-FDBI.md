1. Download Spreadhsheet from Oracle					
2. Fill the data & Validate the Data					
3. Convert the spreadsheet into CSV and .Zip file					
4. Save file in UCM Server	UCM: Universal Content Manager				ADFDI
5. Run Load Interface file for import	Push to Interface Tables				
6.  run Item Import/ Supplier Import/Sales Order Import/etc	Push to Base Tables				ADFDI usually download from particular UI
order import					like manage location, etc
					"once we download the ADFDI, 
we can fill or edit and we can publish or submit the data"
					application
					
Open Data	FBDI	ADFDI	VB Add-In		
On-hand (Inventory Transactions Template)	Yes	No			
Sales Orders(SourceSalesOrderImportTemplate)	Yes	No			
Requisitions(RequisitionImportTemplate)	Yes	No			
Purchase Orders(POPurchaseOrderImportTemplate)	Yes	No			
Blanket Purchase Agreement(POBlanketPurchaseAgreementImportTemplate)	Yes	No			
Purchase Orders Schedules Close	No	Yes	Yes		
Item Import	Yes				
Supplier Master	Yes				
					
					
					
Supplier Master					
Oracle has provided the FBDI tool to import suppliers from External Source to the Oracle fusion. Supplier Import in Oracle fusion we first need to Download the Supplier Import FDBI templates given by the Oracle fusion to import suppliers. Oracle has given 7 Different FBDI templates to Import supplier in Fusion					
					
1. Suppliers Import Template					
2. Suppliers Address Import Template	supplier banks				
3. Suppliers Site Import Template	supplier item category				
4. Suppliers Site Assignment Template					
5. Supplier Contacts Template					
6. Supplier banks and bank branches template					
   Steps to Import Suppliers Data into oracle Application:					
1. Download FBDI template (Suppliers Import Template) from Oracle Enterprise Repository with the same version as per your application version.					
2. Populate the data in POZ_SUP_INT  sheet of template					
<img width="1752" height="1045" alt="image" src="https://github.com/user-attachments/assets/b52eb02a-b357-4c4d-b509-3d5908566565" />
