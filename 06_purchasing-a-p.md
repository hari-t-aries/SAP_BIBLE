6/8/26, 6:05 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:05:45 GMT+0000
SAP Business One | 10.0
Public
Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/68a2e87fb29941b5bf959a184d9c6727?locale=en-
US&state=PRODUCTION&version=10.0
Warning
This document has been generated from SAP Help Portal and is an incomplete version of the official SAP product documentation.
The information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be
missing important aspects and/or correlations to other topics. For this reason, it is not for production use.
For more information, please visit https://help.sap.com/docs/disclaimer.
This is custom documentation. For more information, please visit SAP Help Portal. 1

6/8/26, 6:05 AM
Purchasing - A/P
SAP Business One enables you to manage the entire purchasing process from purchase orders through processing A/P invoices.
Furthermore, you can create various reports to analyze purchasing information such as purchase volume analysis, pricing
information, vendor liabilities aging, and so on.
You can base one purchasing document on another and thus copy all relevant data into the new document. For example, you can
start with the purchase order and base the goods receipt PO on that purchase order. You then proceed to the A/P invoice and base
it on the goods receipt PO.
Since you create a contractual relationship with the vendor, with the exception of the purchase order, all purchasing documents
are legally binding documents. The purchase order is intended, first and foremost, purely as an informational source in SAP
Business One.
 Note
If you have created a purchasing document with reference to an existing purchasing document, you can use the Base
Document option to call up these documents. Position the cursor on the appropriate row and from the menu bar choose Go
To Base Document .
If you have created the follow-up documents with reference to the current purchasing document, you can call up these
documents with the Target Document function. Position the cursor on the appropriate row and from the menu bar choose Go
To Target Document . If more than one target document exists, SAP Business One displays the last target document.
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Transaction Processing
Please note that image maps are not interactive in PDF outputs.
Report Management
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:05 AM
Please note that image maps are not interactive in PDF outputs.
Other Functions
Please note that image maps are not interactive in PDF outputs.
Purchasing Process in SAP Business One
The Purchasing module in SAP Business One:
Describes the documents and functions used in the purchasing process
Follows the changes in inventory during the purchasing process
Process
Please note that image maps are not interactive in PDF outputs.
Additional Purchasing Process Documents
Please note that image maps are not interactive in PDF outputs.
You can create a new document based on one or more of the existing ones. When you create a new document with reference to an
existing document, only the documents that are still open are displayed. All documents for which you have not created a follow-on
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:05 AM
document have an open status. Open documents remain open until you transfer all items completely to the follow-on document,
or until you manually close or reverse them.
Different Operations in Purchasing Process Documents
Please note that image maps are not interactive in PDF outputs.
More Information
Purchasing – A/P
Creating Purchase Requests
Context
The purchase request enables users and employees in the organization to initiate a purchasing process by submitting their needs
for certain goods or services. The purchase request can then be copied to purchase quotation or purchase order for further
processing.
Procedure
1. From SAP Business One Main Menu choose: Purchasing – A/P Purchase Request . In the Purchase Request window,
specify the following details:
Requester — specify whether the initiator of the request is a user in SAP Business One or an employee in the
company and then specify the respective user or employee name. By default, the current user appears in this field.
Requester Name, Branch, Department, E-Mail — populated automatically based on the specified requester. If the
requester is a user, the information in these field is drawn from the respective fields in Users – Setup window in
Administration Setup General Users If the requester is an employee, the information is drawn from the
respective employee master data record in Human Resources Employee Master Data . You can change the
details in these fields for the given purchase request.
Send E-Mail if PO or GRPO is Added — Select this checkbox to send an e-mail to the requester once a purchase
order or goods receipt PO is created based on the given purchase request. When this checkbox selected, the E-Mail
field is mandatory.
The default setting of the checkbox is determined by the settings of the Send E-Mail When PO or Goods Receipt PO
is Created checkbox in Administration System Initialization Document Settings Per Document tab
Purchase Request .
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:05 AM
2. Select the required numbering series, and set the relevant dates in the Posting Date, Valid Until, Document Date, and
Required Date fields. By default, the Posting Date is set to the current date, and the Valid Until date is set to one month
later.
3. (Optional) Specify the reference documents of the purchase request:
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the
current document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
a. Go to the Document Referenced To tab of Document A1.
b. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For
example, journal entries, landed costs and incoming payments are unavailable here.
c. In the Doc. Number field, specify the document number B1.
d. Choose Update.
e. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on
the Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and
duplicate documents? If you confirm the message, the original document is automatically set as a referenced
document. You can view the reference relationship through both the Reference Information window and the relationship
map.
If you duplicate any document with existing document references, the document references are automatically copied from
the original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main
Menu Administration System Initialization Document Settings General tab, and deselect the checkbox Copy
Document References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which
they are created.
4. In the Contents tab, in the Item/Service Type dropdown list, specify whether the purchase request if for items or service. If
the purchase request is for items, specify in the Summary Type field whether to summarize the document by items.
5. Choose the required items or fill in the details of the required services. The field Required Date is mandatory in each line. If
the purchase request is for items, you must enter the required quantity.
6. In the Attachments tab, you can browse and attach documents and files related to the purchase request. If needed, use the
Display and Delete buttons, to view and delete attachments.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:05 AM
7. If needed, specify the owner of the document and enter any relevant remarks.
8. Choose one of the following options:
Add & New
Adds the document and opens a new window for you to create another document.
It is similar to the previous Add button.
Add & View
Adds the document and displays it.
Add & Close
Adds the document and closes the window.
Your last choice will be remembered the next time you open the window of the given document.
Requesting Quotations
Context
In purchasing, you try to find the best offer for goods or services that you require. To do so, you send a purchase invitation to a
number of vendors to indicate their terms and conditions, such as price or delivery date for the supply of materials or provision of
service, by submitting a quotation.
In this purchase quotation, the material or service details, for example, quantity, required date and vendor information, are
specified. You compare the quotations received and determine the vendor that you want to order from.
Working with quotations typically involves the steps outlined below.
Procedure
1. Create purchase quotations.
For more information, see Creating Purchase Quotations.
2. Send quotations to vendors.
3. Record vendors’ answers in purchase quotations.
For more information, see Recording Vendor Replies.
4. Compare quotations to determine the best offer and create a purchase order.
For more information, see Comparing Purchase Quotations.
5. Close related purchase quotations.
For more information, see Closing, Cancelling and Removing Purchase Quotations.
Creating Purchase Quotations
Procedure
There are several ways to create purchase quotations, as described below.
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:05 AM
Creating a Single Purchase Quotation Manually
1. From the SAP Business One Main Menu, choose Purchasing – A/P Purchase Quotation .
The Purchase Quotation window appears.
2. In the general area, specify the vendor code of the vendor from whom a quotation is requested, the expiry date of the
purchase quotation, and the date by which the goods or services are required.
The date entered in the Required Date field is the default value for the required date in the item lines of the table on the
Contents tab.
The Group No. field displays the group number for all items in the same purchase quotation. The number is generated
automatically according to the numbering series defined for Purchase Quotation Group in the Document Numbering -
Setup window.
3. On the Contents tab, enter the following data:
Field Description
Item/Service Type Choose one of the following options:
Item – to create a purchasing document for items
defined in the Inventory module.
Service – to create a purchasing document for a
service, such as a one-time consultation, that has not
been defined as an item in SAP Business One.
The table view on this tab is different for each option.
Item No. Item number of the goods to be procured.
Required Date Date by which the items should be delivered. By default, the
date you specified in the header area of the document is
entered. You can change this date, if required.
Required Qty Number of the items to be procured.
4. On the Logistics tab, enter the shipping and billing information.
5. On the Accounting tab, specify the relevant information.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the
current document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
a. Go to the Document Referenced To tab of Document A1.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:05 AM
b. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For
example, journal entries, landed costs and incoming payments are unavailable here.
c. In the Doc. Number field, specify the document number B1.
d. Choose Update.
e. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on
the Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and
duplicate documents? If you confirm the message, the original document is automatically set as a referenced
document. You can view the reference relationship through both the Reference Information window and the relationship
map.
If you duplicate any document with existing document references, the document references are automatically copied from
the original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main
Menu Administration System Initialization Document Settings General tab, and deselect the checkbox Copy
Document References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which
they are created.
6. To save the document, choose one of the following options:
Add & New
Adds the document and opens a new window for you to create another document.
It is similar to the previous Add button.
Add & View
Adds the document and displays it.
Add & Close
Adds the document and closes the window.
Your last choice will be remembered the next time you open the window of the given document.
In the following scenarios, a system message will appear asking if you want to change the Group No. for the purchase
quotation to the next sequential number in the predefined series:
You and other users add purchase quotations in parallel.
You create a purchase quotation from a draft with a group number which is already used in another purchase
quotation.
Creating Several Purchase Quotation Documents at the Same Time
1. From the SAP Business One Main Menu, choose Purchasing – A/P Purchase Quotation Generation Wizard .
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:05 AM
The Purchase Quotation Generation Wizard window appears.
2. In the introductory window, choose Next.
3. In the Document Generation Options window, select whether to create a new set of parameters for document generation
or to use an existing one. In either case, specify a parameter set name and choose Next.
4. In the Select Items window, enter the following data and choose Next:
Field Description
Item No. Item number of the goods to be procured.
Required Date Date by which the items should be delivered.
Required Quantity Number of the items to be procured.
Unit of Measure Unit of measurement defined for the item.
Free Text Enter any additional information, if required.
The Select Purchase Quotation Line Items window appears. You see the preferred vendors that are associated with the
items you intend to purchase. You can choose to group the list by business partner or by item.
 Recommendation
Requesting a quotation from more than one vendor is possible by defining each vendor as a preferred vendor in the item
master data, for the goods to be procured. It is possible for multiple vendors to be defined as preferred vendor for an
item.
 Note
For selecting Preferred Vendors go to: Purchase Quotation Generation Wizard step 3 or Procurement Confirmation
Wizard step 3 right-click on the Vendor name Select List of Preferred Vendors
5. If there is no preferred vendor for an item, specify a vendor in the Vendor Code column.
6. Optional: To create the purchase quotations as drafts for later editing, select the Create Draft Doc. checkbox.
7. To proceed, select the lines requested to be included in a purchase quotation and choose Next.
In the Preview Results window, the vendors that receive a request for a quotation and the related items are presented.
8. To change any previous data, choose Back and make your changes in the previous windows.
To save your parameters and execute the wizard, choose Next.
9. In the Save and Execute Options window, specify which tasks the wizard should carry out and choose Next:
Execute
Creates one purchase quotation per vendor according to the parameters defined.
Save Parameter Set and Execute
Saves the parameters defined and creates one purchase quotation per vendor.
Save Parameter Set and Exit
Saves the parameters defined and closes the wizard without creating any documents.
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:05 AM
If you choose to execute or save and execute the wizard, select which action to take if an error occurs, for example, skip to
the next vendor or stop the document creation process.
If you choose to execute or save and execute the wizard, the application displays a system message.
10. To proceed, confirm the system message.
The Summary Report window displays which documents were created and any errors that occurred. The documents that
were created share the same group number.
11. To exit the wizard, choose Close.
Creating a Purchase Quotation from a Sales Order
1. Create a sales order and enter the relevant customer and item information.
2. On the Logistics tab, select the Procurement Document checkbox.
3. To save the sales order, choose Add.
The procurement confirmation wizard appears. In the Customer window, the customer for whom you created the sales
order is preselected.
Optional: If you want to create purchase quotations for additional sales orders, you can add customers to the list by
choosing Add and selecting the relevant customers.
4. To proceed, choose Next.
5. In the Sales Orders window, select one or several sales orders that contain the items for which you want to obtain a
purchase quotation, and choose Next.
6. In the Select Order Line Items window, choose purchase quotation as a target document.
If preferred vendors have been defined for an item on the Purchasing Data tab of the item master data, all preferred
vendors are displayed in the table. If no preferred vendors have been defined, you must specify a vendor in this step to be
able to proceed or deselect the item line.
You can deselect any lines that you do not want to create a purchase quotation for. In addition, you can change the vendor
code, vendor name and item quantities. However, you must change the quantity for each vendor individually.
7. Optional: To create the purchase quotations as drafts and edit them later, select theCreate Draft Doc. checkbox.
8. To proceed, choose Next.
The Purchase Quotations window displays which vendor will receive a request for quotation for which items. You can
deselect any lines that you do not want to create a purchase quotation for.
9. Choose Next.
10. In the Consolidations window, specify the system response to errors that may occur in the document generation process.
To do so, make a selection in the If an Error Occurs field and choose Next.
The purchase quotations are consolidated by vendor.
The Preview Results window appears. It displays all purchase quotations that will be created, grouped by vendor and the
consolidations options you selected.
11. To generate the documents, choose Next.
The application creates the relevant documents and displays a summary report of all documents that were created and any
errors that occurred.
Creating a Purchase Quotation from Item Master Data
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:05 AM
1. Open the item master data record of the item for which you want to obtain a quotation.
2. From the menu bar, choose Go-to Create Purchase Quotation .
The Select Items window of the purchase quotation generation wizard appears.
3. In this window, enter the required quantity and date of the item. If required, add other items to the list and choose Next.
4. In the Select Order Line Items window, choose purchase quotation as a target document and select the vendor from whom
you want to obtain the purchase quotation.
If a preferred vendor has been defined for an item in the item master data, the preferred vendor is entered as a default for
the item. You can change this data, if required.
5. Optional: To create the purchase quotations as drafts and edit them later, choose Create Draft Document.
6. To proceed, select the lines that you want to include in a purchase quotation and choose Next.
The Preview Results window appears.
7. To change any of the data, choose Back and make your changes in the previous windows.
To save your parameters and execute the wizard, choose Next.
The Save & Execute Options window appears.
8. In this window, specify which tasks the wizard should carry out and choose Next:
Execute
Creates one purchase quotation per vendor, according to the parameters you defined.
Save Parameter Set and Execute
Saves the parameters you defined and creates one purchase quotation per vendor.
Save Parameter Set and Exit
Saves the parameters you defined and closes the wizard without creating any documents.
If you choose to execute or save and execute the wizard, select which action to take if an error occurs, for example, skip to
the next vendor or stop the document creation process.
If you choose to execute or save and execute the wizard, the application displays a system message.
9. To proceed, confirm the system message.
The Summary Report window displays which documents were created and any errors that occurred.
10. To exit the wizard, choose Close.
11. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field, and choose Next.
The Preview Results window appears. It displays all purchase quotations that will be created grouped by vendor and the
consolidations options you selected.
12. To generate the documents, choose Next.
The application creates the relevant documents and displays a summary report of all documents that were created and any
errors that occurred.
Result
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:05 AM
You created one or several purchase quotations, in which you specified the details of the items or services you require. You can now
send these purchase quotations to the individual vendors by e-mail, fax, or mail.
More Information
Requesting Quotations
Recording Vendor Replies
Prerequisites
You have created one or several purchase quotation documents for your planned purchase.
You have sent the purchase quotation documents to the vendor(s).
You have received replies from the vendors detailing the conditions of their offers.
Procedure
1. Choose Purchasing – A/P Purchase Quotation and open the relevant document.
2. Enter the information provided by the vendor and fill in the following fields:
Field Description
Quoted Date Date by which the vendor claims to deliver the goods included
in the purchase quotation.
Quoted Qty Number of goods that the vendor can deliver at the conditions
quoted.
Unit Price Price per unit at which the vendor intends to sell the item.
3. To close the document, choose Update and OK.
Result
You can use the updated purchase quotation documents to compare the offers and find the best deal for your requirements. For
more information, see Comparing Purchase Quotations.
More Information
Requesting Quotations
Comparing Purchase Quotations
By running this report, you make available a comparison of quotations received from vendors, letting you find the best offer for
procurement. The report highlights the favorable parameters, such as the earliest quoted date or the lowest price. In addition, you
can turn any purchase quotation into a purchase order directly from the report.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:05 AM
Prerequisites
Replies from the vendors detailing the conditions of their offers have been received.
The vendors' details are recorded in the purchase quotations of the application.
Procedure
1. To begin the comparison, do one of the following:
Choose Purchasing Purchase Quotation , open the relevant document, right-click, and choose Comparison
Report.
Choose Inventory Item Master Data , open the relevant item master data, right-click, and choose Comparison
Report.
Choose Reports Purchase Quotation Comparison Report .
In the Purchase Confirmation Comparison report, specify the selection criteria and choose OK.
The Quotation Comparison window appears.
The report displays the price and quantity quoted by the vendor, as well as the promised delivery date. Below are
explanations of several fields and elements in the window:
Field Description
PQ No. The number of the purchase quotation.
Group No. Number of the purchase quotation group. That is, all items that
are contained in one purchase quotation share the same group
number.
Unit Price Price of the item as quoted by the vendor.
Unit Price (LC) Price of the item in local currency as quoted by the vendor.
Required Date Date by which you need the items.
Quoted Date Date by which the vendor agrees deliver the items.
Required Quantity Number of items to be procured.
Quoted Quantity Number of items the vendor promises to deliver.
Status Purchase quotations can have one of the following statuses:
open, closed or canceled.
Create Purchase Order Creates a purchase order for the vendor and the items you
selected.
The results are sorted according to the unit price (LC) in ascending order, and then according to the quoted date in
ascending order within a group. The lowest unit price, the earliest quoted date and the closest quoted quantity to the
required one are highlighted in red.
It is possible to change the sorting as required.
2. To accept one or several of the quotations and order the goods, select the relevant line items and choose Create Purchase
Order.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:05 AM
More Information
Requesting Quotations
Closing, Canceling, and Removing Purchase Quotations
Task Business Scenario Procedure
Closing purchase quotations When you have decided on a winning
1. Open the relevant purchase
vendor for your procurement, you close all
quotation.
purchase quotations that are not turned
into purchase orders.
2. From the upper menu bar, in the
main window, choose Data
Close .
Canceling purchase quotations You cancel a purchase quotation if you have
1. Open the relevant purchase
created it by mistake or if it has become
quotation.
invalid.
2. From the upper menu bar, in the
main window, choose Data
Cancel .
Removing purchase quotations You remove a purchase quotation if the
1. Open the relevant purchase
canceled or closed document is no longer
quotation.
needed for reference purposes.
2. From the upper menu bar, in the
main window, choose Data
Remove .
More Information
Requesting Quotations
Purchase Order
The purchase order is a document used to request items or services from a vendor at an agreed upon price.
When you enter a purchase order in SAP Business One, no value-based changes are posted in the accounting system. However, the
order quantities are listed in inventory management. You can view the ordered quantities in various reports and windows, such as
the Inventory Status report and the Item Master Data window. This information is important for optimizing ordering transactions
and stockholding.
To open the window, choose Purchasing – A/P Purchase Order .
More Information
Creating Purchasing Documents
Purchase Order: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:05 AM
Purchase Order: Accounting Tab
Purchasing Documents: Contents Tab
Purchase Order: Logistics Tab
Purchase Order: General Area
Use this area to enter general information relevant to all items in the document.
To access this area, choose Purchasing – A/P Purchase Order .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Purchase Order General Area Fields
Contact Person
The name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
The vendor reference number, if available.
No.
Field on the left: name of the numbering series.
Specify a series.
Next field: purchase order number.
Field on the right: the additional purchase order number, if defined. If you choose the manual series, enter the document number.
Status
The status of the purchase order:
Open
You can draw the document completely or partially to a higher level document.
Open: Printed
You printed the document and left it open.
Open: E-Mailed
You sent the document to business partners through SAP Business One Mailer and/or Microsoft Outlook and left the
document open.
A document is considered as sent by SAP Business One Mailer if the e-mail is marked as on the Sent Messages tab in
the Messages/Alerts Overview window. With Microsoft Outlook, a document is considered as sent when Microsoft Outlook
opens.
Open: Printed and E-Mailed
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:05 AM
You printed and e-mailed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually, or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
Not Confirmed
The document is not yet confirmed, thus cannot be copied to other documents.
Posting Date
Specify the posting date.
The default value for this field is the current date on which the purchase order is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Delivery Date
Specify the date on which you want to receive the items.
Document Date
The document date of the purchase order, used for tax purposes. The default value is the current date.
Currency
Specify the display currency for the amounts in the document.
For business partners with All currency, you are able to change the currency as long as the purchase order is open and no rows are
drawn.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
Buyer
Specify the buyer who initiated the purchase order.
Owner
Specify the employee who owns the purchase order.
Remarks
Enter additional text information regarding the purchase order. You can also edit the field content after the document is added.
Total Before Discount
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:05 AM
The total amount of the purchase order before the discount for the document is calculated.
 Note
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of the discount for the whole purchase order.
The field on the right displays the amount of the discount.
Freight
This field only appears if Manage Freight in Documents is selected in Administration System Initialization Document
Settings General .
You can define freight for the purchase order. To open the Freight Charges window and to view the corresponding freight, click .
Rounding
This field appears if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
The tax amount for the purchase order calculated according to the tax definitions.
Total Payment Due
The total amount of the purchase order including tax, freight, and discounts.
More Information
Purchase Order
Data Ownership Authorizations Window
Freight Charges Window
This window displays the freight defined in the Freight - Setup window. It enables you to make changes that are relevant for the
current sales or purchasing document.
To access the window, choose Sales – A/R or Purchasing - A/P and open any document. Click in the Freight field.
 Note
This window appears only if you have selected Manage Freight in Documents on the General tab of the Document Settings
window Administration System Initialization Document Settings ).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:05 AM
Freight Charges Window
Do Not Display Freight Charges with Zero Amount
Hides freight with zero amount.
Tax Code
Tax code related to the freight.
 Note
In European localizations, this field is labeled Tax Group.
Total Tax Amount
Total tax amount of the freight.
Externally Calculated Tax Rate
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays the externally calculated tax rate edited through the DI API or Service Layer.
 Note
This value is for informative purposes only and is not used in any system calculations.
Externally Calculated Tax Amount
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays the externally calculated tax amount edited through the DI API or Service Layer.
Source of Tax Amount
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays whether the tax amount is an internal system calculation or external calculation (edited through the DI API or Service
Layer).
Distrib. Method
Distribution method defined for freight in the Freight - Setup window.
Any changes you make are relevant for the current document only and do not affect the original definition.
Net Amount
Freight amount excludes tax.
When the Gross Freight checkbox is unselected in the Freight – Setup window, the default value of this field is the amount
specified in the Fixed Amount field in the Freight – Setup window.
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:05 AM
When you update the value in the this field, the value in the Gross Amount field is updated automatically according to the
predefined tax group.
Any changes you make are relevant for the current document only and do not affect the original definition of the freight.
Status
Displays one of the following:
O – Open. Freight charge status when document is open, for example, not drawn to another document or closed manually.
C – Closed. Freight charge status when the document was drawn to a target document or closed manually.
Gross Amount
Freight amount includes tax.
When the Gross Freight checkbox is selected in the Freight – Setup window, the default value of this field is the amount specified
in the Fixed Amount field in the Freight – Setup window.
When you update the value in this field, the value in the Net Amount field is updated automatically according to the predefined tax
group.
Any changes you make are relevant for the current document only and do not affect the original definition of the freight.
Project
Specify the project that you want to relate to the freight. If you defined the project for the freight in the Freight-Setup window, the
field displays the project code by default.
More Information
Freight - Setup Window
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:05 AM
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:05 AM
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:05 AM
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:05 AM
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:05 AM
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:05 AM
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:05 AM
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:05 AM
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:05 AM
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
Purchase Order: Logistics Tab
This tab contains details regarding the logistics aspects of a purchase order.
To access the tab, choose Purchasing – A/P Purchase Order Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Purchase Order Logistics Tab Fields
Ship to
Purchase orders of type Item: address defined for the warehouse linked to the Contents tab.
Purchase orders of type Service: company address as defined in Administration System Initialization Company Details
General Local Language .
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:05 AM
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the Business Partner Master Data window.
This field appears only if the option Multi-Language Support is selected in Administration System Initialization Company
Details Basic Initialization .
If you specify another language, it is applied to this document only.
Split Purchase Order
Enables you to divide purchase orders that involve more than one warehouse.
Confirmed
Indicates that the purchase order is confirmed and enables copying it to a higher level of purchase document.
This checkbox is selected by default if the checkbox Confirm Purchase Order Automatically in the Administration System
Initialization Document Settings Per Document tab is selected.
More Information
Purchase Order
Purchase Order: Accounting Tab
This tab contains information regarding the financial aspect of a purchase order.
To access the tab, choose Purchasing – A/P Purchase Order Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Purchase Order Accounting Tab Fields
Journal Remark
By default, displays Purchase Orders – XXX, where XXX is the vendor code.
Change this content, if required. If you manage perpetual inventory, enter the journal entry.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the purchase order. This control account can then be copied to any follow-up documents.
 Note
It appears only if the checkbox Allow Control Account Selection is selected in Administration System Initialization
Document Settings Per Document for purchase orders.
Payment Terms
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:05 AM
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
[ ]
Specify when you initiate the payment:
Month End
Half Month
Month Start
+Months...+Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be
entered for the current month or for several months in the future, as well as for the number of days you specify in the last month of
the period.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Cancellation Date
Specify the date after which the purchase order is cancelled, and the company is not committed to the vendor.
Required Date
An informative field to indicate the date on which the goods should leave the vendor's site, in order to arrive at the company's site
by the Delivery date.
Indicator
Indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID, if defined in the company details: Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to the head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:05 AM
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Purchase Order
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:05 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Updating Purchase Orders
Prerequisites
No higher level documents have been created with reference to the purchase order.
Context
After you have added a purchase order, you can change all the data in it, for example:
Delete, add, or duplicate rows
Update prices and discounts
Update quantities
Procedure
1. From the SAP Business One Main Menu, choose Purchasing - A/P Purchase Order .
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:05 AM
2. Change the required data.
3. Choose Update.
Related Information
Purchase Order
Canceling Purchase Orders
Prerequisites
The purchasing process is complete.
The purchase order has not yet been drawn (fully or partially) to a higher level purchasing document, such as a goods
receipt PO or A/P invoice.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Purchase Order , and find the relevant purchase order.
2. In the menu bar, choose Data Cancel .
Result
The status of the purchase order changes to Canceled. The purchase order itself is not deleted. You can still display and duplicate
it, but you cannot change it or draw it to a higher level purchasing document.
More Information
Purchase Order
Closing Purchase Orders
Closing Purchase Orders
Prerequisites
The purchase order has been partially drawn to a higher level purchasing document.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Purchase Order and find the relevant purchase
order.
2. In the menu bar, choose Data Close .
Results
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:05 AM
The status of the purchase order changes to Closed. The purchase order itself is not deleted. You can still display and duplicate it,
but you cannot change it or draw it to a higher level purchasing document.
Related Information
Purchase Order
Canceling Purchase Orders
Goods Receipt PO
You create this document when you receive goods from the vendor.
When you create a goods receipt PO, SAP Business One receives the goods into the warehouse, updates the quantities, and
creates an accounting journal entry if you manage the perpetual inventory.
To access the window, choose Purchasing – A/P Goods Receipt PO .
More Information
Creating Purchasing Documents
Goods Receipt PO: General Area
Purchasing Documents: Contents Tab
Goods Receipt PO: Logistics Tab
Goods Receipt PO: Accounting Tab
Closing Goods Receipt PO
Goods Receipt PO: General Area
Use this area of the goods receipt PO to enter general information relevant to all items in the document.
To access this area, choose Purchasing – A/P Goods Receipt PO .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Receipt PO General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Vendor reference number, if available.
No.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:05 AM
Field on the left: name of the numbering series.
Specify a series.
Next field: goods receipt PO number.
Field on the right: additional goods receipt PO number, if defined. If you choose the manual series, enter the relevant number.
Status
Status of the goods receipt PO:
Open
You can draw the document completely or partially to a higher level document.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually, or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
Posting Date
Specify the posting date.
The default value for this field is the current date on which the goods receipt PO is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Specify the date on which you want to receive the items.
Document Date
Document date of the goods receipt PO used for tax purposes. The default value is the current date.
Currency
Specify the display currency for the amounts in the goods receipt PO.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
Buyer
Specify the buyer who initiated the goods receipt PO.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:05 AM
Owner
Specify the employee who owns the goods receipt PO.
Total Before Discount
Total amount of the goods receipt PO before the discount for the document is calculated.
 Note
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of the discount for the whole goods receipt PO.
The field on the right displays the amount of the discount.
Freight
This field appears only if Manage Freight in Documents is selected in Administration System Initialization Document
Settings General .
You can define freight for the goods receipt PO. To open the Freight Charges window and to view the corresponding freight, click
.
Rounding
This field appears only if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the goods receipt PO calculated according to the tax definitions.
Total Payment Due
Total amount of the goods receipt PO including tax, freight, and discounts.
More Information
Goods Receipt PO
Document Settings: General Tab
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:05 AM
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:05 AM
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:05 AM
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:05 AM
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:05 AM
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:05 AM
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:05 AM
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:05 AM
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
Goods Receipt PO: Logistics Tab
This tab contains details regarding the logistics aspects of a goods receipt PO.
To access the tab, choose Purchasing – A/P Goods Receipt PO Logistics .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Receipt PO Logistics Tab Fields
Ship to
Goods receipt PO of type Item: address defined for the warehouse linked to the Contents tab.
Goods receipt PO of type Service: company address as defined in Administration System Initialization Company Details
General Local Language .
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
 Note
Choose the ellipsis (...) button to access the GLN in the Address Component window.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner.
More Information
Goods Receipt PO
Goods Receipt PO: Accounting Tab
This tab contains information regarding the financial aspect of the goods receipt PO.
To access the tab, choose Purchasing – A/P Goods Receipt PO Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Receipt PO Accounting Tab Fields
Journal Remark
By default, displays Goods Receipt POs – XXX, where XXX is the vendor code. If required, change this content.
Control Account
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:05 AM
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the goods receipt PO. This control account can then be copied to any follow-up documents.
 Note
It appears only if the checkbox Allow Control Account Selection is selected in Administration System Initialization
Document Settings Per Document for goods receipt POs.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Start From
Specify when you initiate the payment:
Month End
Half Month
Month Start
+Months... + Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be given
for the current month or for several months in the future, as well as for the number of days you specify in the last month of the
period.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
Indicator
Indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID, if defined in the company details: Administration System Initialization Company Details
Accounting Data .
Order Number
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:05 AM
Specify the order number of the chain, when you use the direct distribution method. This number is recorded in the file that you
send to the head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Goods Receipt PO
Closing Goods Receipt POs
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:05 AM
Prerequisites
The goods receipt PO has not yet been copied to an A/P invoice or a goods return.
Context
When you close a goods receipt PO, no adjustment posting is carried out in inventory management. This means that the available
inventory, which has been increased by the goods receipt PO, will not be reduced again.
Therefore, if you need to close a goods receipt PO and have the inventory values and quantities updated as well, create a goods
return based on the goods receipt PO to be closed.
 Note
After you have closed a goods receipt PO, you can no longer base other purchasing documents on that goods receipt PO.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Goods Receipt PO and select the relevant
document.
2. In the menu bar, choose Data Close .
You receive a message:
Closing a document is irreversible. Document status will be changed to “Closed” and a
clearing transaction will be created. Do you want to continue?
3. Do one of the following:
To proceed and close the goods receipt PO, choose the Yes button.
 Note
If you are running a non-perpetual inventory company, the goods receipt PO is closed and the document status
is changed to Closed.
If you are running a perpetual inventory company, proceed to step 4 to specify the posting date for the clearing
journal entry.
To cancel the operation, choose the No button.
4. If you confirm that you want to close the goods receipt PO, a dialogue box appears asking you to specify a posting date to
be used in the clearing journal entry. Do one of the following:
To use the current system date, select the Current System Date radio button.
To use the original posting date in the document, select the Original Document Date radio button.
To specify a date other than the above two dates, select the Specified Date radio button, and then either enter a
date or choose a date from the calendar.
If you specify a date that is earlier than or the same as the original posting date of this document, you receive the
message: Enter a specified date that is later than original document posting date.
If you specify a date that is in a locked period, you receive the message: Period is locked for new data.
For more information, see Locking Posting Periods.
5. To save the data, choose the OK button.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:05 AM
When a goods receipt PO (either fully or partially drawn) is closed, the amount of Freight posted to the expense account
and not drawn into an A/P invoice or a goods return is cleared.
Related Information
Goods Receipt PO
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:05 AM
Down Payments
Businesses require down payments from customers to ensure that the customers are committed and will follow through with the
orders they place.
In SAP Business One, you can map this business practice by issuing an A/R down payment request or A/R down payment invoice
to your customer, or by creating an A/P down payment request or A/P down payment invoice, if one of your vendors requires you
to make a down payment before shipping the goods you ordered. After you receive payment from your customer or make the
payment to your vendor, you can deduct the down payment amount from the final invoice.
Please note that image maps are not interactive in PDF outputs.
Down Payment Request Process
A customer ordered some goods from your company. Since you are not sure about the customer's commitment, you request a
payment advance from the customer by issuing a down payment request. You also use this document as a basis for other key
steps in the sales process, for example, creating the final invoice.
 Note
In various localizations there might be few differences in this functionality. For complete information refer to the localized
online help file provided with SAP Business One by choosing: Help Document Localization Specific Info
Process
1. Create an A/R or A/P down payment request for the relevant business partner. If you do this by drawing a base document,
verify that you have defined the required down payment percentage. For more information, see A/R Down Payment
Documents: General Area or A/P Down Payment Request: General Area.
No posting is made at this stage.
2. Once the actual payment for the down payment request is made, create the proper payment document based on the down
payment request. A down payment request can be paid in full or in parts.
 Note
You can use the payment wizard to pay the down payment request.
After you create the payment document, a journal entry is recorded in the down payment accounts. If the down payment
request was paid fully, the down payment request is closed. If it was only paid partially, it remains open for another
payment. You can edit a down payment document that was only partially paid, provided that no rounding amount was
specified on the document.
If only part of the down payment request was paid and you do not expect further payments on it, you can close the request
by choosing Data Close . This closes the down payment request document and you are not able to record payment of
the outstanding amount in the future for the closed down payment request.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:05 AM
3. Create a regular invoice. You can copy the data from the base document drawn into the down payment request, for example
a sales order, since it was not closed as a result of the drawing into the down payment request.
To link the down payment request to the invoice, choose , select the relevant document, and specify the net or gross
amount to be copied into the regular invoice.
You can specify a higher amount in the down payment request than in the invoice. This means that the total amount of the
invoice will then be negative.
 Note
You can link a down payment request to an invoice only when you create the invoice. You cannot do this at a later stage,
for example, when recording the payment in the Banking module or during internal reconciliation.
After you add the invoice, SAP Business One creates the regular postings.
4. If there is still an outstanding balance due on the regular invoice after linking the down payment request to the invoice, you
can create a payment. The table of the payment documents displays the invoice. Select the required document and
continue to process the payment.
More Information
A/R Down Payment Request
A/P Down Payment Request
A/P Down Payment Request
An A/P down payment request is a request by your vendor that a down payment be made at a certain time.
This document does not generate any accounting or inventory posting, so if you create an A/P down payment request based on a
purchase order or a goods receipt PO, the base document is not closed. This lets you copy the same base document to a higher
level purchasing document, such as an A/P invoice or a goods receipt PO.
To access the window, choose Purchasing - A/P A/P Down Payment Request .
 Note
When a down payment request is included in a payment order run, you cannot cancel or close it.
Related Information
Down Payments
Down Payment Request Process
A/P Down Payment Request: General Area
A/P Down Payment Request: General Area
Use this area of the purchasing document to enter general information relevant for all items in the document.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Down Payment General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Specify the vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the A/P down payment document. If you choose the manual series, enter the relevant number.
Status
Status of the A/P down payment document:
Open
Down payment request: You can draw the document completely or partially to a higher-level document.
 Recommendation
A down payment request can be paid partially, but the down payment request document should be closed before linking
it to the final invoice.
Down payment invoice: You can draw the document completely or partially to a higher-level document. The down payment
invoice can be paid partially, but drawn into an invoice.
Open – Printed
You printed the document and left it open.
Canceled
You canceled the document manually.
Closed
Down payment request: The document was paid and thus closed, or closed manually.
Down payment invoice: The document was paid and thus closed.
Draft
The document is still a draft.
Posting Date
Specify the posting date. The default value is the date on which the A/P down payment document is created. If required, change
the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:05 AM
Expected due date of the payment of the down payment. The default date is 30 days after the posting date.
To change it, choose a different payment term in the Payment Terms field, or enter a date manually.
Currency
Specify the display currency for the amounts in the A/P down payment document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Buyer
Specify the buyer who initiated the purchasing document.
Owner
Specify the employee who owns the document.
Remarks
Enter additional information regarding the document.
Total Before Discount
Total amount of the document before the discount for the document is calculated.
Base Discount %
Percentage and amount of the discount from the base document, and they are separated from those of the down payment.
 Note
They appear only if the checkbox Separate Discount % and DPM % Fields is selected in Administration System
Initialization Document Settings Per Document for A/P down payments.
DPM %
In the field on the left, enter the down payment as a percentage rate. The field on the right displays the down payment amount.
Rounding
Difference between the original amount and the rounded amount.
Appears only if the rounding method is defined as By Currency in Administration System Initialization Document Settings
General .
WTax Amount
Withholding tax amount for the document, calculated according to the withholding tax definitions.
Relevant in some localizations only.
Tax
Tax amount for the A/P down payment document.
Total Payment Due
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:05 AM
Total amount of the document including tax and discounts.
Applied Amount
Amount of the A/P down payment invoice cleared by an outgoing payment.
Balance Due
Open amount of the A/P down payment document. This amount has not been paid or credited yet.
More Information
A/P Down Payment Request
A/P Down Payment Invoice
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:05 AM
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:05 AM
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:05 AM
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:05 AM
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:05 AM
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:05 AM
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:05 AM
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:05 AM
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:05 AM
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
Down Payments to Draw
This window displays open and paid down payment requests and invoices created for a specific business partner.
To access the window, create an invoice and click .
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, click in the toolbar.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Down Payments to Draw Fields
Selection
To draw a document into the invoice, select the checkbox in the relevant row.
Document Number
Document number of the down payment document.
Document / Row Type
Indicates the document type.
Remarks
Contents of the Remarks field in the down payment invoice.
Tax Code
Indicates the tax code of the tax group specified in the down payment.
Net Amount To Draw
Specify the net amount of the down payment document that you want to draw to the invoice. This is the amount of the down
payment document that was paid and not yet drawn into an invoice. If you specify the net amount to draw, the gross amount to
draw is calculated automatically and vice versa.
Tax Amount To Draw
Total tax amount of the down payment that is drawn into the invoice. The calculation is based on the net or gross amount to draw
that you specify.
Gross Amount to Draw
Gross amount of the down payment that should be drawn into the invoice. This is the amount of the down payment document that
was paid and not yet drawn into an invoice. If you specify the gross amount to draw, the net amount to draw is calculated
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:05 AM
automatically and vice versa.
Open Net Amount
Amount of the down payment that was paid and can be drawn into the final invoice.
After the invoice is created, this amount is updated according to the amount drawn.
Open Tax Amount
Tax amount of the down payment that is still open and can be drawn into the invoice.
Open Gross Amount
Gross amount of the down payment that was paid and can be drawn into the invoice.
Total Net Amount
Original total net amount from the down payment document.
Total Tax Amount
Original total tax amount from the down payment document.
Total Gross Amount
Original total gross amount (total net amount + total tax amount) from the down payment document.
Document Date
Document date of the down payment document.
More Information
A/P Invoice: General Area
A/R Invoice: General Area
A/P Down Payment Document: Logistics Tab
This tab contains details regarding the logistics aspects of the A/P down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Down Payment Logistics Tab
Ship to
A/P down payment documents of type Item: address defined for the warehouse linked to the Contents tab.
A/P down payment documents of type Service: company address as defined in Administration System Initialization
Company Details General Local Language .
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:05 AM
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner.
More Information
A/P Down Payment Request
A/P Down Payment Invoice
A/P Down Payment Document: Accounting Tab
This tab contains information regarding the financial aspects of A/P down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Down Payment Accounting Tab
Journal Remark
By default, displays A/P Down Payment – XXX, where XXXis the vendor code. Change this content, if required.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the down payment. This control account can then be copied to any follow-up documents.
 Note
For A/P down payment requests, it appears only if the checkbox Allow Control Account Selection is selected in
Administration System Initialization Document Settings Per Document for A/P down payment requests.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if its due date has already expired.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:05 AM
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
The installment-payments feature is unavailable for down payment documents. This field displays the number 1 by default. This
value cannot be modified.
Months +Days
Enter the due date.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
 Note
The two fields are available in all localizations except CZ, SK, HU, PL, RU, UA.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Indicator
Indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID as defined in the company details in Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of a chain. This number is recorded in the file that you send to the head office of a chain store.
Relevant in some localizations only.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:05 AM
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
Related Information
A/P Down Payment Request
A/P Down Payment Invoice
Down Payment Interim Account, Down Payment Clearing Account
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:05 AM
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Down Payment Invoice Process
Companies have a business need to issue and receive invoices that include tax (or VAT) for down payments made or received.
These invoices are then cleared with partial or final invoices. Companies record a down payment received in SAP Business One by
creating a payment not based on an invoice. However, due to legal requirements in certain countries, the recording of a down
payment requires an invoice or a billing document.
The process below explains how to create down payment invoices and how to clear them.
Prerequisites
Before you can use down payment invoices, you must do the following:
Define a clearing account on the Sales and Purchase tabs in the G/L Account Determination window in Administration
Setup Financials . If you intend to use the down payment invoice only for sales or only for purchases, define the
clearing account on the proper tab.
Optionally, for each business partner, you can define a special down payment clearing account on the General tab in the
Accounting window in Business Partners Business Partner Master Data .
Process
1. Create an A/R or A/P down payment invoice for a relevant business partner. If you create the down payment invoice by
drawing a base document, ensure that you have defined the required down payment percentage. .
The down payment invoice:
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:05 AM
Creates an accounting posting
Does not affect inventory values or perpetual inventory
Does not change the status of the base document that was drawn into it
2. Once the actual payment for the down payment invoice is made, create the proper payment document, based on the down
payment invoice. A down payment invoice can be paid partially.
After you create the payment document, a journal entry is recorded in the corresponding control account.
 Note
If you cancel the payment created for the down payment by choosing Data Cancel from within the
incoming/outgoing payment, the paid down payment is reopened and cannot be drawn when you create an invoice.
However, if, for example, the down payment was paid by check and you cancelled the check from within the check
register, then the down payment remains closed and can be drawn when you create an invoice.
 Note
If you copy a down payment invoice to a credit memo, the Items per Unit and Unit of Measure fields cannot be edited.
3. Create a regular invoice. Before you add it, click to open the Down Payments to Draw window. Draw the required down
payments from this window and specify the net or gross amount to be copied into the regular invoice.
The total amount of the drawn down payments is taken from the Total Down Payment field in the invoice. This amount is
deducted from the original total amount of the invoice.
 Note
You can pay the down payment invoices and the regular invoices in the same payment document. The down payment
documents are labeled as document type DT in the payment document.
Result
The invoice total is updated by subtracting the down payment total from the original invoice total.
A down payment invoice that is drawn to an invoice is closed and cannot be drawn again to another invoice.
Example
The following example illustrates the down payment invoice process in the sales area.
Down Payment Invoice Creation by a Sales Person (United States)
Bass Clef Ltd. uses the non-perpetual inventory method of inventory valuation. Tom, the sales employee, creates Sales Order 875
for Horn & Brass for the following items:
1 Music Score Trumpet Solo $60
1 Music Score Guitar Solo $40
1 Music Score Flute Duet $100
Total $200
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:05 AM
Sales Tax (5%) $10
Total including Tax $210
Horn & Brass has decided to pay currently only a deposit of $80. Tom, as a sales employee, does not have authorization to create a
down payment invoice, but in SAP Business One Tom can create a deposit (incoming payment) directly from the sales order, so
that Down Payment Invoice 431 is created automatically once the payment has been received. At this point, no sales tax is
charged.
The journal entry created by the deposit document is:
Debit Credit
Cash 80
Account Receivables 80
Another journal entry created automatically by Down Payment Invoice 431 is:
Debit Credit
Account Receivables 80
Payment Advances 80
Tom creates Delivery 589 and the order is shipped. He issues the final invoice for the total sales order. The amount due is only the
open amount (the remaining amount to be paid). The revenue reflects the full amount, which creates the following journal entries:
Debit Credit
Accounts Receivable 130
Payment Advances 80
Sales Tax 10
Revenue 200
Down Payment Invoice Creation by a Sales Person (United States)
Books & Poems Inc. uses the non-perpetual inventory method of inventory valuation. Anne, the manager, creates Sales Order 361
for the Bloor Street Book Club for the following items:
1 British Novel $30
1 American Novel $45
1 Canadian Novel $25
Total $100
Sales Tax (5%) $5
Total including Tax $105
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:05 AM
After two weeks, Anne has not received payment. She creates Down Payment Invoice 232, for which the following journal entry is
created:
Debit Credit
Accounts Receivables 40
Payment Advances 40
The Bloor Street Book Club pays the deposit once they have received the down payment invoice. At this point, no sales tax is
charged.
The journal entry created is:
Debit Credit
Cash 40
Accounts Receivables 40
Anne creates Delivery 870 and the order is shipped. She issues the final invoice, which creates the following journal entries:
Debit Credit
Accounts Receivables 65
Payment Advances 40
Sales Tax 5
Revenue 100
Related Information
Down Payments to Draw
A/R Down Payment Documents: General Area
A/P Down Payment Document: General Area
A/R Down Payment Invoice
A/P Down Payment Invoice
A/P Down Payment Invoice
When your vendor sends you an invoice for a down payment, you enter it in SAP Business One as an A/P down payment invoice.
The posting created by this document is relevant only for the accounting system and does not affect inventory values. You can
create this document based on a purchase order or a goods receipt PO, just as you do with your regular A/P invoices.
In some localizations, you can create this document based on a paid down payment request. For more information, see the
relevant process/procedure descriptions.
To access the window, choose Purchasing – A/P A/P Down Payment Invoice .
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:05 AM
A/P Down Payment Invoices
Your vendors may require you to pay a down payment when placing an order. The process below describes how to create
simultaneously a purchase order, an outgoing payment for the paid down payment, and an A/P down payment invoice.
Prerequisites
The payment advances account is specified in one of the following locations:
On the General subtab of the Purchasing tab in Administration Setup Financials G/L Account
Determination
On the Accounting subtab of the General tab of the relevant vendor in Business Partners Business Partner
Master Data
The user has Full Authorization for A/P down payment invoices in Administration System Initialization
Authorizations General Authorizations .
Process
1. From the SAP Business One Main Menu, choose Purchasing - A/P Purchase Order . The Purchase Order window
appears.
2. Fill in the purchase order. Before you add it to the data base, choose from the toolbar. The Deposit on Order window
appears.
3. Specify the amount paid as down payment and the payment means used, and choose the OK button.
4. Return to the Purchase Order window and add the purchase order.
Result
The process described above produces the following documents:
Purchase order
A/P down payment invoice for the amount paid, linked to the purchase order
Outgoing payment for the amount paid, linked to the A/P down payment invoice
The Remarks field in the newly added purchase order displays the following text: Linked to Down Payment No. XXX
In addition:
The purchase order is not closed, even if the down payment amount was the full amount of the purchase order. It can be
copied later into a goods receipt PO or an A/P invoice, as any other purchase order.
The A/P down payment invoice created has no impact on inventory (neither on quantities nor on inventory accounting
values).
The A/P down payment invoice does not include tax, and the complete amount of tax related to the purchase order is to be
paid only after the A/P invoice is created.
 Note
To calculate taxes in down payment invoices, select the Enable Tax Calculation in Down Payment Invoices checkbox in
the Administration System Initialization Document Settings Per Document tab for A/P and A/R down
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:05 AM
payments. However, if you do not want to calculate taxes for down payment invoices generated from a certain order, you
can deselect the Enable Tax Calculation in Down Payment Invoices checkbox in the Deposit on Order window.
This feature is available only in the USA and Canada localizations.
Although the creation of an incoming payment directly from within a sales order is an available functionality, sales orders
are not visible in the Incoming Payments table.
You can create more than one A/P down payment invoice for a given purchase order by displaying the purchase order,
choosing from the toolbar, and repeating step 3.
A/P Down Payment Document: General Area
Use this area of the purchasing document to enter general information relevant for all items in the document.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Down Payment General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Specify the vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the A/P down payment document. If you choose the manual series, enter the relevant number.
Status
Status of the A/P down payment document:
Open
Down payment request: You can draw the document completely or partially to a higher-level document.
 Recommendation
A down payment request can be paid partially, but the down payment request document should be closed before linking
it to the final invoice.
Down payment invoice: You can draw the document completely or partially to a higher-level document. The down payment
invoice can be paid partially, but drawn into an invoice.
Open – Printed
You printed the document and left it open.
Canceled
You canceled the document manually.
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:05 AM
Closed
Down payment request: The document was paid and thus closed, or closed manually.
Down payment invoice: The document was paid and thus closed.
Draft
The document is still a draft.
Posting Date
Specify the posting date. The default value is the date on which the A/P down payment document is created. If required, change
the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the payment of the down payment. The default date is 30 days after the posting date.
To change it, choose a different payment term in the Payment Terms field, or enter a date manually.
Currency
Specify the display currency for the amounts in the A/P down payment document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Buyer
Specify the buyer who initiated the purchasing document.
Owner
Specify the employee who owns the document.
Remarks
Enter additional information regarding the document.
Total Before Discount
Total amount of the document before the discount for the document is calculated.
Base Discount %
Percentage and amount of the discount from the base document, and they are separated from those of the down payment.
 Note
They appear only if the checkbox Separate Discount % and DPM % Fields is selected in Administration System
Initialization Document Settings Per Document for A/P down payments.
DPM %
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:05 AM
In the field on the left, enter the down payment as a percentage rate. The field on the right displays the down payment amount.
Rounding
Difference between the original amount and the rounded amount.
Appears only if the rounding method is defined as By Currency in Administration System Initialization Document Settings
General .
WTax Amount
Withholding tax amount for the document, calculated according to the withholding tax definitions.
Relevant in some localizations only.
Tax
Tax amount for the A/P down payment document.
Total Payment Due
Total amount of the document including tax and discounts.
Applied Amount
Amount of the A/P down payment invoice cleared by an outgoing payment.
Balance Due
Open amount of the A/P down payment document. This amount has not been paid or credited yet.
Payment Order Run
If the checkbox is selected, it indicates that this document, or at least one of its installments, is included in a payment order run.
The checkbox is deselected in the following situations:
The payment order row that includes this document or its installment(s) is removed from the payment order run.
To remove a payment order row, in Payment Wizard: Step 6 - Recommendation Report, right-click the payment order row
and choose Remove. The checkbox for this payment order row is deselected in the selection column.
The payment order row that includes this document or its installment(s) is closed in the payment order run.
To close payment order rows in which all the documents are fully paid, in Payment Wizard: Step 6 - Recommendation
Report, choose the Close Payment Order Rows button. The Payment Order Status column displays C for the closed
payment order rows.
The payment order run that includes this document or its installment(s) is executed into a payment run.
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:05 AM
More Information
A/P Down Payment Request
A/P Down Payment Invoice
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:05 AM
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:05 AM
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:05 AM
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:05 AM
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:05 AM
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:05 AM
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:05 AM
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:05 AM
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:05 AM
Document Settings: General Tab
Last Prices Report
A/P Down Payment Document: Logistics Tab
This tab contains details regarding the logistics aspects of the A/P down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Down Payment Logistics Tab
Ship to
A/P down payment documents of type Item: address defined for the warehouse linked to the Contents tab.
A/P down payment documents of type Service: company address as defined in Administration System Initialization
Company Details General Local Language .
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner.
More Information
A/P Down Payment Request
A/P Down Payment Invoice
A/P Down Payment Document: Accounting Tab
This tab contains information regarding the financial aspects of A/P down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:05 AM
A/P Down Payment Accounting Tab
Journal Remark
By default, displays A/P Down Payment – XXX, where XXXis the vendor code. Change this content, if required.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the down payment. This control account can then be copied to any follow-up documents.
 Note
For A/P down payment requests, it appears only if the checkbox Allow Control Account Selection is selected in
Administration System Initialization Document Settings Per Document for A/P down payment requests.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if its due date has already expired.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
The installment-payments feature is unavailable for down payment documents. This field displays the number 1 by default. This
value cannot be modified.
Months +Days
Enter the due date.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
 Note
The two fields are available in all localizations except CZ, SK, HU, PL, RU, UA.
BP Project
Specify a project name linked to the vendor in the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:05 AM
Indicator
Indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID as defined in the company details in Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of a chain. This number is recorded in the file that you send to the head office of a chain store.
Relevant in some localizations only.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:05 AM
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
Related Information
A/P Down Payment Request
A/P Down Payment Invoice
Down Payment Interim Account, Down Payment Clearing Account
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:05 AM
A/P Invoice
The A/P invoice is a request for payment. It also records the cost in the profit and loss statement.
To access the window, choose Purchasing – A/P A/P Invoice .
You can create an A/P invoice from multiple purchase orders and goods receipt POs. You cannot change any accounting-relevant
data on an A/P invoice since it is the legal accounting document that generates entries in the general ledger.
When you receive an A/P invoice, SAP Business One posts the related accounts for the vendor in the accounting system. If no
delivery for a purchase order precedes the A/P invoice, and if you are purchasing items managed in the warehouse, the inventory
increases when the you post the invoice.
SAP Business One enables you to create an A/P invoice with a zero amount when you receive no-charge items, for example, items
that are part of a promotion or under the coverage of a service contract.
Relevant in some localizations only:
If your company does not manage a perpetual inventory system, the A/P invoice is posted to the appropriate expense account:
domestic, foreign, or EU.
 Example
If the company is Danish and the federal tax ID of the business partner is also Danish, the invoice is domestic, so the system
posts the invoice to the domestic expense account. If the federal tax ID does not start with DK (or is empty) and the billing
address country/region of the business partner is an EU country/region, the system posts the invoice to the EU expense
account. If the federal tax ID does not start with DK (or is empty) and the billing address is not EU, the system posts the invoice
to the Non-EU expense account.
 Note
In a perpetual inventory system, when you post an A/P invoice that is copied from a goods receipt PO, the posting account
depends on the current In Stock quantity of an item:
If the In Stock quantity > = A/P invoice quantity, then the Inventory Account is debited.
If the In Stock quantity < A/P invoice quantity, then the price difference is split between Inventory Account and Price
Difference Account.
If the In Stock quantity = Zero, then the price difference is posted to the Price Difference Account.
Price differences pertaining to sold items are considered as an additional expense to appear in the Profit and Loss Statement
report.
More Information
Creating Purchasing Documents
A/P Invoice: General Area
Purchasing Documents: Contents Tab
A/P Invoice: Logistics Tab
A/P Invoice: Accounting Tab
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:05 AM
A/P Invoice: General Area
Use this part of an A/P invoice to enter general information relevant to all items in the document.
To access this area, choose Purchasing – A/P A/P Invoice .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Invoice General Area Fields
Contact Person
Name of the default contact person defined in the business partner master data.
Vendor Ref. No.
Specify the vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the A/P invoice.
Status
Status of the A/P invoice:
Open
You can draw the document completely or partially to a higher level document.
Open – Printed
You printed the document and left it open.
Canceled
You canceled the document manually.
Closed
SAP Business One closed the document automatically when you drew it to another document.
Draft
The document is still a draft.
Posting Date
Specify the posting date.
Due Date
The date by which you must pay the vendor. This date is calculated according to the payment term defined for the vendor, or the
one specified on the Accounting tab of the document. You can change this value manually or by choosing a different option in the
Payment Terms field.
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:05 AM
You can also edit the Due Date after the A/P invoice is partially reconciled. Make sure the new Due Date is on or after the latest
Reconciliation Date.
Document Date
Date of the document for tax reporting purposes. By default, it is the same as the posting date. You can change it manually, if
required.
Currency
Specify the display currency for the amounts in the A/P invoice.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Buyer
Specify the buyer who initiated the A/P invoice.
Owner
Specify the employee who owns the A/P invoice.
Remarks
Enter additional information regarding the document.
Total Before Discount
Total amount of the A/P invoice before the discount for the document is calculated.
If the discount has been defined in the item or service row, the amount displayed in this field considers that discount.
% Discount
In the field on the left, specify the percentage of the discount for the whole A/P invoice. The field on the right displays the amount
of the discount.
Total Down Payment
Amount drawn from the paid down payment invoices or down payment requests. This amount is subtracted from the total amount
of the invoice. Choose to open the Down Payment to Draw window, which displays the details of the amount displayed in this
field.
Freight
This field appears if the Manage Freight in Documents checkbox is selected on the General tab in the Document Settings window.
You can define freight for the A/P invoice. To open the Freight Charges window and to view the corresponding freight, click .
Rounding
This field appears if the rounding method is defined as By Currency on the General tab in the Document Settings window .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/P invoice calculated according to the tax definitions.
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:05 AM
WT Amount
Amount of the withholding tax involved in the A/P invoice, if defined.
Total Payment Due
Total amount of the A/P invoice including tax, freight, and discounts.
Applied Amount
Amount paid or credited by an outgoing payment or credit memo.
Balance Due
Open amount of the A/P invoice. This amount has not been paid or credited yet.
Copy From
A list of base documents from which to create a target document.
Copy To
Choose the target document to be created based on the current one. The Copy To function lets you copy only one document to the
target document.
Payment Order Run
If the checkbox is selected, it indicates that this document, or at least one of its installments, is included in a payment order run.
The checkbox is deselected in the following situations:
The payment order row that includes this document or its installment(s) is removed from the payment order run.
To remove a payment order row, in Payment Wizard: Step 6 - Recommendation Report, right-click the payment order row
and choose Remove. The checkbox for this payment order row is deselected in the selection column.
The payment order row that includes this document or its installment(s) is closed in the payment order run.
To close payment order rows in which all the documents are fully paid, in Payment Wizard: Step 6 - Recommendation
Report, choose the Close Payment Order Rows button. The Payment Order Status column displays C for the closed
payment order rows.
The payment order run that includes this document or its installment(s) is executed into a payment run.
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/P Invoice
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:05 AM
Down Payments to Draw
This window displays open and paid down payment requests and invoices created for a specific business partner.
To access the window, create an invoice and click .
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, click in the toolbar.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Down Payments to Draw Fields
Selection
To draw a document into the invoice, select the checkbox in the relevant row.
Document Number
Document number of the down payment document.
Document / Row Type
Indicates the document type.
Remarks
Contents of the Remarks field in the down payment invoice.
Tax Code
Indicates the tax code of the tax group specified in the down payment.
Net Amount To Draw
Specify the net amount of the down payment document that you want to draw to the invoice. This is the amount of the down
payment document that was paid and not yet drawn into an invoice. If you specify the net amount to draw, the gross amount to
draw is calculated automatically and vice versa.
Tax Amount To Draw
Total tax amount of the down payment that is drawn into the invoice. The calculation is based on the net or gross amount to draw
that you specify.
Gross Amount to Draw
Gross amount of the down payment that should be drawn into the invoice. This is the amount of the down payment document that
was paid and not yet drawn into an invoice. If you specify the gross amount to draw, the net amount to draw is calculated
automatically and vice versa.
Open Net Amount
Amount of the down payment that was paid and can be drawn into the final invoice.
After the invoice is created, this amount is updated according to the amount drawn.
Open Tax Amount
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:05 AM
Tax amount of the down payment that is still open and can be drawn into the invoice.
Open Gross Amount
Gross amount of the down payment that was paid and can be drawn into the invoice.
Total Net Amount
Original total net amount from the down payment document.
Total Tax Amount
Original total tax amount from the down payment document.
Total Gross Amount
Original total gross amount (total net amount + total tax amount) from the down payment document.
Document Date
Document date of the down payment document.
More Information
A/P Invoice: General Area
A/R Invoice: General Area
Payments List
The Payments List window displays the incoming or outgoing payments documents created in response to specific A/R or A/P
invoices.
To access this window, display the relevant invoice and click in the toolbar.
 Note
The Payments List window appears only when the displayed invoice was paid (fully or partially). If the invoice was not paid at
all, the Payment Means window appears.
Payments List Window
The following table describes the fields appear in the Payments List window.
To access this window, display the required A/R or A/P invoice and click in the toolbar.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Payments List Window
Payment No.
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:05 AM
Number of the incoming or outgoing payments document.
Total
Total amount paid through this payment document.
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:05 AM
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:05 AM
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:05 AM
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:05 AM
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:05 AM
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:05 AM
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:05 AM
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:05 AM
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:05 AM
Document Settings: General Tab
Last Prices Report
A/P Invoice: Logistics Tab
This tab displays information regarding the logistics aspect of an A/P invoice.
To access the tab, choose Purchasing – A/P A/P Invoice Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Invoice Logistics Tab Fields
Ship to
A/P invoices of type Item: Address defined for the warehouse in the first row on the Contents tab
A/P invoices of type Service: Company address as defined in Administration System Initialization Company Details
General Local Language .
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data. If required, choose a different address.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner.
More Information
A/P Invoice
A/P Invoice: Accounting Tab
This tab contains information regarding the financial aspects of the A/P invoice.
To access the tab, from the SAP Business One Main Menu, choose Purchasing – A/P A/P Invoice Accounting .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Invoice Accounting Tab Fields
Journal Remark
By default, displays A/P Invoice – XXX, where XXX is the vendor code. Change this content, if required.
Control Account
Specify the control account for the A/P invoice. The default value is the Accounts Payable value in the business partner master
data.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if its due date has already expired.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
Displays the installments details as specified in the business partner master data. To edit the data, click .
+Months...+Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be given
for the current month or for several months in the future, as well as for the number of days you specify in the last month of the
period.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Indicator
Indicator linked to the vendor in the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:05 AM
Federal Tax ID
The company federal tax ID as defined in the company details: Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of the chain, when you use the direct distribution method. This number is recorded in the file that you
send to the head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:05 AM
A/P Invoice
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Goods Return Request
Return Material Agreement describes a scenario where the supplier of a good or product agrees to have a customer ship that item
back in exchange for a refund or credit.
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:05 AM
The purpose of adding a goods return request is to enable creating pre-step of the goods return document, to enter the agreed
quantities, prices, and return reason before the goods are actually returned.
You can either create a goods return request based on Goods Receipt PO or A/P invoices, or create a standalone goods return
request that is not based on any document. For standalone goods return request, the Quantity in the goods return can exceed the
Quantity in the goods return request based on which the goods return is created.
For the goods return request that is generated based on goods receipt PO or A/P invoices, you can also add standalone lines to it.
 Note
When adding standalone lines to goods return request that was based on goods receipt PO, the target document for these
standalone lines can be only goods return. When adding standalone lines to goods return request that was based on A/P
invoice, the target document for these standalone lines can be only A/P credit memo.
If an A/P invoice is copied or partially copied to a goods return request, closing this invoice by fully paying it, or reconciling the
invoice transaction, or fully crediting it shall not be allowed. You need to manually close the goods return request to continue.
To access this window, in Main Menu, choose Purchasing - A/P Goods Return Request .
More Information
Goods Return Request: General Area
Goods Return Request: Contents Tab
Goods Return Request: Logistics Tab
Goods Return Request: Accounting Tab
Assigning Serial Numbers in Goods Return Requests or Return Requests
Assigning Batches in Goods Return Requests or Return Requests
Goods Return Request: General Area
Use this area of the goods return request to enter general information relevant to all items in the document.
To access the window, in Main Menu, choose Purchasing - A/P Goods Return Request .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Return General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Vendor reference number, if available.
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:05 AM
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the goods return request. If you choose the Manual series, enter the relevant number.
Status
Status of the goods return request:
Open
You can copy the document completely or partially to a higher-level document.
Open - Printed
You printed the document and left it open.
Closed
You closed the document manually, orSAP Business One closed it automatically when you copied it to another document.
Draft
The document is still a draft.
Unapproved
The document is not yet approved, thus cannot be copied to other documents.
Posting Date
Specify the posting date.
The default value for this field is the current date on which the goods return request is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected return date of the items to vendors. The default date is equal to the posting date.
To change it, choose a different option in the Payment Terms field, or enter one manually.
Document Date
Document date of the goods return request used for tax purposes. The default value is the current date.
Currency
Specify the display currency for the amounts in the goods return request.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
Buyer
Specify the buyer who initiated the goods return request.
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:05 AM
Owner
Specify the employee who owns the goods return request.
Remarks
Enter additional information regarding the goods return request.
You can edit the field contents even after the document is added.
Total Before Discount
Total amount of the goods return request before the discount for the document is calculated.
 Note
If the discount has been defined in the item row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of the discount for the whole goods return request.
The field on the right displays the amount of the discount.
Freight
This field appears only if Manage Freight in Documents is selected in Administration System Initialization Document
Settings General .
You can define freight for the goods return. To open the Freight Charges window and to view the corresponding freight, click .
Goods Return Request: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Type and Summary Type Fields
Item/Service Type
Goods return requests are supported only on item type of documents. Select Item, and you can create a goods return request for
items defined in the Inventory module.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:05 AM
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Quantity
Quantity that you want to return to the vendor based on the item’s purchasing unit of measure, as defined in the Item Master Data
window.
 Note
For goods return request that is created based on goods receipt PO or A/P invoices, the Quantity cannot exceed the Quantity
in the base documents. For standalone goods return request, the Quantity in the goods return can exceed the Quantity in the
goods return request based on which the goods return is created.
If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the Qty
(Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
Item price from the default price list, before a discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices Report.
Discount %
Displays the discount percentage assigned to the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:05 AM
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then toSAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
UoM Code
Displays the UoM code of the item specified. For a goods return request that is created based on other documents, the UoM code
is copied from the base documents, and cannot be modified.
For a standalone goods return request, this field displays the default sales UoM code you specified in the Item Master Data screen,
and it can be changed manually. If you have not specified a default sales UoM code, this field is by default blank. You can select one
from all the UoM codes in the UoM group to which the item belongs.
 Note
If the item is not assigned to any UoM group, that is, in the Item Master Data screen, in the UoM Group field, you selected
Manual, then the UoM Code field displays Manual here, and the value cannot be changed.
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:05 AM
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current return request only.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:05 AM
Indicates that there is no inventory movement involved, that is, the goods return request does not affect the inventory quantity of
the item. By default, this checkbox is not selected. After copying the goods return request to goods return or credit memo, Without
Qty Posting field will be disabled on the base goods return request.
For standalone goods return request, selecting this checkbox or not affects the target document that could be created based on
this goods return request.
When the checkbox is not selected, you can create goods return or credit memo based on the goods return request.
When the checkbox is selected, you can create only credit memo based on the goods return request.
In the target credit memo, the field is not editable. Still, the user could go back to the goods return request, and manually change
the setting, and then copy it to credit memo again.
The open quantity in the goods return request is updated according to the quantity drawn into the target document.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
Gross Price After Disc.
Gross price after discount equals the unit price (including tax) order minus the discount amount. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key, the Unit
Price field and the Tax/Unit field are updated accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:05 AM
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Gross Total (LC)
Displays the total gross amount of the row in local currency. If the item quantity is 1, the gross total is equal to the amount entered
in the Gross Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Return Reason
Specify the reason why you want to return the goods to your vendor. There are the following options:
Empty
Indicates that there's no reason for the return.
Define New
Select this option and you will be directed to the Return Reasons - Setup screen. Here, you can add a return reason and
then select Update.
All the reasons you added in this screen will be displayed later in the Return Reason drop-down list.
This field is not visible by default. To display the field, in the menu bar, go to Tools Form Settings Return Request . In the
Table Format tab, select the field in the Visible checkbox.
Return Action
Specify the action you want regarding the goods return. There are the following options:
Return (default value)
Indicates that you want to return the goods.
Repair
Indicates that you want the goods to be repaired only.
Replace
Indicates that you want the goods to be replaced by new ones.
Define New
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:05 AM
Select this option and you will be directed to the Return Actions - Setup screen. Here, you can add a return action and then
select Update.
This field is not visible by default. To display the field, in the menu bar, go to Tools Form Settings Return Request . In the
Table Format tab, select the field in the Visible checkbox.
More Information
Goods Return Request
Assigning Serial Numbers in Goods Return Requests or Return Requests
Assigning Batches in Goods Return Requests or Return Requests
Goods Return Request: Logistics Tab
This tab displays information regarding the logistics aspect of the goods return.
To access the tab, in Main Menu, choose Purchasing - A/P Goods Return Request Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Return Request Logistics Tab Fields
Ship From
Goods return requests of type Item: address defined for the warehouse linked to the Contents tab.
Goods return requests of type Service: company address as defined in Administration System Initialization Company
Details General Local Language .
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . The system updates the address only for this marketing document; it does not affect the
warehouse address, the user defaults address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the address IDs and address summaries of your vendor, as defined in the business partner master data. From the
dropdown list, select a destination address ID to which you deliver goods and services to your vendors for return. If required,
change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:05 AM
affect the business partner master data.
Shipping Type
Specify how the customer wants the goods to be returned, for example, by which courier. If there is no shipping types available in
the drop-down list, select Define New to add shipping types in the Shipping Type - Setup screen.
Confirmed
Indicates that the goods return request is approved and enables copying it to the corresponding return or credit memo.
This checkbox is selected by default if the checkbox Confirm Goods Return Request Automatically in the Administration
System Initialization Document Settings Per Document tab is selected.
More Information
Goods Return Request
Goods Return Request: Accounting Tab
This tab contains information regarding the financial aspect of the goods return.
To access the tab, in Main Menu, choose Purchasing - A/P Goods Return Request Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Return Request Accounting Tab Fields
Journal Remark
By default, displays Goods Return Request – XXX, where XXX is the vendor code. Change this content, if required.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
BP Project
Project name linked to the vendor in the business partner master data.
Indicator
Indicator linked to the vendor in the business partner master data. This indicator is used as a selection criterion in various reports.
If required, choose a different indicator.
Federal Tax ID
The company federal tax ID, if defined in the company details in Administration System Initialization Company Details
Accounting Data .
Order Number
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:05 AM
Enter an order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Goods Return Request
Purchasing Document: Attachments Tab
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:05 AM
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Goods Return
The goods return document is used to return delivered goods to vendors or to reverse a purchasing transaction for an item
completely or partially, for example, a goods receipt PO in SAP Business One. Due to legal stipulations, you cannot delete or make
any accounting-relevant changes to these documents. However, to return unwanted or faulty goods, or to correct errors made
when entering the above-mentioned documents, you can create a goods return.
When you create a goods return, the goods are issued from the warehouse and the quantities are reduced. If your company uses
perpetual inventory, SAP Business One automatically creates the relevant posting to update the inventory values as well.
You can create a goods return either based on a goods receipt PO or not. If you choose to do the latter, and run the perpetual
inventory by moving average, make sure that the prices of the items in the independent goods return are identical to the prices
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:05 AM
posted in the respective original purchase transaction.
When you create a goods return document based on a purchase order, you can choose to reopen the item quantity of the order. To
be able to do so, the checkbox Enable Reopening of Orders When Creating Returns Based on Orders must be selected in the
document settings. For more information, see Document Settings: Per Document Tab.
Reopening the item quantity has the following consequences:
The status of the purchase order changes to Open.
The open quantity is increased by the item quantity in the goods return document. If the sum of the remaining open
quantity plus the returned quantity is higher than the quantity in the original order, the open quantity is increased up to the
quantity in the original order.
The delivered quantity is decreased by the quantity in the goods return.
For service type transactions, the open amount is increased accordingly by a value equal to the value from a goods return
line. If the sum of the remaining open amount plus the returned amount is greater than the total amount for the original
order line, the total amount is used as the open amount.
If there are any freight charges related to the returned item, these charges are reopened in the same way as the item
quantities.
If the item is managed by batches, the returned batch-allocated quantity is increased by the quantity from the return line.
To access the window, choose Purchasing – A/P Goods Return .
Prerequisites
No A/P invoice has been created for the goods being returned. If an invoice has been created, you must create an A/P credit
memo. For more information, see A/P Credit Memo.
More Information
Creating Purchasing Documents
Goods Return: General Area
Purchasing Documents: Contents Tab
Goods Return: Logistics Tab
Goods Return: Accounting Tab
Goods Return: General Area
Use this area of the goods return to enter general information relevant to all items in the document.
To access the window, choose Purchasing – A/P Goods Return .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:05 AM
Goods Return General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the goods return. If you choose the manual series, enter the relevant number.
Status
Status of the goods return:
Open
You can draw the document completely or partially to a higher level document.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually, or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
Posting Date
Specify the posting date.
The default value for this field is the current date on which the goods return is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services. The default date is 30 days after the posting date.
To change it, choose a different option in the Payment Terms field, or enter one manually.
Document Date
Document date of the goods return used for tax purposes. The default value is the current date.
Currency
Specify the display currency for the amounts in the goods return.
Branch
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:05 AM
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
Buyer
Specify the buyer who initiated the goods return.
Owner
Specify the employee who owns the goods return.
Total Before Discount
Total amount of the goods return before the discount for the document is calculated.
 Note
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of the discount for the whole goods return.
The field on the right displays the amount of the discount.
Freight
This field appears only if Manage Freight in Documents is selected in Administration System Initialization Document
Settings General .
You can define freight for the goods return. To open the Freight Charges window and to view the corresponding freight, click .
Rounding
This field appears only if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the goods return calculated according to the tax definitions.
Total Credit
Total amount of the goods return including tax, freight charges, and discounts.
More Information
Goods Return
Document Settings: General Tab
Purchasing Documents: Contents Tab
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:05 AM
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:05 AM
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:05 AM
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:05 AM
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:05 AM
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:05 AM
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:05 AM
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
This is custom documentation. For more information, please visit SAP Help Portal. 130

6/8/26, 6:05 AM
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
This is custom documentation. For more information, please visit SAP Help Portal. 131

6/8/26, 6:05 AM
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
Goods Return: Logistics Tab
This tab displays information regarding the logistics aspect of the goods return.
This is custom documentation. For more information, please visit SAP Help Portal. 132

6/8/26, 6:05 AM
To access the tab, choose Purchasing – A/P Goods Return Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Return Logistics Tab Fields
Ship From
Goods returns of type Item: address defined for the warehouse linked to the Contents tab.
Goods returns of type Service: company address as defined in Administration System Initialization Company Details
General Local Language .
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . The system updates the address only for this marketing document; it does not affect the
warehouse address, the user defaults address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the address IDs and address summaries of your vendor, as defined in the business partner master data. From the
dropdown list, select a destination address ID to which you deliver goods and services to your vendors for return. If required,
change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
affect the business partner master data.
Language
Language defined for the business partner.
More Information
Goods Return
Goods Return: Accounting Tab
This tab contains information regarding the financial aspect of the goods return.
To access the tab, choose Purchasing – A/P Goods Return Accounting .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 133

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Goods Return Accounting Tab Fields
Journal Remark
By default, displays Goods Returns – XXX, where XXX is the vendor code. Change this content, if required.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Start From
Specify when you initiate the payment:
Month End
Half Month
Month Start
+Months...+Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be given
for the current month or for several months in the future, as well as for the number of days you specify in the last month of the
period.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
BP Project
Project name linked to the vendor in the business partner master data.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
Indicator
Indicator linked to the vendor in the business partner master data. This indicator is used as a selection criterion in various reports.
If required, choose a different indicator.
Federal Tax ID
The company federal tax ID, if defined in the company details: Administration System Initialization Company Details
Accounting Data .
This is custom documentation. For more information, please visit SAP Help Portal. 134

6/8/26, 6:05 AM
Order Number
Specify the order number of the chain, when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Goods Return
This is custom documentation. For more information, please visit SAP Help Portal. 135

6/8/26, 6:05 AM
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Closing Goods Returns
Prerequisites
The goods return has not yet been copied to an A/P credit memo or a goods receipt PO.
Context
This is custom documentation. For more information, please visit SAP Help Portal. 136

6/8/26, 6:05 AM
When you close goods returns, no adjustment posting is carried out in inventory management. This means that the available
inventory, which has been decreased by the goods returns, is not increased again.
Therefore, if you need to close goods returns and update the inventory values and quantities as well, create a goods receipt PO
based on the goods returns to be closed.
 Note
You cannot create an A/P credit memo or any other purchasing document based on closed goods returns.
Procedure
1. To close goods returns, from the SAP Business One Main Menu, choose Purchasing - A/P Goods Return , and open
the relevant document.
2. In the menu bar, choose Data Close .
You receive the following message:
Closing a document is irreversible. Document status will be changed to “Closed” and a
clearing transaction will be created. Do you want to continue?
3. Do one of the following:
To proceed and close the goods receipt PO, choose the Yes button.
 Note
If you are running a non-perpetual inventory company, the goods receipt return will be closed and the document
status will be changed to Closed.
If you are running a perpetual inventory company, proceed to step 4 to specify the posting date for the clearing
journal entry.
To cancel the operation, choose the No button.
4. If you confirm that you want to close the goods receipt PO, a dialogue box appears asking you to specify a posting date to
be used in the clearing journal entry. Do one of the following:
To use the current system date, select the Current System Date radio button.
To use the original posting date in the document, select the Original Document Date radio button.
To specify a date other than the above two dates, select the Specified Date radio button and then enter a date or
choose a date from the calendar.
If you specify a date which is earlier than or the same as the original posting date of this document, you receive the
following message:
Enter a specified date that is later than original document posting date.
If you specify a date which is in a locked period, you receive the following message:
Period is locked for new data. For more information, see Locking Posting Periods.
5. To save your data, choose the OK button.
 Note
When a goods return is closed (either fully opened or partially drawn), the amount of the freight charges posted to the
expense allocation account and not drawn into an A/P credit memo is cleared.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 137

6/8/26, 6:05 AM
Goods Return
A/P Reserve Invoice
A/P reserve invoices enable you to create relevant posting in the accounting system only and do not affect inventory and inventory
values. You use A/P reserve invoices to document an A/P invoice you receive from a vendor before goods arrive.
After you receive the goods, you create a goods receipt PO based on the A/P reserve invoice to update inventory quantities and
inventory values.
SAP Business One enables you to create an A/P reserve invoice with a zero amount before you receive no-charge items, for
example, items that are part of a promotion or under the coverage of a service contract.
The A/P reserve invoice is relevant for items only and is not available for services.
You close an A/P reserve invoice by creating an outgoing payment.
 Note
Before you begin working with A/P reserve invoices, consult with your accountant.
To access the window, choose Purchasing – A/P A/P Reserve Invoice .
More Information
Creating Purchasing Documents
A/P Reserve Invoice: General Area
Purchasing Documents: Contents Tab
A/P Reserve Invoice: Logistics Tab
A/P Reserve Invoice: Accounting Tab
A/P Reserve Invoice: General Area
Use this part of the A/P reserve invoice to enter general information relevant to all items in the document.
To access the area, choose Purchasing – A/P A/P Reserve Invoice .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Reserve Invoice General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
This is custom documentation. For more information, please visit SAP Help Portal. 138

6/8/26, 6:05 AM
Specify the vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: number of the A/P reserve invoice. If you choose the manual series, enter the relevant number.
Status
Status of the A/P reserve invoice:
Open
You can draw the document completely or partially to a higher level document.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
SAP Business One closed the document automatically when you drew it to another document.
Draft
The document is still a draft.
Delivered
The document was fully copied into Goods Receipt PO, but not yet fully paid.
Paid
The document was fully paid but not yet fully delivered.
 Note
A no-charge A/P reserve invoice is closed automatically, once you add the document.
Posting Date
Specify the posting date.
The default value is the current date on which the A/P reserve invoice is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services.
The default date is 30 days after the posting date. To change it, select a different option in the Payment Terms field, or enter one
manually.
Currency
Specify the display currency for the amounts in the A/P reserve invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 139

6/8/26, 6:05 AM
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Buyer
Specify the employee who initiated the A/P reserve invoice.
Owner
Specify the employee who owns the A/P reserve invoice.
Remarks
Enter additional information regarding the A/P reserve invoice. If required, you can edit the field content even after the A/P reserve
invoice has been created.
Total Before Discount
Total amount of the A/P reserve invoice before the discount for the document is calculated.
 Note
If a discount is defined in the row containing the item or service row, the amount displayed in this field takes that discount into
account.
Discount %
In the field on the left, specify the percentage of the discount for the whole reserve invoice.
The field on the right displays the amount of the discount.
Freight
The field appears only if Manage Freight in Documents is selected in Administration System Initialization Document
Settings General .
You can define freight for the A/P reserve invoice. To open the Freight Charges window and to view the corresponding freight, click
.
Rounding
This field appears only if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/P reserve invoice calculated according to the tax definitions.
WTax Amount
Amount of the withholding tax included in the document, if defined.
Total Payment Due
Total amount of the A/P reserve invoice including tax, freight, and discounts.
This is custom documentation. For more information, please visit SAP Help Portal. 140

6/8/26, 6:05 AM
Applied Amount
Amount paid or credited by an outgoing payment or A/P reserve invoice.
Balance Due
Open amount of the A/P reserve invoice. This amount has not been paid or credited yet.
Payment Order Run
If the checkbox is selected, it indicates that this document, or at least one of its installments, is included in a payment order run.
The checkbox is deselected in the following situations:
The payment order row that includes this document or its installment(s) is removed from the payment order run.
To remove a payment order row, in Payment Wizard: Step 6 - Recommendation Report, right-click the payment order row
and choose Remove. The checkbox for this payment order row is deselected in the selection column.
The payment order row that includes this document or its installment(s) is closed in the payment order run.
To close payment order rows in which all the documents are fully paid, in Payment Wizard: Step 6 - Recommendation
Report, choose the Close Payment Order Rows button. The Payment Order Status column displays C for the closed
payment order rows.
The payment order run that includes this document or its installment(s) is executed into a payment run.
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/P Reserve Invoice
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
This is custom documentation. For more information, please visit SAP Help Portal. 141

6/8/26, 6:05 AM
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
This is custom documentation. For more information, please visit SAP Help Portal. 142

6/8/26, 6:05 AM
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
This is custom documentation. For more information, please visit SAP Help Portal. 143

6/8/26, 6:05 AM
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
This is custom documentation. For more information, please visit SAP Help Portal. 144

6/8/26, 6:05 AM
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
This is custom documentation. For more information, please visit SAP Help Portal. 145

6/8/26, 6:05 AM
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
This is custom documentation. For more information, please visit SAP Help Portal. 146

6/8/26, 6:05 AM
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
This is custom documentation. For more information, please visit SAP Help Portal. 147

6/8/26, 6:05 AM
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
This is custom documentation. For more information, please visit SAP Help Portal. 148

6/8/26, 6:05 AM
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
This is custom documentation. For more information, please visit SAP Help Portal. 149

6/8/26, 6:05 AM
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
A/P Reserve Invoice: Logistics Tab
Use this tab to enter information regarding the logistics aspects of the A/P reserve invoice.
To access the tab, choose Purchasing – A/P A/P Reserve Invoice Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Reserve Invoice Logistics Tab Fields
Ship to
A/P reserve invoices of type Item: address defined for the warehouse linked to the Contents tab.
A/P reserve invoices of type Service: company address as defined in Administration System Initialization Company Details
General Local Language .
This is custom documentation. For more information, please visit SAP Help Portal. 150

6/8/26, 6:05 AM
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the warehouse address, the user defaults
address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data.
More Information
A/P Reserve Invoice
A/P Reserve Invoice: Accounting Tab
Use this tab to specify information regarding the financial aspects of the A/P reserve invoice.
To access the tab, from the SAP Business One Main Menu, choose Purchasing - A/P A/P Reserve Invoice Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Reserve Invoice Accounting Tab Fields
Journal Remark
By default, displays A/P Reserve Invoices – XXX, where XXX is the vendor code. If required, change this content.
Control Account
Specify the control account for the A/P reserve invoice. The default value is the Accounts Payable value in the business partner
master data.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if its due date has already expired.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 151

6/8/26, 6:05 AM
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
Displays details of installments, as specified in the business partner master data. To edit the data, click .
+Months...+Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be given
for the current month or for several months in the future, as well as for the number of days you specify in the last month of the
period.
Net Procedure
Includes the cash discount in the total calculation of the document.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Indicator
Indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID as defined in the company details: Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of the chain, when you use the direct distribution method.
This number is recorded in the file that you send to the head office of the chain store.
More Information
A/P Reserve Invoice
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 152

6/8/26, 6:05 AM
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Crediting A/P Reserve Invoices
Use one of the procedures below to record a credit for A/P reserve invoices, even if you have received some or all of the goods you
ordered. This may be necessary if you have already paid the A/P reserve invoice, but received damaged goods, and would now like
to be reimbursed for the expenses.
Prerequisites
An A/P reserve invoice exists for the vendor.
Procedure
Copying an A/P Reserve Invoice into an A/P Credit Memo
This is custom documentation. For more information, please visit SAP Help Portal. 153

6/8/26, 6:05 AM
1. From the SAP Business One Main Menu, choose Purchasing – A/P A/P Reserve Invoice. and open the relevant
document.
2. Click the Copy To button and select A/P Credit Memo.
The A/P Credit Memo window appears listing all items that were included in the A/P reserve invoice. If not all the items
have been delivered yet, the original item line is divided into two lines – one for delivered items, one for non delivered items.
If there are several related goods receipt POs based on one A/P reserve invoice, the items are divided according to the
goods receipt PO. The goods receipt PO number is displayed in the A/P credit memo.
3. Enter the necessary data and choose Add. The A/P credit memo for the A/P reserve invoice is created.
Copying an A/P Credit Memo from an A/P Reserve Invoice
1. From the SAP Business One Main Menu, choose Purchasing – A/P A/P Credit Memo .
2. Specify the relevant vendor.
3. Click the Copy From button and select A/P Invoices.
The List of A/P Invoices window appears.
4. Select the A/P invoice that you want to credit and click Choose.
5. In the Draw Document Wizard window, select which exchange rate to use and how to copy the data into the credit memo,
and choose Finish.
6. Enter the necessary data and choose Add.
The A/P credit memo for the A/P reserve invoice is created. If not all the items have been delivered yet, the original item
line is divided into two parts – one for delivered items, one for non delivered items. If there are several related goods receipt
POs based on one A/P reserve invoice, the items are divided according to the goods receipt PO. The goods receipt PO
number is displayed in the A/P credit memo.
More Information
A/P Reserve Invoice
A/P Credit Memo
A/P Credit Memo
When you create a delivery for a purchase order or an A/P invoice in SAP Business One, legal stipulations prevent you from
deleting or making any changes to these documents. You may, however, want to return the goods to the vendor for a variety of
reasons, or you may find that you have made a mistake while creating the documents.
The A/P credit memo is the clearing document for the A/P invoice. Therefore, if the vendor has delivered goods, and you have
already created an A/P invoice, you can reverse the transaction either partially or completely by creating an A/P credit memo.
You create the A/P credit memo based on the A/P invoice to establish a link between the two transactions in SAP Business One.
However, it is also possible to create an A/P credit memo without having a base document.
SAP Business One lets you create an A/P credit memo with a zero amount. You can do this when you clear A/P invoices for no-
charge items, such as items that are part of a promotion or covered by a service contract.
You correct both the quantities and the values with the credit memo. SAP Business One reduces the inventory of the credited
items by the quantity specified in the credit memo, posts the value of the credit memo to the vendor account in the accounting
This is custom documentation. For more information, please visit SAP Help Portal. 154

6/8/26, 6:05 AM
system, and reduces the expense account by the same amount.
 Note
You cannot post to an expense account when the item is an inventory item or the company is a perpetual inventory company.
 Note
If you have returned goods to a vendor, and received only a goods return document, enter it into SAP Business One. When the
A/P credit memo is received from the vendor, create it in SAP Business One using the goods return as a base document. That
way, the A/P credit memo updates the financial values only, while quantities and inventory values are updated by the goods
return document.
When you create an A/P credit memo for service, there is no significance to goods returns, since only the financial values are
updated.
When you create an A/P credit memo based on a purchase order, you can choose to reopen the item quantity of the order. To be
able to do so, the checkbox Enable Reopening of Orders When Creating Returns Based on Orders must be selected in the
document settings. For more information, see Document Settings: Per Document Tab.
Reopening the item quantity has the following consequences:
The status of the purchase order changes to Open.
The open quantity is increased by the item quantity in the credit memo. If the sum of the remaining open quantity plus the
returned quantity is higher than the quantity in the original order, the open quantity is increased up to the quantity in the
original order.
The delivered quantity is decreased by the quantity in the credit memo.
For service type transactions, the open amount is increased accordingly by a value equal to the value from a credit memo
line. If the sum of the remaining open amount plus the credited amount is greater than the total amount for the original
order line, the total amount is used as the open amount.
If there are any freight charges related to the credited item, these charges are reopened in the same way as the item
quantities.
If the item is managed by batches, the returned batch-allocated quantity will be increased by the quantity from the return
line.
To access the window, choose Purchasing – A/P A/P Credit Memo .
More Information
Creating Purchasing Documents
A/P Credit Memo: General Area
Purchasing Document: Contents Tab
A/P Credit Memo: Logistics Tab
A/P Credit Memo: Accounting Tab
A/P Credit Memo: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 155

6/8/26, 6:05 AM
Use this part of the A/P credit memo to enter general information relevant to all items in the document.
To access the general area , choose Purchasing – A/P A/P Credit Memo .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Credit Memo General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data.
Vendor Ref. No.
Specify the vendor reference number, if available.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: A/P credit memo number. If you choose the manual series, enter a relevant number.
Status
Statuses of the A/P credit memo:
Open
You can draw the document completely or partially to a higher level document.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
A no-charge A/P credit memo is closed automatically once you add the document.
Posting Date
Specify the posting date. The default value for this field is the current date on which the A/P credit memo is created. If required,
change the date.
If the A/P credit memo is copied from an A/P invoice, make sure this date is on or after the posting date of the invoice.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
This is custom documentation. For more information, please visit SAP Help Portal. 156

6/8/26, 6:05 AM
Expected due date of the items or services. The default due date is the system date (current date). You can change it manually. The
due date becomes blank when posting date is updated.
Document Date
Document date of the A/P credit memo used for tax purposes. The default value is the current date.
Currency
Specify the display currency for the amounts in the A/P credit memo.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
Buyer
Specify the buyer who initiated the A/P credit memo.
Owner
Specify the employee who owns the A/P credit memo.
Remarks
Enter additional information regarding the document.
Total Before Discount
Total amount of the A/P credit memo before the discount for the document is calculated.
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of the discount for the whole credit memo. The field on the right displays the amount
of the discount.
When the A/P credit memo is based on an A/P invoice with the discount on a document level, the discount is not copied to the
rows.
DPM %
In the field on the left, enter the percentage of down payment.
The field on the right displays the down payment amount. If required, you can change the values of these fields.
 Note
To enable separate discount and down payment percentages, go to Administration System Initialization Document
Settings . Open the Per Document tab, choose A/R Down Payment or A/P Down Payment from the Document dropdown
list, and then select the checkbox Separate Discount % and DPM % Fields.
Total Down Payment
Amount drawn from paid down payment invoices or down payment requests.
Freight
This is custom documentation. For more information, please visit SAP Help Portal. 157

6/8/26, 6:05 AM
This field appears if Manage Freight in Documents is selected in Administration System Initialization Document Settings
General .
You can define freight for the A/P credit memo. To open the Freight Charges window and to view the corresponding freight
charges, click .
Rounding
This field appears if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/P credit memo calculated according to the tax definitions.
WT Amount
Amount of withholding tax involved in the A/P invoice, if defined.
Total Credit
Total amount of the document including tax, freight and discounts.
Applied Amount
The actual amount that was copied from the base document to the A/P credit memo:
If the amount copied from the base document is smaller than or equals to the balance due amount at the base document,
this is the amount that is displayed in both Total Credit and Applied Amount fields.
If the amount copied from the base document is bigger than the balance due of the base document (this can be the case if
for example the base document is an A/P invoice that was partially paid, and the A/P credit memo that is now being
created is initiated due to returning of goods with value larger than the balance due of the A/P invoice), the value displayed
in the Applied Amount field is smaller than the total credit of the A/P credit memo. The difference between the applied
amount and the total credit is displayed in the Open Balance field.
Credit Balance
Open amount of the document.
Payment Order Run
If the checkbox is selected, it indicates that this document, or at least one of its installments, is included in a payment order run.
The checkbox is deselected in the following situations:
The payment order row that includes this document or its installment(s) is removed from the payment order run.
To remove a payment order row, in Payment Wizard: Step 6 - Recommendation Report, right-click the payment order row
and choose Remove. The checkbox for this payment order row is deselected in the selection column.
The payment order row that includes this document or its installment(s) is closed in the payment order run.
To close payment order rows in which all the documents are fully paid, in Payment Wizard: Step 6 - Recommendation
Report, choose the Close Payment Order Rows button. The Payment Order Status column displays C for the closed
payment order rows.
The payment order run that includes this document or its installment(s) is executed into a payment run.
This is custom documentation. For more information, please visit SAP Help Portal. 158

6/8/26, 6:05 AM
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/P Credit Memo
Purchasing Documents: Contents Tab
Use this tab to enter items or services that the company purchases from, and returns to, vendors, if required. The Contents tab is
identical in all the purchasing documents.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
item in SAP Business One.
The table view on this tab is different for each option.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 159

6/8/26, 6:05 AM
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents that were created before you upgrade to SAP Business One version 9.3.
Documents that are drawn from documents created before you upgrade to SAP Business One version 9.3.
 Note
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – Default value
By Documents – Summarizes rows with the same base documents into one row that displays the base document number
and reference. Items that appear in the table more than once, and have the same price and description, are summarized in
one row. This option is available only for documents of the type Item and when you copy rows from base documents.
By Items – Summarizes several item rows with the same item into one row. These item rows must have the same
parameters (for example, price, description, and warehouse). This option is available only for documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current purchasing document
only.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Quantity
Quantity that you want to order from the vendor based on the item’s purchasing unit of measure, as defined in the Item Master
Data window. If the purchasing unit of measure is defined as more than one item, the actual quantity of the item is displayed in the
Qty (Inventory UoM) field, which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
 Note
If the available quantity is less than the required quantity level (as defined in the Item Master Data window), SAP Business One
suggests replenishing the quantity.
This is custom documentation. For more information, please visit SAP Help Portal. 160

6/8/26, 6:05 AM
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Price is calculated automatically according to the specified gross price and
tax code and is not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
If the Unit Price is $10 as defined in the Item Master Data window, and the Items per Unit value is 5, the Unit Price in the
purchasing document is $50.
Press CTRL+TAB to view the Last Prices report.
Gross Price
Visible only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Editable only if the document price mode is Gross. Enter the unit price including tax, but before any discount.
When the price mode is Net, Gross Price is calculated automatically according to the specified unit price and tax code and is not
editable.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Enter in this field the unit price including tax. SAP Business One calculates automatically the unit price before tax and the tax
amount, based on the tax code in the row. After pressing the TAB key, the Unit Price field and the Tax/Unit field are updated
accordingly.
The tax amount is calculated as follows:
Gross Price / (1 + Tax %) * Tax % = Tax Amount
 Example
Gross Price = 150
Tax % = 20
Tax Amount = 150 / (1+ 0.2) * 0.2 = 25
 Recommendation
This is custom documentation. For more information, please visit SAP Help Portal. 161

6/8/26, 6:05 AM
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the
Unit Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit
Price and other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a purchasing unit of measure for the item as defined on the Purchasing Data tab in the
Item Master Data window, that is different than 1, the number of item units received by the warehouse equals the number
specified in the Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units received by the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Purchasing Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
The Items per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the credit memo does not affect the inventory quantity of the item.
In this case, only the inventory value of the item is adjusted if the quantity is positive.
 Example
You receive items from a vendor, but all the items were broken during shipment. You ask for a return of the payment and create
a credit memo, and by choosing this checkbox, indicate that there is no return of goods.
The field is available only in the following cases:
This is custom documentation. For more information, please visit SAP Help Portal. 162

6/8/26, 6:05 AM
A/P credit memos not based on other documents or
A/P credit memos based on an A/P invoice or
A/P credit memos based on an A/P reserve invoice, for which items have been received, and
If non-drop-ship warehouses are used
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Change Qty (Inv. UoM) Independently
You can enable this checkbox if you need to change the values in the Qty (Inventory UoM) field manually, independent of the
Quantity values, for example, for rounding purposes.
To use this checkbox, proceed as follows:
1. Define a UoM group for your item and include the predefined UoM Manual in the group.
For more information, see Setting Up Unit of Measure Groups.
2. Display the checkbox Change Qty (Inv. UoM) Independently.
a. Open an existing document or create a new document with your item. Choose the icon in the toolbar menu.
b. In the Form Settings window, choose the Table Format tab.
c. On the tab, find the option Change Qty (Inv. UoM) Independently and select the corresponding checkboxes in both
the Visible column and the Active column.
d. Choose OK.
3. On the Contents tab in your document, choose a row with your item.
4. In the UoM Code field, choose Manual. The checkbox Change Qty (Inv. UoM) Independently becomes available.
5. Select the checkbox for your item.
Now you can enter a quantity in the Qty (Inventory UoM) field manually, without affecting the Quantity value of the same
item.
Discount %
Percent of discount granted for the item.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
This is custom documentation. For more information, please visit SAP Help Portal. 163

6/8/26, 6:05 AM
The rules that are set in the Tax Code Determination – Setup window are inapplicable to purchase request reports, but are
applicable to purchase quotations and purchase orders created directly from the reports.
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Display the unit price including tax, taking into account the discount specified here.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according
to Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Total
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 164

6/8/26, 6:05 AM
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price
(on the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected: Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the vendor.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is
in force with the vendor and automatically relates it to the purchasing document. The unit price determined in the blanket
agreement is copied into the purchasing document, if in the blanket agreement, the Use BP Discount option is selected.
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated to bin locations.
You must allocate the same quantity of items to bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
This is custom documentation. For more information, please visit SAP Help Portal. 165

6/8/26, 6:05 AM
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In goods returns and A/P credit memos, for the document rows with items that are not managed by serials or batches, clicking
in the field opens the Bin Location Allocation - Issue Window instead.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries/regions that customers pay tax on the value of
the miles. By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Localization-Specific Info .
Project
Specify the project that you want to relate to the item.
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Consider Quantity
 Note
The field is available only if you have enabled fixed assets.
This is custom documentation. For more information, please visit SAP Help Portal. 166

6/8/26, 6:05 AM
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
If the asset is planned for quantity maintenance, enter the acquired quantity.
Table View for Document Type Service
Description
Enter a description of the purchased service.
G/L Account
Specify the G/L account to be debited (for an A/P invoice), or credited (for an A/P credit memo).
Project
Specify the project that you want to relate to the service.
WTax Liable
Indicates whether withholding tax applies in this document.
Freight in the header level is not affected, but those items at the row level are.
 Note
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to NO. You can select the value
manually from the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total
Total amount of the row in the relevant currency, calculated according to this formula:
Price x Exchange Rate – Discount for the Row (if defined).
Federal Tax ID
Specify the federal tax ID of the vendor in employee expenses reimbursement.
Expense Type
Specify the expense for use in employee expenses reimbursement.
Receipt Number
This is custom documentation. For more information, please visit SAP Help Portal. 167

6/8/26, 6:05 AM
Specify the receipt number for use in employee expenses reimbursement.
More Information
Creating Purchasing Documents
Alternative Items Window
Document Settings: General Tab
Last Prices Report
A/P Credit Memo: Logistics Tab
This tab contains details regarding the logistics aspects of the A/P credit memo.
To access the tab, choose Purchasing – A/P A/P Credit Memo Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Credit Memo Logistics Tab
Ship From
A/P credit memos of type Item: address defined for the warehouse linked to the Contents tab.
A/P credit memos of type Service: company address as defined in Administration System Initialization Company Details
General Local Language .
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . The system updates the address only for this marketing document; it does not affect the
warehouse address, the user defaults address, or the company details address.
Pay To
Vendor default pay-to address as defined in the business partner master data. If required, select a different address.
To change the address, from the dropdown list, select Bank. The fields display the vendor's bank address as specified in the
payment terms of the business partner master data.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the address IDs and address summaries of your vendor, as defined in the business partner master data. From the
dropdown list, select a destination address ID to which you deliver goods and services to your vendors for return. If required,
change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
affect the business partner master data.
Language
This is custom documentation. For more information, please visit SAP Help Portal. 168

6/8/26, 6:05 AM
Language defined for the business partner.
More Information
A/P Credit Memo
A/P Credit Memo: Accounting Tab
This tab contains information regarding the financial aspects of the A/P credit memo.
To access the tab, from the SAP Business One Main Menu, choose Purchasing – A/P A/P Credit Memo Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/P Credit Memo Accounting Tab Fields
Journal Remark
By default, displays A/P Credit Memos – XXX, where XXX is the vendor code. Change this content, if required.
Control Account
Specify the control account for the A/P credit memo. The default value is the Accounts Payable value in the business partner
master data.
 Note
The control account for a document-based A/P credit memo must be the same as that in the base document.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if its due date has already expired.
Payment Terms
Payment terms approved by the vendor and defined in the business partner master data.
Payment Method
Specify the payment method approved by the vendor and defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Start From
Specify when you initiate the payment:
Month End
Half Month
This is custom documentation. For more information, please visit SAP Help Portal. 169

6/8/26, 6:05 AM
Month Start
+Months...+Days
Specify the due date for an installment.
The calculation is based on the date of the order and the values specified in the payment terms. The payment period can be given
for the current month or for several months in the future, as well as for the number of days you specify in the last month of the
period.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document
is added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to
the current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
Specify a project name linked to the vendor in the business partner master data.
Indicator
The indicator linked to the vendor in the business partner master data.
Federal Tax ID
The company federal tax ID as defined in the company details: Administration System Initialization Company Details
Accounting Data .
Order Number
Specify the order number of the chain, when you use the direct distribution method. This number is recorded in the file that you
send to the head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
This is custom documentation. For more information, please visit SAP Help Portal. 170

6/8/26, 6:05 AM
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
A/P Credit Memo
Purchasing Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
This is custom documentation. For more information, please visit SAP Help Portal. 171

6/8/26, 6:05 AM
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
A/P Debit Memo
An A/P debit memo behaves in the same manner as an A/P invoice. You use A/P debit memos to document debts to your supplier
that are not part of your operating costs, for example, administrative fees or charges.
The prices in Last Purchase Price price list are updated when creating A/P debit memo.
To cancel A/P debit memo, use the A/P credit memo. The cancellation of A/P debit memo does not affect last purchase prices. For
more information see the page Canceling Sales and Purchasing Documents in the general online help file.
In addition, similar to A/P Invoice, once you enable the bin location function for a warehouse, you must record bin locations for all
receipts of inventory in the warehouse, including the processing of A/P debit memo.
Detailed information about A/P Invoice is available in the general help file in: Help Documentation Online Help , or by
choosing F1 from within the A/P Invoice window.
Creating Purchasing Documents
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P and select one of the documents, for example,
purchase order.
2. In the selected document, specify the vendor number, name, and other relevant general information.
3. Specify the required data on the following tabs:
Contents
Logistics
Accounting
4. Choose Add.
5. To confirm the system message and create a new purchasing document, choose one of the following options:
Add & New
Adds the document and opens a new window for you to create another document.
This is custom documentation. For more information, please visit SAP Help Portal. 172

6/8/26, 6:05 AM
It is similar to the previous Add button.
Add & View
Adds the document and displays it.
Add & Close
Adds the document and closes the window.
Your last choice will be remembered the next time you open the window of the given document.
 Note
If you are purchasing from a one-time vendor with whom you do not wish to place regular orders, enter the purchasing
document with a previously defined general master record, which is extended to include the data of the one-time
vendor.
 Note
If you create a no-charge A/P invoice, A/P credit memo, or A/P reserve invoice, a system message appears that gives
you the option of creating a document with a zero total amount. To continue and create such a document, choose OK.
When you are creating a purchasing document, you can move all the rows in the Contents tab up and down if the tab
doesn’t include the following items:
Sales type of Bill of Materials (BOMs).
Alternative items.
Subtotal type of rows.
When you are editing an open purchasing document which doesn't create posting, for example, a purchase order, you can
move all the rows in the Contents tab up and down if the tab doesn’t include the following items:
Sales type of Bill of Materials (BOMs).
Partially or fully closed items or services.
Alternative items.
Purchasing Documents
The following table summarizes the differences between the purchasing documents:
Purchasing Documents
Purchase Order Goods Receipt PO A/P Invoice
Official document/internal Internal (depending on your line Official Official
character of business)
Does the purchasing document Depending on your line of Depending on your line of Yes
have to be created in SAP business business
Business One?
Can the purchasing document Yes No No
be amended after it has been
entered?
This is custom documentation. For more information, please visit SAP Help Portal. 173

6/8/26, 6:05 AM
Purchasing document for Not necessary Goods Returns A/P Credit Memo
correction
Does the purchasing document No Yes Depends (1)
cause quantities to be posted in
inventory management?
Does the purchasing document No Yes (2) Yes
cause values to be posted in
Accounting?
Reference when entering Purchase Order Goods Receipt PO, Purchase
Order
1. When you enter an A/P invoice with reference to a goods receipt PO, SAP Business One does not post any changes to
inventory. If you create the A/P invoice without reference to a goods receipt PO, SAP Business One posts inventory changes
with the incoming invoice.
2. Entering a goods receipt for a purchase order results in a posting in the accounting system, because the inventory
quantities are changed as a result of the delivery for the purchase order. Inventory cannot be changed without a posting in
the Perpetual Inventory System.
 Note
The data that you store for purchasing documents must be identical to the data in the documents that you receive from the
vendor.
If there are differences between the data in your system and the data in the vendor’s document, you must clarify these
differences with the vendor. This may be the case if a vendor invoices you for an amount other than the one entered in the
purchase order. The details in the vendor’s document are legally binding.
For legal reasons, you cannot delete or amend a purchasing document that results in a relevant posting in the accounting system.
If such a purchasing document has to be amended or cancelled, you must enter a clearing transaction.
More Information
Purchasing – A/P
Multiple Shipping Addresses in Purchasing Documents
Context
You can add an Address column to purchasing documents to view and manage multiple shipping addresses.
Procedure
1. Display a purchasing document.
2. In the toolbar, click .
The Form Settings window appears.
3. On the Table Format tab, select Address Visible .
This is custom documentation. For more information, please visit SAP Help Portal. 174

6/8/26, 6:05 AM
The column appears as follows:
Item type documents – by default displays the shipping address of the warehouse from the first line in the
document.
Service type documents – by default displays the company address.
4. To display multiple addresses, choose Document Editing and add an address field to the document line in the editing
window.
Related Information
Creating Purchasing Documents
QR Codes and Purchasing Documents
QR (Quick Response) Codes can be displayed on marketing documents that are created by SAP Business One. QR Codes are
required by law on marketing documents in some jurisdictions. Companies can use QR Codes on marketing documents as a
convenient and customer-friendly way to provide more information.
QR Codes can link to anything that may be required but are typically a link to a webpage that displays information relevant to the
document.
Set up and Process
The following sections describe the set up and process in marketing documents for displaying QR Codes.
General Settings
A tab labeled QR Codes is available in General Settings. You can vary the technical details of QR Codes at the point of generation
by using the settings on QR Codes in General Settings. After changes are made in QR Codes in General Settings, the changes are
only effective for QR Codes if documents are updated or created.
1. From the SAP Business One Main Menu, choose Administration System Initialization General Settings QR Codes
tab .
2. Determine the size of QR Codes by entering numbers between 1 and 40 in the fields Version - Min. Size and Max. Size. To
produce consistently sized QR Codes, you can enter the same number in both fields. Placing an upper limit on the size of
QR Codes restricts the amount of information that can be taken from the field Create QR Code From to create QR Codes.
3. Enter a number between 1 and 20 in Scale (pixels per module) to determine how many pixels are in a square of a bitmap in
the PNG file.
4. Select the checkbox QR Code Expiration to automatically remove QR Codes from the database in a specified number of
days, entered in Expiration Days. Expiration dates are calculated and potentially recalculated from the last update of a
document.
5. Redundant correction bytes are included and vary by the chosen Correction Level of created QR Codes. Choosing a setting
of "High" means that less information can be included in the QR Code but that the QR Code can be read and printed more
easily with less potential for error. Choosing a setting of "Low" means that more information can be included in the QR
Code but that the QR Code can be read and printed less easily with more potential for error.
Marketing Documents
The field Create QR Code From is available on the Accounting tab of marketing documents, for example on A/P invoices. The
information entered in Create QR Code From is used as the source from which QR Codes are saved in system tables and
This is custom documentation. For more information, please visit SAP Help Portal. 175

6/8/26, 6:05 AM
transformed into PNG (Portable Network Graphic) images. Information can be added manually to Create QR Code From, by using
a formula in a formatted search, by DI API input, or by SAP Business One Service Layer on Windows (not on Linux). The source for
QR Codes can also be user-defined fields that are called by API. The information entered into Create QR Code From can be
anything that customers require but is typically a link to a webpage that displays information relevant to the document. You can
display QR Code images on print layouts of marketing documents. Print layouts must be manually adjusted to include QR Code
images based on joined data sources in the system.
1. From the SAP Business One Main Menu, choose Purchasing - A/P A/P Invoice Accounting tab .
2. Enter a link to a webpage for your company in Create QR Code From.
3. Add the A/P invoice to the system to trigger the generation of a QR Code.
 Note
For more information on QR Codes, example queries, and Crystal Report files, see SAP Note 2889899 .
Managing Freight Charges
SAP Business One enables you to manage freight so that you can track any additional costs in sales and purchasing transactions.
Freight charges could include insurance, shipment, and other costs that apply to your goods.
You can add freight in the document or row level. When you do, the total amount of the document is updated accordingly. If you
manage your inventory using perpetual inventory, you can add the value of freight charges in purchasing documents to the cost of
your goods. In addition, you can define whether the last purchase price of your items includes the freight charges that apply to
your purchased goods.
You can print freight and generate various reports for analyzing it.
Prerequisites
In the Freight - Setup window, you have defined the freight you plan to apply to your sales and purchasing documents.
On the G/L Account Determination: Inventory Tab, you have defined an offsetting G/L account for the inventory account for
clearing journal entries created by A/P invoices and goods receipt POs.
On the G/L Account Determination: Purchase Tab, in the Expense Account: Variance Account field, you have defined a
variance G/L account for clearing journal entries created by A/P credit memos based on A/P invoices or by goods returns
based on goods receipt POs in which the freight charges amount was changed.
In the Cash Discount window, by selecting or clearing the Freight checkbox for every cash discount defined in your
company, you have decided whether the discount amount calculated on the invoice total includes freight.
Localization-specific fields, all Europe: For the Output Tax Group and Input Tax Group, you have chosen relevant tax groups
and selected the WT Liable option to apply withholding tax on freight.
Process
Freight in Sales and Purchasing
You can apply freight to both sales and purchasing documents. However, only freight charges in purchasing documents may affect
item cost and the last purchase price.
You can apply freight on:
This is custom documentation. For more information, please visit SAP Help Portal. 176

6/8/26, 6:05 AM
Row level – up to three different types of freight charges on individual document rows
Total level – the entire document
Drawing Base Documents with Freight Charges to Target Documents
When you draw a base document to a target document, the Draw Document Wizard appears and enables you to copy the required
data. In different steps of the wizard, make the necessary settings for copying the row level and the total level freight.
Example
Prerequisites
1. You manage perpetual inventory by standard price.
2. The vendor, item, and freight charges are exempted from tax.
3. There is one additional freight charge at the total level.
| 4. The freight is defined as  | Stock    Yes | .   |     |
| ----------------------------- | ------------ | --- | --- |
5. The standard price of the item and the price in the document are USD 100.
6. The freight amount is USD 10.
Goods Receipt PO
| G/L Acc./BP Code   | Name               | Debit      | Credit     |
| ------------------ | ------------------ | ---------- | ---------- |
| 23000000-01-001-01 | Allocation 1       |            | USD 100.00 |
| 19200000-01-001-01 | Freight Clearing 1 |            | USD 10.00  |
| 52300000-01-001-01 | Variance 1         | USD 10.00  |            |
| 13500000-01-001-01 | Stock 1            | USD 100.00 |            |
|                    |                    | USD 110.00 | USD 110.00 |
Goods Returns and Goods Returns Based on a Goods Receipt PO
| G/L Acc./BP Code   | Name               | Debit       | Credit      |
| ------------------ | ------------------ | ----------- | ----------- |
| 23000000-01-001-01 | Allocation 1       |             | USD -100.00 |
| 19200000-01-001-01 | Freight Clearing 1 |             | USD -10.00  |
| 52300000-01-001-01 | Variance 1         | USD -10.00  |             |
| 13500000-01-001-01 | Stock 1            | USD -100.00 |             |
|                    |                    | USD -110.00 | USD -110.00 |
A/P Invoice Based on a Goods Receipt PO
| G/L Acc./BP Code | Name | Debit | Credit |
| ---------------- | ---- | ----- | ------ |
This is custom documentation. For more information, please visit SAP Help Portal. 177

6/8/26, 6:05 AM
| V6970              | Vendor             |            | USD 110.00 |
| ------------------ | ------------------ | ---------- | ---------- |
| 19200000-01-001-01 | Freight Clearing 1 | USD 10.00  |            |
| 23000000-01-001-01 | Allocation 1       | USD 100.00 |            |
|                    |                    | USD 110.00 | USD 110.00 |
A/P Invoice
| G/L Acc./BP Code   | Name       | Debit      | Credit     |
| ------------------ | ---------- | ---------- | ---------- |
| V6970              | Vendor     |            | USD 110.00 |
| 52300000-01-001-01 | Variance 1 | USD 10.00  |            |
| 13500000-01-001-01 | Stock 1    | USD 100.00 |            |
|                    |            | USD 110.00 | USD 110.00 |
A/P Credit Memo Based on Goods Returns
| G/L Acc./BP Code   | Name               | Debit       | Credit      |
| ------------------ | ------------------ | ----------- | ----------- |
| V6970              | Vendor             |             | USD -110.00 |
| 19200000-01-001-01 | Freight Clearing 1 | USD -10.00  |             |
| 23000000-01-001-01 | Allocation 1       | USD -100.00 |             |
|                    |                    | USD -110.00 | USD -110.00 |
A/P Credit Memo and A/P Credit Memo Based on A/P Invoice
| G/L Acc./BP Code   | Name       | Debit       | Credit      |
| ------------------ | ---------- | ----------- | ----------- |
| V6970              | Vendor     |             | USD -110.00 |
| 52300000-01-001-01 | Variance 1 | USD -10.00  |             |
| 13500000-01-001-01 | Stock 1    | USD -100.00 |             |
|                    |            | USD -110.00 | USD -110.00 |
A/P Credit Memo Based on A/P Invoice – Changing the Freight Charge Amount
The scenario illustrates a situation in which the freight charge amount changes when you copy an A/P invoice into an A/P credit
memo. The freight charge amount in the A/P invoice is USD 10. The freight charge amount in the A/P credit memo is USD 0.
| G/L Acc./BP Code   | Name              | Debit | Credit      |
| ------------------ | ----------------- | ----- | ----------- |
| V6970              | Vendor            |       | USD -100.00 |
| 63500000-01-001-01 | Variance Expenses |       | USD -10.00  |
This is custom documentation. For more information, please visit SAP Help Portal. 178

6/8/26, 6:05 AM
| 52300000-01-001-01 | Variance 1 | USD -10.00              |     |
| ------------------ | ---------- | ----------------------- | --- |
| 13500000-01-001-01 | Stock 1    | USD -100.00             |     |
|                    |            | USD -110.00 USD -110.00 |     |
The variance expense G/L account is used to clear the differences, since the vendor account is not cleared.
Closing a Goods Receipt PO or a Goods Return
When you close a goods receipt PO or a goods return ( Data     Close ), no inventory posting is registered. However, a journal
entry is created to clear the allocation and the freight clearing accounts.
| G/L Acc./BP Code   | Name                    | Debit      | Credit     |
| ------------------ | ----------------------- | ---------- | ---------- |
| 23000000-01-001-01 | Allocation 1            | USD 100.00 |            |
| 19200000-01-001-01 | Add. Expense Clearing 1 | USD 10.00  |            |
| 10000111-02-001-01 | Goods Clearing 1        |            | USD 110.00 |
|                    |                         | USD 110.00 | USD 110.00 |
  Note
The freight clearing G/L account clears the inventory account along with the allocation costs account.
If there is a discrepancy between the amount recorded in the vendor account and that in the inventory account, the variance
G/L account is used in the journal entry.
Adjusting Freight Amounts in Goods Receipts PO Based on A/P
Reserve Invoices
When creating a goods receipt PO (GRPO) based on A/P reserve invoices, you can adjust the freight amounts in the Freight
Charges window. The prerequisite for adjustment is that each freight row (each freight item of a base document takes up one row
in the Freight Charges window) does not exceed the unallocated freight charge.
In a perpetual inventory system, the following adjustments trigger discrepancies in stock value. The discrepancies are posted to
the price difference account:
A row is partly copied to the GRPO and the freight distributed to the row exceeds that in the base invoice.
All remaining open quantity of a row is copied to the GRPO and the newly distributed freight is different from the original
distribution.
The total freight in the GRPO is lower than those in the base invoice.
We provide some simple examples to illustrate the cases above respectively. All freight items in the examples affect stock value.
The base A/P reserve invoice contains the following data:
This is custom documentation. For more information, please visit SAP Help Portal. 179

6/8/26, 6:05 AM
| Row Number | Quantity | Value | Distributed Freight |
| ---------- | -------- | ----- | ------------------- |
| 1          | 5        | 500   | 20                  |
| 2          | 10       | 1000  | 35                  |
Example 1
Copy the base invoice to a GRPO, partly copy the first row, and make adjustment as follows:
| Row Number (Base) | Quantity | Value   | Distributed Freight |
| ----------------- | -------- | ------- | ------------------- |
| 1                 | 4        | USD 400 | 25                  |
Posting
| Account                  | Debit   | Credit  |     |
| ------------------------ | ------- | ------- | --- |
| Stock in transit account |         | USD 420 |     |
| Inventory account        | USD 425 |         |     |
| Price difference account |         | USD 5   |     |
Example 2
Copy the base invoice to a GRPO, fully copy the first row, and make adjustment as follows:
| Row Number (Base) | Quantity | Value   | Distributed Freight |
| ----------------- | -------- | ------- | ------------------- |
| 1                 | 5        | USD 500 | 15                  |
Posting
| Account                  | Debit   | Credit  |     |
| ------------------------ | ------- | ------- | --- |
| Stock in transit account |         | USD 520 |     |
| Inventory account        | USD 515 |         |     |
| Price difference account | USD 5   |         |     |
Example 3
Fully copy the base invoice to a GRPO and make adjustment as follows:
| Row Number (Base) | Quantity | Value    | Total Freight |
| ----------------- | -------- | -------- | ------------- |
| 1                 | 5        | USD 500  | 50            |
| 2                 | 10       | USD 1000 |               |
Posting
This is custom documentation. For more information, please visit SAP Help Portal. 180

6/8/26, 6:05 AM
Account Debit Credit
Stock in transit account USD 1555
Inventory account USD 1550
Price difference account USD 5
Freight Charges Window
This window displays the freight defined in the Freight - Setup window. It enables you to make changes that are relevant for the
current sales or purchasing document.
To access the window, choose Sales – A/R or Purchasing - A/P and open any document. Click in the Freight field.
 Note
This window appears only if you have selected Manage Freight in Documents on the General tab of the Document Settings
window Administration System Initialization Document Settings ).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Freight Charges Window
Do Not Display Freight Charges with Zero Amount
Hides freight with zero amount.
Tax Code
Tax code related to the freight.
 Note
In European localizations, this field is labeled Tax Group.
Total Tax Amount
Total tax amount of the freight.
Externally Calculated Tax Rate
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays the externally calculated tax rate edited through the DI API or Service Layer.
 Note
This value is for informative purposes only and is not used in any system calculations.
Externally Calculated Tax Amount
This is custom documentation. For more information, please visit SAP Help Portal. 181

6/8/26, 6:05 AM
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays the externally calculated tax amount edited through the DI API or Service Layer.
Source of Tax Amount
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Displays whether the tax amount is an internal system calculation or external calculation (edited through the DI API or Service
Layer).
Distrib. Method
Distribution method defined for freight in the Freight - Setup window.
Any changes you make are relevant for the current document only and do not affect the original definition.
Net Amount
Freight amount excludes tax.
When the Gross Freight checkbox is unselected in the Freight – Setup window, the default value of this field is the amount
specified in the Fixed Amount field in the Freight – Setup window.
When you update the value in the this field, the value in the Gross Amount field is updated automatically according to the
predefined tax group.
Any changes you make are relevant for the current document only and do not affect the original definition of the freight.
Status
Displays one of the following:
O – Open. Freight charge status when document is open, for example, not drawn to another document or closed manually.
C – Closed. Freight charge status when the document was drawn to a target document or closed manually.
Gross Amount
Freight amount includes tax.
When the Gross Freight checkbox is selected in the Freight – Setup window, the default value of this field is the amount specified
in the Fixed Amount field in the Freight – Setup window.
When you update the value in this field, the value in the Net Amount field is updated automatically according to the predefined tax
group.
Any changes you make are relevant for the current document only and do not affect the original definition of the freight.
Project
Specify the project that you want to relate to the freight. If you defined the project for the freight in the Freight-Setup window, the
field displays the project code by default.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 182

6/8/26, 6:05 AM
Freight - Setup Window
Copying Sales and Purchasing Documents
SAP Business One enables you to create target documents directly from base documents. For example, you can create a delivery
directly from the sales order. In that case, all the data that you entered in the sales order is automatically copied to the delivery.
You can create a target document for an added document in status Open only. When you create a target document, SAP Business
One copies all its open rows.
 Note
When you work with an All currency business partner and perform the transaction in a currency different from the default one,
the system selects this currency in the relevant target document.
Procedure
John, the sales employee, submits a sales quotation for one of his customers. A week later, the customer calls and wants to order
the selected items. John copies the sales quotation to a sales order.
1. Choose Sales - A/R Sales Quotation .
The Sales Quotation window appears.
2. Find the relevant sales quotation for the customer.
3. Choose Copy To Order .
The Sales Order window appears with the copied details of the sales quotation.
4. Update the sales order, if necessary, and choose Add.
Two days later, the ordered items arrive. John opens the Delivery window to create a delivery and to send the items to the
customer.
1. Choose Sales - A/R Delivery .
The Delivery window appears.
2. Enter the code or name of the customer.
3. Choose Copy From Orders and select the relevant sales order.
The Draw Document Wizard appears. For more information, see Drawing Document Wizard.
4. Update the delivery, if necessary, and choose Add.
Result
You have created the relevant documents.
 Note
When you copy one or more base documents to a target document, SAP Business One observes the following rules:
If all base documents have the same value, that value is copied to the target document.
This is custom documentation. For more information, please visit SAP Help Portal. 183

6/8/26, 6:05 AM
If base values are different, the default value from the business master data is used.
If no default value exists for the business partner, no value is copied to the target document.
More Information
Copying Sales Documents
Copying Purchasing Documents
Copying Purchasing Documents
The information below shows which base document you can use to create a particular target document, and vice versa.
Copy To Documents
Base Document Target Document
Purchase Blanket Agreement Purchase Quotation
Purchase Order
Goods Receipt PO
A/P Down Payment Request
A/P Down Payment Invoice
 Note
A/P invoices are not available because they open without a
default posting date, and thus the validity of the purchasing
blanket agreement cannot be verified.
Purchase Request Purchase Quotation
Purchase Order
Purchase Quotation Purchase Order
Goods Receipt PO
A/P Invoice
A/P Reserve Invoice
Purchase Order Goods Receipt PO
A/P Invoice
Goods Receipt PO A/P Invoice
Goods Return
Goods Return A/P Credit Memo
A/P Invoice A/P Credit Memo
A/P Reserve Invoice A/P Credit Memo
This is custom documentation. For more information, please visit SAP Help Portal. 184

6/8/26, 6:05 AM
Copy From Documents
Target Document Base Document
Purchase Quotation Purchase Request
Blanket Agreement
Purchase Order Purchase Request
Purchase Quotation
Blanket Agreement
Goods Receipt PO Purchase Quotation
Purchase Order
Goods Return
A/P Reserve Invoice
Blanket Agreement
Goods Return Goods Receipt PO
A/P Invoice Purchase Quotation
Purchase Order
Goods Receipt PO
A/P Credit Memo A/P Invoice
Goods Return
A/P Down Payment
A/P Debit Memo A/P Invoice
Goods Return
A/P Down Payment
A/P Reserve Invoice Purchase Quotation
Purchase Order
A/P Down Payment Request Purchase Quotation
Purchase Order
Goods Receipt PO
Blanket Agreement
A/P Down Payment Invoice Purchase Quotation
Purchase Order
Goods Receipt PO
Blanket Agreement
More Information
Copying Sales and Purchasing Documents
This is custom documentation. For more information, please visit SAP Help Portal. 185

6/8/26, 6:05 AM
Updating and Deleting Posted Purchasing Documents
Some purchasing documents such as A/P invoices or goods receipt POs are legally binding. Therefore, you cannot delete them or
make any changes that affect inventory entries or journal entries after you created these documents in SAP Business One.
However, you can change data that is not relevant for inventory or journal entries. For example, if you wish to postpone the
payment date of an invoice or the payment method.
Prerequisites
You have full authorization to modify posted A/P documents (check under Administration System Initialization
Authorizations Purchasing ).
Activities
You can modify the following data in A/P invoices, A/P down payment requests, A/P down payment invoices, A/P reserve invoices,
and A/P credit memos after posting them in SAP Business One:
Due date (if the document was not partially or fully copied into another document, or partially or fully paid)
Payment method (if the document was not partially or fully copied into another document, or partially or fully paid)
Pay-to data (if the document was not partially or fully copied into another document, or partially or fully paid)
Sales employee (can be changed anytime)
Buyer (can be changed anytime)
Owner (can be changed anytime)
Lines of text (can be changed anytime)
Furthermore, it is possible to modify data in goods receipt POs and goods returns. You can change the following data:
Payment terms (if the document was not partially or fully copied into another document, or partially or fully paid)
Payment method (if the document was not partially or fully copied into another document, or partially or fully paid)
Pay-to data (if the document was not partially or fully copied into another document, or partially or fully paid)
Sales employee (can be changed anytime)
Buyer (can be changed anytime)
Owner (can be changed anytime)
Lines of text (can be changed anytime)
You can also change the due date of any open installments (unreconciled, not yet fully or partially paid installments) in A/R
invoices and A/R reserve invoices.
To modify the documents, find the relevant purchase document, modify the data, and choose Update.
The changes you make are tracked in the SAP Business One change log. When you print an already posted purchasing document
after you made some changes to it, the printout includes all modifications and the title “Amended”.
Canceling Sales and Purchasing Documents
This is custom documentation. For more information, please visit SAP Help Portal. 186

6/8/26, 6:05 AM
If a marketing document is added in error, has become invalid, or has no concrete transactions associated with it, you can cancel
the document but still store it in the database. In some countries, it is even legally binding to cancel such documents instead of
closing them (when the closing approach is available, for example, for deliveries) or deleting them from the database.
 Note
If you want to indicate in your print layouts whether or not a document is canceled, or that a document is a cancellation
document, you can make use of the database field “Cancelled”. You can use this field when designing both PLD and Crystal
Reports layouts. The valid values for this field are listed below:
Y (Yes): Indicates a canceled document.
N (No): Indicates that the document is not canceled.
C (Cancellation): Indicates a cancellation document.
Prerequisites
You have full authorization for canceling documents. Note that there are separate authorizations for different cancellation types
that are introduced below.
Cancellation Types
The cancellation of sales and purchasing documents falls into the following two categories:
Cancellation that does not generate new documents
Relevant documents are listed in the table below. In this category, cancellation of a document merely sets its status to
“Cancelled”. For more information, see Updating Sales Quotations, Updating and Cancelling Sales Orders, Closing,
Canceling, and Removing Purchase Quotations, and Canceling Purchase Orders.
Sales Document Purchasing Document
Sales quotation Purchasing quotation
Sales order Purchasing order
A/R down payment request A/P down payment request
Purchase request
Return request Goods return request
Cancellation that generates cancellation documents
 Note
In this category, you cannot cancel documents added prior to SAP Business One version 9.0 or any documents based on
them.
Relevant documents are listed in the table below:
This is custom documentation. For more information, please visit SAP Help Portal. 187

6/8/26, 6:05 AM
Sales Document Purchasing Document
Delivery Goods receipt PO
Return Goods return
A/R invoice A/P invoice
A/R reserve invoice A/P reserve invoice
A/R credit memo A/P credit memo
 Note
Landed costs documents cannot be canceled. Nevertheless, if you manage perpetual inventory, you can achieve the
same result of clearing by creating a new landed costs document fully based on the old one.
You cannot cancel A/R or A/P down payment invoices, either.
In this category, canceling a document results in the following changes:
A cancellation document is created. The data of the canceled document is copied to the cancellation document and
only some data is allowed to be updated.
Both canceled and cancellation documents are closed irreversibly.
The system reverses the accounting, tax, and inventory changes caused by the canceled document.
The system removes the automatic reconciliation between the canceled document and its base documents, if any.
Consequently, the base documents are reopened with balances due restored and can be drawn further to new target
documents.
 Note
Additional documents other than the cancellation document may also be automatically created upon the cancellation of
a marketing document. For more information, see Canceling Documents with Fixed Assets.
 Note
Cancellation of a document does not affect last purchase prices, that is, adding a cancellation document neither
updates nor reverts the Last Purchase Price list.
Related Information
Canceling Documents with Cancellation Documents
Canceling Documents with Cancellation Documents
 Note
You cannot create a draft cancellation document, nor cancellation documents, using the document generation wizard.
Prerequisites
You have full authorization for canceling documents with cancellation documents.
This is custom documentation. For more information, please visit SAP Help Portal. 188

6/8/26, 6:05 AM
You are still within the time range allowed for cancellation after posting the document.
The time range is determined by your definition of the Max. No. of Days for Canceling Marketing Documents Before or
After Posting field in the Document Settings window. For more information, see Document Settings: General Tab.
Procedure
1. Find the particular document you want to cancel.
2. Right-click in the document window and choose Cancel, or choose Data Cancel . A cancellation document appears
with the title <Document Type> - Cancellation.
3. In the cancellation document window, make the necessary data updates.
 Recommendation
Define at least one cancellation series in advance and use a document number of a cancellation series. For more
information, see the description of the Cancellation checkbox at Series - Document - Setup.
4. Choose the Add pushbutton.
The following figure illustrates the cancellation of an A/R invoice based on deliveries:
Editable Fields when Creating a Cancellation Document
When creating a cancellation document (in Add mode), you can edit the following data:
Document numbering series, and numbers of the manual series
Posting Date
Due Date
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 189

6/8/26, 6:05 AM
The due date is automatically updated according to the posting date and payment terms. If there is only one
installment, you can edit the Due Date field directly. If there is more than one installment, you change the due date by
changing the posting date and the installment settings of the payment terms.
Document Date
Remarks
Attachments
After a cancellation document is added, you can edit as much data as for other closed documents of the same document type.
Related Information
Cancellation of Documents with Serial Number and Batch-Managed Items
Cancellation of Documents with Items Stored in Bin Location
Cancellation of Documents Involving Down Payments
Canceling Documents with Fixed Assets
Posting for Canceling Documents with FIFO Items
Reporting for Canceled and Cancellation Documents
Cancellation of Documents with Serial Number and Batch-
Managed Items
If a document contains serial number or batch-managed items, canceling the document follows the rules below:
Cancel an outbound transactional document:
If a serial number or batch is not yet returned, it is automatically selected for the cancellation document and you
cannot deselect it.
If a serial number or batch is already returned, you must select another serial number or batch to replace it.
Cancel an inbound transactional document:
If a serial number or batch is still available for issue, it is automatically selected for the cancellation document and
you cannot deselect it.
If a serial number or batch is already issued, you must select another serial number or batch to replace it.
If customer equipment cards are created upon delivery or invoicing of serial number-managed items, the cancellation
documents are recorded in the cards after the cancellation of the delivery or A/R invoice. Note that this rule is irrelevant to
A/R invoices based on deliveries – these A/R invoices do not generate customer equipment cards. For more information,
see Enabling the Automatic Creation of Customer Equipment Cards.
For information about canceling documents with serial number and batch-managed items in bin locations, see Canceling
Documents with Items Managed by Bin Location.
Example
The following example illustrates the second situation of canceling an outbound transactional document:
1. Create a delivery for item S. Deliver 2 items S with serial numbers x1001 and x1002, respectively.
2. Create a return for item S with the serial number x1001.
This is custom documentation. For more information, please visit SAP Help Portal. 190

6/8/26, 6:05 AM
3. Try to cancel the delivery and add the cancellation document.
The Serial Number Selection window appears. Only serial number x1002 is automatically selected and cannot be
deselected.
4. Create a new serial number or select an available serial number.
You can add the cancellation document now.
Related Information
Cancellation of Documents with Items Stored in Bin Location
Cancellation of Documents with Items Stored in Bin Location
If a document contains items stored in bin location, canceling the document follows the rules below:
Bin locations in the existing document are automatically selected for the cancellation document, but you can always
change the bin location allocation method for regular items. For serial number or batch-managed items, you can change
the bin locations only when you are canceling an outbound transaction.
When canceling an outbound transactional document, one or more bin locations may not be able to receive items back due
to various restrictions on the bin locations. Under such circumstances, you must manually select other appropriate bin
locations to receive the returned items. Note that in this scenario, the system does not automatically allocate items to
receiving or default bin locations.
When canceling an inbound transactional document, if one or more bin locations do not have sufficient items to issue, you
must manually select items from other appropriate bin locations. Note that in this scenario, the system does not
automatically allocate items from bin locations according to the rules for relevant warehouses.
 Note
If you are canceling a document that contains serial number or batch-managed items and some of the items have been
allocated to other bin locations (for example, first delivered and then returned to different bin locations), these items are
still automatically selected and you cannot select other items to replace them.
Example
The following example concerns a bin location WH001-B001 that is restricted in terms of transactions:
1. Restrict bin location WH001-B001 in the following way:
a. From the SAP Business One Main Menu, choose Administration Setup Inventory Bin Locations Bin
Location Master Data and find the bin location B001.
b. From the Transaction Restriction dropdown list, select Outbound Transactions.
c. Choose the Update pushbutton.
2. Create a goods receipt PO for item I001. Receive 100 units of item I001 into bin location WH001-B001.
3. Try to cancel the goods receipt PO and add the cancellation document without changing the bin location allocation.
You are prevented from adding the cancellation document because bin location WH001-B001 cannot be used for issuing
items to business partners.
4. Reallocate the items to appropriate bin locations.
This is custom documentation. For more information, please visit SAP Help Portal. 191

6/8/26, 6:05 AM
You can add the cancellation document now.
Cancellation of Documents Involving Down Payments
This topic deals with the following sales and purchasing documents:
Invoices, including reserve invoices
Credit memos
 Note
Depending on your SAP Business One localization, you pay for the down payment invoice in either of the following ways:
Direct payment: Create a payment based on the down payment invoice
Indirect payment: Create a down payment invoice based on a paid down payment request
If a credit memo is based purely on unpaid down payment invoices, there is no actual down payment involved. Accordingly, this
topic does not consider this type of credit memo.
The following table lists the cancellation rules for different scenarios:
Document to Be Base Document Cancelable Scenarios Down Payment Status After
Canceled Cancellation
Invoice / Either condition is met: Reopened
The invoice is not the base
document of any other
document.
The invoice's target
documents are all canceled
or, in the case of correction
invoice, reversed.
Credit memo Invoice The credit memo does not credit any Remains closed
drawn down payment.
 Note
To credit down payments drawn to
an invoice, in the credit memo
window, click the Total Down
Payment field and keep the drawn
down payments selected in the
Down Payments to Draw window.
Credit memo Indirectly paid down payment Both conditions are met: Reopened
invoice
The base down payment
request has not been recopied
to another down payment
invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 192

6/8/26, 6:05 AM
Document to Be Base Document Cancelable Scenarios Down Payment Status After
Canceled Cancellation
The base down payment
request has not been drawn
to any invoice or reserve
invoice.
Canceling Documents with Fixed Assets
As of SAP Business One 9.0, you can record transactions of fixed assets in marketing documents. You can cancel the marketing
documents with fixed assets shown in the table below. Creating these marketing documents results in the creation of fixed asset
documents. Therefore, when canceling these documents, the corresponding fixed asset documents are also canceled.
Marketing Document Fixed Asset Document
A/P invoice Capitalization
A/P credit memo Capitalization credit memo
A/R invoice Retirement
Canceling marketing documents with fixed assets may result in a status change of the fixed assets. For example, if a fixed asset
has been fully retired with an A/R invoice, cancellation of this A/R invoice resets the fixed asset status from Inactive to Active
; and if you made the first acquisition of a fixed asset with an A/P invoice, cancellation of this A/P invoice resets the fixed asset
status from Active to New.
Cancellation Rules
You can cancel a marketing document with fixed assets after you have canceled all the following documents sequentially from the
latest asset value date:
Marketing documents and payments based on this marketing document
Subsequent manual depreciations of these fixed assets
 Note
Subsequent automatic depreciations as a result of depreciation runs do not prevent you from canceling marketing
documents with fixed assets. Therefore, you are recommended to execute another depreciation run to adjust the fixed
asset value after cancellation.
Subsequent fixed asset documents of these fixed assets, including capitalizations, capitalization credit memos, and
retirements
Posting for Canceling Documents with FIFO Items
Due to the accounting principles of the FIFO valuation method, canceling a document with FIFO items may trigger a special
posting: if the document contains FIFO items whose warehouses are different from those in the base documents and the item
costs in the warehouses are different, the price difference account and COGS (cost of goods sold) account cannot be reverted to
the original balances by cancellation.
This is custom documentation. For more information, please visit SAP Help Portal. 193

6/8/26, 6:05 AM
Prerequisites
On the Basic Initialization tab of the Company Details window, you have selected the following checkboxes:
Use Perpetual Inventory
Manage Item Cost per Warehouse
Procedure
1. A FIFO item F001 is received into two different warehouses with different prices (costs).
| Warehouse | Price | Quantity |     |
| --------- | ----- | -------- | --- |
| WH01      | USD 5 | 10       |     |
| WH02      | USD 1 | 10       |     |
2. Create a return for item F001.
| Warehouse | Price  | Quantity |     |
| --------- | ------ | -------- | --- |
| WH02      | USD 50 | 2        |     |
3. Copy the return fully to a delivery but change the warehouse to warehouse WH01.
Posting
| Account                    |     | Debit | Credit |
| -------------------------- | --- | ----- | ------ |
| Inventory Account          |     |       | $ 10   |
| Price Difference Account   |     | $ 8   |        |
| Cost of Goods Sold Account |     | $ 2   |        |
4. Cancel the delivery.
Posting
| Account                    |     | Debit | Credit |
| -------------------------- | --- | ----- | ------ |
| Inventory Account          |     | $ 10  |        |
| Cost of Goods Sold Account |     |       | $ 10   |
In step 3, the system revalues item F001 by its cost in the warehouse in the target document instead of using its cost in the
warehouse in the base document. In step 4, as there is no price difference for item F001 in the same warehouse WH01, the system
credits additional USD 8 to the COGS account.
Reporting for Canceled and Cancellation Documents
This is custom documentation. For more information, please visit SAP Help Portal. 194

6/8/26, 6:05 AM
In the Document Settings window, by selecting and deselecting the Display Cancelled and Cancellation Marketing Documents in
Reports checkbox, you can determine whether or not to report cancelled and cancellation documents. However, certain reports
are exempt from the setting of this checkbox: some always report canceled and cancellation documents, and the others never
report canceled and cancellation documents.
 Note
If a canceled document and its cancellation document have different posting dates, especially when the documents are in
different posting periods, you may encounter either of the following situations:
The canceled and cancellation documents are reported separately.
The cancellation document is not reported while the canceled document has already been reported.
We recommend that you take these possibilities into consideration when making relevant settings, canceling a document, and
creating reports.
The reports listed below are not affected by the Display Cancelled and Cancellation Marketing Documents in Reports checkbox:
Reporting Both Canceled and Cancellation Documents
Balance Sheet
Balance Sheet Budget Report
Balance Sheet Comparison
Budget Report
Cash Flow Reference Report
Document Journal
General Ledger
Inventory Audit Report
Inventory Posting List
Inventory Valuation Simulation Report (Inventory Valuation Report if your company manages non-perpetual inventory)
Locate Exceptional Discount in Invoice
Locate Journal Transaction by Amount Range
Locate Journal Transaction by FC Amount Range
Profit and Loss Statement
Profit and Loss Statement Budget Report
Profit and Loss Statement Comparison
Purchase Analysis
Sales Analysis
SP Commission by Invoices in Posting Date Cross-Section
Statement of Cash Flows
Transaction Journal Report
This is custom documentation. For more information, please visit SAP Help Portal. 195

6/8/26, 6:05 AM
Transaction Report by Projects
Trial Balance
Trial Balance Budget Report
Trial Balance Comparison
Reporting Neither Canceled nor Cancellation Documents
Backorder
Customer Receivables Aging
Dunning History Report
Open Items List
Vendor Liabilities Aging
Recurring Transactions
Certain business transactions repeat themselves on a regular basis. For example, every month a company orders a stack of
copying paper from their vendor.
In SAP Business One, you can define templates for such recurring transactions using regular sales and purchasing document
drafts. The templates contain the required business partner, item, accounting, and shipping information as well as recurrence
details. For more information, see Managing Recurring Transactions Templates. Based on the recurrence information, individual
recurring transaction instances are generated so that you can execute the transactions individually or by batch in the sales,
purchasing, and inventory area. For more information, see Managing Recurring Transactions.
In addition, you can set up the application in such a way that when you log on to the system, the Recurring Transactions window is
displayed automatically. To achieve this, you must select the Display Recurring Transactions on Execution checkbox in the
General Settings window. For more information, see General Settings: Services Tab.
Managing Recurring Transactions Templates
Prerequisites
You have full authorization for recurring transactions.
To check your authorization settings, go to Administration System Initialization Authorizations General Authorizations
to view the settings for the following fields under Sales – A/R: Recurring Transactions and Recurring Transactions Templates.
To manage templates for recurring transactions, choose one of the following from the SAP Business One Main Menu to open the
Recurring Transactions Templates – Selection Criteria window:
Purchasing – A/P Recurring Transaction Templates
Sales – A/R Recurring Transaction Templates
Inventory Inventory Transactions Recurring Transaction Templates
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 196

6/8/26, 6:05 AM
Filtering Recurring Templates
1. In the Recurring Transactions Templates – Selection Criteria window, specify the start date, end date, business partner
code, business partner group and business partner properties for your desirable templates.
To choose certain document types that you want to include, choose   next to Documents to open the Recurring
Templates - Documents Selection window, where you can filter templates by business area and document type.
2. Choose OK.
The application displays the recurring templates according to your filtering criteria.
Creating Recurring Transactions Templates
1. In the Recurring Transactions Templates – Selection Criteria window, choose OK to open the Recurring Transactions –
Templates window.
2. In the Template column, enter a name for the template you want to create.
3. In the Type column, specify the document type for the transaction, for example, purchase order, A/R invoice, or goods
issue.
4. Place your cursor in the Doc. No. column and press the  Tab  key.
The application displays a list of document drafts that are available for the selected document type.
5. Select a document draft or create a new one by choosing New.
If you decide to create a new document draft, the respective document opens. Enter the relevant customer or vendor data,
the item data, and any logistics or accounting information.
6. Specify the recurrence details, such as recurrence period, recurrence date, and the start date and end date (in the Valid
Until field) of the recurrence (optional).
You can check when the template will be executed for the first time in the Next Execution field.
  Example
Below are some examples of determining the recurrence details.
| Type of transaction                  | Recurrence Period | Recurrence Date |
| ------------------------------------ | ----------------- | --------------- |
| Transaction to be posted every day   | Daily             | Every 1         |
| Transaction to be posted every other | Daily             | Every 2         |
day
| Transaction to be posted every ten days | Daily         | Every 10  |
| --------------------------------------- | ------------- | --------- |
| Transaction to be posted every Monday   | Weekly        | On Monday |
| Transaction to be posted every other    | Every 2 Weeks | On Monday |
Monday
| Transaction to be posted every 15th of | Monthly | On 15 |
| -------------------------------------- | ------- | ----- |
the month
| Transaction to be posted on 15th of | Every 2 Months | On 15 |
| ----------------------------------- | -------------- | ----- |
every other month
This is custom documentation. For more information, please visit SAP Help Portal. 197

6/8/26, 6:05 AM
Type of transaction Recurrence Period Recurrence Date
Transaction to be posted once per Quarterly N/A
quarter
7. To save the template, choose Update.
8. To add another template, repeat the steps above.
To close the window, choose OK.
A template for recurring transactions is created. You can now execute the recurring transaction either manually or
automatically. For more information, see Managing Recurring Transactions.
Editing Recurring Transactions Templates
1. In the Recurring Transactions – Templates window, change the template name, document type, or recurrence details
directly.
If a template is already executed, you can only edit the following fields:
Recurrence Period
Recurrence Date
Valid Until
Prices Update
2. To change the transaction details, choose next to the document number, change the business partner or item data, and
choose Add to close the document draft.
3. To save the changes, in the Recurring Transactions – Templates window, choose Update.
The changes are reflected in the recurring transactions that are to be executed in the future.
Deleting Recurring Transactions Templates
1. In the Recurring Transactions – Templates window, right click a template and choose Delete Row.
2. Choose Update and OK.
The template, as well as any scheduled future instances of the recurring transaction, is deleted.
 Note
You can delete only recurring transaction templates that have never been executed. Recurring transaction templates that have
been executed at least once are grayed out and cannot be deleted.
 Recommendation
If you no longer need a particular template, in the Recurring Transactions - Templates window, specify a Valid Until date to set
the application to stop triggering the template from that date onwards. Nevertheless, the template will continue to be displayed
in the Recurring Transactions - Templates window.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 198

6/8/26, 6:05 AM
Managing Recurring Transactions
Managing Recurring Transactions
To access the function, choose one of the following from the SAP Business One Main Menu:
Purchasing – A/P Recurring Transactions
Sales – A/R Recurring Transactions
Inventory Inventory Transactions Recurring Transactions
The Confirmation of Recurring Transactions window appears, displaying all transactions that are scheduled to be executed today.
It also displays transactions that were scheduled for days in the past, but have not been executed so far.
Prerequisites
You have defined a recurring transactions template. For more information, see Managing Recurring Transactions Templates.
Procedure
Filtering Recurring Transactions
If there is a large number of recurring transactions in the system, you may want to narrow down the number of transactions
displayed, for example, according to the area you work in. To do so, proceed as follows:
1. Choose next to Documents to open the Recurring Templates - Documents Selection window.
2. To exclude transactions for all document types in a particular area, deselect the area, for example, Sales – A/R, Purchasing
– A/P, or Inventory.
To exclude transactions based on certain document types, deselect the relevant document type, for example, sales order or
goods issue.
3. To save the filtering criteria, choose Update.
The application displays the recurring transactions according to your filtering criteria.
Executing Single Recurring Transactions
1. Select the recurring transaction that you want to execute and choose the of the transaction.
This opens the document that is to be posted.
2. If necessary, edit the document.
3. To execute the transaction, choose Add.
The application posts the transaction you selected.
 Note
You can also execute single recurring transactions from the business partner area. To do so, proceed as follows:
1. Open a business partner master data record and choose You Can Also.
2. Select the “View Related Recurring Transactions” option.
This is custom documentation. For more information, please visit SAP Help Portal. 199

6/8/26, 6:05 AM
The Recurring Transactions for Business Partner window appears.
3. Proceed as described in steps 1–3 above.
Executing Recurring Transactions by Batch
1. Select all instances of recurring transactions that you want to execute.
2. Determine what the application should do in case a system message or error occurs. For example, prompt for user
confirmation, skip to the next transaction, or ignore all system warnings and continue executing the transactions.
3. Choose Execute.
The application posts the transactions you selected and displays a summary of any system messages or errors and the
application's response.
Removing Instances of Recurring Transactions
1. Select one or several instances of recurring transactions.
2. Choose Remove.
The application removes the transactions you selected.
Managing Recurring Transaction Templates
1. Choose next to Templates.
2. The Recurring Transactions – Templates window appears.
For more information, see Managing Recurring Transactions Templates.
Related Information
Managing Recurring Transactions Templates
Draw Document Wizard
Context
The draw document wizard enables you to create a new document from an existing one by guiding you step by step through the
process. It provides different options for customization and for altering data based on the target document you are creating and
the source document you are using. For example, you can choose which exchange rate to apply or whether to also draw freight
charges and withholding tax values from a base document to the target document.
Procedure
1. To go to the draw document wizard, from the SAP Business One Main Menu, choose either Sales A/R or Purchasing A/P.
2. Select the marketing document you want to create and specify the business partner code.
3. Choose Copy From and select a document type to draw.
The List of [document type] window of the selected document type appears. It displays the documents that can be drawn.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 200

6/8/26, 6:05 AM
Every marketing document allows drawing only specific document types. For example, you can draw only sales
quotations to sales orders, and only deliveries to returns.
4. Select the document or documents to draw and choose the Choose button.
5. In the Draw Document Wizard window, select the required criteria.
If you selected Draw all Data (Freight and Withholding Tax), choose the Finish button and go to step 11. If you selected
Customize, choose the Next button.
The rows included in the chosen base documents appear.
6. Choose the items you want to draw and make the necessary changes to the rows, quantities, or prices, if any.
If required, select Display BP Catalog Number.
7. If the drawn items are included in documents with freight, choose the Next button. Otherwise, choose the Finish button
and go to step 11.
The Select Freight Charges to Copy window appears.
8. Make the required selection and, if the base document includes withholding tax, choose the Next button. Otherwise,
choose the Finish button and go to step 11.
The Select WT Line to Copy window appears.
9. Verify that the proper values are displayed and make changes as necessary.
10. Choose the Finish button.
The chosen items are drawn and displayed in the new document.
 Note
You can only reduce drawn quantities of legal documents (delivery, invoice, and so on). Therefore, to increase the
quantity of a drawn item, add a new row to the document.
11. Proceed with the document as usual.
To change the order in which the items are displayed, use the up and down arrow buttons on the right side of the Contents
tab.
Results
If you draw the whole base document, it is closed and you will not be able to draw it again to another document. The exception is
the sales quotation, which can be copied if it has been closed, but only if you have selected the Allow Copying Closed Quotations
to Target Doc. checkbox in Document Settings.
If a document is partially drawn, the quantities (for an items type document), freight charges, and withholding tax values in the
base document are updated respectively. In that case, when you decide to copy the base document again, the original values are
replaced by the open quantities (for an items type document), freight charges, and withholding tax amounts.
Draw Document Wizard Window
When you create a sales or purchasing document based on existing documents, SAP Business One opens the Draw Document
Wizard window where you can define factors that affect the document you create.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 201

6/8/26, 6:05 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Draw Document Wizard Fields
Use Row Exchange Rate from Base Document
Copies the row exchange rate determined for the base documents into the target documents.
Use Document and Row Exchange Rate from Base Document
Copies the document and row exchange rate from the base document into the target document.
Use Current Exchange Rate from the Exchange Rate Table
Uses the current exchange rate regardless of the exchange rate determined in the base document.
Draw All Data (Freight and Withholding Tax)
Copies all data from the base document, including freight and withholding tax amounts.
Customize
Select this option to copy part of the data from the base document, or to make the required changes in the base document before
copying it to the target one.
Draw Document Wizard: Select Withholding Tax Line to Copy
This window displays the withholding tax amounts involved in the base documents drawn by the wizard. If required, you can
change the amount displayed.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Select Withholding Tax Line to Copy
Base Document
Number of the base document.
Withholding Tax Code
Code of the withholding tax defined for the business partner.
Taxable Value
The drawn taxable amount.
Withholding Tax Value
Withholding tax amount calculated for the taxable value; editable.
 Note
You cannot enter an amount larger than the total withholding tax amount included in the base document.
This is custom documentation. For more information, please visit SAP Help Portal. 202

6/8/26, 6:05 AM
Draw Document Wizard: Select Freight Charges to Copy
This window displays the details of the freight charges drawn into the target document from the base documents. If required, you
can make changes here.
 Note
The following explanations are relevant for purchasing documents.
When a goods receipt PO (whether fully open or partially drawn) is closed, any freight amount that is posted to the
Expense Allocation Account and is not drawn into an A/P invoice or goods return, is cleared.
When an A/P invoice or goods return is drawn (fully or partially) from a goods receipt PO, the Expense Allocation
Account is cleared with the freight amount that is drawn. In addition:
If the freight amount drawn to the target document is not directly proportional to the freight allocation, the
difference is posted to the Inventory Account or to the Negative Inventory Adjustment Account.
If the A/P invoice or the goods return closes the goods receipt PO final quantity, the Expense Allocation Account
is cleared with the freight amounts of the closed goods receipt PO.
When a goods return (whether fully open or partially drawn) is closed, the freight amount posted to the Expense
Allocation Account and not drawn into the A/P credit memo, is cleared.
When an A/P credit memo is based (fully or partially) on a goods return or on an A/P reserve invoice, the Expense
Allocation Account is cleared with the freight amount that is drawn.
If the A/P credit memo closes the final quantity of the goods return or the A/P reserve invoice, the Expense Allocation
Account is cleared with the freight amounts of the closed goods return or the A/P reserve invoice.
When a goods receipt PO is based (fully or partially) on an A/P reserve invoice, the Expense Allocation Account is
cleared with the freight amount that is drawn.
In databases that use the non-perpetual inventory system, when a goods return is based on a goods receipt PO, the
freight can be changed.
In the draw document wizard, when you select the Customize radio button, in the second step you can select which
freight charges to copy. Alternatively, in the goods return, when you click the golden link arrow next to the Freight field,
the Freight Charges window opens and you can make changes.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Select Freight Charges to Copy
Base Document
Number of the base document.
Amount
Sum of the expenses, calculated according to the set definitions.
If required, you can change the amount.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 203

6/8/26, 6:05 AM
The freight amount cannot be higher than the total amount of freight charges in the base document.
Drawing Method
The drawing method that appears in the document for that freight.
Changing the drawing method updates the freight charges accordingly.
Managing Document Drafts
In SAP Business One, you can save most documents as drafts. This lets you change and process them before adding them to the
database as regular documents. This may be required because a document is only partially filled out and it will be completed later.
Or perhaps someone knows how to fill out one part of the document but needs help from someone else to finish another part.
Document drafts can also be used as templates for documents that must be filled out over and over again with minor changes.
A draft document triggers neither a posting that changes quantities or values in the stock nor changes in the accounting system
for an invoice.
You can save the following types of documents as drafts:
Sales and purchasing documents
Incoming and outgoing payments
Checks for payment
Inventory documents, for example, inventory transfers, goods receipt and goods issue documents
You can also generate and display a list of drafts according to your specifications, enabling you to choose whether to delete,
update, or add certain drafts.
In addition to manually saving documents as drafts, you can also create drafts through approval processes. For more information,
see Working with Approval Processes.
Saving Documents as Drafts
Context
In SAP Business One, you can save sales and purchasing documents, payments, checks for payments and inventory documents as
drafts. This allows you to process them at a later point in time.
Procedure
1. Select the document you want to save as a draft.
2. Specify all required data.
3. To save the document draft, use one of the following options:
In the menu bar, choose File Save as Draft or right-click in the document window and choose Save as Draft.
Sale and purchasing documents:
Choose the Add Draft & New option in the document window. This option saves the document draft and
opens a new document in Add mode.
This is custom documentation. For more information, please visit SAP Help Portal. 204

6/8/26, 6:05 AM
Using the dropdown, choose the Add Draft & View option in the document window. This option saves the
document draft and opens the draft in View mode.
Example
A customer phones to order certain items. During the conversation, you enter the sales order in SAP Business One. If, however, the
customer does not reach a final decision on whether to issue the order, you cannot add it. You save the order as a draft and
process it when the customer has decided to purchase the items.
You create a quotation for a customer. Since this is a large project, you work together with some colleagues to prepare the
quotation. Each of you is responsible for a different area of the quotation. You want to define the quotation data at an early stage to
ensure that you and your colleagues can access the current quotation when required. You save the quotation as a draft to ensure
that you can work on it until all the different areas have been completed.
 Note
This function is not the same as a release procedure. You can also define a release procedure for sales documents in the system
so that they are not posted in the system and subsequent activities are not carried out until the documents have been released.
Creating Regular Documents from Drafts
Procedure
1. Depending on the type of document you want to create, proceed as follows:
Sales documents
Choose Sales – A/R Sales Reports Document Drafts Report . In the Document Drafts – Selection Criteria
window, specify the required parameters and choose OK.
Purchasing documents
Choose Purchasing – A/P Purchasing Reports Document Drafts Report . In the Document Drafts –
Selection Criteria window, specify the required parameters and choose OK.
Incoming payment documents
Choose Banking Banking Reports Payment Drafts Report .
Outgoing payment documents
Choose Banking Banking Reports Payment Drafts Report or Banking Outgoing Payments Checks for
Payment Drafts .
Inventory documents
Choose Inventory Inventory Reports Document Drafts Report . In the Document Drafts – Selection Criteria
window, specify the required parameters and choose OK.
2. Double-click the required draft.
The document window appears in the Add mode.
3. Make any necessary changes and choose Add.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 205

6/8/26, 6:05 AM
Since the number assigned to the regular document created from a draft is the one that currently appears in a new
document, it might be different than the one originally assigned to the draft.
Results
The status of the draft is Closed.
Deleting Drafts (Sales A/R and Purchasing A/P)
Context
You can delete A/R and A/P documents that were saved as drafts.
Procedure
1. From the SAP Business One Main Menu, choose Sales – A/R Sales Reports Document Draft Reports or
Purchasing – A/P Purchasing Reports Document Draft Reports .
2. Specify the required parameters to display the drafts you want to delete.
3. Select the required draft and choose Data Remove .
 Note
You can only delete one draft at a time in the SAP Business One client.
To remove multiple drafts at the same time, please use SAP Business One, Web client. For more information, see the
topic Managing Drafts in the User Guide for the Web client.
Document Drafts - Selection Criteria
Use this window to specify selection criteria for displaying document drafts.
To access the window, choose one of the following:
Sales - A/R Sales Reports Document Drafts Report
Purchasing - A/P Purchasing Reports Document Drafts Report
Inventory Inventory Reports Document Drafts Report
Document Drafts - Selection Criteria Fields
User
Select the user name for which you want to display drafts.
Open Only
If you select this checkbox, the report displays only the drafts that have not been added yet as original documents in SAP Business
One.
If you do not select this checkbox, the report displays all drafts that have been created, including those that are still pending.
Sales - A/R
This is custom documentation. For more information, please visit SAP Help Portal. 206

6/8/26, 6:05 AM
Displays sales document drafts: sales quotations, sales orders, deliveries, returns, A/R down payments, A/R invoices, and A/R
credit memos.
Select one or more options to include the drafts created for these documents.
Purchasing - A/P
Displays purchasing document drafts: purchase orders, goods receipt POs, goods returns, A/P down payments, A/P invoices, and
A/P credit memos.
Select one or more options to include the drafts created for these documents.
Inventory
Displays inventory document drafts: goods receipts, goods issue, and inventory transfers.
Select to include drafts for the inventory transfer documents.
Document Drafts Window
This window displays document drafts based on the selections made in the Document Drafts - Selection Criteria window. You can
double-click a row to display and process a specific document draft.
The following are the default fields:
Document Drafts Window
Document, Document No., Posting Date, BP Code, Total, Remarks
These fields provide general information regarding the displayed document drafts.
To see more details about the drafts displayed, choose and select additional columns.
In the following scenario, you receive a confirmation message with the exiting draft numbers and are asked whether to continue
with the process:
1. You use the Copy To or Copy From function to add one or more base sales or purchasing documents to a target document.
2. If approval isn’t required, you use the Save as Draft function to save the target document. If approval is required, the
system automatically creates a draft after you add the document, pending approval.
3. You (or another user) use the Copy To or Copy From function to copy the same base documents to another target
document again.
4. You (or another user) try to add the target document, save the target document as a draft again, or add the target
document for approval again.
Before making your decision, you can open this window to view details of the existing drafts using the provided draft numbers.
Calculating Landed Costs for Imported Goods
When importing goods, companies incur certain additional costs, such as customs, transport and insurance fees, or taxes. These
additional costs can be allocated to the imported items and reflected in the accounting system using the Landed Costs function in
SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 207

6/8/26, 6:05 AM
If your company runs a perpetual inventory system, creating the landed costs document automatically posts a journal entry in the
accounting system. The journal entry updates the moving average and the FIFO price of the imported items.
If your company does not run a perpetual inventory system, creating the landed costs document does not post a journal entry in
the accounting system.
Prerequisites
You have defined the measurements of the imported goods and assigned the goods to a customs group, if the goods are
liable for customs.
For more information, see Defining Imported Goods.
If your company uses perpetual inventory, you have defined G/L accounts for landed costs.
For more information, see Defining G/L Accounts for Landed Costs (Perpetual Inventory Companies).
You have defined the landed costs that you typically incur.
For more information, see Landed Costs – Setup.
Process
Documents relevant to the import process are in the Purchasing - A/P module:
Purchase order
Goods receipt PO
A/P invoice
Landed costs
1. You create a purchase order for a vendor abroad.
Optional: You create a purchase order for a vendor abroad in exactly the same way you would create a purchase order for
one of your local vendors. When you create a purchase order, SAP Business One updates the available stock quantity of the
ordered items.
2. You create a goods receipt purchase order (PO).
The goods receipt PO creates an inventory receipt transaction and is recorded in the same manner as a goods receipt PO
from a local vendor. SAP Business One uses the goods receipt PO as the base reference for the entire import process;
therefore, you must specify the item prices and quantities correctly.
 Note
The item prices you specify in the goods receipt PO document are the vendor's prices (Ex Works or FOB price),
excluding the additional costs, which are allocated later for the entire shipment.
The total amount of the goods receipt PO should be the overall expected price your vendor charges you for the
shipment, excluding the additional costs you must pay other parties, such as your customs broker.
3. You create an A/P invoice.
To complete the accounting transaction of the import process, create an A/P invoice (item type) based on the goods
receipt PO as soon as you receive the vendor’s invoice. Create the A/P invoice the same way that you would create an A/P
This is custom documentation. For more information, please visit SAP Help Portal. 208

6/8/26, 6:05 AM
invoice sent from one of your local vendors. You can create the A/P invoice at any time and regardless of the date when you
actually record the landed costs document.
4. You create a landed costs document.
To update the cost price of the imported items, you can create a landed costs document based on a goods receipt PO, an
A/P invoice, or on another landed costs document. This is required if you want to reflect accurately the additional costs
associated with the imported inventory valuation and calculating the gross profit, or any other inventory-related
calculation. Typically, you can create the landed costs document after you receive invoices from your customs broker or
shipping agency, but it is possible to use this method to include estimated landed costs prior to official documents being
received.
 Note
In a perpetual inventory system, when you post a landed costs document that is copied from a goods receipt PO, the
posting account depends on the current In Stock quantity of an item:
If the In Stock quantity > = landed costs quantity, then the Inventory Account is debited.
If the In Stock quantity < landed costs quantity, then the landed costs amount is split between the Inventory
Account and the Price Difference Account.
If the In Stock quantity = zero, then all the landed costs are posted to the Price Difference Account.
The item quantity can be sold or issued from the warehouse before the landed costs are added. To verify if this is the
case, you can run the inventory audit report for the item and sort it by system date in order to display the transactions
according to the order in which they were added to the system.
If the landed costs were added after the quantity had already left the warehouse, the item cost shown in the item master
data on the Inventory Data tab will not be updated with the landed costs value.
Costs pertaining to sold items are considered as additional expenses to appear in the Profit and Loss Statement report.
For a broker invoice, you can create an A/P service invoice based on a landed costs document (only in perpetual inventory
system). You can create multiple broker invoices based on the same landed costs. Firstly, you need to select the Enable
Multiple Broker Invoices for Landed Costs checkbox under Administration Document Settings Per Document
Landed Costs and then you can set different brokers in the costs table of the landed costs.
 Note
The customs in the landed costs can only be drawn to a broker invoice of the broker selected in the landed costs header.
 Note
In a perpetual inventory system, when you cancel a goods receipt PO or an A/P invoice that was already copied to a
landed costs, the cancelation journal entry will also reverse the landed costs inventory posting.
More Information
Updating an Item's Cost Price with Landed Costs (Perpetual Inventory Companies)
Updating an Item's Cost Price with Landed Costs (Non-Perpetual Inventory Companies)
Defining Imported Goods
Prerequisites
This is custom documentation. For more information, please visit SAP Help Portal. 209

6/8/26, 6:05 AM
You have defined the units of measure in the setup of SAP Business One:
Administration Setup Inventory Length & Width UoM
Administration Setup Inventory Weight UoM
Context
You define the goods you are importing to enable the proper calculation and allocation of landed costs. For example, if you want to
allocate landed costs according to weight or volume, specify the dimensions of the item as well as the volume and weight. If the
item you are importing is liable to customs, link it to a customs group.
Procedure
1. From the SAP Business One Main Menu, choose Inventory Item Master Data and open the relevant item record.
2. On the Purchasing Data tab, enter the length, width, height, volume, and weight.
If the item you import is liable to customs fees, enter also the customs group. For more information, see Item Master Data:
Purchasing Data Tab.
 Note
If you only enter a value for the dimensions and no unit of measurement, the system automatically inserts the unit of
measurement you defined in the setup. You can also enter a different unit of measurement.
3. Choose the Update button.
Related Information
Calculating Landed Costs for Imported Goods
Landed Costs - Setup
You define the landed costs to process the costs of importing a delivery from abroad. These costs are then distributed among the
items in the delivery according to the specific key that you select.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Purchasing Landed Costs .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Landed Costs Fields
Code
Enter the code of the landed cost.
Name
Enter the name of the landed cost, for example Insurance, Transportation, or Storage.
Allocation By
This is custom documentation. For more information, please visit SAP Help Portal. 210

6/8/26, 6:05 AM
Specify the distribution type for the landed cost. The available values are described below.
Cash Value Before Customs
The related costs are distributed in relation to the share of an item of the total FOB price of the delivery minus customs.
Cash Value After Customs
The related costs are distributed in relation to the share of an item of the total FOB price of the delivery plus customs.
Quantity
The related costs are distributed according to the quantity of an item in proportion to the total quantity of the delivery.
Weight
The related costs are distributed according to the weight of an item in proportion to the total weight of the delivery.
Volume
The related costs are distributed according to the volume of an item in proportion to the total volume of the delivery.
Equal
The related costs are distributed equally among the delivery items.
Landed Costs Alloc. Account
Specify the G/L account for clearing non-customs expenditures (reposted through the landed costs document) between the A/P
invoice (service type) and the landed costs document.
Only for companies using perpetual inventory.
More Information
Calculating Landed Costs for Imported Goods
Defining G/L Accounts for Landed Costs (Perpetual Inventory
Companies)
G/L accounts for landed costs are required only for companies that run a perpetual inventory, as posting a landed costs document
for these companies automatically creates a journal entry. Therefore, if your company manages a perpetual inventory, you must
define the accounts specified below.
Landed costs allocation account: G/L account for clearing non-customs expenditures (reposted through a landed costs
document) between the A/P invoice (service type) and the landed costs document
Customs allocation account: G/L account for clearing customs expenditures (reposted through a landed costs document)
between the A/P invoice (service type) and the landed costs document
Customs expense account: G/L account relating to customs expenditures from a landed costs document distributed to a
particular customs group
Procedure
Defining the Landed Costs Allocation Account
1. From the SAP Business One Main Menu, choose Administration Setup Purchasing Landed Costs .
This is custom documentation. For more information, please visit SAP Help Portal. 211

6/8/26, 6:05 AM
2. In the Landed Costs – Setup window, specify the landed costs allocation account.
3. Choose the Update button and then the OK button.
Defining the Customs Allocation Account
1. From the SAP Business One Main Menu, choose Administration Setup Inventory Customs Groups .
2. In the Customs Group – Setup window, specify the customs allocation account.
3. Choose the Update button and then the OK button.
Defining the Customs Expense Account
1. From the SAP Business One Main Menu, choose Administration Setup Inventory Customs Groups .
2. In the Customs Group – Setup window, specify the customs expense account.
3. Choose the Update button and then the OK button.
Updating an Item's Cost Price with Landed Costs (Perpetual
Inventory Companies)
To update an item’s cost price, which is required for calculating the inventory valuation, gross profit, or any other inventory-related
calculation, you use a landed costs document. On this document, you record the costs incurred when importing goods and you
distribute the costs among the individual goods according to predetermined factors, for example, quantity, weight or volume. You
can use this procedure only if your company runs a perpetual inventory. If you do not run a perpetual inventory, see Updating an
Item's Cost Price with Landed Costs (Non-Perpetual Inventory Companies).
You can base a landed costs document on goods receipt POs that are unpaid or partially paid and on another landed costs
document. For example, you can update the landed costs amounts in the accounting system for incoming insurance or shipping
invoices. Another example is documents that support landed cost estimations that are made in certain countries, such as Canada.
In addition, it is possible to link one goods receipt PO to several landed costs documents.
Prerequisites
You have created a goods receipt PO document for your overseas vendor.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Landed Costs .
2. In the Landed Costs window, select the vendor from whom you purchased the item(s).
3. If the vendor’s currency is different from your currency, specify an exchange rate and select the currency for the landed
costs document.
4. Choose Copy From to base the landed costs document on a goods receipt PO or another landed costs document.
All item lines are copied into the document. If the landed costs document is based on a goods receipt PO, you can delete
some of these lines if necessary.
 Note
If you want to base the landed costs document on several goods receipt POs, repeat this step as needed.
This is custom documentation. For more information, please visit SAP Help Portal. 212

6/8/26, 6:05 AM
5. On the Costs tab, specify the following data for the relevant landed costs type and recalculate the landed costs amounts for
the goods:
Allocation By
Allocation method as defined in the Landed Costs – Setup window for each landed cost.
Amount
Amount of expenditures to be distributed on lines.
When the landed costs document is based on another landed costs document, this field represents the final invoice
amount. That is, the amount difference between the base and the final amount is calculated and posted.
Include for Customs
Specify whether the associated landed cost is allowed for customs calculation and should thus be included in the actual
customs duty calculation and allocation.
 Example
In some circumstances when a company calculates customs duty for transportation, the company does not have to pay
customs on the full cost incurred for the transportation, for example, a company in the European Union (EU) that
imports goods from Asia. The goods' initial point of transportation (point of first shipment) is from outside the EU, so
the company has to pay customs duty on the non-EU portion, but is not subject to paying duty on the proportion of
transport incurred inside the EU. In other words, some portion of the transportation cost is allowed to be included in the
customs calculation, whilst another portion is exempted.
However, all the transportation cost, whether included for customs or not, is allocated to the inventory value.
If any part of the cost is disallowed, we recommend splitting the costs into the allowed and the disallowed parts when you
record the A/P service invoice, for example, for the freight invoice.
If you select the Include for Customs checkbox, actual and projected customs are calculated according to the formula
given below. Note that the fixed customs rate is defined in the Customs Group field on the Purchasing Data tab of the item
master data.
Actual/Projected customs = (FOB + included for customs landed costs) x fixed customs rate %
The system asks you whether you accept the newly calculated customs amount and distribute it according to the selection
made. If you select Yes, both the projected and actual customs value are updated with the recalculated figure and the
customs value per item is recalculated. If you select No, you have to update the actual customs amount and distribute the
actual customs amount at line item level manually. Selecting No may be required if the actual customs value varies from
the value calculated by SAP Business One. This may be the case when the customs or revenues authority assesses the
associated goods customs value or duty rate differently.
 Note
When you copy landed costs to other landed costs after you have created a broker invoice to the original landed costs,
the Include for Customs column is disabled for the costs that were already copied to the broker invoice (fully or
partially), and you cannot update those costs.
Factor
Percentage rate of each landed cost out of the total FOB costs of the shipment. This factor can help you determine the
shipment efficiency in comparison to other shipments or certain standards.
New Landed Costs
This is custom documentation. For more information, please visit SAP Help Portal. 213

6/8/26, 6:05 AM
Opens the Landed Costs – Setup window. If required, use this window to define additional landed costs while you process
the document.
6. In the footer area of the Items tab, specify the actual customs, if required.
If the actual customs differ from the projected customs, you can choose whether to distribute the difference
proportionately among item lines or to use a different distribution method. To distribute the difference proportionately,
choose Yes when answering the system message that appears. To use a different distribution method, choose No and
divide the difference up manually.
 Note
If you do not want customs to affect the inventory value, deselect the Customs Affects Inventory checkbox.
 Note
When you copy landed costs to other landed costs after you have created a broker invoice to the original landed costs,
the Items tab is disabled if the customs were already copied to the broker invoice (fully or partially), and you cannot
update those customs.
7. Choose the Add button.
SAP Business One adds the landed costs document and creates the related journal entry. If the landed costs document is
based on another landed costs document, the posted value is only a delta.
The goods receipt PO is closed for further allocation of landed costs.
 Note
If you need to allocate additional landed costs to a goods receipt PO, open the goods receipt PO and from the menu bar
choose Data Advanced Open for Landed Costs .
If you want to block drawing a specific goods receipt PO to landed costs, open the goods receipt PO, and from the menu
bar choose Data Advanced Close for Landed Costs .
 Note
If you want to use one landed costs document for importing goods from several vendors (for example, consolidation
purchasing in which a single container is used for goods from several vendors to decrease import costs), repeat steps 2-
4 before adding the document.
More Information
Landed Costs Window
Updating an Item's Cost Price with Landed Costs (Non-Perpetual
Inventory Companies)
Prerequisites
You have created a goods receipt PO document for your overseas vendor.
Context
This is custom documentation. For more information, please visit SAP Help Portal. 214

6/8/26, 6:05 AM
Posting the A/P invoice (service type) for the invoices you receive from your shipping company or customs broker reflects the
import costs in the accounting system. You use a landed costs document to update an item’s cost price, which is required for
calculating the inventory valuation, gross profit, or any other inventory-related calculation.
You can base a landed costs document on a goods receipt PO, and you can update the landed costs document with the costs as
they come in, as long as you have not created a journal entry for the landed costs document yet.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Landed Costs .
2. In the Landed Costs window, select the vendor you purchased the item(s) from.
3. If the vendor’s currency is different from your currency, specify an exchange rate and select the currency for the landed
costs document.
4. Choose the Copy From button, to base the landed costs document on a goods receipt PO or another landed costs
document.
All item lines are copied into the document.
5. On the Fixed Costs and Variable Costs subtabs of the Costs tab, enter the following data for the relevant landed costs type
and choose the Recalculate button:
Field Description
Allocation By Specify how landed costs are distributed among the items.
Amount Enter the actual amount of the landed costs.
6. In the footer area of the Items tab, specify the actual customs, if required. If the actual customs differ from the projected
customs, choose whether to distribute the difference proportionately among the item lines.
7. Choose the Add button.
 Note
If you want to use one landed costs document for importing goods from several vendors (for example, consolidation
purchasing, in which a single container is used for goods from several vendors to decrease import costs), repeat steps
2-4 before adding the document.
Later on you can draw landed costs with multiple vendors to another landed costs, if needed.
The landed costs document is added. The goods receipt PO is closed for further allocation of landed costs.
Related Information
Landed Costs Window
Landed Costs Window
In the Landed Costs window, you record and allocate the costs incurred when importing goods. To access the window, choose
Purchasing A/P Landed Costs .
More Information
Landed Costs: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 215

6/8/26, 6:05 AM
Landed Costs: Items Tab
Landed Costs: Costs Tab
Landed Costs: Vendors Tab
Landed Costs: Details Tab
Landed Costs: General Tab
Landed Costs: General Area
Use this area to enter general information relevant to all parts of the document and to the import procedure.
To access the area, choose Purchasing – A/P Landed Costs .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Landed Costs General Area Fields
Vendor
Field on the left: vendor code
Field on the right: vendor name
Specify either the vendor code or the vendor name. The remaining field is filled automatically.
 Note
If you create one landed costs document when you import goods from several vendors, the field on the left displays the string
'********' and the field on the right displays Different Vendors. For example, in consolidation purchasing, a single
container is used for importing goods from several vendors to decrease import costs.
You can view the vendors selected for the document on the Vendors tab.
Broker
Field on the left: broker code
Field on the right: broker name
Specify either the code or the name of the broker hired to assist with the import and customs procedures. The remaining field is
filled automatically.
 Note
You define brokers as other regular vendors in the business partner master data.
Currency
Displays the vendor currency and the exchange rate used for the document. You must enter an exchange rate; otherwise, you are
not able to continue recording the landed costs document.
This is custom documentation. For more information, please visit SAP Help Portal. 216

6/8/26, 6:05 AM
After you specify an exchange rate, you can choose either the vendor currency or your local currency. Your selection determines
the currency in which monetary values are displayed in the document, that is, transport costs or customs, for example.
Closed Document
Select when you finish processing a landed costs document and, if required, clear it as long as the journal entry for the document’s
landed costs has not been created.
SAP Business One selects the checkbox automatically once a journal entry for the document’s landed costs is created. In that
case, it cannot be cleared again.
Number
Sequential number automatically assigned by SAP Business One according to the definition in the system initialization (see
Administration System Initialization Document Numbering ).
Series
Specify a numbering series.
Posting Date
Specify the posting date.
The default value is the current date on which the landed costs document is created. If required, change the date.
Due Date
Specify the due date for the document. The default value is the date on which the landed costs document is created. If required,
change the date.
Reference
Additional reference number for the document, if defined.
File No.
Number of the landed costs document, as provided by your broker.
Copy From
A list of base documents from which to create a target document.
More Information
Calculating Landed Costs for Imported Goods
Document Numbering - Setup
Landed Costs: Items Tab
Use this tab to display the data regarding the imported goods as copied from goods receipt PO documents.
To access the tab, choose Purchasing – A/P Landed Costs Items .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 217

6/8/26, 6:05 AM
Landed Costs Items Tab Fields
Item No.
Item numbers of the imported items, as displayed in the selected goods receipt PO documents.
Qty
Imported quantities of the items in the selected goods receipt PO documents.
Base Doc. Price
Unit price that appears in the Item row of the goods receipt PO documents.
 Note
If a discount was given in the goods receipt PO document, SAP Business One calculates the FOB price as the row price minus
the discount amount. This price reflects the net vendor price, excluding import costs.
Base Doc. Value
Total price that appears in the Item row of the goods receipt PO documents.
 Note
If a discount was given in the goods receipt PO document, SAP Business One calculates the FOB price as the row price minus
the discount amount. This price reflects the net vendor price, excluding import costs.
This field is only available for companies managing a perpetual inventory.
Customs Rate
If required, specify the rate for customs. It can be a different currency rate for each line.
Proj. Cust.
Projected customs. It is calculated per unit by multiplying the base document price by the customs rate defined for each item and
according to the linked customs group. You can change the value if the value calculated in this field is not the actual amount you
are required to pay.
If you selected the Include for Customs checkbox on the Costs tab for one of the landed costs, the projected customs value is
recalculated as follows:
(FOB + Included Landed Costs) * fixed customs rate / quantity per line.
Customs Value
Total value of customs per row. If the value calculated in this field is not the actual amount you are required to pay, you can change
this value.
Expenditure
Expenses for each item unit as calculated in the current document.
According to the landed costs allocation, this value is the weighted ratio of each item, without the overall costs calculated in the
document.
Alloc. Costs Val.
Value of landed costs allocated to the item row.
This field is only available for companies managing a perpetual inventory.
This is custom documentation. For more information, please visit SAP Help Portal. 218

6/8/26, 6:05 AM
Whse Price
The price of the imported item in your warehouse, calculated as follows:
Freight + expected customs + base document price
Total
Value calculated by multiplying the price in the warehouse by the imported quantity.
Total Costs
Sum of the customs value plus the allocated costs value.
This field is only available for companies managing a perpetual inventory.
Warehouse
Warehouse in which the imported item is located.
Release No.
Release number for customs purposes.
Var. Costs
Variable costs per item. This field is only relevant for companies not managing a perpetual inventory.
Const. Costs
Total expenditure taken from the Costs tab divided by quantity.
Customs
Total value of customs per line in local currency.
FOB and Included Costs
This value is calculated as follows:
Free on board, that is, the purchase price + (total amount of landed costs included for customs / total quantity) * (quantity per
line).
Project
If required, specify the project to which the landed cost of the item is allocated. If you defined the project in the source goods
receipt PO or landed cost documents, the field displays the project code by default.
Distr. Rule
If required, specify the distribution rule for the landed costs row. The default value comes from row information of the source
documents (goods receipt POs or landed costs documents).
For perpetual inventory companies:
If you define the distribution rule here, it appears in the Distr. Rule field for the customs allocation account or
customs expense account row in the journal entry.
If you leave this field empty, the default distribution rule for the customs allocation account or customs expense
account appears in the Distr. Rule field for the corresponding journal entry row.
For non-perpetual inventory companies, a change in this field does not apply to journal entries because posting a landed
costs document does not create a journal entry.
Projected Customs
This is custom documentation. For more information, please visit SAP Help Portal. 219

6/8/26, 6:05 AM
Projected customs are calculated automatically as follows:
Projected customs = (FOB + included for customs landed costs) x fixed customs rate %
Actual Customs
Actual customs are calculated as follows:
Actual customs = (FOB + included for customs landed costs) x fixed customs rate %.
 Note
The fixed customs rate is defined in the Customs Group field on the Purchasing Data tab of the item master data.
Specify the actual customs amount. If the data in SAP Business One is accurate, this amount equals the value in the Proj.
Customs field. If the amounts are different, SAP Business One displays a window with an option to divide different amounts
equally.
Customs Affects Inventory
If you select this option, the customs fees affect the inventory value. This field is only available for companies managing a
perpetual inventory.
Total Freight Charges
Sum of expenditure * quantity for all lines.
 Note
For perpetual inventory, this is the sum of total costs.
Amount to Balance
Difference between the sum of amounts on the Costs tab and the Total Freight Charges value on the Items tab.
 Note
In perpetual inventory, you can only post the document if the value is zero.
Remarks
Displays the reference numbers or the vendor numbers for the goods receipt PO used in the landed costs document, and depends
on the default settings made. You can change the remarks, if necessary.
Before Tax
Sum of base document price + (expenditure*quantity) + projected customs.
Tax 1
Enter the tax amount relevant for the imported items. This has no impact on the journal entry.
Tax 2
Enter the tax amount relevant for the landed costs. This has no impact on the journal entry.
Total
Displays the overall amount of the document (before Tax+Tax 1+Tax 2).
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 220

6/8/26, 6:05 AM
Calculating Landed Costs for Imported Goods
Landed Costs: Costs Tab
Use this tab to allocate landed costs to the various items according to specific criteria, for example volume, weight, or quantity.
 Note
To ensure that landed costs are allocated correctly when you choose to allocate by weight or volume, each item master data
record of imported items should contain the item's volume, weight, and customs group.
However, you do not have to specify an amount for each landed costs type. Enter only the amounts relevant to the specific
shipment you are handling at the time.
The tab consists of two subtabs: Fixed Costs and Variable Costs. If your company manages a perpetual inventory system, the
Variable Costs subtab is disabled.
To access the tab, choose Purchasing A/P Landed Costs Costs .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Fixed Costs Subtab Fields
Landed Costs
Landed costs name, as defined in the Landed Costs – Setup window.
Allocation By
Allocation method as defined in the Landed Costs – Setup window for each landed cost.
Amount
Amount of expenditures to be distributed on lines.
When the landed costs document is based on another landed costs document, this field represents the final invoice amount. That
is, the amount difference between the base and the final amount is calculated and posted.
Include for Customs
Specify whether the associated landed cost is allowed for customs calculation and should thus be included in the actual customs
duty calculation and allocation.
 Example
In some circumstances when a company calculates customs duty for transportation, the company does not have to pay
customs on the full cost incurred for the transportation, for example, a company in the European Union (EU) that imports
goods from Asia. The goods' initial point of transportation (point of first shipment) is from outside the EU, so the company has
to pay customs duty on the non-EU portion, but is not subject to paying duty on the proportion of transport incurred inside the
EU. In other words, some portion of the transportation cost is allowed to be included in the customs calculation, whilst another
portion is exempted.
However, all the transportation cost, whether included for customs or not, is allocated to the inventory value.
This is custom documentation. For more information, please visit SAP Help Portal. 221

6/8/26, 6:05 AM
If any part of the cost is disallowed, we recommend splitting the costs into the allowed and the disallowed parts when you record
the A/P service invoice, for example, for the freight invoice.
If you select the Include for Customs checkbox, actual and projected customs are calculated according to the formula given
below. Note that the fixed customs rate is defined in the Customs Group field on the Purchasing Data tab of the item master data.
Actual/Projected customs = (FOB + included for customs landed costs) x fixed customs rate %
The system asks you whether you accept the newly calculated customs amount and distribute it according to the selection made.
If you select Yes, both the projected and actual customs value are updated with the recalculated figure and the customs value per
item is recalculated. If you select No, you have to update the actual customs amount and distribute the actual customs amount at
line item level manually. Selecting No may be required if the actual customs value varies from the value calculated by SAP
Business One. This may be the case when the customs or revenues authority assesses the associated goods customs value or
duty rate differently.
Factor
Percentage rate of each landed cost out of the total FOB costs of the shipment. This factor can help you determine the shipment
efficiency in comparison to other shipments or certain standards.
Recalculate
Recalculates the landed cost amounts if you have updated any data in the table.
Clear Table
Resets all landed cost amounts recorded in the table and changes the allocation methods back to their default values, as defined in
the Landed Costs – Setup window.
New Landed Costs
Opens the Landed Costs – Setup window. If required, use this window to define additional landed costs while you process the
document.
More Information
Calculating Landed Costs for Imported Goods
Landed Costs - Setup
Landed Costs: Vendors Tab
This tab displays all the vendors selected for the current landed costs document.
To access the tab, choose Purchasing – A/P Landed Costs Vendors .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Landed Costs Vendors Tab Fields
Vendor Code
Codes of the vendors related to the landed costs document. To delete vendors from the document, select a row and from the menu
bar, choose Data Delete Row .
This is custom documentation. For more information, please visit SAP Help Portal. 222

6/8/26, 6:05 AM
Vendor Name
Names of the vendors related to the landed costs document. To delete vendors from the document, select a row and from the
menu bar, choose Data Delete Row .
More Information
Calculating Landed Costs for Imported Goods
Landed Costs: Details Tab
Use this tab to find further information about the landed costs rows.
To access the tab, choose Purchasing – A/P Landed Costs Details .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Landed Costs Details Tab Fields
Whse Price
Warehouse price calculated for a single imported item after landed costs are allocated. This price is then updated in the selected
price list according to the currency selected in the landed costs document.
Price List
Specify the price list you want to update with the item price and landed costs.
 Note
The selected price list is updated according to the currency selected in the document. For example, if the landed costs
document is displayed in your local currency, the item prices are updated accordingly in the selected price list, and not by a
foreign currency, if one is defined for the vendor.
Expenditure
To determine whether to allocate landed costs for the current row, select a value from the dropdown list.
If no costs are allocated to a certain item, the item cost is calculated as its FOB price plus the customs. Landed costs that are not
allocated for such items are allocated for the remaining items.
Bill of Lading No.
Specify the number of the bill of lading attached to the landed costs document.
Transport Type
Specify the shipping type.
More Information
Calculating Landed Costs for Imported Goods
This is custom documentation. For more information, please visit SAP Help Portal. 223

6/8/26, 6:05 AM
Landed Costs: General Tab
This tab is available only in companies that manage inventory in warehouses using perpetual inventory.
To access the tab, choose Purchasing – A/P Landed Costs General .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Landed Costs General Tab Fields
Trans. No.
Number of the journal entry created for the landed costs.
Journal Remarks
Enter remarks for the journal entry.
By default, SAP Business One displays Landed Costs — XXX where XXX is the document number. You can change this string, if
required.
More Information
Calculating Landed Costs for Imported Goods
Landed Costs: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
This is custom documentation. For more information, please visit SAP Help Portal. 224

6/8/26, 6:05 AM
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Procurement Confirmation Wizard
Procurement confirmation is a function that assists you in automatically creating one or several procurement documents, such as
purchase quotations, purchase orders, or production orders, directly from one or several sales documents or production orders.
Procurement documents created using this function can include part or all of the items from the base sales or production
documents. However, you cannot use the procurement confirmation function to assign items to existing purchasing documents or
as a tool to guarantee sales order fulfillment by reserving items in the warehouse, for example.
You can use the function to do the following:
Consolidate multiple sales orders into one purchase order
For more information, see Consolidating Multiple Sales Orders for Purchasing.
Create a purchase order directly from a sales order
For more information, see Creating Purchase Orders Directly from Sales Orders.
Consolidate multiple sales orders for production
For more information, see Consolidating Multiple Sales Orders for Production
Create a production order directly from a sales order
For more information, see Creating Production Orders Directly from Sales Orders
Create procurement documents directly from production orders
For more information, see Creating Procurement Documents Directly from Production Orders
Creating Purchase Orders Directly from Sales Orders
Prerequisites
You are authorized to create both sales and purchase orders.
This is custom documentation. For more information, please visit SAP Help Portal. 225

6/8/26, 6:05 AM
You have created a sales order that includes delivery from a drop-ship warehouse, or you have created a sales order
according to the following procedure:
1. From the SAP Business One Main Menu, choose Sales – A/R Sales Order .
2. Specify the customer and item information as well as any billing or shipping information.
3. On the Logistics tab, select the checkbox Procure Non Drop-Ship Items.
This initiates the procurement confirmation wizard, which allows you to create a purchase order for the goods that
are not in stock.
Context
You received an order from one of your customers, and the ordered goods are not in stock. You want to create a purchase order
directly from the sales order to buy the goods from a vendor.
Procedure
1. Create a sales order as indicated above and choose Add.
The Procurement Confirmation Wizard appears. In the Customer window, the relevant customer is displayed and selected.
If required, specify additional customers for whose sales orders you want to create purchase orders.
To be able to create purchase orders for all open sales orders with unfulfilled purchase quantities for the selected business
partners, select the Include All Open Sales Orders checkbox. If you do not select this checkbox, the only sales orders
displayed are those for which the Procurement Document option was checked on the Logistics tab of the sales order or
that use a drop-ship warehouse and have unfulfilled purchase quantities.
2. Choose Next.
In the Sales Orders window, all open sales orders for the selected customers are displayed.
3. Select the sales order or sales orders for which you want to purchase items.
4. Choose Next.
The Base Document Line Items window appears.
5. Select the target document type Purchase Order.
By default, the quantities for the selected items are the quantities from the sales order(s). If required, change the quantities
for the purchase order.
If an item has a preferred vendor assigned to it, this vendor is already entered in the line. If required, change the vendor
code.
For all items that do not have a vendor assigned to them yet, enter a vendor code.
To specify the same vendor for all items, enter the vendor code in the Vendor field of the wizard body.
To specify the vendor for each item individually, enter the vendor code in the Vendor or Vendor Name column of the
table.
By default, the Price Mode field is automatically filled with the default price mode of your vendor. Other associated fields
are automatically filled as well.
You can switch between Net and Gross price modes. If you change the default price mode, all associated prices will be
cleared.
To save the purchase order as a draft, select the Create Draft Document checkbox.
6. Choose Next.
This is custom documentation. For more information, please visit SAP Help Portal. 226

6/8/26, 6:05 AM
7. In the Consolidations window, specify whether to consolidate several sales orders into one purchase order and which
consolidation options to apply.
To do the following: Choose:
Create one purchase order per sales order No Consolidation
The documents are grouped by vendor, that is, one purchase
order is created per vendor.
Consolidate several sales orders into one purchase order Consolidated by and select the relevant option:
Vendor (System Default)
The documents are grouped by vendor, that is, one
purchase order is created per vendor. This setting
cannot be changed.
Warehouse (Split)
The documents are grouped by the warehouse that is
used to ship the items. That is, if items are sold from
different warehouses, one purchase order is created per
warehouse.
Other
You can specify additional grouping criteria, such as the
delivery date or shipping type.
8. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field and choose Next.
The Preview Results window appears. It displays all purchase orders that will be created grouped by vendor and the
consolidations options you selected.
9. To generate the documents, choose Next.
The application creates the relevant documents and displays a summary report of all documents that were created and any
errors that occurred.
Related Information
Sales Order
Purchase Order
Procurement Confirmation Wizard
Consolidating Multiple Sales Orders for Purchasing
Prerequisites
You have several sales orders for items that you want to order from a vendor.
You are authorized to create both sales and purchase orders.
Context
This is custom documentation. For more information, please visit SAP Help Portal. 227

6/8/26, 6:05 AM
You can consolidate multiple sales orders into one single purchase order. This may be valuable, for example, if you receive several
sales orders for certain items and you in turn want to purchase these items in one single item order from your vendor to save on
shipping costs or obtain a quantity discount.
Procedure
1. From the SAP Business One Main Menu, choose Purchasing – A/P Procurement Confirmation Wizard .
The Procurement Confirmation Wizard appears.
2. In the Customer window, choose Add and specify the customers for whose sales orders you want to create a purchase
order.
To be able to create purchase orders for all open sales orders with unfulfilled purchase quantities for the selected business
partners, select the Include All Open Sales Orders checkbox. If you do not select this checkbox, the only sales orders
displayed are those for which the Procurement Document option was checked on the Logistics tab of the sales order or
that use a drop-ship warehouse and have unfulfilled purchase quantities.
3. Choose Next.
4. Select the sales orders for which you want to purchase items.
5. Choose Next.
The Sales Order Line Items window appears, with purchase order selected as the target document. By default, the
quantities for the selected items are the quantities from the sales order(s). If required, change the quantities for the
purchase order.
If an item has a preferred vendor assigned to it, this vendor is already entered in the line.
If required, change the vendor code.
For all items that do not have a vendor assigned to them yet, enter a vendor code.
To specify the same vendor for all items, enter the vendor code in the Vendor field of the wizard body.
To specify the vendor for each item individually, enter the vendor code in the Vendor or Vendor Name column of the
table.
To save the purchase order as a draft, select the Create Draft Document checkbox.
6. Choose Next.
7. In the Consolidations window, specify whether to consolidate several sales orders into one purchase order and which
consolidation options to apply.
To do the following: Choose:
Create one purchase order per sales order No Consolidation
The documents are grouped by vendor, that is, one purchase
order is created per vendor.
Consolidate several sales orders into one purchase order Consolidated by and select the relevant option:
Vendor (System Default)
The documents are grouped by vendor, that is, one
purchase order is created per vendor. This setting
cannot be changed.
Warehouse (Split)
The documents are grouped by the warehouse that is
used to ship the items. That is, if items are sold from
This is custom documentation. For more information, please visit SAP Help Portal. 228

6/8/26, 6:05 AM
To do the following: Choose:
different warehouses, one purchase order is created per
warehouse.
Other
You can specify additional grouping criteria, such as the
delivery date or shipping type.
8. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field and choose Next.
The Preview Results window appears. It displays all purchase orders that will be created, grouped by vendor and the
consolidations options you selected.
9. To generate the documents, choose Next.
The application creates the relevant documents and displays a summary report of all documents that were created and any
errors that occurred.
Related Information
Procurement Confirmation Wizard
Creating Production Orders Directly from Sales Orders
Prerequisites
You are authorized to create both sales and production orders.
The item that you want to produce is defined as a bill of materials (BOM).
You have created a sales order according to the following procedure:
1. From the SAP Business One Main Menu, choose Sales – A/R Sales Order .
2. Specify the customer and item information as well as any billing or shipping information.
3. On the Logistics tab, select the Procurement Document checkbox.
This initiates the procurement confirmation wizard, which allows you to create a production order for the goods that
were ordered.
Context
To support a demand-driven production approach, in which a product is scheduled and built in response to a confirmed order you
received from a customer, you create a production order directly from a sales order.
Procedure
1. Create a sales order as indicated above and choose Add.
The Procurement Confirmation Wizard appears. In the Customer window, the relevant customer is displayed and selected.
If required, specify additional customers for whose sales orders you want to create production orders.
This is custom documentation. For more information, please visit SAP Help Portal. 229

6/8/26, 6:05 AM
To be able to create production orders for all open sales orders for the selected business partners, select the Include All
Open Sales Orders checkbox. If you do not select this checkbox, only those sales orders are displayed for which the
Procurement Document option was selected on the Logistics tab of the sales order or that use a drop-ship warehouse and
have unfulfilled purchase quantities.
2. Choose Next.
The Sales Orders window displays all open sales orders for the selected customers.
3. Select the sales orders for which you want to produce items.
4. Choose Next.
The Sales Order Line Items window appears.
5. Select the target document type Production Order.
All BOMs are displayed.
6. Select the BOMs that you want to produce.
By default, the quantities for the selected items are the quantities from the sales order(s). If required, change the quantities
for the production order.
7. Choose Next.
8. In the Consolidations window, specify whether to consolidate several sales orders into one production order and which
consolidation options to apply.
To do the following: Choose:
Create one production order per item No Consolidation
The documents are grouped by item, that is, one production
order is created per sales order per item, and per warehouse
(system default).
Consolidate several sales orders into one production order Consolidated by and select the relevant option:
Item (System Default)
The documents are grouped by item, that is, one
production order is created per item. This setting
cannot be changed.
Other
You can specify additional grouping criteria, such as the
delivery date or shipping type.
9. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field and choose Next.
The Preview Results window appears. It displays all production orders that will be created grouped by item and the
consolidations options you selected.
10. To generate the documents, choose Next.
The application creates the production orders with the status Planned and a due date that is determined by the lead time
of the production items. It displays a summary report of all documents that were created and any errors that occurred.
Related Information
Procurement Confirmation Wizard
This is custom documentation. For more information, please visit SAP Help Portal. 230

6/8/26, 6:05 AM
Sales Order
Production Orders
Consolidating Multiple Sales Orders for Production
Prerequisites
You have several sales orders for items that you want to produce in your company.
The item that you want to produce is defined as a bill of materials (BOM).
You are authorized to create both sales and production orders.
Context
You can consolidate multiple sales orders into one single production order.
Procedure
1. From the SAP Business One Main Menu, choose Production Procurement Confirmation Wizard .
The Procurement Confirmation Wizard appears.
2. Choose Next.
3. In the Customer window, choose Add and specify the customers for whose sales orders you want to create a production
order.
To be able to create production orders for all open sales orders with unfulfilled purchase quantities for the selected
business partners, select the Include All Open Sales Orders checkbox. If you do not select this checkbox, only those sales
orders are displayed for which the Procurement Document option was selected on the Logistics tab of the sales order or
that use a drop-ship warehouse and have unfulfilled purchase quantities.
4. Choose Next.
5. Select the sales orders for which you want to produce items.
6. Choose Next.
The Sales Order Line Items window appears, with production order selected as the target document. All BOMs are
displayed.
7. Select the BOMs that you want to produce.
By default, the quantities for the selected items are the quantities from the sales order(s). If required, change the quantities
for the production order.
8. Choose Next.
9. In the Consolidations window, specify whether to consolidate several sales orders into one production order and which
consolidation options to apply.
To do the following: Choose:
Create one production order per item No Consolidation
The documents are grouped by item, that is, one production
order is created per sales order per item per warehouse
(system default).
This is custom documentation. For more information, please visit SAP Help Portal. 231

6/8/26, 6:05 AM
To do the following: Choose:
Consolidate several sales orders into one production order Consolidated by and select the relevant option:
Item (System Default)
The documents are grouped by item, that is, one
production order is created per item. This setting
cannot be changed.
Other
You can specify additional grouping criteria, such as the
delivery date or shipping type.
 Note
If the item lines have different distribution rules or project
codes, a separate production order will be generated
according to distribution rule and project code.
10. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field and choose Next.
The Preview Results window appears. It displays all production orders that will be created grouped by item and the
consolidations options you selected.
11. To generate the documents, choose Next.
The application creates the production orders with the status Planned and a due date that is determined by the lead time
of the production items. It displays a summary report of all documents that were created and any errors that occurred.
Related Information
Procurement Confirmation Wizard
Sales Order
Production Orders
Creating Procurement Documents Directly from Production
Orders
Prerequisites
You are authorized to create production orders, purchase orders, purchase requests, and purchase quotations.
You have created a production order that contains item type components and selected the Procure Items checkbox.
Alternatively, you have selected the Procure Items checkbox for an existing production order.
Context
You want to create a purchase order, purchase quotation, or purchase request based on a production order. Alternatively, you want
to procure components on a production order to ensure that production will follow. Creating production orders for goods can help
maintain minimum inventory holding levels.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 232

6/8/26, 6:05 AM
1. Create or update a production order as described above and choose the Add or Update button.
The Procurement Confirmation Wizard is displayed (at Step 1 of 6: Base Document Type and Customers window) with the
Production Order option automatically selected in the Base Doc. field. Additionally, the Product No. and Product
Description fields are automatically displayed based on the production order; selecting the link arrow next to the Product
No. field will display the list of relevant items in the Bill of Materials window or Item Master Data window (depending on
whether the Open Item Master Data Instead of Bill of Materials of a BOM Item When Selecting Link Arrow option is
selected ( Administration General Settings Inventory tab Items tab ). The checkbox next to the Product No. field
indicates whether the Product No. is selected to be included in the wizard.
If you already have item type components with the Allow Procurmt. Doc. checkbox selected in a production order, you can
run the wizard from scratch ( Production Procurement Confirmation Wizard ) and choose the Add button in Step 1. In
the Product Numbers – Selection Criteria window, you can enter the item number or range. Alternatively, choose items
based on item group or properties. Only items which are associated with a production type BOM and for which the Allow
Procurmt. Doc. checkbox is selected are displayed. If necessary, you can deselect the checkbox next to a product number
to exclude it from the procurement documents.
Choose the Next button.
2. In the Base Documents window, select one of more base documents from which you want to generate the procurement
documents and choose the Next button.
3. In the Base Document Line Items window, from the dropdown list in the Target Document field, select one of the following
options as the target document type: Purchase Order, Purchase Quotation, Purchase Request, or Production Order.
The table displays the production order lines for which procurement document creation has been allowed (in other words,
the Allow Procurmt. Doc. checkbox is selected) in the specified production orders. You may change the line items for
inclusion in the procurement documents.
If you chose a purchase order, purchase request, or purchase quotation as the target document, if an item has a preferred
vendor assigned to it, this vendor is already entered in the line. If required, change the vendor code. If a preferred vendor is
not assigned to the item, you are asked to enter a vendor code.
To specify the same vendor for all items, enter the vendor code in the Vendor field of the wizard body.
To specify the vendor for each item individually, enter the vendor code in the Vendor column of the table.
To create the procurement document as a draft, select the Create Draft Document checkbox.
Choose the Next button.
4. In the Consolidations window, specify whether to consolidate several production orders into one procurement document
and which consolidation options apply.
To do the following: Choose:
Create one procurement document for each production order No Consolidation
System behavior depends on the target document type.
For Purchase Order: The documents are grouped by
vendor and target document series.
For Purchase Quotation: The documents are grouped
by vendor and target document series.
For Purchase Request:The documents are grouped by
requester and target document series.
For Production Order: The documents are grouped by
item and target document series.
This is custom documentation. For more information, please visit SAP Help Portal. 233

6/8/26, 6:05 AM
To do the following: Choose:
Create one procurement document for each production order Consolidated By and select the relevant option:
Vendor (System Default)
The documents are grouped by vendor, that is, one
purchase order is created per vendor. This setting
cannot be changed.
Warehouse (Split)
The documents are grouped by the warehouse that is
used to ship the items. That is, if items are sold from
different warehouses, one purchase order is created per
warehouse.
Other
You can specify additional grouping criteria, such as the
delivery date or shipping type.
Choose the Next button.
5. Specify the system response to errors that may occur in the document generation process. To do so, make a selection in
the If an Error Occurs field and choose the Next button.
6. The Preview Results window appears. It displays all production orders that will be created grouped by the system default
values and the consolidations options you selected.
7. To generate the documents, choose the Next button.
The system creates the relevant documents and displays a summary report of all documents that were created and any
errors that occurred.
All procurement documents created by the wizard are linked to the base documents. The procurement document will be
displayed in the production order in the Procurement Doc. field; you can choose the link arrow in this field to open the
related procurement document.
For purchase order, purchase quotation, and purchase request procurement documents created by the wizard, the Base
Type field will display Production Order. You can select the Base Document icon in the toolbar of such documents to open
the corresponding production order base document.
Related Information
Procurement Confirmation Wizard
Production Order Window: General Area
Document Printing
Context
Use this function to print batches of documents according to your required selection criteria. You can choose whether to print the
whole list or specific documents.
Procedure
1. From the SAP Business One Main Menu, choose one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 234

6/8/26, 6:05 AM
Financials Document Printing
Sales – A/R Document Printing
Purchasing – A/P Document Printing
Banking Document Printing
Inventory Document Printing
Service Document Printing
The Document Printing – Selection Criteria window appears.
For more information about printing sales or purchasing documents, see Document Printing – Selection Criteria.
For more information about printing checks for payment, see Document Printing – Selection Criteria: Checks for Payment.
2. Enter the selection criteria and choose the OK button.
3. In the Print Documents Window, select the documents you wish to print and choose the Print button.
Results
SAP Business One prints the desired document(s).
Related Information
Printing in SAP Business One
Document Printing - Selection Criteria
Use this window to enter selection criteria for the documents you want to print.
To open the window, choose one of the following options:
Financials Document Printing
Sales – A/R Document Printing
Purchasing – A/P Document Printing
Banking Document Printing
Inventory Document Printing
Service Document Printing
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Printing Selection Criteria Fields
Document Type
Specify the document type you want to print.
This is custom documentation. For more information, please visit SAP Help Portal. 235

6/8/26, 6:05 AM
Posting Date From ... To
Specify a range of posting dates to print documents included in that range.
For service calls, the Posting Date here refers to the time in the Created On field.
For service contracts, the Posting Date here refers to the Start Date.
Series
Specify a numbering series.
This enables you to print documents assigned to a certain numbering series.
Technician Form
Service Call
These two checkboxes are available only for service calls. You can choose whether to print technician forms or service calls.
When Batch/Serial No. Exist, Print
When Batches or Serial Numbers exist for the document, you can choose whether to print the following information:
Document and Batch/Serial No.
Document Only
Batch/Serial No. Only
This feature is not available for certain document types.
For Multiple Counters
Available only for inventory counting documents and relevant only to the multiple-counter counting type.
The following options are available:
Print All Counters' Results: All individual counters' counting results, as well as the total counting result of team counters,
are printed into one file.
Print per Counter: Each individual counter's or team counter's counting results are printed into a separate file.
Only Documents Still to Be Printed
Prints only documents that have not been printed yet.
Only Documents Yet to Be E-Mailed
Sends only documents that have not been e-mailed yet by e-mail.
Open Only
Prints only documents with the status Open.
This includes documents with a positive open quantity.
For service contracts, this includes service contracts with any status other than Terminated.
For service calls, this includes service calls with any status other than Closed.
Exclude Canceled and Cancellation Marketing Documents
Select this checkbox if you do not wish to include the canceled marketing documents and their corresponding cancellation
documents in your batch printing. Note that this checkbox affects only canceled marketing documents whose cancellation
This is custom documentation. For more information, please visit SAP Help Portal. 236

6/8/26, 6:05 AM
generates cancellation documents. For a complete list of relevant documents, see Canceling Sales and Purchasing Documents.
Internal Number From ... To
Specify the range of document numbers from which to draw documents for printing.
For service calls, the Internal Number here refers to the Call No.
For service contracts, the Internal Number here refers to the Contract No.
No. of Copies
Specify the number of copies you want to print for each document.
Print Documents Window
This window displays all the documents that meet the criteria you specified in the Document Printing – Selection Criteria
window. To print the documents, select the desired rows and choose the Print button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Print Document Fields
Document No.
Document number of the documents found according to the specified selection criteria.
Posting Date
Posting date of the documents found according to the specified selection criteria.
Due Date
Due date of the documents found according to the specified selection criteria.
BP Code
Business partner codes in the documents found according to the specified selection criteria.
Total (LC)
Total amount in local currency of the documents found according to the specified selection criteria.
In addition, you can choose the Form Settings in the toolbar to show more fields when you preview the following types of
document:
Sales document
Purchasing document
Payment
Tax invoice
Journal entry
Goods receipt and goods issue
This is custom documentation. For more information, please visit SAP Help Portal. 237

6/8/26, 6:05 AM
Inventory transfer and inventory transfer request
Production order
Service call
Service contract
Bill of exchange – receivables, bill of exchange – payables, and bill of exchange – transactions
Printing Documents Automatically
Context
You can set SAP Business One in such a way that certain document types, such as orders, are printed automatically when they are
created.
Procedure
1. Choose Administration System Initialization Print Preferences .
The Print Preferences window appears.
2. On the Per Document tab, in the Document dropdown list, select the required document type.
3. Select Print Document.
4. Enter the required number of copies in Copies (Incl. Original).
 Note
You can configure additional settings for the document. For more information, see Print Preferences: Per Document Tab.
5. Choose Update and OK.
Related Information
Print Preferences
Purchasing Reports
Analyzing your purchasing information is necessary for the success and efficiency of your business. SAP Business One provides
several different reports for the Purchasing module that assist you in running your business. Some of the reports also include
graphical displays, which facilitate information analysis. Use the sales reports to do the following:
Analyze purchasing transactions
View open documents
Generate backorder reports
View and process documents saved as drafts
More Information
Purchase Analysis
This is custom documentation. For more information, please visit SAP Help Portal. 238

6/8/26, 6:05 AM
Open Items List
Document Drafts – Selection Criteria
Open Items List
 Note
This topic contains SAP Notes that contain additional information.
This report lets you track the status of your sales and purchasing documents. You can find the customers that still need to pay for
their orders and the vendors that have not provided the items you ordered, and you can track your missing items in stock.
Use the report to view the following document types:
Open sales and purchasing documents, including A/P and A/R reserve invoices that are not yet fully paid or fully delivered
Documents that were partially copied to a target document
 Note
Closed or cancelled documents do not appear in the report.
To access the window, choose one of the following:
Sales – A/R Sales Reports Open Items List
Purchasing - A/P Purchasing Reports Open Items List
Production Production Reports Open Items List
You can also use the open items list report to change the status of relevant documents, for example, to close or cancel open
documents. For production orders, you can change the status from Planned to Released or vice versa, or select multiple
production orders and change their status at once.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Open Items List Fields
Currency
Specify the currency in which you want to display the amounts.
Open Documents
Specify the type of document that you want to display.
Sales and purchasing documents
 Note
A/P and A/R Reserve Invoices have two different statuses:
This is custom documentation. For more information, please visit SAP Help Portal. 239

6/8/26, 6:05 AM
Unpaid – Select this option to display all the open A/P or A/R reserve invoices that are not fully paid yet. This list
may include A/P or A/R reserve invoices that are already partially or fully delivered.
Not Yet Delivered – Select this option to display all the open A/P or A/R invoices that are not fully delivered yet.
This list may include A/P or A/R reserve invoices that are already partially or fully paid.
Production orders with the status Planned or Released
Missing items, that is, a list of all items with available quantity lower than zero.
After you close the window, the last document selection is saved and appears by default the next time you open the window.
Doc. No.
Reference number of the purchasing or sales document.
Installment No.
Appears only for A/P or A/R invoices and displays the successive installment number of the document.
Customer/Vendor
Customer or vendor name as it appears in the sales or purchasing document.
Days Overdue
Appears only for A/P or A/R invoices; displays the number of days beyond the due dates of the invoices.
Customer/Vendor Ref. No.
The number of a customer sales or vendor purchasing document.
Due Date
Due date of the purchasing or sales document.
Amount
Open amount in the document, including tax that is still not drawn into the target document, or not yet paid.
Net
Open amount in the document excluding the tax amount from the Tax field in the general area of the document.
Tax
Open tax amount in the document.
Original Amount
Original total amount of the document, including tax.
Posting Date
Posting date of the document.
Document Date
Date of the document.
Blanket Agreement No.
Choose which blanket agreements to report on.
This is custom documentation. For more information, please visit SAP Help Portal. 240

6/8/26, 6:05 AM
Open Item List – Production Orders
The following columns are displayed when you select the option Production Orders in the Open Documents field:
Doc. No.
The production order number.
Type
The type of production order: Standard, Special, or Disassembly.
Status
The current status of the production order.
Priority
The degree of importance of the production order indicated by integer numbers.
Open Item List – Missing Items
The following columns are displayed when you select the option Missing Items in the Open Documents field:
Item No.
Item code.
Item Description
Item description as defined in the item master data.
In Stock
Total quantity of the item as contained in all the defined company warehouses.
Ordered
Total open quantity of the item that appears in open purchase orders and open A/P reserve invoices not yet delivered.
Committed
Total open quantity of the item that appears in open sales orders and in open A/R reserve invoices that are not delivered yet.
Consignment
Number of items on consignation. The value in this field is a result of the quantity in open deliveries minus the quantity in open
returns
 Note
Drop ship warehouses are not considered in inventory reports and are therefore not included in the consignment quantity. You
can use a script to calculate the total consignation quantity of an item. For more information, see SAP Note 1773671 .
Available
The total available quantity of the item in all the company warehouses. The calculation is based on the following formula:
Qty in Stock + Qty Ordered – Qty Committed
Change To
This is custom documentation. For more information, please visit SAP Help Portal. 241

6/8/26, 6:05 AM
To change the status of a document, select the checkboxes for the relevant documents, choose the Change To button, and choose
one of the following status options (depending on the document type and current status):
Planned (only relevant to production orders)
Closed
Canceled
 Note
Alternatively, you can cancel or close open documents in one the following ways:
In a document, open the context menu and choose Cancel or Close.
Select a document and choose Data main menu Cancel or Close.
The canceled/closed documents will not appear in the report again.
Purchase Analysis
Use the Purchase Analysis report to manage your business purchasing processes efficiently. The report provides you with the
following detailed information about the purchasing volume of your vendors:
Which vendors provide the lowest prices for their products
Which products you purchase most frequently
Which of your buyers obtain the best deals
To access the report, choose one of the following:
Purchase Analysis - Selection Criteria
Purchase Analysis Report
Purchase Analysis - Selection Criteria
Use this window to specify selection criteria for the Purchase Analysis report. The window contains three tabs:
Vendors
Analyze the purchasing volume for each vendor or for vendor groups.
Items
Analyze the purchasing volume either per item or per item group.
Sales Employee
Analyze the purchasing volume per sales employee.
Each tab contains different selection criteria and generates reports that provide different aspects of the purchase volume in your
company.
This is custom documentation. For more information, please visit SAP Help Portal. 242

6/8/26, 6:05 AM
Purchase Analysis: Vendors Tab
Use this tab to specify selection criteria for the Purchase Analysis by Vendors report. This report lets you view a corresponding
purchased volume analysis for each vendor or for vendor groups.
 Note
When you run the Purchase Analysis by Vendors report, SAP Business One automatically adds together the invoices for items
and services.
To access the tab, choose Purchasing – A/P Purchasing Reports Purchase Analysis Vendors , or open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Purchase Analysis Report Vendors Tab
Annual Report, Monthly Report, Quarterly Report
Select whether you want to sum the results of the report for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio buttons, the total for the year is also displayed. In addition, if you
select one of those options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
A/P Invoices, Purchase Order, Goods Receipt PO
Select the document type on which you want to base the purchasing analysis.
 Note
If you base an A/P credit memo on an A/P down payment invoice, that A/P credit memo does not appear in the report.
Cancelled purchase orders do not appear in the report.
Goods returns are displayed as part of the Goods Receipt PO, and they decrease the purchased amount.
Individual Display
Select whether you want to display the report for an individual vendor or for a group of vendors.
Selecting the individual option displays each vendor in a separate row in the report.
Group Display
Select whether you want to display the report for an individual vendor or for a group of vendors.
If you select the group display option, each vendor group appears in a separate row in the report. To display the purchase analysis
for each vendor in a vendor group, double-click the row number of the respective vendor group.
Total by Vendor
Choose how to group the report data.
Total by Blanket Agreement
Choose how to group the report data.
This is custom documentation. For more information, please visit SAP Help Portal. 243

6/8/26, 6:05 AM
Display Amounts in System Currency
Displays amounts in the system currency.
Related Information
Transaction Codes
Journal Entry Window
Purchase Analysis: Items Tab
Use this tab to specify selection criteria for the Purchase Analysis by Items report. This report lets you analyze purchases either
per item or per item group. SAP Business One creates a purchase volume analysis for each item.
 Note
Service invoices are not included when you run the Purchase Analysis by Items report.
Use this tab to create a purchase analysis per item or item group.
To access the tab, choose Purchasing – A/P Purchasing Reports Purchase Analysis Items , or open it from the Reports
module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Items Tab Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want to sum the results of the report for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio buttons, the total for the year is also displayed. In addition, if you
select one of those options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
A/P Invoices, Purchase Order, Goods Receipt PO
Select the document type on which you want to base the purchasing analysis.
 Note
If you base an A/P credit memo on an A/P down payment invoice, that A/P credit memo does not appear in the report.
Cancelled purchase orders do not appear in the report.
Goods returns are displayed as part of the Goods Receipt PO, and they decrease the purchased amount.
As the report displays open quantities only, purchase orders and goods receipt POs are displayed with zero quantities
and zero amounts in the following scenarios:
The purchase orders are closed or fully copied to either goods receipt POs or A/P invoices.
The goods receipt POs are closed or fully copied to either A/R invoices or returns.
This is custom documentation. For more information, please visit SAP Help Portal. 244

6/8/26, 6:05 AM
Purchase orders or goods receipt POs that were partially copied into target documents are listed with remaining open
quantities for deliveries or invoices.
Individual Display, Group Display
Select whether you want to display the report for an individual item or for item groups.
Selecting the group option, displays each item group in a separate row in the report. To display the purchase for each item in an
item group, double-click the row number of the respective item group.
No Totals
Displays one row for each item or item group (depending on whether you selected Individual Display or Group Display).
Total by Vendor
Displays a row for each combination of item (or item group) and vendor from whom you bought that item.
Total by Sales Employee
Creates a row for each combination of item and sales employee who bought the item.
Main Selection: Item
Specify the item range to include in the report.
Define the item codes range, specify an item group by clicking if required, and choose Properties to use the item properties as the
selection criterion.
Secondary Selection
Offers additional selections: by vendor range, group or properties, by sales employee, or both.
Vendor
Enter the vendor code range to be included in the report.
Define vendor code ranges, specify a vendor group if required, and choose Properties to use the vendor properties as a selection
criterion.
Sales Employee
Specify the range of sales employee codes to include in the report.
Display Amounts in System Currency
Select to display the amounts in the system currency.
Purchase Analysis: Sales Employee Tab
Use the Sales Employees tab to specify selection criteria for the Purchase Analysis by Sales Employee report. This report lets you
analyze the purchasing volume per sales employee. When you run the report, SAP Business One creates a corresponding
purchasing volume analysis for each sales employee.
 Note
When you run the Purchase Analysis by Sales Employee report, SAP Business One automatically adds together the
invoices for items and services.
This is custom documentation. For more information, please visit SAP Help Portal. 245

6/8/26, 6:05 AM
The report displays results according to the sales employee of the document and not according to the different rows.
Use this tab to create a purchase analysis per sales employee.
To access the tab, choose Purchasing – A/P Purchasing Reports Purchase Analysis Sales Employee , or open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Employee Tab Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want to sum the results of the report for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio buttons, the total for the year is also displayed. In addition, if you
select one of those options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
A/P Invoices, Purchase Orders, Goods Receipt PO
Select the document type on which you want to base the purchasing analysis.
 Note
If you base an A/P credit memo on an A/P down payment invoice, that A/P credit memo does not appear in the report.
Cancelled purchase orders do not appear in the report.
Goods returns are displayed as part of the Goods Receipt PO, and they decrease the purchased amount.
Display Amounts in System Currency
Displays amounts in the system currency.
Purchase Analysis Report
This window displays the results and the name of the report, based on the selections you have made. The name of the window
consists of the following information:
...by ...for reporting period
Purchase Analysis
Vendor Year
Item Month
Sales Employee Quarter
 Example
When you select the option Annual Report on the Vendors tab, the name of the window is: Purchase Analysis by Vendor
(Annual).
This is custom documentation. For more information, please visit SAP Help Portal. 246

6/8/26, 6:05 AM
The criteria you select determine the details displayed in this window. Changing the selection criteria changes the columns in the
report.
To view a detailed breakdown of the data of a row in the report, double-click its row number in the first "#" column. A detailed
report appears.
To display the results of a report as a graph, click . The graph for the report appears in a new window.
Choose Settings to define the parameters for displaying the graph.
Purchase Analysis Report: Detailed View
This window displays the details for a specific row of the purchase analysis report. It comprises two sections:
A detailed table view
A graphical view of the purchase analysis
Specify the required type of chart display by clicking Chart Style.
To print the chart when you print the report, select Print Graphs.
Regardless of the selection you have made, decide whether to display the vendor code, item number, sales employee code, or
name in the report. To do this, choose Go To in the menu bar.
Graph Settings
Use the setting parameters in this window to define the appearance of graphs.
To access the window, create a report whose data you want to display in a graph, and click .
To display the Graph Settings window, choose Settings.
Preferences for Graph Fields
Graph Type
Select a suitable graph type.
 Note
You can create a pie chart only when the selected value for the No. of Rows field is 1.
No. of Rows
Specify the desired number of rows to be displayed in the report.
Default
Displays the default number of rows.
Display Legend
Details of the graph elements.
Element
This is custom documentation. For more information, please visit SAP Help Portal. 247

6/8/26, 6:05 AM
Description of the field included in the graph.
Including
Displays the element data in the graph.
Purchase Request Report
The purchase request report provides you with an overview of the purchase requests created in the company, and enables you to
create directly purchase quotations or purchase orders based on selected purchase requests.
1. To generate the Purchase Request Report choose: Purchasing — A/P Purchasing Reports Purchase Request Report
.
2. In the Purchase Request Report – Selection Criteria window specify the required parameters, and choose OK.
3. The Purchase Request Report window appears, displaying the information based on your selection criteria.
For Item type report, by default, the report results are grouped by item, you can group the results it by vendors if
needed.
For Service type report, by default, the report results are grouped by G/L account. You can group it be vendor if
needed.
4. To sort the report results, choose the Sort button. The Purchase Request Sort Table appears, enabling you to choose the
required sorting parameters
For Item type report, the default sorting is by Required Date and Required Quantity (per grouping). You can also
sort the results by PR No, and Target Price.
For Service type report, you can sort by Required Date and Amount.
Creating Purchase Quotations or Purchase Orders from
Purchase Request Report
Context
You can create purchase quotations or purchase orders based on selected purchase requests, directly from within the Purchase
Request Report window.
 Note
When using this option, the target documents are created and added automatically, and the user cannot make any adjustments
beforehand.
1. In the Purchase Request Report window select the rows of the purchase requests for which you want to create the
purchase quotations or purchase orders.
2. Choose the Create button, and indicate the required document type (Purchase Quotations or Purchase Orders).
3. A system message appears notifying that target documents will be created automatically for the selected rows. To
continue, choose Yes.
4. A message notifying that target documents were added successfully appears.
This is custom documentation. For more information, please visit SAP Help Portal. 248

6/8/26, 6:05 AM
 Note
The target documents are grouped by vendors. If several selected items from different purchase requests have the
same vendor , one target document is created listing all of these items.
The target date that appears in the purchase request row in the report is drawn to:
The Required Date in the Purchase Quotation document row. The Required Date in the document header is
determined by the target date of the first row drawn from the report.
The Delivery Date in the Purchase Orders document row. The Delivery Date in the document header is
determined by the target date of the first row drawn from the report.
Go To Menu - Sales and Purchasing Documents
When you process a document from the SAP Business One Sales - A/R or Purchasing - A/P module, the Go To menu contains
only functions that relevant for the specific document you are working on.
 Note
You can display the same options as on the Go To menu through the Context menu by clicking the right mouse button.
Go To Menu Options
Base Document
If rows are created with reference to an existing sales document (for example, an order or a delivery note), use this option to
display the document by positioning the cursor on the appropriate row.
Target Document
If follow-up transactions for a document were created with a reference (for example, a delivery for an order), use this option to
display the document by positioning the cursor on the row.
If more than one delivery note was created for an order row, for example, you can see the delivery note that was created last in
each case. If you want to see all the subsequent documents for an order item, use the functions under the Drag & Relate menu.
List of Business Partners
Opens the List of Business Partners window, in which you can choose the required business partner.
Row Details...
Opens the Row Details... window for a selected row in the document, which displays additional information, for example,
warehouse or sales employee details.
Row Text Details...
Opens the Text Editor window in which you can view and edit full text included in the text row.
New Activity
Opens the Activity window in the Add mode, where you can create a new activity for the business partner.
Payment Means
Opens the Payment Means window. When creating an A/R invoice, you can use it in order to enter the payment details, if the
payment is done at the same time. When using this option from an A/R invoice that was added in the past, it displays the payment
This is custom documentation. For more information, please visit SAP Help Portal. 249

6/8/26, 6:05 AM
means used for paying for the invoice.
Gross Profit
Opens the Gross Profit window, in which you can see in detail the gross profit calculated for each row of the document you are
processing.
Last Prices Report
Opens the Last Prices Report window, in which you can observe the prices used for the selected items in other documents.
Volume and Weight Calculation
Opens the Volume and Weight Calculation window, which displays the volume and weight calculation for each item.
Wtax Table
Opens details about the withholding tax involved in the respective document. For more information, see Withholding Tax Table.
Packaging
Opens the Define Packages window. This option is enabled only when you create delivery documents.
Opening and Closing Remarks
Opens the Opening and Closing Remarks window, in which you can type any relevant remarks for the documents. These remarks
appear in the printed document only.
Related Activities
Opens a window which displays all the activities related to the business partner for whom the current document is being created.
Transaction Journal
Opens the Transaction Journal – Selection Criteria window, in which you can define the required parameters for the transaction
journal report.
Document Journal
Opens the Document Journal - Selection Criteria window, in which you can define the required parameters for the document
journal report.
General Ledger
Opens the General Ledger - Selection Criteria window, in which you can define the required parameters for the general ledger
report.
Approval Status Report
Opens the Approval Status Report window, which displays the documents included in the approval process.
Serial Number Transactions Report
Opens the Serial Numbers Transactions Report window, which displays in detail the transactions of the serial numbers related to
the items in the document. For more information, see Generating the Serial Number Transactions Report.
Batch Number Transactions Report
Opens the Batch Number Transactions Report window, which displays in detail the transactions of the batch numbers related to
the items in the document.
Business Partner Code, First Row, Last Row, Remarks
Use these options to go directly to the relevant fields and rows when you create a marketing document.
This is custom documentation. For more information, please visit SAP Help Portal. 250

6/8/26, 6:05 AM
Opening and Closing Remarks
This window enables you to include additional text related to the current document. You can enter it manually or you can insert a
predefined text. This text appears in the printed document, if the print layout is designed for that purpose.
To access the window, create a sales or purchasing document and choose Go To Opening and Closing Remarks .
You can update and delete the opening and closing remarks. Display the Opening and Closing Remarks window as described
above, make the necessary changes and choose Update and then OK.
Opening and Closing Remarks
Opening Remarks
Add the required text.
Closing Remarks
Add the required text.
Insert Predefined Text
Opens a list of predefined texts. To select more than one item, use the ctrl+shift option. Choose New to add more texts to this
list.
More Information
Predefined Text - Setup
Item Availability Check
The item availability check enables you to assess the following:
If a specific item is available
If a specific item is in a particular warehouse
If a specific item quantity is available
If a specific item is available for delivery on the required date
In addition, you can check:
The item quantity available on the requested delivery date
The earliest delivery date for the full quantity required in the sales order
A basic Available-to-Promise (ATP) report that provides additional information about item availability, such as the
uncommitted stock and receipts available to satisfy potential customer orders. See Inventory Status Window.
The Item Availability Check window only appears when the quantity of an item required in a sales order is larger than the available
quantity on the delivery date, minus the minimum level. The minimum level is defined at the warehouse level (as defined in the
Item Master Data window).
The quantity is calculated as follows:
Available = In Stock + Ordered – Committed from the current date to the requested delivery date.
This is custom documentation. For more information, please visit SAP Help Portal. 251

6/8/26, 6:05 AM
If you update an existing sales order (instead of creating a new one), SAP Business One does not take into account the existing
sales order values when calculating available quantity, as it does when you create a new sales order.
 Example
A purchase order was created with a quantity of 10 items.
Sales order 1 was created with a quantity of 6 items.
Sales order 2 was created (this is a new sales order) with a quantity of 5 items, and the available quantity is calculated
as 4 items.
If the quantity in sales order 1 is updated from 6 to 8 items the available quantity is calculated as 10 items.
 Note
This window appears only if the Activate Automatic Availability Check checkbox is selected (see Administration System
Initialization Document Settings Per Document for the document type Sales Order).
To access the window, from the menu bar choose Go To Item Availability Check .
Item Availability Check Window Fields
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Warehouse
Warehouse from which the item is ordered.
Quantity Ordered
The quantity that has been ordered by customers (sales orders), based on the following calculation:
Quantity (as defined in the sales order) × Sales UoM (as defined in Inventory Item Master Data Sales Data tab = IUoM.
If units of measure are not defined for the item, this calculation is not displayed, and only the SUoM or IUoM appears.
Requested Due Date
The delivery date (for the row) when the customer requires the ordered items.
Available Quantity
The quantity of an item that will be available for delivery on the Requested Due Date for the selected warehouse. If the Requested
Due Date is beyond the item's lead time, then the Available Quantity is the requested quantity.
SAP Business One determines the available quantity by checking that the amount in the Available Quantity field is greater than
the minimum level defined at the warehouse level.
 Note
If a Delivery Date is not entered in the sales order the current system date is used.
Earliest Availability
The earliest date on which the requested stock will be available according to ATP logic (see Viewing Detailed Confirmation Status).
This is custom documentation. For more information, please visit SAP Help Portal. 252

6/8/26, 6:05 AM
If the Earliest Availability date is beyond the lead time, a message appears.
Lead time (LT) is the planned time interval between the shipping of a delivery in the ship-from location and the expected time of
arrival at the location receiving the delivery (customer or ship-to location).
The calculation of lead time is done as follows:
Current date + lead time (as defined in Inventory Item Master Data Planning Data tab) + holidays (as defined in
Administration System Initialization Company Details Accounting Data tab).
 Example
The example below describes how to calculate the earliest available date for an item.
Lead Time − When calculating the Earliest Availability date for an item:
The current date is Thursday May 22, 2008.
The lead time defined in the Item Master Data window is 3 days.
The weekend is defined as Saturday and Sunday in the Company Details window. In addition, May 27, 2008 is defined as a
holiday.
The earliest available date is calculated as Wednesday May 28, 2008.
Thursday Friday Saturday Sunday Monday Tuesday Wednesday
May 22, 2008 May 23, 2008 Weekend Weekend May 26, 2008 Holiday May 28, 2008
(1st day LT) (2nd day LT) (3rd day LT)
Select Action
Select one of the following options:
Continue – ignores the warning and creates the order as planned regardless, of the insufficient quantity available.
Change to Available Quantity – changes the quantity that appears in the order to the available quantity of the item
displayed in this window. If the available quantity is equal to or less than zero, this option is disabled.
Change to Earliest Availability − copies the Earliest Availability date to the row's Del. Date. When the earliest availability
date cannot be calculated, this option is deselected.
Display Available to Promise Report − opens the ATP report, which displays the available quantity that is required to be
delivered, on the requested due date, for the currently selected item and warehouse at the row level.
Display Quantities in Other Warehouses – opens a window that displays the quantities of the item in other warehouses.
You can choose a different warehouse if required.
Display Alternative Items – opens the Alternative Items – Selection Criteria window, from which you can choose a
different item for the order.
Delete Row – deletes the item row from the sales order.
More Information
Alternative Items – Selection Criteria
Inventory Status Window
This is custom documentation. For more information, please visit SAP Help Portal. 253

6/8/26, 6:05 AM
Row Details
Context
You can use this option to call up detailed information on a sales document row.
Procedure
1. In the sales document, position the cursor on the row and select Go To Row Details from the menu bar or simply
double-click the row number.
The detailed information displayed contains five different types of data:
Data that is copied from the item master record, such as the item description
Data that has been entered in a row, such as the order quantity
Data that is copied to the document as a result of the settings for the respective sales document, such as the item
storage location for an invoice
Data that is generated when the sales document is created, such as the total amount of an invoice row
Individual user fields that have been defined for a marketing document - rows
You can determine the fields that are displayed in the detailed information and the order in which they are displayed in the
settings for the respective sales document.
You can also display fields that you use frequently and that are displayed in the detailed information in the table.
2. To select serial numbers for a certain row, place the cursor in the Quantity column in the appropriate row and press
Ctrl+Tab .
This opens the Serial Number Selection window.
Text Row
When you create a marketing document, SAP Business One enables you to add text rows to the Contents tab for inserting any
relevant free or predefined text.
Procedure
1. In the menu bar, choose the icon to open the Form Settings window.
2. Switch to the Table Format tab. Select the Visible and Active checkboxes of the option Type.
The Type column appears in the Contents tab of your document.
3. Open the dropdown list in the Type column and select T - Text.
4. A text box pops up. Enter your free text in the text box.
To insert predefined text, choose Insert Predefined Texts.
5. Choose OK.
The document displays only the first row of the added text.
If the text is longer than displayed, double-click the row to view the entire text and edit it as necessary.
This is custom documentation. For more information, please visit SAP Help Portal. 254

6/8/26, 6:05 AM
 Note
You can copy text rows to target documents in the same way you copy other rows.
The content of the text row can be printed when you print the document, provided that you use a printing layout
designed for this purpose.
Related Information
Subtotal Row
Predefined Text - Setup
Alternative Item Row
The sales quotation may suggest alternatives to a customer request, enabling you to add alternative items to a sales quotation.
Activities
To add an alternative item, choose Table Format and select the Visible and Active checkboxes of the option Type. The
Type column appears in the relevant document. Choose A in the Type column on the Contents tab. All item details, such as
description, price, and so on, are displayed. However, the price of the item and freight costs are not included in the total amount of
the sales quotation, or in the subtotal rows.
You include alternative item rows in a target document in the same way that you include regular rows. When you create a sales
quotation with an alternative item row, the application lets you include the alternative item row as well.
 Note
The alternative item row is not related to other rows in the sales quotation and is independent – as any other regular row.
More Information
Alternative Items
Subtotal Row
This function lets you calculate and display subtotals of the preceding regular rows.
To add a subtotal row in a document, choose Table Format and select the Visible and Active checkboxes of the option
Type. The Type column appears in the relevant document. Choose and .
A subtotal line summarizes all regular lines from the previous subtotal line, the first document line, or subtotals from the previous
level.
You can add a subtotal row to any line in the document.
SAP Business One recalculates the subtotal with every change. For example, deleting a row may lead to a change in the
subtotal values.
This is custom documentation. For more information, please visit SAP Help Portal. 255

6/8/26, 6:05 AM
You copy subtotal rows to target documents the same way you copy regular rows. If you have not copied the whole
document; the subtotal is recalculated according to the values of the target document.
When a subtotal row is created, the Item Description field displays Subtotal. You can modify the value if required.
Subtotal summary amounts appear in the Total and Freight columns respectively.
Rows of Alternative Item type are not included in the subtotal calculation.
You can create an unlimited number of subtotal levels. However, the special design that defers one subtotal level from
another is limited to the 3 levels only.
Example
The following table is taken from a sales quotation. The rows with no value in the Type column are regular rows that contain items.
| Level   | #   | Type | Item No. | Quantity | Price | Total (Doc) |
| ------- | --- | ---- | -------- | -------- | ----- | ----------- |
|         | 1   |      | 001      | 10       | 15    | 150         |
|         | 2   |      | 002      | 5        | 20    | 100         |
| Level 1 | 3   |      |          |          |       | 250         |
|         | 4   |      | 005      | 3        | 10    | 30          |
|         | 5   |      | 006      | 4        | 70    | 280         |
| Level 1 | 6   |      |          |          |       | 310         |
| Level 2 | 7   |      |          |          |       | 560         |
|         | 8   |      | 008      | 1        | 50    | 50          |
|         | 9   |      | 007      | 2        | 100   | 200         |
| Level 1 | 10  |      |          |          |       | 250         |
|         | 11  |      | 011      | 5        | 30    | 150         |
|         | 12  |      | 012      | 5        | 25    | 125         |
| Level 1 | 13  |      |          |          |       | 275         |
| Level 2 | 14  |      |          |          |       | 525         |
| Level 3 | 15  |      |          |          |       | 1085        |
Rows 3 and 6 are first level subtotal rows, calculated as follows:
150 (row 1) + 100(row 2) = 250 (row 3)
30 (row 4) + 280 (row 5) = 310 (row 6)
Rows 10 and 13 are first level subtotal rows, calculated as the sum of the regular rows above them.
Row 7 is a second level subtotal row, calculated as follows:
250 (row 3) + 310 (row 6) = 560 (row 7)
This is custom documentation. For more information, please visit SAP Help Portal. 256

6/8/26, 6:05 AM
Row 14 is a second level subtotal row, calculated as the sum of rows 10 and 13.
Row 15 is a third level subtotal row, calculated as follows:
560(row 7) + 525(row 14) = 1085 (row 15)
Calculating Volume and Weight
Context
If you maintain length measurements, volume specifications, and weights for the items in the master record, you can calculate the
total volume and weight of the delivery using sales documents.
Procedure
1. When you process a sales document, choose Go To Volume and Weight Calculation .
2. In the Volume & Weight Calculation window, click to choose the relevant entries and change the volume or weight units.
3. To return to the sales document window, choose OK. If you have made changes, choose Update and OK.
Serial No. and Batch No. Transaction Reports
This report displays all transactions made for serial and batch numbers currently in the system and those that have been released
in the past.
To open the report, do the following:
Open an inventory receipt or issue document.
From the Go To menu, choose Serial Number Transactions Report or Batch Number Transactions Report.
To generate the report, enter the necessary information and choose the OK button.
More Information
Generating the Serial Number Transactions Report
Generating the Batch Number Transactions Report
Withholding Tax Table
This window appears when you create a document related to withholding tax-liable business partners. The window displays the
default ITW and VATW codes.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Table Fields
This is custom documentation. For more information, please visit SAP Help Portal. 257

6/8/26, 6:05 AM
Code, Name
Code and name of the withholding tax codes defined as defaults for the business partner.
You can change these codes and choose any code that appears in the income tax withholding codes and in the VAT withholding
codes.
Type
Displays whether the WT code is an income tax withholding or VAT withholding.
Rate
Tax rate in percents.
Base Amount
Base amount of the document for tax calculation, depending on the base type defined for the WT code.
Taxable Amount
Amount of the document that is subject to tax. You can change this amount if required.
WTax Amount
Tax amount calculated; editable value.
Category
Displays whether the tax code is related to the invoice category or the payment category.
Base Type
Base type of the WT code:
Net: Amount before taxes
VAT: Uses the VAT amount as the base amount
Criteria
Displays the selections made in the business partner master data.
Account
G/L account in which the journal entry for the tax is recorded.
More Information
Withholding Tax Codes – Setup Window
Adjusting Tax Amount
You can manually adjust the tax amounts of purchasing documents in Add mode.
Procedure
To adjust the tax amount from a document or line item level:
This is custom documentation. For more information, please visit SAP Help Portal. 258

6/8/26, 6:05 AM
1. For a specific document, choose Form Settings Table Format / Row Format Tax Amount (LC) , and select the
Visible and Active checkboxes to activate them.
2. On the Contents tab of the document window, adjust the Tax Amount (LC).
To adjust the tax amount for freight:
1. From the SAP Business One Main Menu, choose Administration System Initialization Document Settings .
2. On the General tab, select the checkbox Manage Freight in Documents.
3. For a specific document, choose Form Settings Table Format / Row Format , and select the Visible and Active
checkboxes for the freight taxes.
4. On the Contents tab of the document window, adjust the freight taxes.
Related Information
Purchasing Documents: Contents Tab
Adjusting Tax Amount
Blanket Agreements
Blanket agreements are long-term arrangements between a purchasing organization and a vendor, or a sales organization and a
customer, for the supply of items or provision of services over a period of time based on predefined terms and conditions. Blanket
agreements can be used as a basis for expected revenue forecasts and capacity planning.
In SAP Business One, you can have two types of blanket agreements:
General blanket agreements: Are used to track fulfillment of terms to obtain a special bonus at year end, for example, for
selling or purchasing a certain quantity of an item or for achieving a defined turnover.
Specific blanket agreements: Are used to track fulfillment of terms to obtain a special discount for the individual sales or
purchasing transaction. They are also used to determine a delivery schedule, for example, by defining at which intervals
which quantity of goods should be delivered.
If a valid blanket agreement exists with a customer or vendor, SAP Business One automatically links sales and purchasing
documents to the blanket agreement. This way, the prices agreed upon with the business partners can be copied directly into the
sales and purchasing documents. You can also choose to remove the link and create a sales or purchasing document that is not
governed by a blanket agreement.
How to Work with Blanket Agreements
Blanket agreements can be set up in different ways, depending on the type of agreement and the terms and conditions you have
negotiated with your business partner. Below you can find some scenarios that show how blanket agreements can be used.
Process
Scenario 1: Generate a specific turnover with the business partner and buy or sell goods at a defined price
1. You create a blanket agreement for the business partner and specify the following:
The items governed by the agreement
This is custom documentation. For more information, please visit SAP Help Portal. 259

6/8/26, 6:05 AM
The turnover you intend to generate
The prices negotiated with the business partner
If you want to buy or sell items at specific intervals, use the agreement type Specific.
If the blanket agreement does not call for the goods to be provided at a certain date or time, use the agreement type
General.
For more information about how to create a blanket agreement, see Managing Blanket Agreements.
2. You buy or sell goods associated with the blanket agreement and create the corresponding sales or purchasing documents.
For more information, see Purchasing Goods Related to a Blanket Agreement and Selling Goods Related to a Blanket
Agreement.
3. You check the fulfillment status of the agreement. You can do this at any time according to your business needs, either by
opening the relevant blanket agreement or by displaying a list of all blanket agreements. For more information about the
latter, see Displaying Available Blanket Agreements.
4. When the turnover you planned to generate with the business partner has been reached, the blanket agreement can be
terminated. If you realize that the terms of the agreement may not be reached within the validity period of the agreement,
you find countermeasures or renegotiate with your business partner.
Scenario 2: Buy or sell a defined quantity of goods and receive a value credit memo
1. You create a blanket agreement for the business partner, specifying the number of items you plan to buy or sell.
If you want to buy or sell items at specific intervals, use the agreement type Specific.
If the blanket agreement does not call for the goods to be provided at a certain date or time, use the agreement type
General.
For more information about how to create a blanket agreement in the system, see Managing Blanket Agreements.
2. You buy or sell goods associated with the blanket agreement and create the corresponding sales or purchasing documents.
For more information, see Purchasing Goods Related to a Blanket Agreement and Selling Goods Related to a Blanket
Agreement.
3. You check the fulfillment status of the agreement. You can do this at any time according to your business needs, either by
opening the relevant blanket agreement or by displaying a list of all blanket agreements. For more information about the
latter, see Displaying Available Blanket Agreements.
4. When the planned quantity of the agreement has been reached, you issue a credit memo for your customer, or, if you are
the buyer, receive a credit memo from your vendor. To record this in the system, create an A/R credit memo or A/P credit
memo without inventory movement.
 Note
You can create multiple blanket agreements with the same business partner, same items and same period.
Managing Blanket Agreements
Use the procedures below to add, approve, and update blanket agreements.
Procedure
Adding a New General Blanket Agreement
This is custom documentation. For more information, please visit SAP Help Portal. 260

6/8/26, 6:05 AM
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
The Blanket Agreement window opens in Find mode. Switch to Add mode.
2. In the general area, specify the following:
Business partner code or name
Start date of the agreement
End date of the agreement
3. Optional: In the Description field, enter a short description of the blanket agreement.
4. On the General tab, select the agreement type General and do the following:
Specify the status of the agreement.
 Note
You can create sales and purchasing documents associated with a blanket agreement only if the blanket
agreement has the status Approved or Terminated. If the status is Terminated, the posting date of the
document must be within the date range of the agreement, that is, between the start date and the termination
date.
Choose whether to use the prices you specify on the Items tab of the blanket agreement or to use the prices defined
in the price list. In the latter case, leave the Ignore Prices Specified in Blanket Agreement checkbox selected.
If you want a reminder to appear before the blanket agreement expires, select the Renewal checkbox.
For more information about the individual fields on this tab, see Blanket Agreement: General Tab.
5. On the Items tab, specify at least one item, and the prices and quantities governed by the agreement.
For more information, see Blanket Agreement: Items Tab.
6. To attach the signed agreement document to the blanket agreement in SAP Business One, on the Attachments tab, choose
the Browse button to navigate to and append the file.
7. To save the blanket agreement, choose Add.
Adding a New Specific Blanket Agreement
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
The Blanket Agreement window opens in Find mode. Switch to Add mode.
2. In the general area, specify the following:
Business partner code or name
Start date of the agreement
End date of the agreement
3. Optional: In the Description field, enter a short description of the blanket agreement.
4. On the General tab, select the agreement type Specific and do the following:
Specify the status of the agreement.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 261

6/8/26, 6:05 AM
You can create sales and purchasing documents associated with a blanket agreement only if the blanket
agreement has the status Approved or Terminated. If the status is Terminated, the posting date of the
document must be within the date range of the agreement, that is, between the start date and the termination
date.
Choose whether to use the prices you specify on the Items tab of the blanket agreement or to use the prices defined
in the price list. In the latter case, leave the Ignore Prices Specified in Blanket Agreement checkbox selected.
If you want a reminder to appear before the blanket agreement expires, select the Renewal checkbox.
For more information about the individual fields on this tab, see Blanket Agreement: General Tab.
5. On the Items tab, specify the items, prices, and quantities governed by the agreement.
For more information, see Blanket Agreement: Items Tab.
6. To enter detailed information, such as the intervals at which items should be released against the blanket agreement,
double-click the item line.
The Blanket Agreement Details window appears.
a. Enter the following mandatory information:
Frequency
From and To date
Quantity
Consume Forecast
b. After you have made your entries in the Blanket Agreement Details window, choose Update and OK.
For more information, see Blanket Agreement Details.
7. To attach the signed agreement document to the blanket agreement in SAP Business One, on the Attachments tab of the
Blanket Agreements window, choose the Browse button to navigate to and append the file.
8. To save the blanket agreement, choose Add.
Approving a Blanket Agreement
To be able to buy or sell items according to a blanket agreement, the agreement must be approved.
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
2. Open the relevant blanket agreement in Find mode.
3. Set the status of the blanket agreement to Approved and choose Update.
4. To save the changes, choose OK.
 Note
An authorizer can reject a blanket agreement after it has been approved. However, rejection is not possible if the
agreement has linked sales or purchasing documents.
Changing a Blanket Agreement
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
2. Open the relevant blanket agreement in Find mode.
This is custom documentation. For more information, please visit SAP Help Portal. 262

6/8/26, 6:05 AM
3. Modify the necessary fields and choose Update.
4. To save the changes, choose OK.
The following validation rules apply when you change the blanket agreement in marketing documents:
If the target document is a Return Request, changing the blanket agreement for it is not allowed.
If a Credit Memo is drawn from a Reserve Invoice, changing a blanket agreement in the Credit Memo is not
allowed for the non-delivered lines.
Changing a blanket agreement for the following documents is not allowed:
A/R Invoices that are drawn from Deliveries
A/P Invoices that are drawn from Goods Receipt POs
A/R Credit Memos that are drawn from Returns
A/P Credit Memos that are drawn from Goods Returns
Deliveries that are drawn from A/R Reserve Invoices
Goods Receipt POs that are drawn from A/P Reserve Invoices
Deliveries that are drawn from A/R Correction Invoices
Goods Receipt POs that are drawn from A/P Correction Invoices
A/R Credit Memos that are drawn from A/R Down Payment Requests
A/P Credit Memos that are drawn from A/P Down Payment Requests
Terminating a Blanket Agreement
To terminate a blanket agreement before it has reached its end date, proceed as follows:
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
2. Open the relevant blanket agreement in Find mode.
3. In the Termination Date field of the General area, specify the date on which the agreement ceases to be effective and
choose Update.
The agreement status changes to Terminated and further sales or purchases associated with this agreement can only be
made if the posting date of the sales or purchasing document lies between the start date and the termination date of the
agreement.
4. To save the changes, choose OK.
Copying from a Blanket Agreement to Another Document
1. Create a sales blanket agreement or purchasing blanket agreement with the Items Method option as the agreement
method.
2. Choose Add and exit the window.
3. Open the blanket agreement again and choose Copy To.
You can copy an existing sales blanket agreement to the following document types:
Sales Quotation
This is custom documentation. For more information, please visit SAP Help Portal. 263

6/8/26, 6:05 AM
Sales Order
Delivery
A/R Invoice
A/R Down Payment Request (where available)
A/R Down Payment Invoice
Similarly, you can copy an existing purchasing blanket agreement to the following document types:
Purchase Quotation
Purchase Order
Goods Receipt PO
A/P Down Payment Request (where available)
A/R Down Payment Invoice
 Note
A/P invoices are unavailable because they open without a default posting date, and thus the validity of the
purchasing blanket agreement cannot be verified.
Copying from an Existing Document to a Blanket Agreement
1. Create a sales blanket agreement or purchasing blanket agreement with the Items Method option as the agreement
method.
2. Choose Add and exit the window.
3. Open any of the documents listed in the above scenario and enter the business partner for which the blanket agreement
was created.
4. Choose Copy From.
The Copy From dropdown list displays all lower type documents and blanket agreement.
If you select the Blanket Agreement option from the dropdown list, all blanket agreements valid at the posting date of the
document are displayed. When working on an A/P invoice, you must enter the posting date before choosing Copy From,
since the posting date determines whether a purchasing blanket agreement is valid or not.
Once you choose a blanket agreement, the Draw Document Wizard (DDW) allows you to either choose Draw All Data or
Customize. If you select Customize, you can select the rows you want to copy.
It is not possible to change the quantity of an item to be copied at this stage. You can change an item´s quantity later in the
Quantity field of the document row. The Remarks field in the target document displays the blanket agreement information.
Displaying Available Blanket Agreements
To see at a glance all blanket agreements that may exist with particular business partners or for certain date ranges, you can
generate a blanket agreement list report.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 264

6/8/26, 6:05 AM
1. From the SAP Business One Main Menu, choose Sales – A/R Sales Reports Blanket Agreement Fulfillment Report
or Purchasing – A/P Purchasing Reports Blanket Agreement Fulfillment Report . Alternatively, open it from the
Reports module.
2. In the Blanket Agreement Fulfillment Report – Selection Criteria window, specify the selection criteria for the report, for
example:
Blanket agreement number
Business partner code
Start date
End date
Termination date
Agreement type
Agreement status
Fulfillment status
3. Choose OK.
Result
The blanket agreement fulfillment report shows the following information:
Agreement No.
Sequential number of the agreement, which is assigned automatically by SAP Business One.
BP Code
Code of the business partner with whom you have made the agreement.
BP Name
Name of the business partner with whom you have made the agreement.
Start Date
Date on which the agreement becomes effective.
You can change the date when no document is linked to the blanket agreement, and the status of the blanket agreement is On
Hold.
End Date
Date until which the agreement is effective.
Termination Date
Date on which the blanket agreement ceases to be effective, if the agreement is terminated before the actual end date. When you
enter a date, the agreement status changes to Terminated.
Fulfilled Status
Shows whether the terms of the agreement have been fulfilled for a particular item, that is, whether the agreed number of items or
agreed monetary amount has been reached.
Agreement Type
This is custom documentation. For more information, please visit SAP Help Portal. 265

6/8/26, 6:05 AM
The kind of agreement you have made with your business partner:
General
Used if the terms of the agreement aim at achieving a certain number of items sold or turnover with the business partner
and thus obtaining a special bonus at year end.
Specific
Used if a special discount is to be given for each business transaction related to the agreement, or if a certain delivery plan
has been agreed upon, for example, the sale or purchase of a certain quantity or value of items at regular intervals.
Owner
Name of the employee who is responsible for the blanket agreement.
Item No.
Number of the item that is covered by the blanket agreement.
Item Description
Item description as maintained in the item master data.
Unit Price
Price of the item that you agreed upon with the business partner.
Planned Quantity
Total quantity of items that are supposed to be sold or bought within the realm of the blanket agreement.
Cumulative Quantity
The number of those items that are included in sales or purchasing transactions associated with the blanket agreement. This value
is filled in by the system.
Open Quantity
The number of items that are not yet included in sales or purchasing transactions associated with the blanket agreement. That is,
the planned quantity minus the cumulative quantity. This value is filled in by the system.
Cumulative Amount
The monetary value of those items that are included in sales or purchasing transactions associated with the blanket agreement.
This value is filled in by the system.
Open Amount
The monetary value of the open quantity. That is, of the items that are not yet included in sales or purchasing transactions
associated with the blanket agreement. This value is filled in by the system.
Cumulative Ordered Qty
The cumulative open quantity in purchase orders or sales orders which relates to the blanket agreement.
Cumulative Ordered Amount
The cumulative open amount in purchase orders or sales orders which relates to the blanket agreement.
Total Open Qty
The sum total of Planned Quantity - (Cumulative Quantity + Cumulative Ordered Quantity).
This is custom documentation. For more information, please visit SAP Help Portal. 266

6/8/26, 6:05 AM
Total Open Amount
The sum total of Planned Amount - (Cumulative Amount + Ordered Amount) in local currency.
Purchasing Goods Related to a Blanket Agreement
Prerequisites
A blanket agreement exists for the business partner, and the posting date of the purchasing transaction falls into the validity
period of the agreement.
Context
You negotiated a blanket agreement with your vendor governing the purchase of a certain number of goods over a certain period of
time at a certain price. To record purchasing transactions in relation to the blanket agreement, you create purchasing documents
such as purchase orders or invoices that are linked to the blanket agreement.
In addition, you can set up recurring transactions to support the recurring purchasing transactions governed by the blanket
agreement. For more information about recurring transactions, see Recurring Transactions.
Procedure
1. Start to create a new purchasing document, for example, a purchase order or goods receipt PO, by opening a purchasing
document in Add mode.
2. Specify at least the following information:
Vendor code
Posting and delivery date
Item code
Quantity
SAP Business One checks whether a blanket agreement for this vendor exists that is valid at the specified posting date and
covers the desired items. If there is such an agreement, it enters the blanket agreement number into the Blanket
Agreement column for each item. It also inserts the unit prices agreed upon in the blanket agreement. If the Ignore Prices
Specified in Blanket Agreement checkbox on the General tab of the blanket agreement has been selected, the prices
defined in the price list are used.
 Note
If the item quantity you entered is larger than the open quantity of the blanket agreement, a system message appears.
3. If required, specify any additional data.
4. To save the document, choose Add and OK.
Results
SAP Business One creates a purchasing document associated with a blanket agreement. If the document involves inventory
movement, the purchasing document has the following impact on the blanket agreement:
Increases the cumulative quantity and cumulative amount
Decreases the open quantity and open amount
This is custom documentation. For more information, please visit SAP Help Portal. 267

6/8/26, 6:05 AM
 Note
If you cancel the purchasing document later, linked blanket agreements in the cancellation document remain the same,
regardless of whether the posting date of the cancellation document is still within the durations of the agreements. After the
cancellation, the above-mentioned cumulative and open values in all linked agreements are reverted.
Selling Goods Related to a Blanket Agreement
Prerequisites
A blanket agreement exists for the business partner, and the posting date of the sales transaction falls into the validity period of
the agreement.
Context
You negotiated a blanket agreement with your customer governing the sale of a certain number of goods over a certain period of
time at a certain price. To record sales transactions in relation to the blanket agreement, you create sales documents such as
deliveries or invoices that are linked to the blanket agreement.
In addition, you can set up recurring transactions to support the recurring sales transactions governed by the blanket agreement.
For more information about recurring transactions, see Recurring Transactions.
Procedure
1. Start to create a new sales document, for example, a sales order or delivery, by opening a sales document in Add mode.
2. Specify at least the following information:
Customer code
Posting and delivery date
Item code
Quantity
SAP Business One checks whether a blanket agreement for this customer exists that is valid at the specified posting date
and covers the desired items. If there is such an agreement, it enters the blanket agreement number into the Blanket
Agreement column for each item. It also inserts the unit prices agreed upon in the blanket agreement. If the Ignore Prices
Specified in Blanket Agreement checkbox on the General tab of the blanket agreement has been selected, the prices
defined in the price list are used.
 Note
If the item quantity you entered is larger than the open quantity of the blanket agreement, a system message appears.
3. If required, specify any additional data.
4. To save the document, choose Add and OK.
Results
SAP Business One creates a sales document associated with a blanket agreement. If the document involves inventory movement,
the sales document has the following impact on the blanket agreement:
This is custom documentation. For more information, please visit SAP Help Portal. 268

6/8/26, 6:05 AM
Increases the cumulative quantity and cumulative amount
Decreases the open quantity and open amount
 Note
If you cancel the sales document later, linked blanket agreements in the cancellation document remain the same, regardless of
whether the posting date of the cancellation document is still within the durations of the agreements. After the cancellation,
the above-mentioned cumulative and open values in all linked agreements are reverted.
Blanket Agreement: General Area
Use this part of the blanket agreement to specify general information relevant to all items in the agreement.
To access this area, choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
General Area Fields
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
BP Code
Code of the business partner with whom you have made the agreement.
BP Name
Name of the business partner with whom you have made the agreement.
Customer Ref. No.
Displays the customer reference number.
Editable when the blanket agreement status is Draft or On Hold.
Vendor Ref. No.
Displays the vendor reference number.
Editable when the blanket agreement status is Draft or On Hold.
BP Currency
Currency of the business partner with whom you have made the agreement. Business partners with All Currencies will be handled
as local currency business partners.
Agreement No.
Sequential number of the agreement, which is assigned automatically by SAP Business One.
Start Date
Date on which the agreement becomes effective.
You can change the date when no document is linked to the blanket agreement, and the status of the blanket agreement is On
Hold.
Exchange Rate
This is custom documentation. For more information, please visit SAP Help Portal. 269

6/8/26, 6:05 AM
Available only when the following apply:
The business partner currency is a foreign currency
On the General tab of the Document Settings window, at least one of the following checkboxes is selected
Block Multiple Blanket Agreements for Same A/P Document
Block Multiple Blanket Agreements for Same A/R Document
Determines a exchange rate to be used to calculate the local currency amount in monetary blanket agreements. Calculation is not
applied to the closed rows.
When the status of the blanket agreement is Draft or On Hold, you can update or remove this exchange rate even if there are
documents linked to the blanket agreement.
 Note
When you copy a blanket agreement to a marketing document, the exchange rate of this blanket agreement overrides the
document exchange rate. Purchase quotation is an exception.
End Date
Date until which the agreement is effective.
BP Project
Select the project that you want to relate to the blanket agreement.
When a blanket agreement is associated with a marketing document, either automatically or manually, the project defined in the
blanket agreement will be taken into the BP Project field in the document.
Termination Date
Date on which the blanket agreement ceases to be effective, if the agreement is terminated before the actual end date. When you
enter a date, the agreement status changes to Terminated.
Signing Date
Date which the agreement was signed.
Description
Descriptive text for the agreement, if required.
Blanket Agreement: General Tab
Use this part of the blanket agreement to specify the general terms of the agreement.
To access this tab, choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
General Tab Fields
Agreement Type
The kind of agreement you have made with your business partner:
General
This is custom documentation. For more information, please visit SAP Help Portal. 270

6/8/26, 6:05 AM
Used if the terms of the agreement aim at achieving a certain number of items sold or turnover with the business partner
and thus obtaining a special bonus at year end.
Specific
Used if a special discount is to be given for each business transaction related to the agreement, or if a certain delivery plan
has been agreed upon, for example, the sale or purchase of a certain quantity or value of items at regular intervals.
Ignore Prices Specified in Blanket Agreement
When the blanket agreement is with the type of General, the checkbox is selected and grayed out. It means that when you relate
the blanket agreement to sales or purchasing documents, any special prices that may have been defined for the business partner
in price lists take precedence in sales and purchasing documents over the price you specify in the blanket agreement.
When the blanket agreement is with the type of Specific, the checkbox is deselected and grayed out. It means that when you relate
the blanket agreement to sales or purchasing documents, the prices specified in the blanket agreement take precedence in sales
and purchasing documents over other prices you define.
Payment Terms
Define the payment terms for the blanket agreement.
 Note
When you copy a blanket agreement to a marketing document, the payment term defined in this blanket agreement
overrides the document payment terms.
When you copy multiple blanket agreements to a marketing document, and the payment terms defined in the blanket
agreements are not the same, the document payment term remains unchanged.
When a blanket agreement is linked to the document lines without using the Copy To function, the payment term
defined in the blanket agreement has no impact on the document.
Payment Method
Define the payment method for the blanket agreement.
 Note
When you copy a blanket agreement to a marketing document, the payment method defined in this blanket agreement
overrides the document payment method.
When you copy multiple blanket agreements to a marketing document, and the payment methods defined in the
blanket agreements are not the same, the document payment method remains unchanged.
When a blanket agreement is linked to the document lines without using the Copy To function, the payment method
defined in the blanket agreement has no impact on the document.
Shipping Type
Define a shipping type for the blanket agreement.
When a blanket agreement is associated with a marketing document, either automatically or manually, the shipping type defined
in the blanket agreement will be taken into the Shipping Type field in the document.
Settlement Probability %
Specify a percentage value to indicate how probable it is that the business partner will pay for the goods.
Status
This is custom documentation. For more information, please visit SAP Help Portal. 271

6/8/26, 6:05 AM
Select the status of the blanket agreement.
Approved
You can sell or buy items and thus create sales or purchasing documents associated with the blanket agreement.
On Hold
Blanket agreement is set to inactive, and you cannot sell or buy items and thus create sales or purchasing documents
associated with the blanket agreement.
When the document status is On Hold, you can still edit user-defined fields in the rows section of a blanket agreement. For
more information about user-defined fields, see How to Create User-Defined Fields and Tables in SAP Business One 10.0.
Draft
The blanket agreement is not approved, and you cannot sell or buy items and thus create sales or purchasing documents
associated with the blanket agreement.
Terminated
The blanket agreement is terminated. Once you set a blanket agreement as terminated, regardless of the Termination Date
you define, SAP Business One considers this blanket agreement as terminated, and you can no longer create sales or
purchasing documents associated with the blanket agreement.
Price List
Select the price list for monetary blanket agreement.
Owner
Name of the employee who is responsible for the blanket agreement.
Renewal
If you select this checkbox, you can set a reminder for renewing a blanket agreement before it expires.
Reminder
The number of days, weeks, or months for the alert to appear prior to the termination of the blanket agreement. You can specify a
value in this field only after you select the Renewal checkbox.
Price Mode
Appears only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Determine the price mode for the blanket agreement.
Net - On the Details tab of the Blanket Agreement window, the Unit Price column is enabled. The prices you enter are the
item prices excluding tax.
Gross - On the Details tab of the Blanket Agreement window, the Gross Price column is enabled. The prices you enter are
item prices including tax.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Blanket Agreement: Items Tab
This is custom documentation. For more information, please visit SAP Help Portal. 272

6/8/26, 6:05 AM
Use this tab to specify the items that can be purchased or sold within the realm of the blanket agreement.
To access this tab, choose Sales – A/R Sales Blanket Agreement Items or Purchasing – A/P Purchase Blanket
Agreement Items .
Items Tab Fields
Item No.
Number of the item that is covered by the blanket agreement.
Item Description
Item description as maintained in the item master data.
Item Group
Item group as maintained in the item master data.
Planned Quantity
Total quantity of items that are supposed to be sold or bought within the realm of the blanket agreement.
Unit Price/Gross Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
If the Price Mode defined on the General tab is Net, Unit Price is displayed. Enter the item net price you agreed on
with the business partner.
If the Price Mode defined on the General tab is Gross, Gross Price is displayed. Enter the item gross price you
agreed on with the business partner.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter the item prices that you agreed on with the business partner.
Cumulative Committed Quantity
Display the sum of the quantity of the item in the open lines of the sales orders and non-delivered A/R reserve invoices that are
associated with the blanket agreement.
Cumulative Committed Amount
The total monetary value of those items from open lines in sales orders and non-delivered A/R reserve invoices associated with
the blanket agreement. This value is filled in by the system.
Cumulative Ordered Quantity
Display the sum of the quantity of the item in the open lines of the purchase orders and non-delivered A/P reserve invoices that
are associated with the blanket agreement.
Cumulative Ordered Amount
The total monetary value of the items in the open lines of the purchase orders and non-delivered A/P reserve invoices that are
associated with the blanket agreement.
This is custom documentation. For more information, please visit SAP Help Portal. 273

6/8/26, 6:05 AM
Cumulative Quantity
The number of those items that are included in sales or purchasing transactions associated with the blanket agreement. This value
is filled in by the system.
Cumulative Amount
The monetary value of those items that are included in sales or purchasing transactions associated with the blanket agreement.
This value is filled in by the system.
Open Quantity
The number of items that are not yet included in sales or purchasing transactions associated with the blanket agreement. That is,
the planned quantity minus the cumulative quantity. This value is filled in by the system.
Open Amount
The monetary value of the open quantity. That is, of the items that are not yet included in sales or purchasing transactions
associated with the blanket agreement. This value is filled in by the system.
Shipping Type
Display the shipping type defined for the blanket agreement. You can change the shipping type when the status of the blanket
agreement is Draft or On Hold.
When you link the blanket agreement to the document row, either manually or automatically, this shipping type will be taken into
the marketing document rows.
Project
Display the project defined for the blanket agreement. You can change the project in open lines when the status of the blanket
agreement is Draft or On Hold.
When you link the blanket agreement to the document row, either manually or automatically, this project will be taken into the
marketing document rows.
UoM
Type of unit by which the inventory is managed as defined in the item master data.
Portion of Returns %
Specify a percentage value for the probability that damaged goods will be returned by the business partner.
End of Warranty
Specify the date on which the warranty of the goods expires.
 Note
This field is not related to any warranties you may have defined in the Service module of SAP Business One.
Blanket Agreement: Details Tab
Use this window to specify details of a delivery plan for an item, for example, the intervals at which an item should be delivered.
To access this window, open a blanket agreement of type Specific, choose the Items tab, and double-click an item line.
Frequency
Period of item release, for example, daily, weekly, monthly, or one-time.
This is custom documentation. For more information, please visit SAP Help Portal. 274

6/8/26, 6:05 AM
Daily: The quantity is divided by each day within the period you define for the item line.
Weekly: The quantity is divided by the number of weeks within the period starting from the From date with the end of last
week falling closest to or on the To date. If the period is less than a week, the total quantity is assigned to the From date.
Monthly, Quarterly, Semi-Annually, and Annually follow the same principle as Weekly.
One Time: This represents a single instance, so the whole quantity relates to the From date only.
From
Start date of the release plan, that is, the date as of which release against the blanket agreement starts. This date cannot be earlier
than the start date of the blanket agreement.
To
End date of the release plan, that is, date until which release against the blanket agreement takes place. This date cannot be later
than the end date of the blanket agreement.
Release
Enter Information related to a specific release against the blanket agreement, for example, release date, and remarks.
Quantity
Number of items to be released during the release period. The number must be lower than or equal to the planned quantity on the
Blanket Agreement Items tab.
Warehouse
Warehouse from which the goods should be released.
Consume Forecast
To the item in blanket agreements to consume forecast, select the checkbox.
 Note
To consume forecast using blanket agreements, you must also select the Consume Forecast checkbox on the General Settings:
Inventory Tab.
In the MRP run, the application subtract the item's open quantities in blanket agreements with the type of Specific from the
forecasted quantities.
For more information, see Managing Forecasts.
Activity
To record an activity, such as a phone call or meeting, associated with the blanket agreement, click the yellow arrow and specify
the required information.
More Information
General Settings: Inventory Tab
Blanket Agreement: Documents Tab
Use this tab to view the documents associated with the blanket agreement.
This is custom documentation. For more information, please visit SAP Help Portal. 275

6/8/26, 6:05 AM
To access this tab, choose Sales – A/R Sales Blanket Agreement Documents or Purchasing – A/P Purchase Blanket
Agreement Documents .
Documents Tab Fields
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Type
Type of document that was created and associated with the blanket agreement, for example, a sales order or A/P invoice.
Document No.
Number of the document that was created and associated with the blanket agreement.
Row No.
Number of the row in the document that is associated with the blanket agreement.
Unit Price
Price of the item used in the sales or purchasing document.
Document Status
Display the status of the document that was associated with the blanket agreement.
Blanket Agreement: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However,
if it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
This is custom documentation. For more information, please visit SAP Help Portal. 276

6/8/26, 6:05 AM
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
This is custom documentation. For more information, please visit SAP Help Portal. 277