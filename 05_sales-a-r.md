6/8/26, 6:04 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:04:35 GMT+0000
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

6/8/26, 6:04 AM
Sales Process in SAP Business One
The sales process moves from issuing a sales quotation for goods to selling the goods (and services) to delivering the goods to
invoicing the customer for the goods. Each step involves a document, such as a sales order or A/R invoice. SAP Business One
moves all relevant information from one document to the next in the document flow. You can adapt the steps according to your
needs and business processes.
Prerequisites
To avoid problems during document creation in later stages of the sales process, make sure that the following key data is
maintained correctly before you start creating sales documents:
Business partner master data, especially the customer's bill-to and ship-to address, payment terms and dunning
parameters
Item master data
Process
Please note that image maps are not interactive in PDF outputs.
Additional Sales Process Documents
Please note that image maps are not interactive in PDF outputs.
It is possible to create new documents based on existing ones. When you do so, only the documents that are still open are
displayed. Open documents:
Are those for which you have not created a follow-on document
Remain open until you transfer all items completely to the follow-on document, or until you manually close or reverse them
Different Operations in Sales Process Documents
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
More Information
Sales – A/R
Sales Quotation
You create the sales quotation document as an offer or proposal that you send either to a customer, or to a lead.
The sales quotation, as it is displayed in SAP Business One, is not a legally binding document. It is generally used for information
purposes only, and can be the first link in the sales process chain.
Entering a quotation does not result in any posting that alters quantities or values in inventory management or accounting.
To open the window, choose Sales – A/R Sales Quotation .
More Information
Creating Sales Documents
Sales Quotation: General Area
Sales Document: Contents Tab
Sales Quotation: Logistics Tab
Sales Quotation: Accounting Tab
Sales Quotation: General Area
Use this part of the sales quotation to enter general information relevant to all items in the document.
To open the window, choose Sales – A/R Sales Quotation .
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Quotation General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
Specify the customer reference number, if required.
No.
Field on the left: name of the numbering series.
Specify a series.
Field on the right: the number of the sales quotation. If you choose the manual series, enter the relevant number.
Status
Status of the sales quotation:
Open
You can draw the document completely or partially to a document of a higher level.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
Not Confirmed
The document is not yet confirmed, thus cannot be copied to other documents.
Posting Date
Specify the posting date. The default value for this field is the current date on which the sales quotation is created. If required,
change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Valid Until
Enter the date until which the sales quotation is valid.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:04 AM
The current default date is 30 days after the posting date. If you specify a default Valid Until date for Sales Quotation documents in
the Administration System Initialization Document Settings Per Document tab, the default date becomes the number
of days/weeks/months after the posting date that you specify.
You can change it manually if needed. The field is informative only.
Document Date
Document date of the sales quotation, used for tax purposes. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the sales quotation.
Owner
Specify the code of the employee who owns the sales quotation.
Remarks
Enter additional information regarding the sales quotation. You can edit the field contents after the sales quotation is added.
Total Before Discount
Total amount of the sales quotation before the discount for the document is calculated.
 Note
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of discount.
The field on the right displays the amount of the discount.
Updating one of the fields updates the other field accordingly.
Freight
Displays the total freight for the sales quotation.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
Rounding
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:04 AM
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the sales quotation calculated according to your tax definitions.
Total
Total amount of the sales quotation, including tax, freight and discounts. You can edit the value.
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
Sales Quotation
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:04 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:04 AM
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
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
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:04 AM
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:04 AM
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:04 AM
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
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
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:04 AM
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:04 AM
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:04 AM
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
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
Table View for Document Type Service
Description
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:04 AM
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
Alternative Items - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:04 AM
Use this window to select an alternative item for a missing item when creating sales and purchasing documents.
1. In a sales or purchasing document, on the Contents tab, in the Item No. field, enter an item number.
2. Place your cursor In the Item No. field and press CTRL+TAB .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Alternative Items Selection Criteria Fields
Warehouse
Displays the warehouse of the original item.
 Note
A list of alternative items with a positive quantity for the selected warehouse is displayed. To view alternative items in all
warehouses, leave the Warehouse field empty.
The warehouse in the document will not be updated automatically when you select an alternative item from a different
warehouse. If this is required, change the warehouse manually before adding the document.
Price
Displays the price of the alternative item.
 Note
If the business partner has special prices for some of the alternative items, the item and the special price appear in blue.
You can change the price in the marketing document only after selecting the alternative item.
Available
The available quantity of an item is displayed. This figure comprises:
Inventory in warehouse + Ordered quantities – Committed Quantities from sales orders
In Stock
Displays the quantity of the alternative items in the warehouse. The value is displayed for the warehouse selected above. If the field
is empty, the total quantity of the alternative items in all warehouses is displayed.
Match Factor
Displays the value to specify the matching degree in points. A higher value represents a higher match.
 Example
Item 1001 has two alternative items: 1002 and 1003. The matching factor defined for item 1002 is 100 and for item 1003 is 80. If
there is no item 1001 in the warehouse, item 1002 can replace it, as it has the highest matching factor.
Additional Match
Displays an additional value for a match factor.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:04 AM
You can link a saved query to this field. In this case, use the formatted search to calculate the correct value. You can also enter
the value manually.
Total Match
Displays the total of Match Factor and Additional Match.
Remarks
Displays the remarks for the alternative items.
Choose
Choose to select the alternative item for the marketing document.
Show Tree
Choose to display the Alternative Items (Show Tree) window. This window displays the relationship between the items and shows
hierarchies.
Define Items
Choose to display the Alternative Items window to define additional alternative items.
More Information
Alternative Items
Alternative Items Window
Sales Quotation: Logistics Tab
Use this tab to specify information regarding the logistics aspects of the sales quotation.
To access the tab, choose Sales – A/R Sales Quotation Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Quotation Logistics Tab Fields
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description for this document only; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:04 AM
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
Procure Non Drop-Ship Items
If you select this option, the Procurement Confirmation Wizard opens when you add sales quotations with items from non-drop
ship warehouses.
Procure Drop-Ship Items
If you select this option, the Procurement Confirmation Wizard opens when you add sales quotations with items from drop ship
warehouses.
Confirmed
Indicates that the sales quotation is confirmed and enables copying it to a higher level of sales document.
This checkbox is selected by default if the checkbox Sales Quotation Confirmed in the Administration System Initialization
Document Settings Per Document tab is selected.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
Sales Quotation
Sales Quotation: Accounting Tab
Use this tab to specify information regarding financial aspects of the sales quotation.
To access the tab, choose Sales – A/R Sales Quotation Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Quotation Accounting Tab Fields
Journal Remark
By default, displays Sales Quotation – XXX, where XXXis the customer code. You can change this content, if required.
Payment Terms
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:04 AM
By default, displays the payment terms for the customer, as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Federal Tax ID
The customer's or lead's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master
Data General Area .
Order Number
Enter an order number of the chain when you use the direct distribution method. This number is recorded in the file that you send
to a head office of the chain store.
Use Shipped Goods Account
Select this checkbox to post the delivery of the inventory to the shipped goods account instead of the COGS account, when the
delivery of inventory and the issue of the invoice occur in different posting periods.
The default status of this checkbox is inherited from the same checkbox in the Business Partner Master Data window of the
customer for which the sales quotation is created . You can change the status of this checkbox if needed.
 Note
This checkbox is available for perpetual inventory companies only.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:04 AM
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
Sales Quotation
Sales Document: Attachments Tab
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
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:04 AM
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
Updating Sales Quotations
After you create a sales quotation, you can update it, as long as no higher level documents have been created with reference to that
sales quotation (For more information about updating the quantity of a sales quotation which is partially copied to a target
document, see SAP Note 1823500 ). Some of the possible changes include:
Delete, add, and duplicate rows
Update prices and discounts
Update quantities
Procedure
Cancelling and Closing Sales Quotations
If you stop the sales process before you copy the sales quotation (fully or partially) to a higher level sales document, such as a
delivery or A/R Invoice, you can cancel it:
1. Choose Sales – A/R Sales Quotation and find the sales quotation you want to cancel.
2. In the menu bar, choose Data Cancel .
The status Cancelled appears in the header of the sales quotation and in the Journal Remark field on the Accounting tab.
Closing Sales Quotations
If you have partially copied a sales quotation to a higher level sales document, you can only close it.
1. Choose Sales – A/R Sales Quotation and find the sales quotation you want to close.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:04 AM
2. In the menu bar, choose Data Close .
The status Closed appears in the header of the sales quotation.
Result
In both cases the sales quotation is not deleted. You can still display and duplicate it, but you cannot change it or copy it to a higher
level sales document.
The system does not display cancelled or closed sales quotations in the Open Items List report.
More Information
Sales Quotation
Sales Order
The sales order is a commitment from a customer or lead to buy a product or service. The document serves as a foundation for
planning production or purchase orders.
Your line of business determines whether or not a sales order is a legally binding document - your company may not manufacture
products or ship items before a sales order has been created.
Creating sales orders does not post value-related changes in the accounting system. However, if the sales order is created for
items, the ordered quantities are listed in Inventory Management as reserved for the customer. You can view the ordered
quantities in various reports, such as the Inventory Status report, as well as other windows in SAP Business One. This information
is important for:
Optimizing ordering transactions and stockholding
Ensuring that customer requirements are dealt with quickly and satisfactorily
To open this window, choose Sales – A/R Sales Order .
More Information
Creating Sales Documents
Sales Order: General Area
Sales Document: Contents Tab
Sales Order: Logistics Tab
Sales Order: Accounting Tab
Sales Order: General Area
Use this part of the sales order to specify general information relevant to all items in the document.
To access this area, choose Sales – A/R Sales Order .
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Order General Area Fields
Contact Person
The name of the default contact person as defined in the business partner master data. If required, specify a different contact
person.
Customer Ref. No.
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series.
Specify a series.
Field on the right: the number of the sales order. If you choose the manual series, specify the relevant number.
Status
The sales order status can be as follows:
Open
You can draw the document completely or partially to a document of a higher level.
Open: Printed
You printed the document and left it open.
Open: E-Mailed
You sent the document to business partners through SAP Business One Mailer and/or Microsoft Outlook and left the
document open.
A document is considered as sent by SAP Business One Mailer if the e-mail is marked as on the Sent Messages tab in
the Messages/Alerts Overview window. With Microsoft Outlook, a document is considered as sent when Microsoft Outlook
opens.
Open: Printed and E-Mailed
You printed and e-mailed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is a draft.
Not Confirmed
You cannot copy the sales order to a higher-level document.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:04 AM
Posting Date
Specify the posting date. The default value is the date on which the sales order is created. If required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document is interrupted.
Delivery Date
Specify the date on which you deliver the goods and create the delivery document.
 Note
When you enter or modify the Delivery Date in the General area of the window, the date is copied to the Delivery Date for all the
rows on the Contents tab, including new and existing items. Confirm the system message to copy the Delivery Date to the row
level.
Document Date
The document date of the sales order, which is used for tax purposes. Change the date if required.
Currency
Specify the currency for the amounts in the sales order.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the sales order.
Owner
Specify the code of the employee who owns the sales order.
Remarks
Enter additional information regarding the sales order. You also can edit the field content after the document is added.
Total Before Discount
The total amount of the sales order before the discount is calculated.
 Note
If the discount has been defined in the item or service row, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of discount.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:04 AM
The field on the right displays the amount of the discount. When you update one field, the other field is updated respectively. You
can change the values for these fields, if required.
Freight
Displays the total freight for the sales order.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
Rounding
This field only appears if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
The tax amount for the sales order calculated according to your tax definitions.
Total
The total amount of the sales order including tax and discounts.
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
Sales Order
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:04 AM
Item Availability Check
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:04 AM
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:04 AM
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:04 AM
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:04 AM
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:04 AM
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:04 AM
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:04 AM
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:04 AM
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:04 AM
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
Sales Order: Logistics Tab
Use this tab to specify details regarding the logistics aspects of the sales order.
To access the tab, choose Sales A/R Sales Order Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Order Logistics Tab Fields
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description for this document only; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
Procure Non Drop-Ship Items
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:04 AM
If you select this option, the Procurement Confirmation Wizard opens when you add sales orders with items from non-drop ship
warehouses.
Procure Drop-Ship Items
If you select this option, the Procurement Confirmation Wizard opens when you add sales orders with items from drop ship
warehouses.
Print Picking Sheet
Select to activate the following options when you print the Sales Order.
Order Only
Pick List Only
Order and Pick List
Deselect to print the Sales Order directly, without the option of printing the Pick List.
 Note
If the Sales Order includes an Assembly BOM item, an Assembly Components Pick List is printed in addition to the standard
Pick List.
Procurement Document
Select this option to create purchase orders or production orders for the items that appear in the sales order automatically. This
opens the Procurement Confirmation Wizard once you add the sales order.
Confirmed
Indicates that the sales order is confirmed and enables copying it to a higher level of sales document.
This checkbox is selected by default if the checkbox Confirm Sales Order Automatically in the Administration System
Initialization Document Settings Per Document tab is selected.
Allow Partial Delivery
Allows partial delivery of the sales order. If you select the checkbox, you can partially copy the sales order to a higher level sales
document.
Pick and Pack Remarks
Enter relevant remarks for the pick and pack procedure.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
Sales Order
Procurement Confirmation
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:04 AM
Sales Order: Accounting Tab
Use this tab to specify information regarding the accounting aspect of the sales order.
To access the tab, choose Sales – A/R Sales Order Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Order Accounting Tab Fields
Journal Remark
By default, displays Sales Order – XXX, where XXXis the customer code. Change this content, if required.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the sales order. This control account can then be copied to any follow-up documents.
 Note
It appears only if the checkbox Allow Control Account Selection is selected in Administration System Initialization
Document Settings Per Document for sales orders.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
BP Project
By default displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Cancellation Date
Specify the last date on which the customer accepts the goods. The default value is 30 days after the Delivery Date.
Required Date
Specify the expected date on which the goods will be delivered to the customer. The default value is the Delivery Date.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:04 AM
Indicator
By default, displays the indicator linked to the customer ( Business Partners Business Partner Master Data General tab).
The indicator is used as a selection criteria in various reports. If required, choose a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
If the sales order is based on a sales quotation, the federal tax ID that appears in this field is the one copied from the sales
quotation.
Order Number
Enter an order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Use Shipped Goods Account
Select this checkbox to post the delivery of the inventory to the shipped goods account instead of the COGS account, when the
delivery of inventory and the issue of the invoice occur in different posting periods.
For standalone sales orders, the default status of this checkbox is inherited from the same checkbox in the Business Partner
Master Data window of the customer for which the sales order is created; for sales orders that are created based on sales
quotations, the default status of this checkbox is inherited from the same checkbox in the base quotation.You can change the
status of this checkbox if needed.
 Note
This checkbox is available for perpetual inventory companies only.
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
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:04 AM
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
Sales Order
Sales Document: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:04 AM
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Updating and Cancelling Sales Orders
After you create a sales order, you can change all its data, provided that no target documents have been created based on it. Some
of the possible changes include:
Delete, add, or duplicate rows
Update prices and discounts
Update quantities
Procedure
Cancelling Sales Orders
If the sales process has been interrupted and the sales order has not yet been drawn (fully or partially) to a target sales document,
you can cancel it:
1. Choose Sales – A/R Sales Order and find the sales order you want to cancel.
2. In the menu bar, choose Data Cancel .
Or right-click the window to open the context menu. In the context menu, choose Cancel.
The status Cancelled appears.
Closing Sales Orders
When the sales order has been partially copied to a higher level sales document, you can close it but you cannot cancel it.
1. Choose Sales – A/R Sales Order and find the sales order you want to close.
2. In the menu bar, choose Data Close .
Or right-click the window to open the context menu. In the context menu, choose Close.
The status Closed appears.
Result
When you cancel or close a sales order for items, the quantity reserved for the customer is reduced by the quantity that appears in
the cancelled or closed order.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:04 AM
A cancelled or closed sales order is not deleted. You can still display or duplicate it, but you cannot change it or copy it to a higher
level sales document.
The system does not display cancelled or closed sales orders in the Open Items List report.
More Information
Sales Order
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
quantity on the delivery date, minus the minimum level. The minimum level is defined at the warehouse level (as defined in the Item
Master Data window).
The quantity is calculated as follows:
Available = In Stock + Ordered – Committed from the current date to the requested delivery date.
If you update an existing sales order (instead of creating a new one), SAP Business One does not take into account the existing
sales order values when calculating available quantity, as it does when you create a new sales order.
 Example
A purchase order was created with a quantity of 10 items.
Sales order 1 was created with a quantity of 6 items.
Sales order 2 was created (this is a new sales order) with a quantity of 5 items, and the available quantity is calculated as
4 items.
If the quantity in sales order 1 is updated from 6 to 8 items the available quantity is calculated as 10 items.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:04 AM
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
SAP Business One determines the available quantity by checking that the amount in the Available Quantity field is greater than the
minimum level defined at the warehouse level.
 Note
If a Delivery Date is not entered in the sales order the current system date is used.
Earliest Availability
The earliest date on which the requested stock will be available according to ATP logic (see Viewing Detailed Confirmation Status).
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
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:04 AM
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
Delivery
The Delivery is a legally binding document indicating that the shipment of goods or the delivery of services has occurred. Without
this document, goods can be delivered only if an invoice has already been created.
When you create a delivery, the corresponding goods issue is also posted. The goods leave the warehouse and the relevant
inventory changes are posted. When the inventory is changed, the values in the accounting system change as well (only when you
use perpetual inventory).
To open the window, choose Sales – A/R Delivery .
More Information
Creating Sales Documents
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:04 AM
Delivery: General Area
Delivery: Contents Tab
Delivery: Logistics Tab
Delivery: Accounting Tab
Closing Deliveries
Delivery: General Area
Use this part of the delivery document to enter general information relevant to all items in the document.
To access this area, choose Sales – A/R Delivery .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Delivery General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
If defined, displays the customer reference number.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: the number of the delivery. If you choose the manual series, enter the relevant number.
Status
Status of the delivery:
Open
You can draw the document completely or partially to a document of a higher level.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:04 AM
Posting Date
Specify the posting date. The default value for this field is the current date on which the delivery is created. If required, change the
date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Delivery Date
Specify the expected delivery date of the items or services. By default, this is the current date.
 Note
Even if the Delivery is created based on Sales Order, the Delivery Date is not copied from the base document
Document Date
Document date of the delivery used for tax purposes. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the delivery.
Owner
Specify the code of the employee who owns the delivery.
Remarks
Enter additional information regarding the delivery.
You can edit the field contents even after the document has been created.
Total Before Discount
Total amount of the document before the calculated discount.
 Note
If the discount is defined in the row for the item or service, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of discount.
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:04 AM
The field on the right displays the discount amount. You can change the values of these fields, if required.
Freight
Displays the total freight for the delivery.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the delivery calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Copy From
A list of base documents for creating a target document.
 Note
When you copy a sales order to a delivery, only one delivery is created, even if several ship to addresses are used for different
rows.
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
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:04 AM
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
Delivery
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:04 AM
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:04 AM
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:04 AM
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:04 AM
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:04 AM
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:04 AM
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:04 AM
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
Gross Total
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:04 AM
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
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:04 AM
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
Delivery: Logistics Tab
This tab contains details regarding the logistics aspects of the delivery.
To access the tab, choose Sales – A/R Delivery Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Delivery Logistics Tab Fields
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description for this document only; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:04 AM
Tracking No.
Specify the tracking number of the package as received from the delivery company.
Stamp No.
Enter the number that you receive from a chain as a confirmation of a delivery. You copy the stamp number to the A/R invoice and
use it to create a file that is sent to the marketing chain for payments.
Pick and Pack Remarks
Enter relevant remarks for the pick and pack procedure.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
Delivery
Delivery: Accounting Tab
This tab contains information regarding the financial aspect of the delivery.
To access the tab, choose Sales – A/R Delivery Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Delivery Accounting Tab Fields
Journal Remark
By default, displays Delivery – XXX, where XXX is the customer code.
If required, change this content.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the delivery. This control account can then be copied to any follow-up documents.
 Note
It appears only if the checkbox Allow Control Account Selection is selected in Administration System Initialization
Document Settings Per Document for deliveries.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:04 AM
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
Indicator
By default, displays the indicator linked to the customer ( Business Partners Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
If the delivery is copied from a base document, the federal tax ID that appears in this field is the one copied from the base
document.
Order Number
Enter an order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Use Shipped Goods Account
Select this checkbox to post the delivery of the inventory to the shipped goods account instead of the COGS account, when the
delivery of inventory and the issue of the invoice occur in different posting periods.
For standalone deliveries, the default status of this checkbox is inherited from the same checkbox in the Business Partner Master
Data window of the customer for which the delivery is created; for deliveries that are created based on sales orders, the default
status of this checkbox is inherited from the same checkbox in the base order. You can change the status of this checkbox if
needed.
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:04 AM
If you want to draw multiple deliveries to the same invoice, make sure that the status of this chekbox is the same for all the
deliveries.
 Note
This checkbox is available for perpetual inventory companies only.
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
Delivery
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:04 AM
Sales Document: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
Closing Deliveries
Context
If a delivery has not yet been copied to an A/R invoice or to a returns, you can close it.
Procedure
1. Choose Sales - A/R Delivery and call up the required delivery.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:04 AM
2. From the menu bar, choose Data Close .
Results
When you close a delivery, no adjustment posting is carried out in warehouse management. This means that the available inventory
that has been reduced by the delivery will not be increased again.
The inventory is only increased when you create a returns document based on the delivery.
Once a delivery has been closed, you cannot:
Create an invoice from that delivery
Create another sales document with reference to the delivery
Make changes to the closed delivery
Related Information
Delivery
Creating and Printing Packing Slips
Prerequisites
You have defined one or more package types in SAP Business One. For more information see Package Types - Setup.
You have opened one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
You have picked the items for the sales document that you open.
Context
You create and print packing slips in SAP Business One after you pick the items of a shipment and you are ready to send the
shipment.
You can create and print packing slips for only the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
The packing and packing slip printing process includes the following procedures:
1. Create a new packing slip.
2. Select items for shipment.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:04 AM
3. Move items to package contents.
4. Preview and print both your sales document and packing slips, or preview and print packing slips only.
Procedure
1. Create a new packing slip.
a. Open one of the aforementioned sales documents.
b. Open the Packing Slip window by doing one of the following:
In the menu bar, choose Go To Packing Slip .
Right-click in the document and choose Packing Slip.
c. In the Package No. field in the upper Existing Packages area, enter an identifying number for the package. SAP
Business One automatically assigns a sequential number, but you can change it.
For more information, see Packing Slip Window.
d. Open the List of Package Types window in one of the following ways:
Place your cursor in the Type field and press the Tab key.
In the Type field, click .
e. In the List of Package Types window, select a package type and choose the Choose button.
f. (Optional) If you want to convert the package weight to a different unit of measure, in the Units dropdown list, select
the unit of measure you want to display in the Total Weight field.
 Note
The Total Weight field displays the total weight of the package. The value of the field is calculated according to
the weight you have defined in the Item Master Data window, on the Sales Data tab. If the item weight is not
defined, the Total Weight field is blank.
g. To add another package, right click the existing package row and choose Add Row. Repeat the above steps.
2. Select items for shipment.
a. In the Packing Slip window, go to the lower Available Items area.
b. In the Selected field, enter the number of items to include in the package for shipment.
The Available Items table displays a list of available items and their quantities. To find an item quickly, in the Find
field, enter the item number. The row with the corresponding item number is selected.
 Note
You cannot enter an item quantity that is higher than the quantity displayed in the Available field. The value in the
Available field shows the quantity of the item that you have not yet assigned to a package.
To add additional columns, such as UoM, Items per Unit, Weight, or Height to the Available Items table, right-
click the table header and choose Form Settings.
Alternatively, in the toolbar, click and in the Form Settings window, select the required columns.
You can add several packages to each shipment.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:04 AM
If you are creating a shipment of 30 items, and each package of the selected type can contain only ten items, you
must create three packages. You may use a combination of package types.
3. Move items to package contents.
Proceed as follows to move a selected quantity of items from the Available Items table to the Package Contents table.
a. In the Available Items table, select the rows of the items that you want to include in the package for shipment.
b. Choose the right arrow button. The Package Contents table shows the contents of the packages for delivery.
c. Add additional packages as required. Choose Update, and then choose OK.
4. In your sales document, choose Update to update the packing slips information in your sales document.
5. Preview and print your sales document and packing slips.
To preview and print both the sales document and the packing slips, proceed as follows:
a. Open your sales document.
b. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One automatically previews or prints both the sales document and the packing slips at the
same time.
To preview and print only the packing slips, proceed as follows:
a. Open your sales document.
b. Open the Packing Slip window. Make sure that the Packing Slip window is the currently active window.
c. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One only previews or prints the packing slips.
Related Information
File Menu
Printing in SAP Business One
Working with Pick and Pack
Delivery
A/R Invoice
A/R Invoice + Payment
Packing Slip Window
Use this window to enter packing details for items and to create and print packing slips.
To access this window:
1. Open one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
2. Do one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:04 AM
From the menu bar, choose Go To Packing Slip .
Right-click in the open document and choose Packing Slip.
If you select the Recommend Packaging from Item Master Data checkbox in the Documents Settings window, SAP Business One
fills the recommended packaging information for you in packing slips. You can change this information manually.
 Note
Printing Information
You can print a packing slip directly from the Packing Slip window. When you print one of the documents listed in step 1, the
packaging information is automatically printed on a separate page.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Packages Setup Window Fields
Package No.
Enter the number for the package. By default, the system automatically enters a sequential number.
Type
Select a type of package. Alternatively, press TAB and select one of the types. To define a new package type, select New.
Total Weight
Displays the total weight of the package. The value of the field is calculated according to the weight you have defined on the Sales
Data tab in the Item Master Data .
Units
Select the unit of measurement for the weight of the package.
Find Available Items
Enter the item code to find the necessary item from the list.
Available
Displays the quantity (in purchasing UoM) of items available for packing.
Selected
Enter the number of items that you actually plan to pack in the special package. The value cannot be larger than the value in the
Available field.
Package Contents
Displays the number of different items making up the package.
Quantity
Displays the quantity (in purchasing UoM) of items in the package.
UoM
Displays the UoM specified for an item in associated purchasing documents.
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:04 AM
Related Information
Creating and Printing Packing Slips
Transaction Codes
Journal Entry Window
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
payment advance from the customer by issuing a down payment request. You also use this document as a basis for other key steps
in the sales process, for example, creating the final invoice.
 Note
In various localizations there might be few differences in this functionality. For complete information refer to the localized online
help file provided with SAP Business One by choosing: Help Document Localization Specific Info
Process
1. Create an A/R or A/P down payment request for the relevant business partner. If you do this by drawing a base document,
verify that you have defined the required down payment percentage. For more information, see A/R Down Payment
Documents: General Area or A/P Down Payment Request: General Area.
No posting is made at this stage.
2. Once the actual payment for the down payment request is made, create the proper payment document based on the down
payment request. A down payment request can be paid in full or in parts.
 Note
You can use the payment wizard to pay the down payment request.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:04 AM
After you create the payment document, a journal entry is recorded in the down payment accounts. If the down payment
request was paid fully, the down payment request is closed. If it was only paid partially, it remains open for another
payment. You can edit a down payment document that was only partially paid, provided that no rounding amount was
specified on the document.
If only part of the down payment request was paid and you do not expect further payments on it, you can close the request
by choosing Data Close . This closes the down payment request document and you are not able to record payment of
the outstanding amount in the future for the closed down payment request.
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
A/R Down Payment Request
You can create a request for a down payment for the company’s customers. This document does not create any accounting or
inventory posting. If you create an A/R down payment request based on a delivery or sales order, the base document is not closed.
This allows you to copy the same base document later to a higher-level sales document such as an A/R invoice or delivery.
To access the window, choose Sales - A/R A/R Down Payment Request .
 Note
When a down payment request is included in a payment order run, you cannot cancel or close it.
More Information
Down Payments
Down Payment Request Process
A/R Down Payment Documents: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:04 AM
A/R Down Payment Documents: General Area
Use the General Area in the sales document to enter general information relevant for all items in the document.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
Displays the customer reference number, if defined.
No.
From the field on the left, specify a numbering series.
If you choose the manual series, in the field on the right, specify the number of the relevant A/R down payment document.
Status
Statuses of the A/R down payment:
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
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:04 AM
Specify the posting date. The default value for this field is the current date on which the A/R down payment document is created. If
required, change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the payment of the down payment.
The default date is 30 days after the posting date. You can change it manually or choose a different payment term in the Payment
Terms field of the A/R down payment document.
Document Date
Document date of the A/R down payment document used for tax purposes. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R down payment document.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the sales document.
Owner
Specify the code of the employee who owns the sales document.
Remarks
Enter additional information regarding the A/R down payment document.
You can edit the field contents even after the document has been created.
Total Before Discount
Total amount of the document before the calculated discount.
If the discount is defined in the row for the item or service, the amount displayed in this field considers that discount.
Base Discount %
Percentage and amount of the discount from the base document, and they are separated from those of the down payment.
 Note
They appear only if the checkbox Separate Discount % and DPM % Fields is selected in Administration System
Initialization Document Settings Per Document for A/R down payments.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:04 AM
DPM %
In the field on the left, enter the percentage of down payment.
The field on the right displays the down payment amount. If required, you can change the values of these fields.
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
WTax Amount
The amount withheld, according to the withholding tax definitions, and paid over or reported to the tax authorities on behalf of the
person subject to tax.
Appears only if you have selected Withholding Tax on the Tax subtab of the Sales tab in Administration Setup Financials
G/L Account Determination .
To open the Withholding Tax Table window, click .
Tax
Tax amount for the A/R down payment document calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Applied Amount
Amount of the A/R down payment invoice copied to a payment document or to a credit memo.
Balance Due
Amount of the A/R down payment document that has not been paid or credited yet.
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
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:04 AM
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/R Down Payment Request
A/R Down Payment Invoice
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:04 AM
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:04 AM
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:04 AM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:04 AM
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:04 AM
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
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:04 AM
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:04 AM
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:04 AM
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:04 AM
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
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:04 AM
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
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
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:04 AM
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
A/R Down Payment Documents: Logistics Tab
This tab contains details regarding the logistics aspects of A/R down payment documents.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:04 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment Logistics Tab
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description only for this document; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the multi-
language support function.
Tracking No.
Specify the tracking number of the package as received from the delivery company.
Block Dunning Letters
Excludes the A/R down payment invoice from dunning wizard runs.
 Note
A/R down payment requests are always excluded from dunning wizard runs. Selecting, or not selecting, this checkbox for an
A/R down payment request has no impact on the document appearing in dunning wizard runs.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
A/R Down Payment Request
A/R Down Payment Invoice
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:04 AM
A/R Down Payment Documents: Accounting Tab
The Accounting tab contains information regarding the financial aspects of A/R down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment Accounting Tab Fields
Journal Remark
By default, displays A/R Down Payment – XXX, where XXX is the customer code. If required, change this content.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the down payment. This control account can then be copied to any follow-up documents.
 Note
For A/R down payment requests, it appears only if the checkbox Allow Control Account Selection is selected in
Administration System Initialization Document Settings Per Document for A/R down payment requests.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if the due date has already expired.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
The installment-payments feature is unavailable for down payment documents. This field displays the number 1 by default. This
value cannot be modified.
+Months...+Days
Enter the due date.
The calculation is based on the date of the order and the values specified in the payment terms.
The payment period can be given for the current month or for several months in the future, as well as for the number of days you
specify in the last month of the period.
Consolidation Type, Consolidating BP
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:04 AM
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
 Note
The two fields are available in all localizations except CZ, SK, HU, PL, RU, UA.
BP Project
Project name linked to the customer in the business partner master data. If required, specify a different project name.
Indicator
Indicator linked to the customer on the General tab in the Business Partner Master Data window.
The indicator is used as selection criteria in various reports. If required, select a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
Order Number
Enter the order number of a chain when you use the direct distribution method.
This number is recorded in the file that you send to the head office of a chain store.
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
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:04 AM
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
A/R Down Payment Request
A/R Down Payment Invoice
Down Payment Interim Account, Down Payment Clearing Account
Sales Document: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:04 AM
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
Creates an accounting posting
Does not affect inventory values or perpetual inventory
Does not change the status of the base document that was drawn into it
2. Once the actual payment for the down payment invoice is made, create the proper payment document, based on the down
payment invoice. A down payment invoice can be paid partially.
After you create the payment document, a journal entry is recorded in the corresponding control account.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:04 AM
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
Sales Tax (5%) $10
Total including Tax $210
Horn & Brass has decided to pay currently only a deposit of $80. Tom, as a sales employee, does not have authorization to create a
down payment invoice, but in SAP Business One Tom can create a deposit (incoming payment) directly from the sales order, so
that Down Payment Invoice 431 is created automatically once the payment has been received. At this point, no sales tax is
charged.
The journal entry created by the deposit document is:
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:04 AM
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
After two weeks, Anne has not received payment. She creates Down Payment Invoice 232, for which the following journal entry is
created:
Debit Credit
Accounts Receivables 40
Payment Advances 40
The Bloor Street Book Club pays the deposit once they have received the down payment invoice. At this point, no sales tax is
charged.
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:04 AM
The journal entry created is:
| Debit                |     | Credit |
| -------------------- | --- | ------ |
| Cash 40              |     |        |
| Accounts Receivables |     | 40     |
Anne creates Delivery 870 and the order is shipped. She issues the final invoice, which creates the following journal entries:
| Debit                   |     | Credit |
| ----------------------- | --- | ------ |
| Accounts Receivables 65 |     |        |
| Payment Advances 40     |     |        |
| Sales Tax               |     | 5      |
| Revenue                 |     | 100    |
Related Information
Down Payments to Draw
A/R Down Payment Documents: General Area
A/P Down Payment Document: General Area
A/R Down Payment Invoice
A/P Down Payment Invoice
A/R Down Payment Invoice
When your company needs to create a down payment invoice for a customer, use the A/R down payment invoice to document this
payment.
The A/R down payment invoice is an invoice that is cleared by an incoming payment. Unlike the A/R invoice, the A/R down
payment invoice creates a posting in the accounting system but has no influence on inventory accounting values and quantities.
| To access the window, choose  | Sales – A/R  |  A/R Down Payment Invoice. |
| ----------------------------- | ------------ | -------------------------- |
More Information
Down Payment Invoices
A/R Down Payment Documents: General Area
Sales Document: Contents Tab
A/R Down Payment Documents: Logistics Tab
A/R Down Payment Invoice: Accounting Tab
A/R Down Payment Documents: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:04 AM
Use the General Area in the sales document to enter general information relevant for all items in the document.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
Displays the customer reference number, if defined.
No.
From the field on the left, specify a numbering series.
If you choose the manual series, in the field on the right, specify the number of the relevant A/R down payment document.
Status
Statuses of the A/R down payment:
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
Specify the posting date. The default value for this field is the current date on which the A/R down payment document is created. If
required, change the date.
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:04 AM
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the payment of the down payment.
The default date is 30 days after the posting date. You can change it manually or choose a different payment term in the Payment
Terms field of the A/R down payment document.
Document Date
Document date of the A/R down payment document used for tax purposes. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R down payment document.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the sales document.
Owner
Specify the code of the employee who owns the sales document.
Remarks
Enter additional information regarding the A/R down payment document.
You can edit the field contents even after the document has been created.
Total Before Discount
Total amount of the document before the calculated discount.
If the discount is defined in the row for the item or service, the amount displayed in this field considers that discount.
Base Discount %
Percentage and amount of the discount from the base document, and they are separated from those of the down payment.
 Note
They appear only if the checkbox Separate Discount % and DPM % Fields is selected in Administration System
Initialization Document Settings Per Document for A/R down payments.
DPM %
In the field on the left, enter the percentage of down payment.
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:04 AM
The field on the right displays the down payment amount. If required, you can change the values of these fields.
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
WTax Amount
The amount withheld, according to the withholding tax definitions, and paid over or reported to the tax authorities on behalf of the
person subject to tax.
Appears only if you have selected Withholding Tax on the Tax subtab of the Sales tab in Administration Setup Financials
G/L Account Determination .
To open the Withholding Tax Table window, click .
Tax
Tax amount for the A/R down payment document calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Applied Amount
Amount of the A/R down payment invoice copied to a payment document or to a credit memo.
Balance Due
Amount of the A/R down payment document that has not been paid or credited yet.
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
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:04 AM
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/R Down Payment Request
A/R Down Payment Invoice
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:04 AM
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:04 AM
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:04 AM
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:04 AM
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Enter in this field the unit price including tax, taking into account the discount specified here. SAP Business One calculates
automatically the unit price before tax and the tax amount, based on the tax code in the row. After pressing the TAB key,
the Unit Price field and the Tax/Unit field are updated accordingly.
 Recommendation
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
The Discount is 8%
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:04 AM
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:04 AM
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:04 AM
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
Gross Total
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:04 AM
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
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:04 AM
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
A/R Down Payment Documents: Logistics Tab
This tab contains details regarding the logistics aspects of A/R down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment Logistics Tab
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description only for this document; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the multi-
language support function.
Tracking No.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:04 AM
Specify the tracking number of the package as received from the delivery company.
Block Dunning Letters
Excludes the A/R down payment invoice from dunning wizard runs.
 Note
A/R down payment requests are always excluded from dunning wizard runs. Selecting, or not selecting, this checkbox for an
A/R down payment request has no impact on the document appearing in dunning wizard runs.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
A/R Down Payment Request
A/R Down Payment Invoice
A/R Down Payment Documents: Accounting Tab
The Accounting tab contains information regarding the financial aspects of A/R down payment documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Down Payment Accounting Tab Fields
Journal Remark
By default, displays A/R Down Payment – XXX, where XXX is the customer code. If required, change this content.
Control Account
The default value is from the Business Partner Master Data Accounting General subtab. If required, change the control
account for the down payment. This control account can then be copied to any follow-up documents.
 Note
For A/R down payment requests, it appears only if the checkbox Allow Control Account Selection is selected in
Administration System Initialization Document Settings Per Document for A/R down payment requests.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if the due date has already expired.
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:04 AM
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Installments
The installment-payments feature is unavailable for down payment documents. This field displays the number 1 by default. This
value cannot be modified.
+Months...+Days
Enter the due date.
The calculation is based on the date of the order and the values specified in the payment terms.
The payment period can be given for the current month or for several months in the future, as well as for the number of days you
specify in the last month of the period.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
 Note
The two fields are available in all localizations except CZ, SK, HU, PL, RU, UA.
BP Project
Project name linked to the customer in the business partner master data. If required, specify a different project name.
Indicator
Indicator linked to the customer on the General tab in the Business Partner Master Data window.
The indicator is used as selection criteria in various reports. If required, select a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
Order Number
Enter the order number of a chain when you use the direct distribution method.
This number is recorded in the file that you send to the head office of a chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:04 AM
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
Related Information
A/R Down Payment Request
A/R Down Payment Invoice
Down Payment Interim Account, Down Payment Clearing Account
Sales Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:04 AM
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
A/R Invoice
The invoice is a legally binding document. When an invoice is received, the posting is made to the related customer accounts in the
accounting system. If a delivery did not precede the invoice and you sell the warehouse items, inventory quantities are also
updated accordingly when you issue the invoice.
If you create an invoice without reference to the delivery, the system automatically posts changes to the inventory. In other words,
if a delivery already exists for the transaction and you create an invoice without reference to this delivery, errors can occur in
inventory management because the delivery quantity is posted twice in the system.
SAP Business One enables you to create an A/R invoice with a zero amount. You can do this when delivering items without a
charge, for example, items that are part of a promotion or covered by a service contract.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:04 AM
When you create the delivery and the invoice for a sales process simultaneously, first enter the delivery and then proceed with
the invoice. However, it may be sufficient to create the invoice, since that is what affects the inventory and the accounting
systems.
To access this function, choose Sales – A/R A/R Invoice .
More Information
Creating Sales Documents
A/R Invoice: General Area
Sales Document: Contents Tab
A/R Invoice: Logistics Tab
A/R Invoice: Accounting Tab
A/R Invoice: General Area
Use this part of the A/R invoice to enter general information relevant to all items in the document.
To access this area, choose Sales – A/R A/R Invoice .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Invoice General Area Fields
Contact Person
Name of the default contact person defined in the business partner master data. If required, specify a different contact person.
Customer Ref. Number
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: the number of the A/R invoice. If you choose the manual series, enter the relevant number.
Status
Status of the A/R invoice:
Open
You can draw the document completely or partially to a document of a higher level.
Open – Printed
You printed the document and left it open.
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:04 AM
Canceled
You canceled the document manually.
Closed
SAP Business One closed the document automatically when you drew it to another document.
Draft
The document is still a draft.
 Note
A no-charge A/R invoice is closed automatically once you add the document.
The following statuses apply to A/R reserve invoices only:
Delivered
The document is fully drawn to a delivery, but not yet fully paid.
Paid
The document is fully paid but not yet fully drawn to a delivery.
Posting Date
Specify the posting date. The default value for this field is the current date on which the A/R invoice is created. If required, change
the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services.
The default date is 30 days after the posting date. To change it, choose a different payment term in the dropdown list for the
Payment Terms field in the A/R Invoice. Alternatively, change the due date manually.
You can also edit the Due Date after the A/R invoice is partially reconciled. Make sure the new Due Date is on or after the latest
Reconciliation Date.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Currency
Specify the display currency for the amounts in the A/R invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:04 AM
Sales Employee
Specify the sales employee who initiated the A/R invoice.
Owner
Specify the code of the employee who owns the A/R invoice.
Remarks
Enter additional information regarding the A/R invoice. You can edit the field contents even after the document is added.
Total Before Discount
Total amount of the A/R invoice before the discount for the document is calculated.
 Note
If the discount is defined in the row for the item or service, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of discount. The field on the right displays the discount amount. If required, you can
change the values of these fields.
Total Down Payment
Amount drawn from the paid down payment invoices or down payment requests, and subtracted from the total amount of the
invoice.
To view the details of the amount, choose to open the Down Payment to Draw window.
Freight
Displays the total freight for the A/R invoice.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
WTax Amount
The amount withheld, according to the withholding tax definitions, and paid over or reported to the tax authorities on behalf of the
person subject to tax.
Appears only if you have selected Withholding Tax in Administration Setup Financials G/L Account Determination Sales
tab, Tax subtab.
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/R invoice calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Applied Amount
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:04 AM
The amount of the A/R invoice that was copied to a payment document or to a credit memo.
Balance Due
Amount of the A/R invoice that has not been paid or credited yet.
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
 Caution
The only possible way of crediting an A/R invoice based on an A/R down payment invoice is to reopen it. To change the A/R
invoice status, choose Data Advanced Change Document Status to Open .
More Information
A/R Invoice
Payments List
The Payments List window displays the incoming or outgoing payments documents created in response to specific A/R or A/P
invoices.
To access this window, display the relevant invoice and click in the toolbar.
 Note
The Payments List window appears only when the displayed invoice was paid (fully or partially). If the invoice was not paid at
all, the Payment Means window appears.
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:04 AM
Payments List Window
The following table describes the fields appear in the Payments List window.
To access this window, display the required A/R or A/P invoice and click in the toolbar.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Payments List Window
Payment No.
Number of the incoming or outgoing payments document.
Total
Total amount paid through this payment document.
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
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:04 AM
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
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table Header Fields
Item/Service Type
Choose one of the following options:
Item – to create a purchasing document for items defined in the Inventory module.
Service – to create a purchasing document for a service, such as a one-time consultation, that has not been defined as an
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:04 AM
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
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
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:04 AM
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:04 AM
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:04 AM
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
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
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:04 AM
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:04 AM
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:04 AM
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
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
Table View for Document Type Service
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:04 AM
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
A/R Invoice: Logistics Tab
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:04 AM
This tab contains details regarding the logistical aspects of the A/R invoice.
To access the tab, choose Sales – A/R A/R Invoice Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Invoice Logistics Tab Fields
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description only for this document; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data; change if required.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
Tracking No.
Specify the tracking number of the package as received from the delivery company.
Block Dunning Letters
Excludes the A/R invoice from the dunning wizard run.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
A/R Invoice
A/R Invoice: Accounting Tab
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:04 AM
This tab contains information regarding the financial aspects of the A/R invoice.
To access the tab, choose Sales – A/R A/R Invoice Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Invoice Accounting Tab Fields
Journal Remark
By default, displays A/R Invoice – XXX, where XXXis the customer code. Change this content, if required.
Control Account
Specify the control account for the A/R invoice. The default value is the Accounts Receivable value in the business partner master
data.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if the due date has already expired.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Installments
Displays the installments details as specified in the business partner master data. To edit the data, click .
Print SEPA Direct Debit Prenotification
Applicable to SEPA (Single Euro Payment Area) relevant localizations only.
If selected, when printing an invoice you can choose from Invoice Only, Prenotification Only, and Invoice and Prenotification.
Where applicable, a Crystal Reports (CR) layout is available for a direct debit prenotification letter, for more information search for
the latest SAP Notes on SEPA.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:04 AM
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
By default, displays the project code linked to the customer in the business partner master data. If required, specify a different
project.
Indicator
By default, displays the indicator linked to the customer Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator from the dropdown list.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
If the A/R invoice is copied from base document, the federal tax ID that appears in this field is copied from the base document.
Order Number
Enter an order number of the chain when you use the direct distribution method. This number is recorded in the file that you send
to a head office of the chain store.
Use Shipped Goods Account
Indicate whether to post the delivery of the inventory to the shipped goods account instead of the COGS account.
For A/R invoices that are created based on deliveries, the status of this checkbox is inherited from the same checkbox in the base
delivery.
 Note
This checkbox is not available for standalone A/R invoices.
This checkbox is for perpetual inventory companies only.
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
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:04 AM
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
Asset Value Date
 Note
The field is available only if you have enabled fixed assets.
If you use the A/R invoice to retire a fixed asset, specify the date on which the retirement takes place in this field.
Different from the posting date which is the date of the journal entry from the accounting perspective, the asset value date is the
date of the retirement from the asset perspective.
More Information
A/R Invoice
Installments Window
Use the window to define the number of the installments and the way to apply the tax amount.
There are two methods to set the due date in the A/R and A/P invoices:
Fixed day – you make the payment on fixed days that you define in the Payment Dates window.
Regular – you make the payment on the due date that is calculated according to the Payment Terms - Setup window.
To access the window, choose Sales – A/R A/R Invoice Accounting Installments .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 130

6/8/26, 6:04 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Installment Window Fields
No. of Installments
Enter the number of installments.
Apply Tax in First Installment
Adds the tax amount to the first installment only.
Apply Tax Proportionally
Adds the tax amount proportionally to each installment, according to the % field.
Date
Specify a due date for the installments.
You can change the due date of any open installments (that is, unreconciled, not yet paid fully or partially paid installments) even
after you posted the A/R or A/P invoice or A/R or A/P reserve invoice. This may be necessary if your business partner wants to
postpone the payment of an installment.
%
Displays the installments as a percent of the total payment amount.
The total amount must be 100%.
Total
Amount calculated according to the installment percentage.
Payment Order Amount
Displays the value requested for payment of this installment in the payment order run.
Payment Order Run Name
Displays the name of the payment order run that includes this installment.
Restore Default
Restore the data as defined in the Payment Terms window.
More Information
Holiday Details
Sales Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 131

6/8/26, 6:04 AM
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
Creating A/R Invoices Based on A/R Down Payment Invoices
Context
The following procedure describes how to create A/R invoices based on existing A/R down payment invoices. Such process is
required after goods or services that were ordered are fully delivered, a partial payment was received, and now the customer
should be invoiced.
Procedure
1. From SAP Business One Main Menu, choose Sales - A/R A/R Invoice . The A/R Invoice window appears.
2. Specify the customer for whom the A/R invoice is created. At the bottom of the window, choose Copy From. If the sales
order for which the A/R invoice is created was already copied to delivery, click Deliveries, if not, click Sales Orders. A list of
documents to copy appears.
3. Choose the required document(s), and make the relevant choices in the Draw Document Wizard. The data from the selected
documents appears in the A/R Invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 132

6/8/26, 6:04 AM
4. If the copied document(s) is linked to an A/R down payment invoice, the amount of the A/R down payment invoice is
automatically displayed in the Total Down Payment field. Otherwise, this field is empty. To link specific A/R down payment
invoice(s) to the A/R invoice, choose the button next to the Total Down Payment field. The Down Payments to Draw
window appears.
5. Mark the A/R down payments invoice(s) you want to draw and adjust the amount to be drawn if required (the drawn
amount can be equal or smaller than the open amount of the A/R down payment invoice), and choose OK. The cumulative
amount marked is copied to the Total Down Payment field in the A/R invoice. This field is read-only.
 Note
The total down payment amount can be equal or smaller than the total amount of the A/R invoice.
You can draw to the A/R invoice A/R down payment invoice(s) created for documents that are not the base
documents copied. This might occur if a customer placed several sales orders and paid a down payment for each
one. Eventually one of the sales orders was cancelled. The A/R down payment invoice and the incoming payment
were not cancelled, and therefore can be used.
6. To add the A/R invoice, choose Add.
Results
Once you add the A/R invoice the following happens:
The base document is updated accordingly (if it was fully copied it is closed, otherwise the open quantities and amounts are
updated).
If the A/R down payment was fully drawn, its status turns to Closed. Otherwise, the balance due and the applied amount
are updated according to the amount drawn.
The total amount of the A/R invoice is calculated as follows: (total after discount + freight charges + tax) - total down
payment.
Creating and Printing Packing Slips
Prerequisites
You have defined one or more package types in SAP Business One. For more information see Package Types - Setup.
You have opened one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
You have picked the items for the sales document that you open.
Context
You create and print packing slips in SAP Business One after you pick the items of a shipment and you are ready to send the
shipment.
You can create and print packing slips for only the following sales documents:
Delivery
This is custom documentation. For more information, please visit SAP Help Portal. 133

6/8/26, 6:04 AM
A/R invoice
A/R invoice + payment
The packing and packing slip printing process includes the following procedures:
1. Create a new packing slip.
2. Select items for shipment.
3. Move items to package contents.
4. Preview and print both your sales document and packing slips, or preview and print packing slips only.
Procedure
1. Create a new packing slip.
a. Open one of the aforementioned sales documents.
b. Open the Packing Slip window by doing one of the following:
In the menu bar, choose Go To Packing Slip .
Right-click in the document and choose Packing Slip.
c. In the Package No. field in the upper Existing Packages area, enter an identifying number for the package. SAP
Business One automatically assigns a sequential number, but you can change it.
For more information, see Packing Slip Window.
d. Open the List of Package Types window in one of the following ways:
Place your cursor in the Type field and press the Tab key.
In the Type field, click .
e. In the List of Package Types window, select a package type and choose the Choose button.
f. (Optional) If you want to convert the package weight to a different unit of measure, in the Units dropdown list, select
the unit of measure you want to display in the Total Weight field.
 Note
The Total Weight field displays the total weight of the package. The value of the field is calculated according to
the weight you have defined in the Item Master Data window, on the Sales Data tab. If the item weight is not
defined, the Total Weight field is blank.
g. To add another package, right click the existing package row and choose Add Row. Repeat the above steps.
2. Select items for shipment.
a. In the Packing Slip window, go to the lower Available Items area.
b. In the Selected field, enter the number of items to include in the package for shipment.
The Available Items table displays a list of available items and their quantities. To find an item quickly, in the Find
field, enter the item number. The row with the corresponding item number is selected.
 Note
You cannot enter an item quantity that is higher than the quantity displayed in the Available field. The value in the
Available field shows the quantity of the item that you have not yet assigned to a package.
This is custom documentation. For more information, please visit SAP Help Portal. 134

6/8/26, 6:04 AM
To add additional columns, such as UoM, Items per Unit, Weight, or Height to the Available Items table, right-
click the table header and choose Form Settings.
Alternatively, in the toolbar, click and in the Form Settings window, select the required columns.
You can add several packages to each shipment.
 Example
If you are creating a shipment of 30 items, and each package of the selected type can contain only ten items, you
must create three packages. You may use a combination of package types.
3. Move items to package contents.
Proceed as follows to move a selected quantity of items from the Available Items table to the Package Contents table.
a. In the Available Items table, select the rows of the items that you want to include in the package for shipment.
b. Choose the right arrow button. The Package Contents table shows the contents of the packages for delivery.
c. Add additional packages as required. Choose Update, and then choose OK.
4. In your sales document, choose Update to update the packing slips information in your sales document.
5. Preview and print your sales document and packing slips.
To preview and print both the sales document and the packing slips, proceed as follows:
a. Open your sales document.
b. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One automatically previews or prints both the sales document and the packing slips at the
same time.
To preview and print only the packing slips, proceed as follows:
a. Open your sales document.
b. Open the Packing Slip window. Make sure that the Packing Slip window is the currently active window.
c. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One only previews or prints the packing slips.
Related Information
File Menu
Printing in SAP Business One
Working with Pick and Pack
Delivery
A/R Invoice
A/R Invoice + Payment
Packing Slip Window
Use this window to enter packing details for items and to create and print packing slips.
To access this window:
This is custom documentation. For more information, please visit SAP Help Portal. 135

6/8/26, 6:04 AM
1. Open one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
2. Do one of the following:
From the menu bar, choose Go To Packing Slip .
Right-click in the open document and choose Packing Slip.
If you select the Recommend Packaging from Item Master Data checkbox in the Documents Settings window, SAP Business One
fills the recommended packaging information for you in packing slips. You can change this information manually.
 Note
Printing Information
You can print a packing slip directly from the Packing Slip window. When you print one of the documents listed in step 1, the
packaging information is automatically printed on a separate page.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Packages Setup Window Fields
Package No.
Enter the number for the package. By default, the system automatically enters a sequential number.
Type
Select a type of package. Alternatively, press TAB and select one of the types. To define a new package type, select New.
Total Weight
Displays the total weight of the package. The value of the field is calculated according to the weight you have defined on the Sales
Data tab in the Item Master Data .
Units
Select the unit of measurement for the weight of the package.
Find Available Items
Enter the item code to find the necessary item from the list.
Available
Displays the quantity (in purchasing UoM) of items available for packing.
Selected
Enter the number of items that you actually plan to pack in the special package. The value cannot be larger than the value in the
Available field.
Package Contents
This is custom documentation. For more information, please visit SAP Help Portal. 136

6/8/26, 6:04 AM
Displays the number of different items making up the package.
Quantity
Displays the quantity (in purchasing UoM) of items in the package.
UoM
Displays the UoM specified for an item in associated purchasing documents.
Related Information
Creating and Printing Packing Slips
Transaction Codes
Journal Entry Window
Return Request
Return Material Agreement describes a scenario where the supplier of a good or product agrees to have a customer ship that item
back in exchange for a refund or credit.
The purpose of adding a return request is to enable creating pre-step of the return document, to enter the agreed quantities,
prices, and return reason before the goods are actually returned.
You can either create a return request based on Deliveries or A/R Invoices, or create a standalone return request that is not based
on any document. For standalone return request, the Quantity in the return can exceed the Quantity in the return request based on
which the return is created.
For the return request that is generated based on deliveries or invoices, you can also add standalone lines to it.
 Note
When adding standalone lines to return request that was based on delivery, the target document for these standalone lines can
be return only. When adding standalone lines to return request that was based on A/R invoice, the target document for these
standalone lines can be A/R credit memo only.
If an A/R invoice is copied or partially copied to a return request, closing this invoice by fully paying it, or reconciling the invoice
transaction, or fully crediting it shall not be allowed. You need to manually close the return request to continue.
For the standalone return request, you can copy it to returns or A/R credit memos. The Allow Setting Item Cost When Document
is Not Based field is applicable to such returns or A/R credit memos.
To access Return Request window, in Main Menu, choose Sales - A/R Return Request .
More Information
Return Request: General Area
Return Request: Contents Tab
Return Request: Logistics Tab
Return Request: Accounting Tab
This is custom documentation. For more information, please visit SAP Help Portal. 137

6/8/26, 6:04 AM
Additional Information
Return Request: General Area
This part of the sales document is used to enter general information pertinent to all items in the document.
To access this area, in Main Menu, choose Sales - A/R Return Request .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return Request General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series. Specify a series. Field on the right: the number of the return request. If you choose
the Manual series, enter the relevant number.
Status
Status of the return request:
Open
You can copy the document completely or partially to a document of a higher level.
Open - Printed
You printed the document and left it open.
Closed
You closed the document manually or SAP Business One closed it automatically when you copied it to another document.
Draft
The document is still a draft.
Not Confirmed
The document is not yet confirmed, thus cannot be copied to other documents.
Posting Date
Specify the posting date. The default value for this field is the current date on which the return request is created. If required,
change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
This is custom documentation. For more information, please visit SAP Help Portal. 138

6/8/26, 6:04 AM
Due Date
Expected return date of the items.
The default date is equal to the posting date. You can change it manually.
Document Date
Document date, used for tax purposes, of the return request. Change the date if required.
Currency
Specify the display currency for the amounts in the return request.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the return request.
Owner
Specify the code of the employee who owns the return request.
Remarks
Enter additional information regarding the return request.
You can edit the field contents even after the document is added.
Total Before Discount
Displays the total amount of the document before the calculated discount.
 Note
If the discount is defined in the row for the item, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of discount.
The field on the right displays the discount amount. You can change the values of these fields, if required.
Freight
Displays the total freight for the return request.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization General .
Rounding
This is custom documentation. For more information, please visit SAP Help Portal. 139

6/8/26, 6:04 AM
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the return request calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
More Information
Return Request
Return Request: Contents Tab
Use this tab to specify items to be returned.
Some of the fields described below are not displayed by default, but must be selected in the Form Settings window. To open the
Form Settings window, in the menu bar, choose Tools Form Settings , or in the toolbar, click .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Type and Summary Type Fields
Item/Service Type
Return requests are supported only on item type of documents. Select Item, and you can create a return request for items defined
in the Inventory module.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Item No.
Specify the item number.
Press CTRL+TAB to view the Alternative Items.
Quantity
This is custom documentation. For more information, please visit SAP Help Portal. 140

6/8/26, 6:04 AM
Quantity that the customer wants to return based on the item’s sales unit of measure, as defined on the Sales Data tab in the Item
Master Data window. The default value is 1.
 Note
For return request that is created based on deliveries or A/R invoices, the Quantity cannot exceed the Quantity in the deliveries
or invoices. For standalone return request, the Quantity in the return can exceed the Quantity in the return request based on
which the return is created.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in the return request.
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
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then toSAP Business
This is custom documentation. For more information, please visit SAP Help Portal. 141

6/8/26, 6:04 AM
One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
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
Displays the UoM code of the item specified. For a return request that is created based on other documents, the UoM code is
copied from the base documents, and cannot be modified.
For a standalone return request, this field displays the default sales UoM code you specified in the Item Master Data screen, and it
can be changed manually. If you have not specified a default sales UoM code, this field is by default blank. You can select one from
all the UoM codes in the UoM group to which the item belongs.
 Note
If the item is not assigned to any UoM group, that is, in the UoM Group field of Item Master Data screen, you selected Manual,
then the UoM Code field displays Manual here, and the value cannot be changed.
Blanket Agreement No.
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
BP Catalog Number
Specify the business partner catalog number, instead of the item code and description, if you have defined it ( Inventory Item
Management Business Partner Catalog Numbers Use BP Catalog Number in Documents ).
Item Description
Specify an item description after you have entered the item number.
If required, change the description and press CTRL+TAB to save. The change is relevant for the current return request only.
This is custom documentation. For more information, please visit SAP Help Portal. 142

6/8/26, 6:04 AM
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the return request does not affect the inventory quantity of the
item. By default, this checkbox is not selected. After copying the return request to return or credit memo, Without Qty Posting field
will be disabled on the base return request.
For standalone return request, selecting this checkbox or not affects the target document that could be created based on this
return request.
When the checkbox is not selected, you can create return or credit memo based on the return request.
When the checkbox is selected, you can create only credit memo based on the return request.
In the target credit memo, the field is not editable. Still, the user could go back to the return request, and manually change the
setting, and then copy it to credit memo again.
The open quantity in the return request is updated according to the quantity drawn into the target document.
This is custom documentation. For more information, please visit SAP Help Portal. 143

6/8/26, 6:04 AM
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Gross Total (LC)
This is custom documentation. For more information, please visit SAP Help Portal. 144

6/8/26, 6:04 AM
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
Specify the reason why the customer wants to return the goods. There are the following options:
Empty
Indicates that there's no reason for the return.
Define New
Select this option and you will be directed to the Return Reasons - Setup screen. Here, you can add a return reason and
then select Update.
All the reasons you added in this screen will be displayed later in the Return Reason drop-down list.
This field is not visible by default. To display the field, in the menu bar, go to Tools Form Settings Return Request . In the
Table Format tab, select the field in the Visible checkbox.
Return Action
Specify the action the customer wants regarding the return. There are the following options:
Return (default value)
Indicates that the customer wants to return the goods.
Repair
Indicates that the customer wants the goods to be repaired only.
Replace
Indicates that the customer wants the goods to be replaced by new ones.
Define New
Select this option and you will be directed to the Return Actions - Setup screen. Here, you can add a return action and then
select Update.
This field is not visible by default. To display the field, in the menu bar, go to Tools Form Settings Return Request . In the
Table Format tab, select the field in the Visible checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 145

6/8/26, 6:04 AM
More Information
Return Request
Return Request: Logistics Tab
This tab contains details regarding the logistics aspects of the return request.
To access the tab, in Main Menu, choose Sales A/R Return Request Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return Request Logistics Tab Fields
Ship From
Displays the customer’s ship-from address ID and an additional summary of address components as defined in the business
partner master data. If required, change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
affect the business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; you can change it, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the destination address to which your customer delivers their goods and services for return.
If the Use Warehouse Address option is selected in the Document Settings General tab, this field displays the warehouse
address from the first row of the Contents tab of the current return document. If Use Warehouse Address is deselected, this field
displays your company address.
Shipping Type
Specify how the customer wants the goods to be returned, for example, by which courier. If there is no shipping types available in
the drop-down list, select Define New to add shipping types in the Shipping Type - Setup screen.
Confirmed
Indicates that the return request is approved and enables copying it to the corresponding return or credit memo.
This checkbox is selected by default if the checkbox Confirm Return Request Automatically in the Administration System
Initialization Document Settings Per Document tab is selected.
BP Channel Name
If this document is created for an indirect sale that was achieved through another business partner, specify the code of that
business partner.
BP Channel Contact
This is custom documentation. For more information, please visit SAP Help Portal. 146

6/8/26, 6:04 AM
Default contact person of the BP Channel, as defined in the business partner master data; you can change it, if required.
More Information
Return Request
Return Request: Accounting Tab
This tab contains information regarding the financial aspects of the return.
To access the tab, in Main Menu, choose Sales - A/R Return Request Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return Request Accounting Tab Fields
Journal Remark
By default, displays Return Request – XXX, where XXX is the customer code. Change this content, if required.
Payment Terms
By default, it displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Indicator
By default, displays the indicator linked to the customer (see Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in Business Partners Business Partner Master Data
General Area .
Order Number
Enter an order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
This is custom documentation. For more information, please visit SAP Help Portal. 147

6/8/26, 6:04 AM
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
Return Request
Sales Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
This is custom documentation. For more information, please visit SAP Help Portal. 148

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
Additional Information
Copy From Method
In SAP Business One, some documents can be generated based on some other documents, that is, a document can be copied from
another, or multiple other documents.
Example:
A return request can be copied from a delivery or a A/R invoice. The delivery or A/R invoice is called the base document, while the
return request is called the target document. However, there's a slight difference regarding the number of base documents from
which target document is copied. To be more concise, a return request can be copied from multiple deliveries, but only from one
A/R invoice.
Likewise, there are other documents which cannot be copied from multiple base documents. Here is a list of such target and base
documents which follow this rule:
A return request cannot be copied from multiple A/R invoices.
A goods return request cannot be copied from multiple A/P invoices.
This is custom documentation. For more information, please visit SAP Help Portal. 149

6/8/26, 6:04 AM
A goods return request cannot be copied from multiple Goods Receipt PO which has a foreign currency or a system
currency that's different from the local currency.
A goods return cannot be copied from multiple goods return requests which have a foreign currency or a system currency
that's different from the local currency.
An A/R credit memo cannot be copied from multiple return requests.
An A/P credit memo cannot be copied from multiple goods return requests.
Assembly BoM Handle
Return request which is created based on other document will keep the actual Assembly BoM structure included in the base
document, even if the BoM structure was changed in between the creation of the base document and the target document. While
standalone return request will take the current Assembly BoM structure.
The return/credit that are generated based on standalone return request will keep the Assembly BoM structure included in the
base return request.
More Information
Return Request
Return
For legal reasons, you cannot delete a delivery or invoice that you enter in SAP Business One, or change accounting-relevant data in
these documents. However, the customer might send the goods back for various reasons, or you might have made a mistake when
you entered the documents.
In such situations, create a return document.
When you enter a return document, you can reverse the posting of a delivery. When you create the return, the system corrects the
inventory quantities. If your company runs a perpetual inventory, creating a return automatically generates a journal entry that
updates the inventory value.
The return is the clearing document for a delivery. Therefore, if an A/R invoice has not yet been created for the delivery you want to
reverse, use the return document. If you have already recorded an invoice, use the A/R Credit Memo function to correct values and
quantities for the transaction in SAP Business One.
When you create a return document based on a sales order, you can choose to reopen the item quantity of the order. To be able to
do so, the checkbox Enable Reopening of Orders When Creating Returns Based on Orders must be selected in the document
settings. For more information, see Document Settings: Per Document Tab.
Reopening the item quantity has the following consequences:
The status of the sales order changes to Open.
The open quantity is increased by the item quantity in the return document. If the sum of the remaining open quantity plus
the returned quantity is higher than the quantity in the original order, the open quantity is increased up to the quantity in
the original order.
The delivered quantity is decreased by the quantity in the return.
For service type transactions, the open amount is increased accordingly by a value equal to the value from a return line. If
the sum of the remaining open amount plus the returned amount is greater than the total amount for the original order line,
This is custom documentation. For more information, please visit SAP Help Portal. 150

6/8/26, 6:04 AM
the total amount is used as the open amount.
If there are any freight charges related to the returned item, these charges are reopened in the same way as the item
quantities.
If the item is managed by batches, the returned batch-allocated quantity is increased by the quantity from the return line.
To access the window, choose Sales – A/R Return .
More Information
Creating Sales Documents
Return: General Area
Sales Document: Contents Tab
Return: Logistics Tab
Return: Accounting Tab
Return: General Area
This part of the sales document is used to enter general information pertinent to all items in the document.
To access this area, choose Sales – A/R Return .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. No.
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series.
Specify a series.
Field on the right: the number of the delivery. If you choose the manual series, enter the relevant number.
Status
Status of the return:
Open
You can draw the document completely or partially to a document of a higher level.
This is custom documentation. For more information, please visit SAP Help Portal. 151

6/8/26, 6:04 AM
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
Posting Date
Specify the posting date. The default value for this field is the current date on which the goods return is created. If required, change
the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services.
The default date is 30 days after the posting date. You can change it manually, or choose a different payment term in the Payment
Terms field.
Document Date
Document date, used for tax purposes, of the goods return. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the return.
Owner
Specify the code of the employee who owns the return.
Remarks
Enter additional information regarding the return.
This is custom documentation. For more information, please visit SAP Help Portal. 152

6/8/26, 6:04 AM
You can edit the field contents even after the document is added.
Total Before Discount
Displays the total amount of the document before the calculated discount.
 Note
If the discount is defined in the row for the item or service, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, enter the percentage of discount.
The field on the right displays the discount amount. You can change the values of these fields, if required.
Freight
Displays the total freight for the return.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the return calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
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
This is custom documentation. For more information, please visit SAP Help Portal. 153

6/8/26, 6:04 AM
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
Return
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
This is custom documentation. For more information, please visit SAP Help Portal. 154

6/8/26, 6:04 AM
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
This is custom documentation. For more information, please visit SAP Help Portal. 155

6/8/26, 6:04 AM
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
This is custom documentation. For more information, please visit SAP Help Portal. 156

6/8/26, 6:04 AM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
This is custom documentation. For more information, please visit SAP Help Portal. 157

6/8/26, 6:04 AM
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Gross Price after Disc.
By default, the field is hidden. To make it visible, use the Form Settings window to enable it.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
This is custom documentation. For more information, please visit SAP Help Portal. 158

6/8/26, 6:04 AM
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
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
Example:
The Unit Price of Item A is 28.07
This is custom documentation. For more information, please visit SAP Help Portal. 159

6/8/26, 6:04 AM
The Discount is 8%
The Quantity is 50 items
Parameter: Calculate the Row Total using the Unit Price Calculation of total row amount
Selected Total = Unit Price x Quantity x Discount = 28.07 x 50 x 0.92 =
1291.22
Not selected Price after Discount = Unit Price x Discount = 28.07 x 0.92 =
25.82 (the price was rounded from 25.8244)
Total = Price after Discount x Quantity = 25.82 x 50 = 1291
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
This is custom documentation. For more information, please visit SAP Help Portal. 160

6/8/26, 6:04 AM
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
This is custom documentation. For more information, please visit SAP Help Portal. 161

6/8/26, 6:04 AM
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
This is custom documentation. For more information, please visit SAP Help Portal. 162

6/8/26, 6:04 AM
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
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
This is custom documentation. For more information, please visit SAP Help Portal. 163

6/8/26, 6:04 AM
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
Return: Logistics Tab
This tab contains details regarding the logistics aspects of the delivery.
To access the tab, choose Sales A/R Return Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return Logistics Tab Fields
Ship From
Displays the customer’s ship-from address ID and an additional summary of address components as defined in the business
partner master data. If required, change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
affect the business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the destination address to which your customer delivers their goods and services for return.
If the Use Warehouse Address option is selected in the Document Settings General tab, this field displays the warehouse
address from the first row of the Contents tab of the current return document. If Use Warehouse Address is deselected, this field
This is custom documentation. For more information, please visit SAP Help Portal. 164

6/8/26, 6:04 AM
displays your company address.
Language
Language defined for the business partner in the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
Stamp No.
Enter the number that you receive from a chain as a confirmation of a return document.
You copy the stamp number to the A/R invoice and use it to create a file that is sent to the marketing chain for payments.
BP Channel Name
If this document is created for an indirect sale that was achieved through another business partner, specify the code of that
business partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
Return
Return: Accounting Tab
This tab contains information regarding the financial aspects of the return.
To access the tab, choose Sales – A/R Delivery Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Return Accounting Tab Fields
Journal Remark
By default, displays Return – XXX, where XXX is the customer code. Change this content, if required.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
This is custom documentation. For more information, please visit SAP Help Portal. 165

6/8/26, 6:04 AM
Specify a central bank indicator for documents created for foreign business partners.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
Indicator
By default, displays the Indicator linked to the customer (see Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
If the return is created based on a delivery, the federal tax ID that appears in this field is the one copied from the delivery.
Order Number
Enter an order number of the chain when you use the direct distribution method.
This number is recorded in the file that you send to a head office of the chain store.
Use Shipped Goods Account
Indicate whether to post the delivery of the inventory to the shipped goods account instead of the COGS account.
For returns that are created based on deliveries, the status of this checkbox is inherited from the same checkbox in the base
delivery.
 Note
This checkbox is not available for standalone returns.
This checkbox is for perpetual inventory companies only.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
This is custom documentation. For more information, please visit SAP Help Portal. 166

6/8/26, 6:04 AM
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
Return
Sales Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
This is custom documentation. For more information, please visit SAP Help Portal. 167

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
A/R Reserve Invoice
The A/R reserve invoice allows you to issue invoices for warehouse items without deducting the items from the inventory. If you
create a reserve invoice, SAP Business One creates an accounting journal entry without creating an inventory entry.
SAP Business One enables you to create an A/R reserve invoice with a zero amount. You can do this when delivering items without
a charge, for example, items that are part of a promotion or covered by a service contract.
Like an ordinary invoice, a reserve invoice is closed against an incoming payment. However, inventory closure takes place in the
delivery.
To access the window, choose Sales – A/R A/R Reserve Invoice . The A/R reserve invoice tabs are similar to the A/R invoice
tabs.
More Information
Creating Sales Documents
A/R Invoice
This is custom documentation. For more information, please visit SAP Help Portal. 168

6/8/26, 6:04 AM
Crediting A/R Reserve Invoices
Use one of the procedures below to credit customers for A/R reserve invoices, even if these have been delivered fully or partially.
This may be necessary if the customer has already received the A/R reserve invoice, but received damaged goods, and would now
like to be reimbursed for the expenses.
Prerequisites
An A/R reserve invoice exists for the customer.
Procedure
Copying an A/R Reserve Invoice into an A/R Credit Memo
1. From the SAP Business One Main Menu, choose Sales – A/R A/R Reserve Invoice and open the relevant document.
2. Click the Copy To button and select A/R Credit Memo.
The A/R Credit Memo window appears listing all items that were included in the A/R reserve invoice. If not all the items
have been delivered yet, the original item line is divided into two parts – one for the delivered items, one for the non
delivered items. If there are several related deliveries based on one A/R reserve invoice, the items are divided according to
the delivery. The delivery number is displayed in the A/R credit memo.
3. Enter the necessary data and choose Add.
The A/R credit memo for the A/R reserve invoice is created.
Copying an A/R Credit Memo from an A/R Reserve Invoice
1. From the SAP Business One Main Menu, choose Sales – A/R A/R Credit Memo .
2. Specify the relevant customer.
3. Click the Copy From button and select A/R Invoices.
The List of A/R Invoices window appears.
4. Select the A/R invoice that you want to credit and click Choose.
5. In the Draw Document Wizard window, select which exchange rate to use and how to copy the data into the credit memo,
and choose Finish.
6. Enter the necessary data and choose Add.
The A/R credit memo for the A/R reserve invoice is created. If not all the items have been delivered yet, the original item
line is divided into two parts – one for the delivered items, one for the non delivered items. If there are several related
deliveries based on one A/R reserve invoice, the items are divided according to the delivery. The delivery number is
displayed in the A/R credit memo.
Result
The A/R credit memo for the A/R reserve invoice is created.
More Information
A/R Reserve Invoice
This is custom documentation. For more information, please visit SAP Help Portal. 169

6/8/26, 6:04 AM
A/R Credit Memo
A/R Reserve Invoice: General Area
Use this part of the A/R reserve invoice to enter general information relevant to all items in the document.
To access the area, choose Sales – A/R A/R Reserve Invoice .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Reserve Invoice General Area Fields
Contact Person
Name of the default contact person defined in the business partner master data. If required, specify a different contact person.
Customer Ref. Number
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: the number of the A/R reserve invoice. If you choose the manual series, enter the relevant number.
Status
Status of the A/R reserve invoice:
Open
You can draw the document completely or partially to a document of a higher level.
Open – Printed
You printed the document and left it open.
Canceled
You canceled the document manually.
Closed
SAP Business One closed the document automatically when you drew it to another document.
Delivered
The document is fully drawn to a delivery, but not yet fully paid.
Paid
The document is fully paid but not yet fully drawn to a delivery.
Draft
The document is still a draft.
Posting Date
This is custom documentation. For more information, please visit SAP Help Portal. 170

6/8/26, 6:04 AM
Specify the posting date. The default value for this field is the current date on which the A/R reserve invoice is created. If required,
change the date.
 Caution
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services.
The default date is 30 days after the posting date. To change it, choose a different payment term in the dropdown list for the
Payment Terms field in the A/R Reserve Invoice. Alternatively, change the due date manually.
Currency
Specify the display currency for the amounts in the A/R reserve invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the A/R reserve invoice.
Owner
Specify the employee who owns the A/R reserve invoice.
Total Before Discount
Total amount of the A/R reserve invoice before the discount for the document is calculated.
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
This is custom documentation. For more information, please visit SAP Help Portal. 171

6/8/26, 6:04 AM
Rounding
This field appears only if the rounding method is defined as By Currency in Administration System Initialization Document
Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/R reserve invoice calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Applied Amount
The amount of the A/R reserve invoice that was copied to a payment document or to a credit memo.
Balance Due
Amount of the A/R reserve invoice that has not been paid or credited yet.
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
A/R Reserve Invoice
Sales Document: Contents Tab
This is custom documentation. For more information, please visit SAP Help Portal. 172

6/8/26, 6:04 AM
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
No Summary – the default value for this field.
This is custom documentation. For more information, please visit SAP Help Portal. 173

6/8/26, 6:04 AM
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 174

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
This is custom documentation. For more information, please visit SAP Help Portal. 175

6/8/26, 6:04 AM
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
Items per Unit is 6.
This is custom documentation. For more information, please visit SAP Help Portal. 176

6/8/26, 6:04 AM
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
This is custom documentation. For more information, please visit SAP Help Portal. 177

6/8/26, 6:04 AM
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
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
This is custom documentation. For more information, please visit SAP Help Portal. 178

6/8/26, 6:04 AM
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
This is custom documentation. For more information, please visit SAP Help Portal. 179

6/8/26, 6:04 AM
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
This is custom documentation. For more information, please visit SAP Help Portal. 180

6/8/26, 6:04 AM
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 181

6/8/26, 6:04 AM
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
This is custom documentation. For more information, please visit SAP Help Portal. 182

6/8/26, 6:04 AM
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
A/R Reserve Invoice: Logistics Tab
Use this tab to enter information regarding the logistics aspects of the A/R reserve invoice.
To access the tab, choose Sales – A/R A/R Reserve Invoice Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Reserve Invoice Logistics Tab Fields
Ship To
Displays the customer’s ship-to address and additional description as defined in the business partner master data. If required,
change the address and the description.
To change the description, either enter in the free-text field, or specify in the address component. To open the Address Component
window, choose . SAP Business One updates the address and the description only for this document; it does not affect the
business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Language
Language defined for the business partner in the business partner master data; change if required.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
Tracking No.
Specify the tracking number of the package as received from the delivery company.
Block Dunning Letters
Excludes the A/R reserve invoice from the dunning wizard run.
BP Channel Name
If you are creating this document for an indirect sale achieved through another business partner, specify the code of that business
partner.
BP Channel Contact
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
This is custom documentation. For more information, please visit SAP Help Portal. 183

6/8/26, 6:04 AM
More Information
A/R Reserve Invoice
A/R Reserve Invoice: Accounting Tab
Use this tab to enter information regarding the financial aspects of the A/R reserve invoice.
To access the tab, choose Sales – A/R A/R Reserve Invoice Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Reserve Invoice Accounting Tab Fields
Journal Remark
By default, displays A/R Invoice – XXX, where XXXis the customer code. Change this content, if required.
Control Account
Specify the control account for the A/R reserve invoice. The default value is the Accounts Receivable value in the business partner
master data.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if the due date has already expired.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Installments
Displays the installments details as specified in the business partner master data. To edit the data, click .
Print SEPA Direct Debit Prenotification
Applicable to SEPA (Single Euro Payment Area) relevant localizations only.
If selected, when printing an invoice you can choose from Invoice Only, Prenotification Only, and Invoice and Prenotification.
Where applicable, a Crystal Reports (CR) layout is available for a direct debit prenotification letter, for more information search for
the latest SAP Notes on SEPA.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
This is custom documentation. For more information, please visit SAP Help Portal. 184

6/8/26, 6:04 AM
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Indicator
By default, displays the indicator linked to the customer Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator from the dropdown list.
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
If the A/R reserve invoice is copied from base document, the federal tax ID that appears in this field is copied from the base
document.
Order Number
Enter an order number of the chain when you use the direct distribution method. This number is recorded in the file that you send
to a head office of the chain store.
Asset Value Date
 Note
The field is available only if you have enabled fixed assets.
If you use the A/R reserve invoice to retire a fixed asset, specify the date on which the retirement takes place in this field.
Different from the posting date which is the date of the journal entry from the accounting perspective, the asset value date is the
date of the retirement from the asset perspective.
More Information
A/R Reserve Invoice
Sales Document: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
This is custom documentation. For more information, please visit SAP Help Portal. 185

6/8/26, 6:04 AM
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
A/R Invoice + Payment
Use the invoice with payment for cash sales to one-time customers, who have to pay the full invoice amount immediately.
Prerequisites
You create a separate master record once for one-time customers. This master record is defined during system initialization, when
G/L account determination is defined as a standard customer for invoices with payment.
When you access the A/R Invoice + Payment function, the data relating to the one-time customer is copied to the transaction. You
can then maintain the customer’s name and address.
SAP Business One manages the invoice with payment as it does a standard invoice. The corresponding posting in the accounting
system and any posting in Inventory Management are processed automatically by the system when the invoice with payment is
This is custom documentation. For more information, please visit SAP Help Portal. 186

6/8/26, 6:04 AM
added.
The customer has to pay the invoice amount in full. Attempting to enter a partial payment generates an error message.
To access the window, choose Sales – A/R A/R Invoice+Payment .
More Information
Creating Sales Documents
A/R Invoice
Creating and Printing Packing Slips
Prerequisites
You have defined one or more package types in SAP Business One. For more information see Package Types - Setup.
You have opened one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
You have picked the items for the sales document that you open.
Context
You create and print packing slips in SAP Business One after you pick the items of a shipment and you are ready to send the
shipment.
You can create and print packing slips for only the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
The packing and packing slip printing process includes the following procedures:
1. Create a new packing slip.
2. Select items for shipment.
3. Move items to package contents.
4. Preview and print both your sales document and packing slips, or preview and print packing slips only.
Procedure
1. Create a new packing slip.
a. Open one of the aforementioned sales documents.
This is custom documentation. For more information, please visit SAP Help Portal. 187

6/8/26, 6:04 AM
b. Open the Packing Slip window by doing one of the following:
In the menu bar, choose Go To Packing Slip .
Right-click in the document and choose Packing Slip.
c. In the Package No. field in the upper Existing Packages area, enter an identifying number for the package. SAP
Business One automatically assigns a sequential number, but you can change it.
For more information, see Packing Slip Window.
d. Open the List of Package Types window in one of the following ways:
Place your cursor in the Type field and press the Tab key.
In the Type field, click .
e. In the List of Package Types window, select a package type and choose the Choose button.
f. (Optional) If you want to convert the package weight to a different unit of measure, in the Units dropdown list, select
the unit of measure you want to display in the Total Weight field.
 Note
The Total Weight field displays the total weight of the package. The value of the field is calculated according to
the weight you have defined in the Item Master Data window, on the Sales Data tab. If the item weight is not
defined, the Total Weight field is blank.
g. To add another package, right click the existing package row and choose Add Row. Repeat the above steps.
2. Select items for shipment.
a. In the Packing Slip window, go to the lower Available Items area.
b. In the Selected field, enter the number of items to include in the package for shipment.
The Available Items table displays a list of available items and their quantities. To find an item quickly, in the Find
field, enter the item number. The row with the corresponding item number is selected.
 Note
You cannot enter an item quantity that is higher than the quantity displayed in the Available field. The value in the
Available field shows the quantity of the item that you have not yet assigned to a package.
To add additional columns, such as UoM, Items per Unit, Weight, or Height to the Available Items table, right-
click the table header and choose Form Settings.
Alternatively, in the toolbar, click and in the Form Settings window, select the required columns.
You can add several packages to each shipment.
 Example
If you are creating a shipment of 30 items, and each package of the selected type can contain only ten items, you
must create three packages. You may use a combination of package types.
3. Move items to package contents.
Proceed as follows to move a selected quantity of items from the Available Items table to the Package Contents table.
a. In the Available Items table, select the rows of the items that you want to include in the package for shipment.
b. Choose the right arrow button. The Package Contents table shows the contents of the packages for delivery.
This is custom documentation. For more information, please visit SAP Help Portal. 188

6/8/26, 6:04 AM
c. Add additional packages as required. Choose Update, and then choose OK.
4. In your sales document, choose Update to update the packing slips information in your sales document.
5. Preview and print your sales document and packing slips.
To preview and print both the sales document and the packing slips, proceed as follows:
a. Open your sales document.
b. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One automatically previews or prints both the sales document and the packing slips at the
same time.
To preview and print only the packing slips, proceed as follows:
a. Open your sales document.
b. Open the Packing Slip window. Make sure that the Packing Slip window is the currently active window.
c. In the menu bar, from the File menu, choose Preview... or Print....
SAP Business One only previews or prints the packing slips.
Related Information
File Menu
Printing in SAP Business One
Working with Pick and Pack
Delivery
A/R Invoice
A/R Invoice + Payment
Packing Slip Window
Use this window to enter packing details for items and to create and print packing slips.
To access this window:
1. Open one of the following sales documents:
Delivery
A/R invoice
A/R invoice + payment
2. Do one of the following:
From the menu bar, choose Go To Packing Slip .
Right-click in the open document and choose Packing Slip.
If you select the Recommend Packaging from Item Master Data checkbox in the Documents Settings window, SAP Business One
fills the recommended packaging information for you in packing slips. You can change this information manually.
 Note
Printing Information
This is custom documentation. For more information, please visit SAP Help Portal. 189

6/8/26, 6:04 AM
You can print a packing slip directly from the Packing Slip window. When you print one of the documents listed in step 1, the
packaging information is automatically printed on a separate page.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Packages Setup Window Fields
Package No.
Enter the number for the package. By default, the system automatically enters a sequential number.
Type
Select a type of package. Alternatively, press TAB and select one of the types. To define a new package type, select New.
Total Weight
Displays the total weight of the package. The value of the field is calculated according to the weight you have defined on the Sales
Data tab in the Item Master Data .
Units
Select the unit of measurement for the weight of the package.
Find Available Items
Enter the item code to find the necessary item from the list.
Available
Displays the quantity (in purchasing UoM) of items available for packing.
Selected
Enter the number of items that you actually plan to pack in the special package. The value cannot be larger than the value in the
Available field.
Package Contents
Displays the number of different items making up the package.
Quantity
Displays the quantity (in purchasing UoM) of items in the package.
UoM
Displays the UoM specified for an item in associated purchasing documents.
Related Information
Creating and Printing Packing Slips
Transaction Codes
Journal Entry Window
A/R Credit Memo
This is custom documentation. For more information, please visit SAP Help Portal. 190

6/8/26, 6:04 AM
For legal reasons, you cannot delete a delivery or invoice that you enter in SAP Business One or change accounting-relevant data in
these documents. However, the customer might send the goods back for various reasons, or you may have made a mistake when
you entered the documents.
If a sales transaction for which you record an accounting and an inventory posting has been completely or partially reversed, you
must enter a corresponding sales document to clear it. This document reverses the changes in terms of inventory quantities and
monetary values.
The credit memo is the clearing document for the invoice and for the returns. If the goods were delivered to the customer and an
invoice has already been created, you can partially or completely reverse the transaction by creating a credit memo. With the credit
memo you correct both the quantities and the monetary values. The system increases the inventory of the credited items by the
amount specified in the credit memo. The credit memo credits the value in the customer account in the accounting system and
amends the revenue account by the same amount. The system corrects the tax amounts automatically.
SAP Business One enables you to create an A/R credit memo with a zero amount. You can do this when you clear A/R invoices for
items delivered without a charge, for example, items that are part of a promotion or covered by a service contract.
When you create an A/R credit memo based on a sales order, you can choose to reopen the item quantity of the order. To be able to
do so, the checkbox Enable Reopening of Orders When Creating Returns Based on Orders must be selected in the document
settings. For more information, see Document Settings: Per Document Tab.
Reopening the item quantity has the following consequences:
The status of the sales order changes to Open.
The open quantity is increased by the item quantity in the credit memo. If the sum of the remaining open quantity plus the
returned quantity is higher than the quantity in the original order, the open quantity is increased up to the quantity in the
original order.
The delivered quantity is decreased by the quantity in the credit memo.
For service type transactions, the open amount is increased accordingly by a value equal to the value from a credit memo
line. If the sum of the remaining open amount plus the credited amount is greater than the total amount for the original
order line, the total amount is used as the open amount.
If there are any freight charges related to the credited item, these charges are reopened in the same way as the item
quantities.
If the item is managed by batches, the returned batch-allocated quantity is increased by the quantity from the return line.
To access the window, choose Sales – A/R A/R Credit Memo .
More Information
Creating Sales Documents
A/R Credit Memo: General Area
Sales Document: Contents Tab
A/R Credit Memo: Logistics Tab
A/R Credit Memo: Accounting Tab
A/R Credit Memo: General Area
This is custom documentation. For more information, please visit SAP Help Portal. 191

6/8/26, 6:04 AM
Use the general area in the A/R credit memo to enter general information relevant to all items in the document.
To access this area from the SAP Business One Main Menu, choose Sales – A/R A/R Credit Memo .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Credit Memo General Area Fields
Contact Person
Name of the default contact person as defined in the business partner master data. If required, specify a different contact person.
Customer Ref. Number
Displays the customer reference number, if defined.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: the number of the A/R credit memo. If you choose the manual series, enter the relevant number.
Status
Status of the A/R credit memo:
Open
You can draw the document completely or partially to a document of a higher level.
Open – Printed
You printed the document and left it open.
Cancelled
You cancelled the document manually.
Closed
You closed the document manually or SAP Business One closed it automatically when you drew it to another document.
Draft
The document is still a draft.
 Note
A no-charge A/R credit memo is closed automatically once you add the document.
Posting Date
Specify the posting date. The default value for this field is the current date on which the A/R credit memo is created. If required,
change the date.
If the A/R credit memo is copied from an A/R invoice, make sure this date is on or after the posting date of the invoice.
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 192

6/8/26, 6:04 AM
If you change this date, the continuity of the numbers and dates on a document will be interrupted.
Due Date
Expected due date of the items or services. The default due date is the system date (current date).
You can change it manually. The due date becomes blank when posting date is updated.
Document Date
Document date of the A/R credit memo used for tax purposes. Change the date if required.
Currency
Specify the display currency for the amounts in the A/R invoice.
If the customer currency equals the local currency, the options are Local Currency and System Currency.
If the customer currency is a foreign currency, the options include BP Currency.
Your selection does not change the original currency of the document.
Branch
Select a branch for which you want to create the document.
 Note
This field is available only if you have enabled multiple branches.
Sales Employee
Specify the sales employee who initiated the A/R credit memo.
Owner
Specify the code of the employee who owns the A/R credit memo.
Remarks
Enter additional information regarding the A/R credit memo.
You can edit the field contents even after you have created the document.
Total Before Discount
Total amount of the A/R credit memo before the discount for the document is calculated.
 Note
If the discount is defined in the row for the item or service, the amount displayed in this field takes that discount into account.
Discount %
In the field on the left, specify the percentage of discount.
The field on the right displays the discount amount.
If required, you can change the values of these fields.
If the rounding method used by the company is By Document, this field displays the difference between the document total and
the document rounded total.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 193

6/8/26, 6:04 AM
When the A/R credit memo is based on an A/R invoice with the discount on a document level, the discount is not copied to the
rows.
DPM %
In the field on the left, enter the percentage of down payment.
The field on the right displays the down payment amount. If required, you can change the values of these fields.
 Note
To enable separate discount and down payment percentages, go to Administration System Initialization Document
Settings . Open the Per Document tab, choose A/R Down Payment or A/P Down Payment from the Document dropdown
list, and then select the checkbox Separate Discount % and DPM % Fields.
Total Down Payment
Amount drawn from the paid down payment invoices or down payment requests, and subtracted from the total amount of the
invoice.
Freight
Displays the total freight for the A/R credit memo.
This field appears only if you have selected Manage Freight in Documents in Administration System Initialization Document
Settings General .
WTax Amount
The amount withheld, according to the withholding tax definitions, and paid over or reported to the tax authorities on behalf of the
person subject to tax.
Appears only if you have selected Withholding Tax in Administration Setup Financials G/L Account Determination
Sales Tax .
Rounding
This field appears only if the rounding method has been defined as By Currency in Administration System Initialization
Document Settings General .
When the total amount of the document is rounded according to the rounding method determined by the currency, the difference
between the original amount and the rounded amount appears in this field.
Tax
Tax amount for the A/R credit memo calculated according to your tax definitions.
Total
Total amount of the document including tax and discounts.
Applied Amount
The actual amount that was copied from the base document to the A/R credit memo:
If the copied amount is smaller than or equal to the Balance Due amount in the base document, this is the amount that is
displayed in both the Total and Applied Amount fields.
If the copied amount is bigger than the balance due in the base document (this can be the case if, for example, the base
document is an A/R invoice that was partially paid, and the A/R credit memo that is now being created is initiated due to a
goods return with a value larger than the balance due of the A/R invoice), the value displayed in the Applied Amount field is
smaller than the Total of the A/R credit memo.
This is custom documentation. For more information, please visit SAP Help Portal. 194

6/8/26, 6:04 AM
The difference between the Applied Amount and the Total is displayed in the Open Balance field.
 Example
Fred's Factory creates an invoice for George's Store for two items:
Small Bench $300
Wood bench $400
Total $700
George's Store pays $500 towards the invoice, so the remaining balance on the invoice is $200. Then George returns the small
bench; therefore, he is owed $300.
Fred creates a credit memo based on the invoice. Of the $300 that is owed, $200 is applied to the invoice, and $100 remains as
credit not based.
This credit is due to George's Store and may be used towards future purchases. The invoice is fully paid since the $700 is
accounted for, by $500 in the partial payment and $200 in the credit memo.
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
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, the Copy From and the Copy To functions are disabled.
 Note
When this checkbox is selected, you cannot change values in the Due Date field in the general area and in the Payment Block
field on the Accounting tab.
More Information
A/R Credit Memo
This is custom documentation. For more information, please visit SAP Help Portal. 195

6/8/26, 6:04 AM
Sales Document: Contents Tab
Use this tab to specify items or services to be sold.
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
Item in SAP Business One.
The table view on this tab is different for each option.
Including both items and services in the same sales document is not possible. However, you can define the respective services as
items in SAP Business One. You then can enter the related items and services in one document along with their respective prices
and quantities. It is possible to run the usual sales analysis and reports on these services.
Price Mode
This field appears only if you selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Choose one of the following modes:
Net – Select this option to enter prices and amounts in net mode; all prices and amounts related to gross prices are
calculated automatically according to the specified tax code and are not editable.
Gross - Select this option to enter prices and amounts in gross mode; all prices and amounts related to net prices are
calculated automatically according to the specified tax code and are not editable.
Net and Gross – This option is displayed for the documents that meet one of the following conditions:
Documents created before you upgrade to SAP Business One version 9.3
Documents drawn from others that were created before you upgrade to SAP Business One version 9.3.
To change the price mode before adding the document, delete all existing rows.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Summary Type
Choose one of the following types:
This is custom documentation. For more information, please visit SAP Help Portal. 196

6/8/26, 6:04 AM
No Summary – the default value for this field.
By Documents – summarizes rows with the same base documents into one row that displays the base document number
and reference. If an item appears in the table more than once and has the same price and description each time, it will be
summarized to one row. This option is available only for documents of the type Item and when you copy rows from base
documents.
By Items – summarizes several item rows with the same item into one row. However, this is possible only when these item
rows have the same parameters (for example, price, description, and warehouse). This option is available only for
documents of the type Item.
Table View for Document Type Item
Quantity
Quantity that you want to sell to the customer based on the item’s sales unit of measure, as defined on the Sales Data tab in the
Item Master Data window. The default value is 1.
If the sales unit of measure is defined as more than one item, the actual item quantity is displayed in the Qty (Inventory UoM) field,
which is the value displayed in the Quantity field multiplied by Items Per Unit.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
You can update the quantity in a sales order or purchase order.
Delivered
Delivered quantity of the item that has already been delivered to the customer.
Qty to Ship
Displays quantity still to be shipped from the line after the current delivery.
Ordered
Displays the original ordered quantity.
Unit Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
Editable only if the document price mode is Net or Net and Gross. Enter the item net price, before any discount.
When the document price mode is Gross, Unit Prices are calculated automatically according to the specified gross price
and tax code and they are not editable.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
Item price from the default price list, before any line discount.
If the value specified in the Inventory UoM field is Yes, the price is the Unit Price.
If the value specified in the Inventory UoM field is No, the price is the Unit Price x Items per Unit.
This is custom documentation. For more information, please visit SAP Help Portal. 197

6/8/26, 6:04 AM
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
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or the Unit
Price field. We do not recommend to have in the same document rows in which the items are priced according to Unit Price and
other rows where the items are priced by Gross Price.
Inventory UoM
Define whether the quantity displayed in the Items per Unit field is a single item unit:
No - default value; if you specified a sales unit of measure for the item as defined on the Sales Data tab in the Item Master
Data window that is different than 1, the number of item units issued by the warehouse equals the number specified in the
Quantity field, multiplied by the Items per Unit value.
 Example
Quantity x Items per Unit = Qty (Inventory UoM).
Yes - the number of item units issued from the warehouse equals the number specified in the Quantity or Qty (Inventory
UoM) field. The Items per Unit value is one.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 198

6/8/26, 6:04 AM
Quantity x 1 (Items per Unit) = Qty (Inventory UoM).
UoM Name
When a UoM code is specified, SAP Business One takes the corresponding UoM name from the UoM setup.
You can edit this field only when the UoM group of an item is Manual.
Items per Unit
The number of items specified for the selected UoM as defined on the Sales Data tab in the Item Master Data window. The
number must be greater than zero.
You can edit this field when the UoM group for an item is Manual. When inventory transactions are created from the document, the
Items per Unit value from the document is used, not the value from the Item Master Data window.
 Note
TheItems per Unit field cannot be edited in the following situations:
The UoM group of an item is not Manual.
A document is based on another document.
Rows in a document are partially open, for example, when some of the items have been copied to another document.
Without Qty Posting
Indicates that there is no inventory movement involved, that is, the marketing document does not affect the inventory quantity of
the item.
 Example
You delivered items to a customer, but some items were broken during shipment. Since the customer is asking for a return of
the payment, you create a credit memo and, by choosing this checkbox, indicate that there is no return of goods.
Other example reasons include price increases due to inflation, agreed quantities not being fulfilled, and subsidiary donations of
initial sales.
The field is available in the following cases:
A/R credit memos not based on other documents or
A/R credit memos based on an A/R invoice or
A/R credit memos based on an A/R reserve invoice, for which items have been delivered, and
If non-drop-ship warehouses are used.
A/R invoices. Not available in localizations for Argentina, Brazil, Chile, and India.
A/R invoices + payments. Not available in localizations for Argentina, Brazil, Chile, and India.
Qty (Inventory UoM)
The total quantity (per row), calculated as follows:
Quantity x Items per Unit = Qty (Inventory UoM)
 Example
Quantity is 2.
This is custom documentation. For more information, please visit SAP Help Portal. 199

6/8/26, 6:04 AM
Items per Unit is 6.
Qty (Inventory UoM) = 12.
Discount %
Displays the discount percentage assigned to the item.
Price after Discount
Displays the amount calculated from Unit Price x Discount.
Item Cost
Real-time item cost of the item at the time the document is added.
WTax Liable
Indicates if withholding tax is applicable in this document.
Freight in the header level is not affected, but those items on the row level are.
When the checkbox Tax only is selected, the WTax Liable field is automatically updated to No. You can select the value manually in
the dropdown list.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
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
This is custom documentation. For more information, please visit SAP Help Portal. 200

6/8/26, 6:04 AM
When creating a document, make sure that for all of the items in the document, you fill in either the Gross Price field or
the Unit Price field. We do not recommend having in the same document rows in which the items are priced according to
Unit Price and other rows where the items are priced by Gross Price.
The value displayed in the Tax Amount field is calculated as follows:
Gross Price * (1 - discount) / (1 + Tax %) * Tax % * Quantity = Tax Amount
 Example
Gross Price = 150
Quantity = 2
Tax % = 20
Discount % = 10
Tax Amount = 150 *(1 - 10%) / (1 + 0.2) * 0.2 *2 = 45
Project
Specify the project that you want to relate to the item.
Total (LC)
Displays the total amount of the row in the relevant currency. The amount is calculated as follows: Total = Unit Price x Quantity x
Discount.
 Note
The following applies to companies that use an original version of SAP Business One prior to SAP Business One 2007 A or 2007
B and upgraded to SAP Business One 8.8 directly or upgraded to SAP Business One 2007 A or 2007 B and then to SAP
Business One 8.8.
The calculation method depends on whether you have selected the parameter Calculate the Row Total using the Unit Price (on
the General tab in Administration System Initialization Document Settings window).
Selected: Unit Price x Discount x Quantity
Not selected:Price after Discount x Quantity
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
This is custom documentation. For more information, please visit SAP Help Portal. 201

6/8/26, 6:04 AM
Blanket Agreement
Number of the linked blanket agreement that exists with the customer.
After you have entered a business partner, an item and a posting date, SAP Business One checks whether a blanket agreement is in
force with the customer and automatically relates it to the sales document. The unit price determined in the blanket agreement is
copied into the sales document, if in the blanket agreement, the Use BP Discount option is checked.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many items are allocated from bin locations.
You must allocate the same quantity of items from bin locations as the quantity you specified in the document row; otherwise, the
field is marked in red and you cannot add the document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
 Note
In returns and A/R credit memos, for the document rows with items that are not managed by serials or batches, clicking in
the field opens the Bin Location Allocation - Receipt Window instead.
Consume Forecast
To enable the item to consume forecast using sales orders, select Yes.
 Note
To consume forecast using sales orders, you must also select the Consume Forecast checkbox on theGeneral Settings:
Inventory Tab.
In the MRP run, the application subtract the sales order quantities from the forecasted quantities.
For more information, see Managing Forecasts.
Allow Procmnt. Doc.
This checkbox is available for sales quotations and sales orders.
Select this checkbox to enable automatically creating procurement documents with the Procurement Confirmation Wizard after
you add a sales document.
For more information, see Procurement Confirmation Wizard.
This is custom documentation. For more information, please visit SAP Help Portal. 202

6/8/26, 6:04 AM
Ship-to Name, Ship-to Description
Displays the ship-to name and description as defined on the Logistics tab. If required, specify different names and descriptions for
each row. By default, these two fields are hidden. You can activate their display in the Form Settings window.
 Note
The following is only relevant to sales orders and A/R reserve invoices:
When you create deliveries in the pick and pack process, SAP Business One copies the ship-to names and ship-to descriptions
from the selected sales order rows or A/R reserve invoice rows to the delivery documents. Separate delivery documents are
created for sales orders and A/R reserve invoices. The documents of either type having the same customer, same row-level
ship-to address, and ship-to description are copied to one delivery document.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
Partial Retirement
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row.
Select the checkbox to indicate the asset retirement is partial, for example. only part of the asset quantity or value is removed from
the portfolio.
Retired Quantity
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the retired acquisition and production costs, it is not effective.
This is custom documentation. For more information, please visit SAP Help Portal. 203

6/8/26, 6:04 AM
Retired APC
 Note
The field is available only if you have enabled fixed assets.
By default, the field is hidden. To make it visible, use the Form Settings.
And, the field is editable only when you select a fixed asset in the row and the asset retirement is partial.
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the retired quantity, it is not effective.
Distribute Freight
Choose whether to distribute total level freight on this row.
If you choose No, the row is not affected by the total level freight and it is distributed on other rows in the document.
This field is not available for down payment documents.
Freight 1,2,3
Specify a relevant freight type.
This field is not available for down payment documents.
Freight 1,2,3 (LC)
Specify each freight charge in the appropriate currency.
The freight amount is automatically recalculated according to exchange rate changes.
This field is not available for down payment documents.
Freight 1,2,3 Project
If required, specify the project for each freight. If you defined the project for the freight in the Freight-Setup window, the field
displays the project code by default.
 Note
The freight-related fields appear only if you have selected Manage Freight in Documents on the General tab of the Document
Settings window in Administration System Initialization .
Gross Total
Displays the total gross amount of the row. If the item quantity is 1, the gross total is equal to the amount entered in the Gross
Price field. The amount in this field is calculated as follows:
Gross Price * Quantity = Gross Total
 Example
Gross Price = 5
Quantity = 10
Total Gross = 5 * 10 = 50
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 204

6/8/26, 6:04 AM
In some cases small differences between the sum of the amounts appear in the Gross Total field in the document rows and the
amount appears in the Total field at the document footer may occur. This is a result of different calculation method that is used
in the Total field. For more information, see the How to Work with Gross Prices guide. You can download this document from
the SAP Help Portal.
Table View for Document Type Service
Description
Enter a description of the sold service.
G/L Account
Choose the G/L account to be credited if the document created is an A/R invoice. Press TAB to display the List of G/L Accounts
and choose one. The list displays general ledger accounts of the sales, expenditures, and other account types.
Project
Specify the project that you want to relate to the service.
Tax Code
Tax code to be applied to the item. The application proposes a default tax code depending on the following:
Tax code determination rules defined (if applicable)
Tax code defined in the business partner master data
Tax code defined in the item master data
Tax code defined in the freight setup
Tax code defined in the G/L account determination
If required, choose a different tax code.
Total (LC)
Displays the total amount of the row in the relevant currency.
Tax Only
Select this checkbox to charge or credit the business partner only for the tax that is calculated on the value of the item or service.
In certain industries, such as the airlines industry, companies may be required to generate a no charge invoice with tax only. As air
miles become a popular benefit to travelers, it is a requirement in some countries that customers pay tax on the value of the miles.
By selecting this checkbox you can charge customers solely for tax based on the value of the air miles.
 Note
The Tax Only setting cannot be edited, if you selected the checkbox for a specific line and copied this line into a follow-on
document that is a formal document, such as a delivery, A/R or A/P invoice, and the checkbox Allow Changes to Existing
Orders for sales orders under Administration System Initialization Document Settings Per Document was not
selected.
This option is available in most of the localizations. Additional information may be found in the localized online help file under:
Help Documentation Country-Specific Info .
Tax Amount (LC)
Displays the tax amount in local currency.
This is custom documentation. For more information, please visit SAP Help Portal. 205

6/8/26, 6:04 AM
Distribute Freight
Specify whether to distribute the freight amount from the Total level onto the row.
This field is not available for down payment documents.
A/R Credit Memo: Logistics Tab
This tab contains details regarding the logistics aspects of the A/R credit memo.
To access the tab, choose Sales – A/R A/R Credit Memo Logistics .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Credit Memo Logistics Tab Fields
Ship From
Displays the customer’s ship-from address ID and an additional summary of address components as defined in the business
partner master data. If required, change the address.
To change the address, either enter full text in the free-text field, or specify the address components. To open the Address
Component window, choose . SAP Business One updates the address and the description for this document only; it does not
affect the business partner master data.
Bill To
The customer bill-to address defined in the business partner master data; change, if required.
To change an address component, click the address field. In the Address Component window, specify the address component. The
system updates the address only for this marketing document; it does not affect the business partner master data.
Ship To
Displays the destination address to which your customer delivers their goods and services for return.
If the Use Warehouse Address option is selected in the Document Settings General tab, this field displays the warehouse
address from the first row of the Contents tab of the current return document. If Use Warehouse Address is deselected, this field
displays your company address.
Language
Language defined for the business partner on the General tab of the business partner master data.
If required, choose a different language.
 Note
You display or print the document in the selected foreign language only if you have translated the field values using the Multi-
Language Support function.
BP Channel Name
If you are creating this document for an indirect sale that was achieved through another business partner, specify the code of that
business partner.
BP Channel Contact
This is custom documentation. For more information, please visit SAP Help Portal. 206

6/8/26, 6:04 AM
Default contact person of the BP Channel, as defined in the business partner master data; change, if required.
More Information
A/R Credit Memo
A/R Credit Memo: Accounting Tab
This tab contains information regarding the financial aspects of the A/R credit memo.
To access the tab, choose Sales – A/R A/R Credit Memo Accounting .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
A/R Credit Memo Accounting Tab Fields
Journal Remark
By default, displays A/R Credit Memo – XXX where XXXis the customer code. If required, change this content.
Control Account
Specify the control account for the A/R credit memo. The default value is the Accounts Receivable value in the business partner
master data.
 Note
The control account for a document-based A/R credit memo must be the same as that in the base document.
Payment Block
To define the document as blocked and exclude it from payment, select this checkbox and the proper payment block reason.
Max. Cash Discount
Calculates the discount in the payment run, even if the due date has already expired.
Payment Terms
By default displays the payment terms for the customer as defined in the business partner master data. If required, specify
different payment terms.
Payment Method
Specify the payment method for the customer as defined in the business partner master data.
Central Bank Ind.
Specify a central bank indicator for documents created for foreign business partners.
Manually Recalculate Due Date
Specify the formula to calculate the due date for the installment.
The calculation uses the values specified in the payment terms. When adding the document, you can manually change the
calculation formula. You may set the payment period for the current month, several months in the future, or a specific number of
This is custom documentation. For more information, please visit SAP Help Portal. 207

6/8/26, 6:04 AM
days in the last month of the period. You can also choose whether the payment period ends at the start, middle, or end of the
month.
Consolidation Type, Consolidating BP
You can view and update the consolidating business partner and consolidation type of this document. When you are creating the
document, the default values are taken from the business partner master data. You cannot change the values after the document is
added. The consolidation type (payment consolidation and delivery consolidation) only takes effect when the type is related to the
current document and a consolidating business partner is defined.
For more information about consolidating business partner and consolidation type, see Business Partner Master Data Accounting
Tab, General.
BP Project
By default, displays the project name linked to the customer in the business partner master data. If required, specify a different
project name.
Indicator
By default, displays the indicator linked to the customer ( Business Partners Business Partner Master Data General tab).
The indicator is used as selection criteria in various reports. If required, choose a different indicator by clicking .
Federal Tax ID
The customer's federal tax ID, if defined in the Federal Tax ID field in: Business Partners Business Partner Master Data
General Area .
Order Number
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
This is custom documentation. For more information, please visit SAP Help Portal. 208

6/8/26, 6:04 AM
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
A/R Credit Memo
Sales Document: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 209

6/8/26, 6:04 AM
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
A/P and A/R Tax Invoice - General Information
A/P and A/R tax invoices are documents issued by vendors and sellers, respectively. For taxation purposes, you are legally
obligated to issue tax invoices for sold goods or services.
Use tax invoices to summarize an A/P or A/R invoice issued or received by your organization. Additional types of tax invoices
linking different documents are available.
After you post tax invoices, they are registered in the purchasing and sales ledgers. There is no accounting posting behind a tax
invoice. For more information about the ledgers, see Sales and Purchase Ledger Reports - Creation Procedure.
You cannot modify tax invoices after you post, but you can cancel improper tax invoices as a whole. In such a case they will not
affect the corresponding ledger. Their base documents can be linked to a new tax invoice.
If you cancel or reverse a document (for example, cancel a payment or create a credit memo based on an invoice) that has been
linked to a tax invoice, it is necessary to cancel the tax invoice and create a new one. You must then regenerate the relevant ledger.
The following types of tax invoices are available and have different base documents respectively:
Invoice
A collection of one or more A/P or A/R invoices (including reserve invoices) which represent an outgoing or incoming goods
delivery. Only base documents that have been issued in the same currency can be included on the same tax invoice.
 Note
You cannot cancel an invoice that is linked to a tax invoice unless you cancel the tax invoice first. Neither can you include
canceled invoices and their corresponding cancellation documents in a tax invoice.
Payment (for A/R tax invoice only)
A link to a down payment (a payment not based on an invoice), which must be registered in the sales ledger due to VAT
reporting.
Journal Entry
A link to a journal entry, which posts VAT to an incoming or outgoing VAT G/L account. This journal entry must be formatted
in such a way that:
For an A/R tax invoice, an output VAT G/L account is credited and its base amount is specified
For an A/P tax invoice an input VAT G/L account is debited and its base amount is specified
This is custom documentation. For more information, please visit SAP Help Portal. 210

6/8/26, 6:04 AM
 Recommendation
We recommend using a special indicator field value for those journal entries that you want to include on a tax invoice,
because SAP Business One lets you filter by this criterion during journal entry selection.
The structures of A/P and A/R tax invoices are very similar. The following describes the common elements. For specific issues, see
A/P tax invoice or A/R tax invoice documentation.
Header Area
Customer/Vendor
Specify the customer or vendor code.
No.
Current number of the document.
Specify a numbering series. You can select Manual to specify a non-system tax invoice number (a number assigned outside the
system). The system creates the sales document as a copy of the external document rather than as an original document.
Posting Date
Specify the posting date.
The default value for this field is the current date on which the document is created.
Changing this date is allowed, but interrupts the continuity of the numbers and dates on a document.
Value Date
Date on which the document was issued.
Tax Date
Date which enables you to determine the time period for the sales or purchase documents to be included in a report.
Vendor Ref. No. (A/P Tax Invoice only)
Vendor reference number, if available.
Currency
Specify the display currency for the amounts in the document.
Contents Tab
Type
The type of base documents you want to include in the tax invoice.
The following base document types are available:
Invoice
Base documents are A/R or A/P invoices (including reserve invoices). Canceled, reversed, and corrected invoices are not
included. Cancellation invoices are not included either.
Payment
For A/R tax invoices only; base documents are incoming payments based on down payment requests.
This is custom documentation. For more information, please visit SAP Help Portal. 211

6/8/26, 6:04 AM
Journal Entry
The base document is a journal entry with an appropriate structure, including output or input VAT posting.
Correction Invoice
Base documents are correction invoices that are not reversed.
Down Payment
For A/P tax invoices only; base documents are A/P down payment invoices.
Invoice No.
Number of the base invoice linked as the base document to the tax invoice.
Total
Total net sum on the invoice.
Tax
Total tax (VAT) for the invoice for all VAT groups.
Total (incl. Tax)
Total sum for the invoice, including VAT.
Indicator
Filter criterion for journal entries, applied when you search for a journal entry to be included on the tax invoice.
 Example
You create journal entries with TI as the value of the Indicator field on the journal entry.
You can select this value here.
When you click the Choose button of the Journal Entry VAT field, SAP Business One proposes only those journal entries
that have this value set in the Indicator field.
Journal Entry VAT
The actual link to the journal entry.
Click Choose to display a list of journal entries for selection.
If you have chosen any value for the Indicator field, only those journal entries that have a matching value in this field are displayed .
Posting Date
Date on which the journal entry was posted to the system.
Description
Text field for stating the reason for creating this type of tax invoice.
Details
Displays the linked journal entry.
Bottom Area
This is custom documentation. For more information, please visit SAP Help Portal. 212

6/8/26, 6:04 AM
Payment Document No.
Specify the number of the referenced payment document.
If the tax invoice is of type Payment, the value of this field is copied from the selected payment.
Payment Document Date
Specify the date of the referenced payment document. If the tax invoice is of type Payment, the value of this field is copied from
the selected payment.
Total
Total net sum for all included base documents (Invoice and Journal Entry types only).
Tax
Total tax (VAT) for all included base documents, for all VAT groups.
Total (incl. Tax)
Total sum for all base documents, including VAT.
Creating Sales Documents
Procedure
1. From the SAP Business One Main Menu, choose Sales – A/R and choose one of the documents.
The required document appears.
2. Enter the customer code, name, and other relevant general information.
3. On the Contents tab, select either Service or Item and enter data, as appropriate, in the remaining fields.
4. On the Logistics tab, make the necessary selection and entries.
5. On the Accounting tab, enter the required data.
6. To create a new sales document, choose one of the following options and confirm the system message.
Add & New
Adds the document and opens a new window for you to create another document.
It is similar to the previous Add button.
Add & View
Adds the document and displays it.
Add & Close
Adds the document and closes the window.
Your last choice will be remembered the next time you open the window of the given document.
 Note
When you create a no-charge A/R invoice, A/R credit memo, or A/R reserve invoice, the system displays a message with
the option to create a document with a zero total amount. To continue and create such a document, choose OK.
When you are creating a sales document, you can move all the rows in the Contents tab up and down if the tab doesn’t
include the following items:
This is custom documentation. For more information, please visit SAP Help Portal. 213

6/8/26, 6:04 AM
Sales type of BOMs.
Alternative items.
Subtotal type of rows.
When you are editing an open sales document which doesn't create posting, for example, a sales order or a return request,
you can move all the rows in the Contents tab up and down if the tab doesn’t include the following items:
Sales type of BOMs.
Partially or fully closed items or services.
Alternative items.
Manually Changing COGS Accounts in Sales Documents
Prerequisites
You have prepared the relevant sales document, but have not yet added it to the database.
Context
When you create a sales document, the costs of goods sold for the items are automatically attributed to the default COGS account.
If the sales document is based on another document, the default COGS account is taken from the base document. If the sales
document is not based on another document, the default COGS account depends on the Set G/L Accounts By setting on the
Inventory Data tab in the item master data. You can manually attribute the costs on a row level to a different COGS account.
You can change the COGS account in all sales documents except the following:
A/R down payment invoices
A/R down payment requests
A/R invoices based on deliveries
Credit memos based on returns
Correction invoices
You cannot change the COGS account in:
Documents that create journal entries and have already been added to the database
Rows that have been closed or copied to a follow-on document
Procedure
1. Open the window of the sales document.
2. On the Table Format tab, select the Visible and Active options for COGS Account and choose OK.
The COGS Account column is now visible and can be edited on the Contents tab of the sales document.
3. To change the COGS account at the row level, place the cursor in the COGS Account column in the item row and specify the
new COGS account.
4. To save the sales document in the database, choose Add.
This is custom documentation. For more information, please visit SAP Help Portal. 214

6/8/26, 6:04 AM
Related Information
Creating Sales Documents
Creating Sales and Purchasing Documents with Negative Totals
Use
You can create invoices with negative totals. This allows you to bill and refund a customer or vendor in one single document. This
may be convenient for example, if you as a sales person are on the phone with a customer who is ordering certain items, but at the
same time wants to return some items that he ordered previously. In this case, instead of posting an A/R invoice and a credit
memo, you enter the items that the customer purchases as a positive quantity and the goods the customer intends to return as a
negative quantity.
 Recommendation
We recommend that you consider carefully whether you would like to record two opposite transactions in one document.
Posting two documents helps to improve transparency in accounting.
You can generate the following documents with a negative total:
A/R and A/P invoice
A/R and A/P credit memo
An A/R delivery
An A/R return
An A/P goods receipt
An A/P goods return
The inventory valuation behavior of the documents with negative totals is as outlined in the table below.
Inventory valuation behavior of documents with negative totals
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
Goods receipt P/O Goods return Inventory Allocation
Goods return Goods receipt P/O Inventory Allocation
A/P Invoice A/P credit memo Inventory Vendor Negative Adjustment
Account, Price
Differences Account
A/P credit memo A/P invoice Inventory Vendor Negative Adjustment
Account, Price
Differences Account
Delivery A/R return Inventory COGS
Return Delivery Sales Return COGS
A/R invoice A/R credit memo Inventory COGS
A/R credit memo A/R invoice Sales Return COGS
This is custom documentation. For more information, please visit SAP Help Portal. 215

6/8/26, 6:04 AM
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
Goods receipt P/O based Goods return based on Inventory Allocation Negative Adjustment
| on goods return | goods receipt P/O |     | Account, Price |
| --------------- | ----------------- | --- | -------------- |
Differences Account
Goods return based on Goods receipt P/O based Inventory Allocation Negative Adjustment
| goods receipt P/O | on goods return |     | Account, Price |
| ----------------- | --------------- | --- | -------------- |
Differences Account
| A/P invoice based on | Credit memo based on | No inventory transaction |     |
| -------------------- | -------------------- | ------------------------ | --- |
| goods receipt P/O    | goods return         |                          |     |
A/P credit memo based A/P invoice based on Vendor, Allocation Price Differences
| on goods return | goods receipt P/O |     | Account, Negative |
| --------------- | ----------------- | --- | ----------------- |
Adjustment Account
A/P credit memo based Invoice based on credit Inventory Vendor Negative Adjustment
| on A/P invoice | memo |     | Account, Price |
| -------------- | ---- | --- | -------------- |
Differences Account
Delivery based on return Delivery based on return Inventory COGS Negative Adjustment
Account
Return based on delivery Return based on delivery Sales Return COGS Negative Adjustment
Account, Price
Differences Account
| A/R invoice based on  | Credit memo based on | No inventory transaction |     |
| --------------------- | -------------------- | ------------------------ | --- |
| delivery              | return               |                          |     |
| A/R credit memo based | A/R invoice based on | No inventory transaction |     |
| on return             | delivery             |                          |     |
A/R credit memo based A/R invoice based on Sales Return COGS Negative Adjustment
| on invoice | credit memo |     | Account, Price |
| ---------- | ----------- | --- | -------------- |
Differences Account
QR Codes and Sales Documents
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
This is custom documentation. For more information, please visit SAP Help Portal. 216

6/8/26, 6:04 AM
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
easily with less potential for error. Choosing a setting of "Low" means that more information can be included in the QR Code
but that the QR Code can be read and printed less easily with more potential for error.
Marketing Documents
The field Create QR Code From is available on the Accounting tab of marketing documents, for example on A/R invoices. The
information entered in Create QR Code From is used as the source from which QR Codes are saved in system tables and
transformed into PNG (Portable Network Graphic) images. Information can be added manually to Create QR Code From, by using
a formula in a formatted search, by DI API input, or by SAP Business One Service Layer on Windows (not on Linux). The source for
QR Codes can also be user-defined fields that are called by API. The information entered into Create QR Code From can be
anything that customers require but is typically a link to a webpage that displays information relevant to the document. You can
display QR Code images on print layouts of marketing documents. Print layouts must be manually adjusted to include QR Code
images based on joined data sources in the system.
1. From the SAP Business One Main Menu, choose Sales - A/R A/R Invoice Accounting tab .
2. Enter a link to a webpage for your company's A/R sales team in Create QR Code From.
3. Add the A/R invoice to the system to trigger the generation of a QR Code.
 Note
For more information on QR Codes, example queries, and Crystal Report files, see SAP Note 2889899 .
Canceling Sales and Purchasing Documents
If a marketing document is added in error, has become invalid, or has no concrete transactions associated with it, you can cancel
the document but still store it in the database. In some countries, it is even legally binding to cancel such documents instead of
closing them (when the closing approach is available, for example, for deliveries) or deleting them from the database.
 Note
If you want to indicate in your print layouts whether or not a document is canceled, or that a document is a cancellation
document, you can make use of the database field “Cancelled”. You can use this field when designing both PLD and Crystal
Reports layouts. The valid values for this field are listed below:
Y (Yes): Indicates a canceled document.
N (No): Indicates that the document is not canceled.
This is custom documentation. For more information, please visit SAP Help Portal. 217

6/8/26, 6:04 AM
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
Sales Document Purchasing Document
Delivery Goods receipt PO
Return Goods return
A/R invoice A/P invoice
A/R reserve invoice A/P reserve invoice
A/R credit memo A/P credit memo
 Note
Landed costs documents cannot be canceled. Nevertheless, if you manage perpetual inventory, you can achieve the
same result of clearing by creating a new landed costs document fully based on the old one.
This is custom documentation. For more information, please visit SAP Help Portal. 218

6/8/26, 6:04 AM
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
You are still within the time range allowed for cancellation after posting the document.
The time range is determined by your definition of the Max. No. of Days for Canceling Marketing Documents Before or
After Posting field in the Document Settings window. For more information, see Document Settings: General Tab.
Procedure
1. Find the particular document you want to cancel.
2. Right-click in the document window and choose Cancel, or choose Data Cancel . A cancellation document appears
with the title <Document Type> - Cancellation.
3. In the cancellation document window, make the necessary data updates.
 Recommendation
This is custom documentation. For more information, please visit SAP Help Portal. 219

6/8/26, 6:04 AM
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
The due date is automatically updated according to the posting date and payment terms. If there is only one installment,
you can edit the Due Date field directly. If there is more than one installment, you change the due date by changing the
posting date and the installment settings of the payment terms.
Document Date
Remarks
Attachments
After a cancellation document is added, you can edit as much data as for other closed documents of the same document type.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 220

6/8/26, 6:04 AM
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
3. Try to cancel the delivery and add the cancellation document.
The Serial Number Selection window appears. Only serial number x1002 is automatically selected and cannot be
deselected.
4. Create a new serial number or select an available serial number.
You can add the cancellation document now.
Related Information
Cancellation of Documents with Items Stored in Bin Location
This is custom documentation. For more information, please visit SAP Help Portal. 221

6/8/26, 6:04 AM
Cancellation of Documents with Items Stored in Bin Location
If a document contains items stored in bin location, canceling the document follows the rules below:
Bin locations in the existing document are automatically selected for the cancellation document, but you can always change
the bin location allocation method for regular items. For serial number or batch-managed items, you can change the bin
locations only when you are canceling an outbound transaction.
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
You can add the cancellation document now.
Cancellation of Documents Involving Down Payments
This topic deals with the following sales and purchasing documents:
Invoices, including reserve invoices
Credit memos
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 222

6/8/26, 6:04 AM
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
documents are all canceled or,
in the case of correction
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
The base down payment
request has not been drawn to
any invoice or reserve invoice.
Canceling Documents with Fixed Assets
As of SAP Business One 9.0, you can record transactions of fixed assets in marketing documents. You can cancel the marketing
documents with fixed assets shown in the table below. Creating these marketing documents results in the creation of fixed asset
documents. Therefore, when canceling these documents, the corresponding fixed asset documents are also canceled.
This is custom documentation. For more information, please visit SAP Help Portal. 223

6/8/26, 6:04 AM
Marketing Document Fixed Asset Document
A/P invoice Capitalization
A/P credit memo Capitalization credit memo
A/R invoice Retirement
Canceling marketing documents with fixed assets may result in a status change of the fixed assets. For example, if a fixed asset has
been fully retired with an A/R invoice, cancellation of this A/R invoice resets the fixed asset status from Inactive to Active;
and if you made the first acquisition of a fixed asset with an A/P invoice, cancellation of this A/P invoice resets the fixed asset
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
Prerequisites
On the Basic Initialization tab of the Company Details window, you have selected the following checkboxes:
Use Perpetual Inventory
Manage Item Cost per Warehouse
Procedure
1. A FIFO item F001 is received into two different warehouses with different prices (costs).
Warehouse Price Quantity
WH01 USD 5 10
This is custom documentation. For more information, please visit SAP Help Portal. 224

6/8/26, 6:04 AM
| Warehouse | Price | Quantity |     |
| --------- | ----- | -------- | --- |
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
In the Document Settings window, by selecting and deselecting the Display Cancelled and Cancellation Marketing Documents in
Reports checkbox, you can determine whether or not to report cancelled and cancellation documents. However, certain reports are
exempt from the setting of this checkbox: some always report canceled and cancellation documents, and the others never report
canceled and cancellation documents.
  Note
If a canceled document and its cancellation document have different posting dates, especially when the documents are in
different posting periods, you may encounter either of the following situations:
The canceled and cancellation documents are reported separately.
The cancellation document is not reported while the canceled document has already been reported.
This is custom documentation. For more information, please visit SAP Help Portal. 225

6/8/26, 6:04 AM
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
Transaction Report by Projects
Trial Balance
Trial Balance Budget Report
Trial Balance Comparison
Reporting Neither Canceled nor Cancellation Documents
Backorder
Customer Receivables Aging
This is custom documentation. For more information, please visit SAP Help Portal. 226

6/8/26, 6:04 AM
Dunning History Report
Open Items List
Vendor Liabilities Aging
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
This is custom documentation. For more information, please visit SAP Help Portal. 227

6/8/26, 6:04 AM
When you copy one or more base documents to a target document, SAP Business One observes the following rules:
If all base documents have the same value, that value is copied to the target document.
If base values are different, the default value from the business master data is used.
If no default value exists for the business partner, no value is copied to the target document.
More Information
Copying Sales Documents
Copying Purchasing Documents
Copying Sales Documents
Use the information below to copy sales documents.
Copy To Documents
Base Document Target Document
Sales Blanket Agreement Sales Quotation
Sales Order
Delivery
A/R Invoice
A/R Down Payment Request
A/R Down Payment Invoice
Sales Quotation Sales Order
Delivery
A/R Invoice
A/R Reserve Invoice
Sales Order Delivery
A/R Invoice
A/R Reserve Invoice
Delivery A/R Invoice
Return
Return A/R Credit Memo
A/R Invoice A/R Credit Memo
A/R Reserve Invoice Delivery
A/R Credit Memo
Copy From Documents
This is custom documentation. For more information, please visit SAP Help Portal. 228

6/8/26, 6:04 AM
Target Document Base Document
Sales Quotation Blanket Agreement
Sales Order Sales Quotation
Blanket Agreement
Return Delivery
Delivery Sales Quotation
Sales Order
A/R Reserve Invoice
Return
Blanket Agreement
A/R Invoice Sales Quotation
Sales Order
Delivery
Blanket Agreement
A/R Reserve Invoice Sales Quotation
Sales Order
A/R Down Payment Request Sales Quotation
Sales Order
Delivery
Blanket Agreement
A/R Down Payment Invoice Sales Quotation
Sales Order
Delivery
Blanket Agreement
A/R Debit Memo Sales Quotation
Sales Order
Delivery
A/R Credit Memo Return
A/R Invoice
A/R Down Payment
A/R Invoice + Payment Sales Quotation
Sales Order
Delivery
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 229

6/8/26, 6:04 AM
Copying Sales and Purchasing Documents
Return to Open Orders
In real businesses, it is quite common for a company to cancel a delivery or a reserve invoice. And due to certain reasons, such as
receipt of faulty goods or the need for order postponement, the orders need to be reused.
To enable reopening orders, proceed as follows:
1. From the SAP Business One Main Menu, choose Administration System Initialization Document Settings Per
Document .
2. On the Per Document tab, do the following:
For sales orders:
In the Document dropdown list, select the checkbox Sales Order option. Then select the Reopen Doc. By Creating
Returns/Goods Returns/Credit Memos Based on Doc. .
For purchase orders:
In the Document dropdown list, select the checkbox Purchase Order option. Then select the Reopen Doc. By
Creating Returns/Goods Returns/Credit Memos Based on Doc. .
You can decide whether to reopen a sales or purchase order when you create the following:
A return or goods return document that is based on a delivery or goods return PO that is copied from a sales or
purchase order
A credit memo based on an invoice or reserve invoice that is copied from a sales or purchase order
The application prompts you for a decision every time you create a return, goods return, or credit memo.
 Recommendation
If you try to cancel such a return, goods return, or credit memo, you will find that it cannot be canceled. You will see this
message: Cancellation is not possible; base orders reopened.
We recommend that you create a new document from the re-opened sales or purchase order.
3. [Optional] Select the Without User Confirmation checkbox. Sales or purchase orders are always reopened when you create
return or goods return documents that are based on the sales or purchase orders, without prompting a confirmation each
time.
This field is available only if the checkbox Reopen Doc. by Creating Returns/Goods Returns/Credit Memos Based on Doc.
is selected.
For sales orders, if items included were managed by serial numbers or batches, the serial numbers or batches can also be returned
to the sales order when it is reopened. When you credit a reserve invoice, the serial numbers or batches can be returned to the
reopened sales order only when the following conditions are met:
Serial numbers or batches must be originally deallocated from the order due to the creation of the delivery or reserve
invoice that is created based on that sales order.
The reserve invoice that is copied from the sales order must be fully copied to a credit memo.
Example
This is custom documentation. For more information, please visit SAP Help Portal. 230

6/8/26, 6:04 AM
Scenario 1: A fully copied A/R reserve invoice is fully copied to an A/R credit memo
Process
Step Action Quantity Movement S&B Allocation
1 Create a sales order. In the order: open qty=3 S&Bs allocated to the order: S01, S02,
and S03
2 Fully copy the sales order to an A/R In the reserve invoice: open qty=3 S&Bs de-allocated from the order: S01,
reserve invoice. S02, and S03
In the order: open qty=0
3 Fully copy the A/R reserve invoice to an In the credit memo: qty=3 S&Bs de-allocated from the reserve
A/R credit memo. invoice: S01, S02, and S03
In the reserve invoice: open qty=0
In the order: qty=3
Return of S&B:
Serial numbers de-allocated from the sales order: S01, S02, and S03
Serial numbers to be returned (caused by the credit memo): S01, S02, and S03
Serial numbers can be returned: S01, S02, and S03
Result
The sales order is reopened. From the credit memo, 3 quantities are returned; serial number S01, S02, and S03 are returned.
Scenario 2: Manually update serial numbers during the creation of a fully copied A/R reserve invoice; then fully copy it to an
A/R credit memo
Process
Step Action Quantity Movement S&B Allocation
1 Create a sales order. In the order: open qty=3 S&Bs allocated to the order: S01, S02,
and S03
2 Fully copy the sales order to the A/R In the reserve invoice: open qty=3 S&Bs de-allocated from the order: S01,
reserve invoice. S02, and S03
In the order: open qty=0
In the opened A/R reserve invoice, S&Bs allocated to the reserve invoice:
manually update serial number S03 to S01, S02, and S04
S04
3 Fully copy the A/R reserve invoice to an In the credit memo: qty=3 S&Bs de-allocated from the reserve
A/R credit memo. invoice: S01, S02, and S03
In the reserve invoice: open qty=0
In the order: qty=3
Return of S&B:
Serial numbers de-allocated from the sales order: S01, S02, and S03
Serial numbers to be returned (caused by the credit memo): S01, S02, and S04
This is custom documentation. For more information, please visit SAP Help Portal. 231

6/8/26, 6:04 AM
Serial numbers can be returned: S01 and S02
S04 was not originally de-allocated from the sales order, therefore it cannot be returned to the reopened sales order.
Result
The sales order is reopened. From the credit memo, 3 quantities are returned; serial numbers S01 and S02 are returned.
Drop Shipping
Drop shipping entails shipping goods directly from your vendor to your customer without holding the items as inventory in your
warehouses.
A drop ship warehouse does not actually contain items; it is a ʻvirtual’ warehouse. The moment the goods ʻenter’ the drop ship
warehouse, you ship them to your customer.
In order to work with drop shipping in SAP Business One, you must create a drop ship warehouse. For more information, see
Defining Drop-Ship Warehouses. You can use drop ship warehouses to manage serial and batch items as well. SAP Business One
does not record any inventory postings when you use drop ship warehouses in documents.
When you work with a perpetual inventory system, documents in which drop ship warehouses are used create journal entries that
do not reflect the inventory value of the items received or released from a drop ship warehouse.
 Note
When you manage items in a drop ship warehouse, as well as in other warehouses, inventory posting occurs when you
create documents involving the real warehouses.
You cannot use drop ship warehouses for the MRP run.
More Information
Creating Sales and Purchase Orders for Drop Shipping
Creating Sales and Purchase Documents for Drop Shipping
Prerequisites
You have defined at least one warehouse as a drop-ship warehouse.
Context
When you select a drop-ship warehouse in a sales order document, SAP Business One immediately opens a purchase document
for ordering the goods from one of your vendors. Creation of documents involving drop-ship warehouses does not create any
inventory postings.
Procedure
1. From the SAP Business One Main Menu, choose Sales – A/R Sales Order or Sales Quotation.
2. Enter the required customer and item data.
This is custom documentation. For more information, please visit SAP Help Portal. 232

6/8/26, 6:04 AM
3. Select a drop-ship warehouse for one or more of the ordered items.
 Note
Click and add the Whse column if it does not appear in the sales order.
4. Go to the Logistics tab. Select the Procure Drop-Ship Items checkbox to enable creating purchase documents only for
drop-ship items; or select the checkbox Procure Non Drop-Ship Items to enable creating purchase documents for all items
that appear in the sales document and not only for drop-ship items.
5. Add the sales document to the system.
The Procurement Confirmation Wizard window opens.
This window enables the automatic creation of a purchase document based on the sales document that you just added. A
purchase document created using this window can include all or part of the items in the sales document.
If you create a purchase order in this way, it is identical to any purchase order you create in the Purchase Order window.
 Note
You cannot use this window to add items that are not included in base sales orders.
6. For items that you want to include in the purchase order, if the BP Code field is empty, select a vendor from the BP Code
dropdown list. Then, select the item rows and click .
7. To save your changes, choose the Add button.
Results
A purchase document is created; the sales document retains its Open status.
 Note
When you select an item defined as a bill of materials (BOM) in a sales order, the Procurement Confirmation Wizard
window displays the BOM' child items. This applies only to a sales BOM.
When you update a sales order linked to a purchase order that contains a drop-ship warehouse, the following message is
displayed:
Item is linked to a purchase order that has a drop-ship warehouse. Continue?
If you choose Yes, SAP Business One updates the sales order without updating the purchase order.
Every update you make to an existing sales order that has not been linked to a purchase order, opens the Procurement
Confirmation Wizard window, displaying item rows that have not yet been copied to a purchase order.
Related Information
Drop Shipping
Managing Freight Charges
SAP Business One enables you to manage freight so that you can track any additional costs in sales and purchasing transactions.
Freight charges could include insurance, shipment, and other costs that apply to your goods.
You can add freight in the document or row level. When you do, the total amount of the document is updated accordingly. If you
manage your inventory using perpetual inventory, you can add the value of freight charges in purchasing documents to the cost of
This is custom documentation. For more information, please visit SAP Help Portal. 233

6/8/26, 6:04 AM
your goods. In addition, you can define whether the last purchase price of your items includes the freight charges that apply to your
purchased goods.
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
4. The freight is defined as Stock Yes .
5. The standard price of the item and the price in the document are USD 100.
6. The freight amount is USD 10.
Goods Receipt PO
This is custom documentation. For more information, please visit SAP Help Portal. 234

6/8/26, 6:04 AM
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
| G/L Acc./BP Code   | Name               | Debit      | Credit     |
| ------------------ | ------------------ | ---------- | ---------- |
| V6970              | Vendor             |            | USD 110.00 |
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
| G/L Acc./BP Code | Name | Debit | Credit |
| ---------------- | ---- | ----- | ------ |
This is custom documentation. For more information, please visit SAP Help Portal. 235

6/8/26, 6:04 AM
| V6970              | Vendor             |             | USD -110.00 |
| ------------------ | ------------------ | ----------- | ----------- |
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
| G/L Acc./BP Code   | Name              | Debit       | Credit      |
| ------------------ | ----------------- | ----------- | ----------- |
| V6970              | Vendor            |             | USD -100.00 |
| 63500000-01-001-01 | Variance Expenses |             | USD -10.00  |
| 52300000-01-001-01 | Variance 1        | USD -10.00  |             |
| 13500000-01-001-01 | Stock 1           | USD -100.00 |             |
|                    |                   | USD -110.00 | USD -110.00 |
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
This is custom documentation. For more information, please visit SAP Help Portal. 236

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 237

6/8/26, 6:04 AM
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
| Account                  | Debit    | Credit   |     |
| ------------------------ | -------- | -------- | --- |
| Stock in transit account |          | USD 1555 |     |
| Inventory account        | USD 1550 |          |     |
| Price difference account | USD 5    |          |     |
Freight Charges Window
This window displays the freight defined in the Freight - Setup window. It enables you to make changes that are relevant for the
current sales or purchasing document.
To access the window, choose Sales – A/R or Purchasing - A/P and open any document. Click   in the Freight field.
  Note
This window appears only if you have selected Manage Freight in Documents on the General tab of the Document Settings
| window  Administration  |  System Initialization  |  Document Settings | ).  |
| ----------------------- | ----------------------- | ------------------ | --- |
  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Freight Charges Window
Do Not Display Freight Charges with Zero Amount
This is custom documentation. For more information, please visit SAP Help Portal. 238

6/8/26, 6:04 AM
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
When you update the value in the this field, the value in the Gross Amount field is updated automatically according to the
predefined tax group.
This is custom documentation. For more information, please visit SAP Help Portal. 239

6/8/26, 6:04 AM
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
Backorder Processing
You use backorder processing to track customer sales orders received for which the inventory has not yet been shipped. Normally,
this occurs when the available quantity is insufficient to fill the order. The backorder process lets you check how much is missing,
and once the inventory is replenished, you can ship the required quantity to your customers.
When you receive information on a backorder, handle it in one of the following ways:
Deliver the necessary quantity to the customer.
Update the quantity (after the delivery has been shipped).
Close the remaining open quantity for the row.
In addition, you are able to deliver a zero quantity.
Process
The examples below illustrate several typical business scenarios for backorder processing.
Regular Backorder Process
Your customer calls and orders 100 chairs from your company, but you have only 80 chairs in stock. You can deliver the available
items immediately and the remainder when you receive them from your vendor.
1. From the SAP Business One Main Menu, choose Sales - A/R Sales Order .
This is custom documentation. For more information, please visit SAP Help Portal. 240

6/8/26, 6:04 AM
2. Create a new sales order for 100 chairs for the current date. For more information, see Creating Sales Documents.
3. Choose Sales - A/R Delivery .
4. Copy the sales order you just created to the delivery, changing the quantity to 80. For more information, see Draw
Document Wizard.
5. Choose Sales - A/R Sales Reports Backorder . The system displays a backorder for 20 chairs.
6. To enter the 20 items you received from your vendor, choose Purchasing - A/P Goods Receipt PO .
7. Create a new delivery to provide the customer with 20 remaining items. When you run the Backorder report again, you see
that a backorder no longer exists for the customer.
8. Choose Sales - A/R A/R Invoice and issue an A/R invoice for 100 chairs.
 Note
You can update the Quantity and Delivery Date fields for the partially delivered sales order lines.
You can decrease the quantity to the Delivered Qty field level. You can also increase the quantity.
Backorder Process Based on Priority Customer
Your company has a shortage in tables. Two of your biggest customers, Blink and Zeroll, have ordered 100 tables each, but they
have each received only 50 tables so far. Both companies are still waiting for another 50 tables. Finally, you receive 50 more tables.
1. From the SAP Business One Main Menu, choose Sales - A/R Sales Reports Backorder .
This report displays two back orders, each for 50 tables, for your customers Blink and Zeroll.
2. Choose Sales - A/R Delivery .
Since Zeroll is your most important customer, you create a delivery for the 50 tables you received and ship them to Zeroll.
Blink must wait another week for the delivery of 50 additional tables.
Manual Backorder Closure
Zeroll orders 50 tables, 100 chairs, and 40 boards. You have 40 tables, no chairs, and 300 boards in stock. You create a delivery for
40 tables and 40 boards and send it to the customer.
A week later you receive another 50 tables and 100 chairs. Unfortunately, one chair has a defect.
1. From the SAP Business One Main Menu, choose Sales - A/R Delivery .
2. Create a delivery for the 10 tables remaining on the order and 99 chairs, and send it to Zeroll. Following negotiations with
the customer, you decide to cancel the open sales order for one missing chair.
3. To cancel the order for the missing chair, select the line in the sales order and choose Data Close Row .
The delivery is now complete and you can send the A/R invoice for 50 tables, 99 chairs, and 40 boards to Zeroll.
 Note
In some cases, due to item shortages, you cannot deliver an item as planned. To correct this, you enter a zero quantity for that
line in the delivery or A/R invoice. The open quantity then appears in the Open to Ship field.
This is custom documentation. For more information, please visit SAP Help Portal. 241

6/8/26, 6:04 AM
Dunning
Every time goods or services are sold, the liabilities of the respective customer(s) to the business are increased. From that
moment, incoming payments are monitored to ensure that customer debts are paid on time. When they are not, the company
needs to activate a multilevel collection process, such as telephone or written reminders, for the remiss customer.
SAP Business One provides a dunning wizard for producing reminder letters. It runs through all the customers, checks all
outstanding A/R invoices and transactions that represent debt, and enables you to print and send reminder letters of different
levels of severity. In addition, the dunning wizard lets you automatically post service invoices for interest and fees charged with a
dunning letter.
The dunning system covers the following documents:
Open A/R invoices, including invoices that are partially credited or partially paid
Invoices that include installments
A/R credit memos
Incoming payments that are not based on invoices
Manual journal entries with at least one row posted to a customer
Opening and closing balances transactions
To use the dunning wizard, you must first set preliminary definitions.
The following describes the setup of the dunning process and explains the results of running the wizard.
Prerequisites
To run the Dunning Wizard, you have defined:
Dunning interest and dunning fee accounts, on the Sales tab in Administration Setup Financials G/L Account
Determination to be able to automatically post interest or fees using service invoices
Dunning terms, in Administration Setup Business Partners Dunning Terms
Dunning terms are based on dunning levels and contain parameters and values required for the dunning process run.
Default Dunning Term for Customer, on the BP tab in Administration System Initialization General Settings
Dunning terms for customers, in the Dunning Term field on the Payment Terms tab in Business Partners Business
Partner Master Data
You have used the following options to exclude irrelevant A/R invoices from the dunning process:
To exclude a specific invoice:
1. Display the invoice before running the wizard.
2. On the Logistics tab, select Block Dunning Letters.
You can deselect the option later to include the invoice in any future dunning process.
To exclude all invoices created for a specific customer:
1. Display the Business Partner Master Data record for that customer.
2. On the Accounting tab, select Block Dunning Letters.
This is custom documentation. For more information, please visit SAP Help Portal. 242

6/8/26, 6:04 AM
Process
You choose Sales – A/R Dunning Wizard and follow the procedure below. In each step, you choose:
Next, to proceed to the next step of the wizard
Back, to return to the previous step
Cancel, to cancel the dunning wizard creation
1. Step 1: Wizard Options. Select whether to run a new dunning wizard or to load a saved one.
2. Step 2: General Parameters. Modify a name of the default dunning wizard and choose a dunning level.
3. Step 3: Business Partners – Selection Criteria. Choose a range of customer codes for the wizard.
4. Step 4: Document Parameters. Enter the range of the posting or due dates to include in the wizard. In addition, select the
relevant document types and other letter parameters, for example Allow Negative Dunning Letter and Display All Open
Items.
5. Step 5: Recommendation Report. Enter a new date until which payments are expected and select invoices that are included
in the wizard for each customer. Specify whether to automatically post interest or fees and create service invoices for this
purpose.
6. Step 6: Viewing Recommended Service Documents. If you selected automatic posting of interest or fees for the dunning
letters, you can view the recommended service invoices and decide whether to add them.
7. Step 7: Processing. Select one of the following options to process the dunning wizard:
Save Selection Parameters and Exit
Save Recommendation Report as Draft and Exit
Execute Only, Print Later and Exit
Print Dunning Letters and Exit
Result
When you execute the dunning run, the dunning level and the last date of the dunning letter are updated for overdue invoices
included in the dunning run. When you create a dunning letter for a customer, the business partner master data record is updated.
On the Accounting tab, the Dunning Date field displays the date on which the dunning letters were created for the last time.
If you chose to automatically create service invoices for interest or fees, the respective service invoices are created. The summary
report in step 8 of the wizard shows which dunning letters have been created and which errors may have occurred.
To view the history of dunning letters and the list of all invoices, choose Business Partners Business Partners Reports
Dunning History Report .
More Information
Dunning Levels - Setup Window
Dunning Terms - Setup Window
Recurring Transactions
This is custom documentation. For more information, please visit SAP Help Portal. 243

6/8/26, 6:04 AM
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
Filtering Recurring Templates
1. In the Recurring Transactions Templates – Selection Criteria window, specify the start date, end date, business partner
code, business partner group and business partner properties for your desirable templates.
To choose certain document types that you want to include, choose next to Documents to open the Recurring
Templates - Documents Selection window, where you can filter templates by business area and document type.
2. Choose OK.
The application displays the recurring templates according to your filtering criteria.
Creating Recurring Transactions Templates
1. In the Recurring Transactions Templates – Selection Criteria window, choose OK to open the Recurring Transactions –
Templates window.
2. In the Template column, enter a name for the template you want to create.
3. In the Type column, specify the document type for the transaction, for example, purchase order, A/R invoice, or goods
issue.
This is custom documentation. For more information, please visit SAP Help Portal. 244

6/8/26, 6:04 AM
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
| Transaction to be posted once per | Quarterly | N/A |
| --------------------------------- | --------- | --- |
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
This is custom documentation. For more information, please visit SAP Help Portal. 245

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 246

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 247

6/8/26, 6:04 AM
1. Choose next to Templates.
2. The Recurring Transactions – Templates window appears.
For more information, see Managing Recurring Transactions Templates.
Related Information
Managing Recurring Transactions Templates
Document Generation Wizard
The document generation wizard enables you to perform batch processing of target sales documents. The wizard recommends a
simple way to include rows from several base documents in a single target document, according to the parameters you define.
Some target documents, such as A/R invoices and deliveries, cannot be deleted or changed after you create them.
 Note
The document generation wizard lets you save the defined parameter set. First, you enter and save numerous parameters for
base and target documents. Based on these definitions, you can select consolidation methods and choose a list of relevant
business partners.
Once you save the defined parameter set, you can run the wizard periodically according to your company’s business practices.
 Note
The document generation wizard does not support All currency business partners.
More Information
Running Document Generation Wizard
Running the Document Generation Wizard
The wizard guides you step-by-step through the definition of parameters required to generate the documents.
Procedure
From the SAP Business One Main Menu, choose Sales – A/R Document Generation Wizard and follow the steps below:
This is custom documentation. For more information, please visit SAP Help Portal. 248

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
More Information
Document Generation Wizard
Step 1: Starting the Wizard
Use the Document Generation Options page to define whether to generate the wizard for target documents according to an
existing parameter set or a new parameter set.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Generation Options Fields
This is custom documentation. For more information, please visit SAP Help Portal. 249

6/8/26, 6:04 AM
New Parameter Set
Select to define new parameters for the wizard run.
Existing Parameter Set
Select this option to load predefined parameters.
When you run the wizard for the first time, this option is disabled.
Set Name
Enter the name for a new parameter set to identify it later.
Set Description
Enter the description for a new parameter set.
Last Modified
Date on which you last modified the parameter set.
This field appears only if you have selected Existing Parameter Set.
More Information
Document Generation Wizard
Step 2: Specifying Target Document
Use the Target Document page to specify the document type and the characteristics of the target documents.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Target Document Fields
Target Document
Specify a target document type by clicking and choosing one of the following:
Sales Order
Delivery
Returns
A/R Invoice
 Note
In each wizard run, you can choose only one target document type.
Branch
Select a branch for which you want to run the document generation wizard.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 250

6/8/26, 6:04 AM
This field is available only if you have enabled multiple branches.
Posting Date
Enter the posting date on which the target document will be created.
By default, this field displays the current date.
Document Date
Specify the document creation date of the target document.
By default, this field displays the current date.
Series
The series of the document type.
The value appears after you choose the document type. If required, you can change the series.
Items
Determines the type of target rows that will consolidate the base rows.
To choose one of the summary display options, click .
Service
Determines the type of target rows that will consolidate the base rows.
To choose one of the summary display options, click .
Exchange Rate
Select a method for setting the exchange rate of the target rows.
Reopen Items in the Original Sales Order
Reopens the item quantities in the sales order on which the document is based.
Selecting this checkbox produces the following results:
The base document status changes to Open.
The row status changes to Open.
The open quantity is increased by the quantity specified in the return.
The delivered quantity is decreased by the quantity specified in the return.
For service type transactions, the open amount is increased accordingly by a value equal to the value from a return line. If
the sum of the remaining open amount plus the returned amount is greater than the total amount for the original order line,
the total amount is used as the open amount.
If there are any freight charges related to the returned or credited item, these charges are reopened in the same way as the
item quantities.
If the item is managed by batches, the returned batch-allocated quantity is increased by the quantity from the return line.
This checkbox is available only if the field Enable Reopening of Orders When Creating Returns Based on Orders on the Per
Document tab in the Document Settings window is selected.
Include Manually Closed or Canceled Sales Order Lines or Documents
This is custom documentation. For more information, please visit SAP Help Portal. 251

6/8/26, 6:04 AM
To reopen the item quantities in sales order lines that were manually closed or canceled, select this checkbox.
This checkbox is available only if the Reopen Items in the Original Sales Order field is selected.
Create Draft Documents
Saves target documents as drafts.
 Note
When you run the wizard for an existing parameter set, the posting and document dates always display the current date. If the
parameter set includes other dates related to the selection criteria of base documents, change those dates for the current
parameter run.
More Information
Document Generation Wizard
Step 3: Defining Base Documents
Use the Base Documents page to define base documents that you want to process. Choose the appropriate document types and
other selection criteria.
SAP Business One always selects base documents according to all the criteria defined in the general area and on the Logistics and
Accounting tabs of each document.
 Note
If you create an invoice or delivery based on a sales order with batch-managed items, you must allocate batch numbers for the
entire quantity of the batch-managed items.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Base Document Fields
Doc. Types
Displays the list of document types you can choose as base documents.
The list depends on your selection of a target document in the Target Document window.
 Example
Choosing Delivery as a target document displays Sales Quotations, Sales Orders, and A/R Reserve Invoice as the base
document types.
Posting Date
Specify a range of the posting dates to include in the wizard run.
Delivery Date
Specify a range of the delivery dates to include in the wizard run.
This is custom documentation. For more information, please visit SAP Help Portal. 252

6/8/26, 6:04 AM
Series
If you selected one document only, displays the series of the base document.
If required, you can change the value. If you selected more than one document type, the field is disabled.
Allow Partial Delivery
Creates target documents based on sales orders that allow partial delivery.
This option is available if the following applies:
Sales order was selected as a base document
Either the Block Release field and/or the Block Negative Inventory field is selected in Administration System
Initialization Document Settings General . If neither of these fields is selected, inventory can go below the minimum
level and partial deliveries are irrelevant.
Expanded Selection Criteria
Displays additional selection fields.
SAP Business One copies base documents that match the additional selection criteria to target documents. No matter how many
of the expanded selection criteria you choose, the selected base documents match each of the criteria.
Ignore Quotations with Alternative Items
Wizard disregards sales quotations with alternative items during the document generation wizard run.
If you do not select the checkbox, the wizard includes sales quotations but not the alternative items.
 Note
This field appears only if you selected sales quotations.
Sort by
Select the fields according to which the document generation wizard processes documents that are considered in the run. You can
select up to three sorting parameters and their sorting order.
 Example
You choose the following sorting parameters:
1. Due Date
2. Posting Date
3. Document Amount
The application first arranges the documents according to their due date; then, within a specific due date, it sorts according to
the posting date; and finally, within a specific posting date, it sorts by the document amount value.
 Note
The document generation wizard copies text lines to the target document.
The subtotal lines are copied when you select the No Consolidation checkbox, or when one base document is copied to the
target document, regardless of the setting of the No Consolidation checkbox.
Moreover, if you have partially copied the document before the wizard run, the subtotal lines are not copied when:
This is custom documentation. For more information, please visit SAP Help Portal. 253

6/8/26, 6:04 AM
No items exist above the first summary level
No lower level subtotals exist above the higher level
 Note
If you have a sales order with batch allocation details, it will not be included in the document generation wizard run.
More Information
Document Generation Wizard
Step 4: Defining Consolidation Criteria
Use the Consolidation Options page to define the criteria for consolidating base documents into target documents. You may also
choose to create one target document for each base document, rather than consolidating.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Consolidation Options Fields
Consolidate By
Select to consolidate base documents into target documents.
System Defaults
By default, appears selected.
The application consolidates all base rows with the same system defaults into the target document. The system defaults are:
Same customer
Same base document type
Same item or service type
Sort by criteria
Same document price mode
Ship-to Address
Consolidates all base rows with the same Ship-to Address entry into one target document.
Payment Terms
Consolidates all base documents with the same payment terms into one target document.
If you do not select this parameter, the application consolidates base documents with different payment terms into one target
document. In this document, the payment terms are those that you have defined for the customer (see Business Partners
Business Partner Master Data Payment Terms ).
Payment Method
This is custom documentation. For more information, please visit SAP Help Portal. 254

6/8/26, 6:04 AM
Consolidates all base documents with the same payment method into one target document.
If you do not select this parameter, the system consolidates base documents with different payment methods into one target
document. In this document, the payment method is the one that you have defined as default for the customer (see Business
Partners Business Partner Master Data Payment System ).
Expanded Consolidation Options
Select additional selection criteria for the marketing documents that you use to consolidate target documents.
No Consolidation
Select this option to create one target document for each base document.
Consider Customer Sequence
If you select this option, the application arranges the documents by business partner number and then within each business
partner number, according to the Sort by criteria specified in step 3 of the document generation wizard.
If you do not select this option, the application arranges the documents according to the Sort by criteria.
If you select both this option and Consider Base Doc Type, the application arranges the documents first according to business
partner, then according to document type, and finally according to the Sort by criteria.
Consider Base Doc Type
If you select this option, the application arranges the documents by a base document type sequence and then within each base
document type, according to the Sort by criteria specified in step 3 of the document generation wizard.
If you do not select this option, the application arranges the documents according to the Sort by criteria.
If you select both this option and Consider Customer Sequence, the system arranges the documents first according to business
partner, finally according to document type, and then according to the Sort by criteria.
More Information
Document Generation Wizard
Step 5: Selecting Customers
Use the Customers page to select those customers for whom you want to perform a summary.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Customers Fields
Control Account
Specify the control account for the A/R invoice.
 Note
This field appears only when you select an A/R invoice as the target document for the wizard run.
Add Customers
This is custom documentation. For more information, please visit SAP Help Portal. 255

6/8/26, 6:04 AM
Displays the Business Partner – Selection Criteria window, where you can enter the range of business partners to include in the
document generation wizard.
[]
Includes the customers for whom you run the wizard.
 Note
If you work with a consolidating business partner, the document generation wizard includes it in the run. As such, all
consolidated business partner transactions are included in the wizard run.
If the consolidated business partner is not included in the selection criteria, the transactions are included in the original
business partner run.
For example, if Blink is a consolidating business partner of Zerol, the document generation wizard includes the relevant
documents of Zerol in the run for Blink.
More Information
Document Generation Wizard
Step 6: Defining Messages and Alerts
Use the Messages and Alerts page to define how SAP Business One responds to missing data, bookkeeping, or inventory.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Messages and Alerts Fields
Missing Data
Select a response to missing data, such as the exchange rate:
Skip to Next Document – proceed with the same business partner but skip the current document.
Skip to Next Customer – skip the current customer and proceed to the next one. This option is available only if you
selected No Consolidation and did not select Consider Customer Sequence in step 4 of the document generation wizard.
Ask for User Confirmation – request user confirmation before proceeding.
Bookkeeping
Select a response to bookkeeping alerts such as Deviation from credit limit:
Skip to Next Document – proceed with the same business partner but skip the current document.
Skip to Next Customer – skip the current customer and proceed to the next one. This option is available only if you
selected No Consolidation and did not select Consider Customer Sequence in step 4 of the document generation wizard.
Ask for User Confirmation – request user confirmation before proceeding.
Inventory
This is custom documentation. For more information, please visit SAP Help Portal. 256

6/8/26, 6:04 AM
Select a response for inventory alerts, such as Releasing inventory below the minimum level:
Skip to Next Document – proceed with the same business partner but skip the current document.
Skip to Next Customer – skip the current customer and proceed to the next one. This option is available only if you
selected No Consolidation and did not select Consider Customer Sequence in step 4 of the document generation wizard.
Ask for User Confirmation – request user confirmation before proceeding.
More Information
Document Generation Wizard
Step 7: Saving and Executing the Wizard
Use the Save & Execute Options page to do one of the following:
Execute the wizard.
Save the parameters you have set, and execute the wizard.
Save the parameters for a future run, and exit.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Save & Execute Options Fields
Execute
Executes the document generation wizard.
Save Parameter Set & Execute
Saves the parameter set before you execute the wizard.
Enter a name and description for the parameter set. If you defined the set name and description in step 1, they appear by default.
Save Parameter Set and Exit
Saves the parameter set for a future run and exits the wizard.
Set Name
For a new parameter set, displays the name of the parameter set, if you defined it in step 1. You can overwrite the existing name. If
you enter an existing parameter set name, an error message appears.
For an existing parameter set, if you have updated the steps of the wizard, SAP Business One updates the wizard and saves it under
the existing name without displaying an error message.
Description
Enter meaningful text about the parameter set.
 Caution
If you select Execute or Save Parameter Set & Execute, the following system message appears:
This is custom documentation. For more information, please visit SAP Help Portal. 257

6/8/26, 6:04 AM
It is recommended to back up the company data before performing this operation. Continue?
To generate the target documents and to move to the next step, choose Yes.
To remain in the current window, choose No.
More Information
Document Generation Wizard
Step 8: Displaying Summary Report
Use the Summary Report page to view the summary of target documents created per customer, as well as error and warning
messages.
Summary Report
Message
Displays messages in the following format:
Target document name and number (target document numerator) –
No. of base documents which have been consolidated: Number (base document numerator)
 Example
A/R Invoices No. 44 – 2 Sales Order(s) consolidate: 16, 17
Errors, Warnings
Either includes or excludes errors and warnings from the document generation wizard summary report.
SAP Business One creates a different row for each target document.
If you choose Save Parameter Set & Execute in step 7, the following remark appears at the top of the message list:
Your Parameter Set was Saved Successfully.
In case of failure, the following message appears: Your Parameter Set was not Saved.
If an approval process is required for the document, the following message appears:
Draft document number X was created. Request for approval was sent.
More Information
Document Generation Wizard
Draw Document Wizard
Context
The draw document wizard enables you to create a new document from an existing one by guiding you step by step through the
process. It provides different options for customization and for altering data based on the target document you are creating and
This is custom documentation. For more information, please visit SAP Help Portal. 258

6/8/26, 6:04 AM
the source document you are using. For example, you can choose which exchange rate to apply or whether to also draw freight
charges and withholding tax values from a base document to the target document.
Procedure
1. To go to the draw document wizard, from the SAP Business One Main Menu, choose either Sales A/R or Purchasing A/P.
2. Select the marketing document you want to create and specify the business partner code.
3. Choose Copy From and select a document type to draw.
The List of [document type] window of the selected document type appears. It displays the documents that can be drawn.
 Note
Every marketing document allows drawing only specific document types. For example, you can draw only sales
quotations to sales orders, and only deliveries to returns.
4. Select the document or documents to draw and choose the Choose button.
5. In the Draw Document Wizard window, select the required criteria.
If you selected Draw all Data (Freight and Withholding Tax), choose the Finish button and go to step 11. If you selected
Customize, choose the Next button.
The rows included in the chosen base documents appear.
6. Choose the items you want to draw and make the necessary changes to the rows, quantities, or prices, if any.
If required, select Display BP Catalog Number.
7. If the drawn items are included in documents with freight, choose the Next button. Otherwise, choose the Finish button and
go to step 11.
The Select Freight Charges to Copy window appears.
8. Make the required selection and, if the base document includes withholding tax, choose the Next button. Otherwise, choose
the Finish button and go to step 11.
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
This is custom documentation. For more information, please visit SAP Help Portal. 259

6/8/26, 6:04 AM
If a document is partially drawn, the quantities (for an items type document), freight charges, and withholding tax values in the
base document are updated respectively. In that case, when you decide to copy the base document again, the original values are
replaced by the open quantities (for an items type document), freight charges, and withholding tax amounts.
Draw Document Wizard Window
When you create a sales or purchasing document based on existing documents, SAP Business One opens the Draw Document
Wizard window where you can define factors that affect the document you create.
 Note
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
This window displays the withholding tax amounts involved in the base documents drawn by the wizard. If required, you can change
the amount displayed.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Select Withholding Tax Line to Copy
Base Document
Number of the base document.
Withholding Tax Code
Code of the withholding tax defined for the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 260

6/8/26, 6:04 AM
Taxable Value
The drawn taxable amount.
Withholding Tax Value
Withholding tax amount calculated for the taxable value; editable.
 Note
You cannot enter an amount larger than the total withholding tax amount included in the base document.
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
This is custom documentation. For more information, please visit SAP Help Portal. 261

6/8/26, 6:04 AM
Base Document
Number of the base document.
Amount
Sum of the expenses, calculated according to the set definitions.
If required, you can change the amount.
 Note
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
This is custom documentation. For more information, please visit SAP Help Portal. 262

6/8/26, 6:04 AM
1. Select the document you want to save as a draft.
2. Specify all required data.
3. To save the document draft, use one of the following options:
In the menu bar, choose File Save as Draft or right-click in the document window and choose Save as Draft.
Sale and purchasing documents:
Choose the Add Draft & New option in the document window. This option saves the document draft and
opens a new document in Add mode.
Using the dropdown, choose the Add Draft & View option in the document window. This option saves the
document draft and opens the draft in View mode.
Example
A customer phones to order certain items. During the conversation, you enter the sales order in SAP Business One. If, however, the
customer does not reach a final decision on whether to issue the order, you cannot add it. You save the order as a draft and process
it when the customer has decided to purchase the items.
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
This is custom documentation. For more information, please visit SAP Help Portal. 263

6/8/26, 6:04 AM
Choose Inventory Inventory Reports Document Drafts Report . In the Document Drafts – Selection Criteria
window, specify the required parameters and choose OK.
2. Double-click the required draft.
The document window appears in the Add mode.
3. Make any necessary changes and choose Add.
 Note
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
This is custom documentation. For more information, please visit SAP Help Portal. 264

6/8/26, 6:04 AM
Select the user name for which you want to display drafts.
Open Only
If you select this checkbox, the report displays only the drafts that have not been added yet as original documents in SAP Business
One.
If you do not select this checkbox, the report displays all drafts that have been created, including those that are still pending.
Sales - A/R
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
2. If approval isn’t required, you use the Save as Draft function to save the target document. If approval is required, the system
automatically creates a draft after you add the document, pending approval.
3. You (or another user) use the Copy To or Copy From function to copy the same base documents to another target
document again.
4. You (or another user) try to add the target document, save the target document as a draft again, or add the target
document for approval again.
Before making your decision, you can open this window to view details of the existing drafts using the provided draft numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 265

6/8/26, 6:04 AM
Dunning Wizard
The dunning wizard enables you to create and send letters to customers that have not paid their debts before a specific due date
and to remind them of their overdue payments. It allows you to automatically post service invoices for interest or fees charged with
each dunning letter.
In addition, the dunning wizard keeps track of a customer’s "payment behavior" in the database to deliver this important
information to appropriate organizations.
The dunning wizard considers the following transactions and documents:
Open A/R invoices (including partially paid and partially credited)
A/R credit memos
Manual journal entries with at least one row posted to a customer
Opening and closing balance transactions
Incoming payments that are not based on invoices
Prerequisites
You have set up dunning levels and dunning terms in the Dunning Levels - Setup Window and the Dunning Terms - Setup Window.
Procedures
To access the wizard, choose Sales – A/R Dunning Wizard . Here, you'll find the following steps to guide you through the
process:
Please note that image maps are not interactive in PDF outputs.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 266

6/8/26, 6:04 AM
You can remove dunning wizards with status "Saved Parameters" or "Saved Recommendations" via the right-click menu or
Data Remove in the menu bar.
More Information
Dunning
Step 1: Starting the Wizard
On the Wizard Options page, select whether to run a saved wizard or to create a new one.
To access the window, choose Sales – A/R Dunning Wizard .
Wizard Options Fields
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Start a New Dunning Run or Load a Saved Dunning Run
Select whether to start entering data to execute a wizard run according to a new parameter set, or to run a previously saved wizard.
Find
Locate a saved dunning run. Enter a full or partial name. SAP Business One displays the first dunning run that fits the search
parameters.
Dunning Name
Name of the saved dunning run.
Date
Creation date of the saved dunning run.
Status
Status of the dunning run:
Saved Parameters – you have not executed the dunning run and SAP Business One has not created the recommendation
report yet.
Recommended – SAP Business One has created the recommendation report but has not executed the dunning run. The
system saves it as a draft.
Partially Executed, Not Yet Printed – SAP Business One has saved the dunning run and created dunning letters. However, it
failed to create service invoices that were supposed to be created to post interest and/or fees automatically, and did not
print the dunning letters.
Executed, Not Yet Printed Wizard – SAP Business One has executed the dunning run, but not yet printed the dunning
letters. It created service invoices that were supposed to be created to post interest and/or fees automatically.
Executed and Printed – SAP Business One has executed the dunning run and printed the dunning letters. It created service
invoices that were supposed to be created to post interest and/or fees automatically.
This is custom documentation. For more information, please visit SAP Help Portal. 267

6/8/26, 6:04 AM
More Information
Dunning Wizard
Step 2: Defining General Parameters
Use the General Parameters page to modify the dunning name and define the dunning level.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Parameters Fields
Dunning Name
By default, displays the dunning name calculated according to the formula: Wiz+system date+successive number. Change
the name if required.
Date of Dunning Run
By default, displays the read-only current date.
Dunning Level
Specify one particular dunning level or All.
Dunning Term
Specify one particular dunning term or All. The terms available are taken from the Dunning Terms – Setup window.
If you select All, all business partners can be included in the run, provided that a dunning term is assigned to them and there is
some open document to be displayed.
If you select a particular dunning term, only business partners with this dunning term assigned to them are included in the dunning
run.
More Information
Dunning Wizard
Step 3: Specifying Customers
Use the Business Partner - Selection Criteria page to specify the range of customers to include in the dunning run.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Business Partner Selection Criteria Fields
Customer Code
This is custom documentation. For more information, please visit SAP Help Portal. 268

6/8/26, 6:04 AM
Code of a customer included in the dunning wizard run.
Customer Name
Displays the name of a customer included in the dunning wizard run.
BP Balance (FC)
Current balance for the business partner in foreign currency.
BP Balance (LC)
Current balance for the business partner in local currency.
Clear Table
Removes the business partner selections for the dunning run.
Add
Choose Add to display the BP Properties window and enter the range of the business partners to include in the dunning wizard.
Include Customers with Credit or Zero Balance
Includes customers whose balance is not negative. Such customers might have unpaid or partially paid A/R Invoices and other
open transactions that reflect existing debts.
Consider Connected Vendors
If a customer is also a vendor and you have connected the related vendor record to the customer from the Business Partner Master
Data Accounting Tab, General sub-tab, you can use this option to display the transactions and documents posted to the connected
vendor in the recommendation report in Step 5 of this dunning wizard.
By comparing the transactions and documents posted to the selected customers and their connected vendors in the
recommendation report, you can better decide if a dunning letter is required.
 Note
If you select a particular dunning term in Step 2, only business partners with this dunning term assigned to them can be added
to the list of selected business partners.
More Information
Dunning Wizard
Step 4: Defining Document Parameters
Use the Document Parameters page to specify the range of invoice posting dates and to define the document types.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Parameters Fields
Posting Date From... To...
This is custom documentation. For more information, please visit SAP Help Portal. 269

6/8/26, 6:04 AM
By default displays the current dates. However, you can enter a different date range to include in the dunning wizard.
Due Date From... To...
Select the documents to include in the dunning wizard by entering a specific due date or a due date range.
Include Payments Not Based on Invoices
Includes payments that are not based on invoices.
Include Credit Memos Not Based on Invoices
Includes credit memos that are not based on invoices.
Include Manual Journal Entries
The dunning wizard run considers manual journal entries created for the selected customers. Journal entries originating from JE
(created via the Journal Entry and Journal Vouchers windows), OB, and CB (created via Opening Balances or Period End Closing
functions) are considered as manual journal entries by the dunning wizard. If the customer is debited (or credited with negative
amount) in the manual journal entry, this journal entry is considered in the dunning wizard run as an A/R invoice. If the customer is
credited (or debited with negative amount) in the journal entry, this journal entry is considered as A/R credit memo.
 Note
If the option Block Dunning Letters (in the Form Settings - Journal Entry window) is selected for a specific manual journal
entry, this journal entry is not considered by the dunning wizard run, even if the customer for whom it was created is included in
the dunning wizard run.
Allow Negative Dunning Letter
Specify whether the application should generate a dunning letter if negative document amounts exceed positive ones.
Display All Open Items
Includes invoices and manual journal entries of type invoice that are not yet eligible for a new dunning letter (at a higher dunning
level) or any dunning letter. When you choose this option, the dunning letter shows all open invoices, irrespective of their due date,
that have not been paid, credited, or reconciled. This field is enabled and visible only if you selected All in the Dunning Level field in
step 2 of the dunning wizard.
Enable Quick Load
When there are too many records, the dunning wizard may be quite slow to load the recommendation report in step 5. Select this
checkbox to load the recommendation report faster.
Note that when you select this checkbox, the following happens:
The BoE information does not appear in the recommendation report.
The folio numbers do not appear in the recommendation report.
The collapse and expand functions are disabled in the recommendation report.
You cannot print the recommendation report using the corresponding Crystal Reports layouts.
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
More Information
Dunning Wizard
This is custom documentation. For more information, please visit SAP Help Portal. 270

6/8/26, 6:04 AM
Step 5: Choosing from Recommendation Report
The Recommendation Report page lists the transactions and documents, grouped by customers, for which SAP Business One
recommends creating dunning letters. You can select the customers and documents to be included in the dunning run.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Recommendation Report Fields
Time
The exact time you displayed the Recommendation Report.
Transactions and/or documents that comply with the specified parameters, but were posted after the displayed time, are not
included in the recommendation report, and therefore will not be dunned in this run.
User
The name of the user who initiated the dunning wizard run.
Include Payments Up To
Specify a date that informs customers up until when payments were last recorded in the application. Customers who have made
payments after this date will know that they can disregard the dunning letter.
 Example
An SAP Business One user runs the dunning wizard on Monday morning, August 16, 2010. However, payments received during
the weekend have not been entered in the application yet. The customer receiving the reminder is informed that the payment
made during the weekend is not yet applied and the dunning letter can therefore be disregarded.
New Due Date
Date to be displayed on printed dunning letter informing customer by when the company expects the payment for outstanding
items. This date is not copied to displayed invoices or manual journal entries of type invoice.
Customer Code
The codes of the selected customers. Use the Expand/Collapse icon to view the documents and/or transactions related to a
specific customer.
Letter No.
The successive numbers of the dunning letters that are recommended for a specific customer. Use the Expand/Collapse icon to
view the list of transactions and/or documents included in each letter.
Level
Dunning level associated with the respective document and/or transaction. If required, you can change this value up to the level
defined in the dunning term assigned to the customer.
Doc. No.
The document type, document number, and the specific row number in the document to which the dunning run is applied.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 271

6/8/26, 6:04 AM
The value IN 172/1 indicates that the dunning run is applied to A/R invoice no. 172, row number 1 in the journal entry created by
the A/R invoice. This row is the one that is posted to the customer.
 Note
If the document type is JE (manual journal entry), OB (opening balance), or BC (closing balance), the row numbering starts with
0 and not with 1. So the value JE 285/0 would represent the first row in journal entry no. 285.
Due Date
The due date of each document or transaction to be dunned in this dunning run. If you specified a different due date in the New
Due Date field, the new date is considered in the dunning run.
Last Dunning Date
Date of the last dunning run, if a transaction or document was included in a previous dunning run.
Document Amount (FC)
Relevant only for foreign currency documents.
The original total amount of the document or the journal entry in foreign currency (FC). Negative amounts represent transactions
in which the customer is credited (such as incoming payments).
Document Amount (LC)
The original total amount of the document or the journal entry in local currency (LC). Negative amounts represent transactions in
which the customer is credited (such as incoming payments).
When you enter a local currency amount, the foreign currency is not calculated accordingly.
Open Amount (FC)
Relevant only for foreign currency documents.
The amount of the document or transaction that is not yet paid, credited, or reconciled in foreign currency (FC). This is the amount
to be dunned in this dunning run. Negative amounts represent transactions that credit the customer (such as A/R credit memos).
These transactions are not dunned.
Open Amount (LC)
The amount of the document or transaction that is not yet paid, credited, or reconciled in local currency (LC). This is the amount to
be dunned in this dunning run. Negative amounts represent transactions that credit the customer (such as A/R credit memos).
These transactions are not dunned.
When you enter a local currency amount, the foreign currency is not calculated accordingly.
Interest Days
The number of days for which interest is calculated. You can change this value if required.
The days are counted from the due date of the document or transaction, and based on the number of days in one month as defined
in the Dunning Terms - Setup window.
Interest %
The interest rate for the dunning period. The calculation is based on a formula comprising the annual interest rate and the number
of interest days in the year as defined in the Dunning Terms - Setup window.
 Example
Number of days in year: 360
This is custom documentation. For more information, please visit SAP Help Portal. 272

6/8/26, 6:04 AM
Annual interest rate: 14%
Interest days: 53
Interest % = (Interest days X Annual interest rate)/number of days in year
(53X14%)/360=2.06%
Interest Amount (FC)
The interest amount in foreign currency (FC) calculated for this document or transaction. The calculation is based on the
definitions made in the Dunning Levels - Setup and Dunning Terms - Setup windows. If required, you can change the amount.
When you enter a foreign currency amount, the local currency is calculated accordingly.
Interest Amount (LC)
The interest amount in local currency (LC) calculated for this document or transaction. The calculation is based on the definitions
made in the Dunning Levels - Setup and Dunning Terms - Setup windows. If required, you can change the amount.
When you enter a local currency amount, the foreign currency is not calculated accordingly.
Total incl. Interest (FC)
The total amount to be dunned per document or transaction, including the interest amount, if it exists, in foreign currency (FC). You
can change this value if required. When you change the foreign currency amount, the local currency is calculated accordingly.
In the letter row, the total amount to be dunned with this letter (from all the transactions and/or documents), including the interest
amounts for each document or transaction. If you change the total or interest amount of a specific transaction/document, the total
of the letter is updated accordingly.
Total incl. Interest (LC)
The total amount to be dunned per document or transaction, including the interest amount, if it exists, in local currency (LC). You
can change this value if required. When you change the local currency amount, the foreign currency is not calculated accordingly.
In the letter row, the total amount to be dunned with this letter (from all the transactions and/or documents), including the interest
amounts for each document or transaction. If you change the total or interest amount of a specific transaction/document, the total
of the letter is updated accordingly.
Fee (FC)
The fee per letter in foreign currency (FC), as defined in the Dunning Terms - Setup window. If you change this amount, the new fee
is applicable for the current letter only. When you enter a foreign currency amount, the local currency is calculated accordingly.
Fee (LC)
The fee per letter in local currency (LC), as defined in the Dunning Terms - Setup window. If you change this amount, the new fee is
applicable for the current letter only. When you enter a local currency amount, the foreign currency is not calculated accordingly.
Overall Total (FC)
The total amount per letter in foreign currency (FC), including the interest and fee.
Overall Total (LC)
The total amount per letter in local currency (LC), including the interest and fee.
Auto Posting
Indicates whether interest and fee, interest only, fee only, or neither of the two is posted automatically when executing the dunning
run and creating dunning letters. The default value is taken from the business partner master data. You can change the setting, if
required.
This is custom documentation. For more information, please visit SAP Help Portal. 273

6/8/26, 6:04 AM
More Information
Dunning Wizard
Step 6: Viewing Recommended Service Documents
Use the Recommended Service Documents page to view the details of the service invoices and decide if you want to add them.
Each line represents one dunning letter according to the previous step of the wizard. The window appears only if service invoices
for interest and/or fees are recommended by the dunning wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Recommended Service Documents Fields
Execution Date
Date on which the dunning takes place.
Posting Date
Specify the posting date. The default value for this field is the date on which the service invoice is created. If required, change the
date.
Due Date
Specify the due date of the service invoice.
Document Date
Specify the document date which is used for tax purposes. If required, change the date.
Series
Specify a numbering series for the service invoice.
Project
Specify the project to which you want to attribute the service invoice.
Distr. Rule
Specify the distribution rule according to which the service invoices will be allocated to cost centers.
Interest Tax Code
Specify the code of the tax to be applied to the dunning interest for all recommended service invoices. If necessary, you can specify
a different tax code for individual service invoices in the table below.
Fee Tax Code
Specify the code of the tax to be applied to dunning fees for all recommended service invoices. If necessary, you can specify a
different tax code for individual service invoices in the table below.
Auto. Remarks
If you select this checkbox, the Remarks field in the service invoice is updated with the dunning name and dunning letter number.
This is custom documentation. For more information, please visit SAP Help Portal. 274

6/8/26, 6:04 AM
If you deselect this checkbox, the Remarks field remains empty or you can specify your own text that should appear on the service
invoice.
Add
If you select this checkbox, service invoices for the interest and fee amounts will be added during the dunning run.
Doc. No.
Number of the service invoice that is created when the wizard is executed successfully.
Letter No.
The successive numbers of the dunning letters that are recommended for a specific customer.
Interest Tax Code
Specify the code of the tax to be applied to the dunning interest for a particular service invoice.
 Note
If you do not specify a tax code, the wizard will fail and no service invoices will be created.
Fee Tax Code
Specify the code of the tax to be applied to the dunning fee for a particular service invoice.
 Note
If you do not specify a tax code, the wizard will fail and no service invoices will be created.
More Information
Dunning Wizard
Step 7: Processing the Wizard
Use the Processing page to select an option for processing the dunning wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Processing Fields
Save Selection Parameter and Exit
Saves the selection parameters but not the recommendation report. It is possible that the next time you run the dunning wizard,
the recommendation report will be different due to new or paid invoices.
Save Recommendation Report as Draft and Exit
Creates dunning letters based on a specific recommendation report in the future. In addition, invoices, credit memos and
payments included in will not be covered by other dunning runs. You can cancel the saved recommendation report.
Execute Only and Exit. Print or E-Mail Later
Executes and exits the dunning run for all selected customers and documents.
This is custom documentation. For more information, please visit SAP Help Portal. 275

6/8/26, 6:04 AM
If in the previous steps you chose to automatically post interest or fees by creating service invoices, the following system message
appears: Service invoices will be added. Do you want to continue? If you choose Yes, the wizard is executed.
If you choose No, the wizard is not executed and you can go back to step 6 and select not to post the service invoices.
The dunning level and the last dunning run date are updated for invoices included in the dunning run, unless the invoices were
included only as a consequence of your having selected Display All Open Items.
When you select this option and the wizard is executed successfully, the run is set to status Executed, Not Yet Printed. If the
wizard fails, for example, if service invoices could not be created due to missing tax codes, the run is set to status Partially
Executed, Not Yet Printed. In this case, no dunning letters are created and the dunning level and last dunning date information is
not updated. You can then load and execute the wizard again after you make the necessary amendments in the wizard (that is, you
specify the tax codes or select not to automatically post service invoices for fees or interest).
When a dunning letter is created for a customer, the business partner master data record is updated. On the Accounting tab, the
Dunning Date field displays the date on which the dunning letters were created for the last time.
You can print the dunning letters at a later time. To do so, the next time you access the dunning wizard, choose the option
Executed, Not Yet Printed in step 1.
Print Dunning Letters and Exit
Executes, prints, and exits the dunning run for all selected customers and documents.
If in the previous steps you chose to automatically post interest or fees by creating service invoices, the following system message
appears: Service invoices will be added. Do you want to continue? If you choose Yes, the wizard is executed.
If you choose No, the wizard is not executed and you can go back to step 6 and select not to post the service invoices.
The dunning level and the last dunning run date are updated for invoices included in the dunning run, unless the invoices were
included only as a consequence of your having selected Display All Open Items.
When a dunning letter is created for a customer, the business partner master data record is updated. On the Accounting tab, the
Dunning Date field displays the date on which the dunning letters were created for the last time.
When you select this option and the wizard is executed successfully, the run is set to status Executed and Printed Wizard. If the
wizard fails, for example, if service invoices could not be created due to missing tax codes, the dunning letters are not printed and
the run is set to Partially Executed, Not Yet Printed. In this case, no dunning letters are created and the dunning level and last
dunning date information is not updated. You can then load and execute the wizard again after you make the necessary
amendments in the wizard (that is, you specify the tax codes or select not to automatically post service invoices for fees or
interest).
If the wizard has already been executed because you selected Execute Only, Print Later and Exit earlier, dunning letters are
printed only as recorded on the recommendation report.
E-Mail Dunning Letters and Exit
Executes, sends the dunning letters by e-mail, and exits the dunning run for all selected customers and documents.
More Information
Dunning Wizard
Step 8: Displaying Summary Report
The Summary Report page displays a summary of the service invoices created per dunning letter, as well as error and warning
messages that appear during the dunning wizard run.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 276

6/8/26, 6:04 AM
Dunning Wizard
Gross Profit Recalculation Wizard
The wizard enables you to recalculate cost of goods sold (COGS) and gross profit in sales documents using the current
serial/batch cost as the base price for the documents.
Items managed by the serial/batch valuation method and purchased or produced can be sold before final costs are determined.
Product costs are determined by components' cost, which can change after receipt from production.
Purchased items might be sold before related costs are fully recorded and posted. There could be a cost adjustment based
on revaluating transactions such as: AP Invoice based on a goods receipt PO (GRPO), Landed Cost and Material
Revaluation.
Produced serial/batch items received to stock might not be fully costed before being sold.
This is applicable only if we calculate gross profit based on Item Cost, and any other method would not affect the gross profit.
To deal with gross profit discrepancies, the Gross Profit Recalculation Wizard is available in SAP Business One to help you make
any adjustments required. The wizard recalculates COGS and gross profit in sales documents using the current serial/batch cost
as the base price for the documents.
 Note
Documents with an outgoing quantity like a Goods Issue are not impacted by COGS postings or price differences.
The Gross Profit Recalculation Wizard enables the recalculation of gross profit for items managed by the serial/batch valuation
method. By using the current cost of a serial or batch, the wizard recalculates the gross profit in sales documents. If any items were
received from production, then the cost is reconstructed first using the current cost of serial/batch components before
recalculating gross profit.
 Note
To recalculate the gross profit, you must first ensure that gross profit manages base price by item cost. To do so, go to
Administration System Initialization Document Settings General and in the Base Price Origin field (Base Price Origin
appears only when the Calculate Gross Profit checkbox is selected), select Item Cost as a default value. Or you can go to
Sales - A/R Any Sales Document Gross Profit to open the Gross Profit of [Document Name] window, and select Item
Cost in the Base Price By field.
For more information, please see Document Settings: General Tab and Gross Profit.
To access the Gross Profit Recalculation Wizard, from SAP Business One Main Menu, choose Sales - A/R Gross Profit
Recalculation Wizard . Here, you'll find the following steps to guide you through the process:
This is custom documentation. For more information, please visit SAP Help Portal. 277

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
Step 1: Starting the Wizard
Use the Wizard Options page to select whether to run a simulation, start a new run, or load a saved run.
Wizard Options Fields
Run Gross Profit Recalculation Simulation
Select to simulate a gross profit recalculation run. The simulation gives you a preview of the expected results of the actual wizard
run.
Start Gross Profit Recalculation Run
Select to create a new gross profit recalculation run.
Load Saved Gross Profit Recalculation Run
Select to view a saved gross profit recalculation run which is not yet executed.
Related Information
Gross Profit Recalculation Wizard
Step 2: Specifying Wizard Parameters
Use this step to specify wizard parameters.
On the Wizard Parameters page, specify parameters for the wizard run. The parameters that you select will determine the range of
sales documents to which the Gross Profit Recalculation Wizard will be applied.
Gross Profit Recalculation Name
This is custom documentation. For more information, please visit SAP Help Portal. 278

6/8/26, 6:04 AM
Specify a name for the gross profit recalculation run if required. The default name is a unique code automatically defined by SAP
Business One.
Date of Run
By default displays the current date and cannot be changed.
Remarks
Enter remarks about the gross profit recalculation run if required.
Sales Documents Posting Date From…To…
Specify a range of sales documents posting date to filter the items that you want to recalculate gross profits for.
Item No. From…To…
Specify a range of the item number to filter the items that you want to recalculate gross profits for.
Group
Select an item group to filter the items that you want to recalculate gross profits for.
Additional Filters Fields
Additional Filters
Select this checkbox and click the icon to add additional filters to narrow the search.
Find items with only the selected properties
Select this checkbox and properties you want to apply to the search.
Search Condition
Choose whether to search with And or Or condition.
Find Items With
Automatically summarizes the search condition and properties you have specified for the search.
Display Inactive Items
Select this checkbox to display items that do not appear in any of the selected sales documents since a specified date.
Search
Select this button to start searching.
 Note
Starting a new search will clear selections in the search results table.
Item List
Displays every item that is managed by serial/batch valuation method and falls into the above selection criteria.
Selected Items
Displays the selected items that are moved from the Item List table.
 Note
You can use the buttons between the Item List table and the Selected Items table to move all rows or only selected rows
between the two tables.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 279

6/8/26, 6:04 AM
Gross Profit Recalculation Wizard
Step 3: Selecting Sales Documents
Use this step to select relevant sales documents.
On the Sales Documents Selection page, you can select the documents whose base price in the gross profit window needs to be
adjusted to the current serial/batch cost. Deselect documents that you do not want to adjust.
Related Information
Gross Profit Recalculation Wizard
Step 4: Recalculating Production Cost
Use this step to recalculate the production cost.
The Recalculation of Production Cost page will help you to recalculate the production cost according to the current cost of the
serial/batch components. The corresponding serial/batch is included in the Sales Documents Selection step.
 Note
If you have run the Production Cost Recalculation Wizard before running this wizard, you will not see any recommendations
here.
Related Information
Gross Profit Recalculation Wizard
Step 5: Viewing Recalculation Results
Use this step to view the recalculation results.
On the Recommendations page, you can view the recalculation results. Only documents that were selected in the Sales
Documents Selection step will be included.
Related Information
Gross Profit Recalculation Wizard
Step 6: Viewing Material Revaluation Details
Use this step to view material revaluation details.
On the Material Revaluation Details page, you can view the details of the material revaluation document, which adjusts production
costs to current cost of the components. Documents will only be created when Automatic Posting in the next step is selected.
Posting Date
Specify a posting date for the material revaluation document. The date displayed by default is the current date.
This is custom documentation. For more information, please visit SAP Help Portal. 280

6/8/26, 6:04 AM
Document Date
Specify a document date for the material revaluation document. The date displayed by default is the current date.
Series
Use the dropdown list to determine the numbering series for the material revaluation document.
Reference 2
Specify an additional reference number if required.
Journal Remarks
Enter remarks for the journal entry.
Material Revaluation No.
Automatically determined by the selected numbering series.
 Note
If you have run the Production Cost Recalculation Wizard before running this wizard, you will not see any material revaluation
details here.
Related Information
Gross Profit Recalculation Wizard
Step 7: Viewing Journal Entry Details
Use this step to view journal entry details.
On the Journal Entry Details page, you can view the details of the adjustment journal entry and confirm the journal entry creation
by selecting Automatic Posting. The journal entry will adjust the cost of goods sold (COGS) to the current cost of serials or
batches. The sum total of COGS variance grouped by COGS account will be posted to COGS account versus price difference
account.
Posting Date
Specify a posting date for the journal entry. The date displayed by default is the current date.
Document Date
Specify a document date for the journal entry. The date displayed by default is the current date.
Due Date
Specify a due date for the journal entry. The date displayed by default is the current date.
Series
Use the dropdown list to determine the numbering series for the journal entry.
Transaction Code
Select a transaction code for the journal entry.
Journal Remarks
Enter remarks for the journal entry.
Trans. No.
This is custom documentation. For more information, please visit SAP Help Portal. 281

6/8/26, 6:04 AM
Number of the journal entry, automatically determined by the selected numbering series.
Reference 1&2
Specify additional reference numbers if required.
 Note
Only if the Automatic Posting checkbox is selected will the wizard allow to post the journal entry in the next step.
Related Information
Gross Profit Recalculation Wizard
Step 8: Saving or Executing the Wizard
Use this step to save or execute the wizard run.
On the Save and Execute Options page, choose Execute to adjust gross profit in the selected documents and to generate
adjustment journal entry to the cost of goods sold (COGS). Or choose one of the save options to save your predefined parameters
or to save wizard recommendations for later review.
Save Wizard Parameters and Exit
Select to save the parameters for a future run and exit the wizard.
Save Wizard Simulation and Exit
Select to save the wizard simulation for later review of the simulated results, and exit the wizard.
Execute
Select to recalculate the gross profit and a system message will pop out:
Executing the wizard creates an inventory revaluation for adjustment of the production cost,
and a journal entry for adjusting costs of goods sold and gross profit. Creation of documents
depends on input data. Do you want to continue?
Press Yes to generate a new Material Revaluation (MRV) transaction to recalculate the production cost.
Wizard Parameters Name
Specify a name for the wizard parameters if required. The default name is a unique code automatically defined by SAP Business
One.
Description
Enter description for the wizard parameters if required.
Summary
After choosing Finish, you will see a wizard run summary which displays the results of the wizard run.
Related Information
Gross Profit Recalculation Wizard
Sales Reports
Analyzing your sales information is necessary for the success and efficiency of your business. SAP Business One provides several
different reports for the Sales module that assist you in running your business. Some of the reports also include graphical displays,
which facilitate information analysis. Use the sales reports to do the following:
This is custom documentation. For more information, please visit SAP Help Portal. 282

6/8/26, 6:04 AM
Analyze sales transactions
View open documents
Generate backorder reports
View and process documents saved as drafts
More Information
Sales Analysis
Open Items List
Backorder Report
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
This is custom documentation. For more information, please visit SAP Help Portal. 283

6/8/26, 6:04 AM
Currency
Specify the currency in which you want to display the amounts.
Open Documents
Specify the type of document that you want to display.
Sales and purchasing documents
 Note
A/P and A/R Reserve Invoices have two different statuses:
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
This is custom documentation. For more information, please visit SAP Help Portal. 284

6/8/26, 6:04 AM
Original total amount of the document, including tax.
Posting Date
Posting date of the document.
Document Date
Date of the document.
Blanket Agreement No.
Choose which blanket agreements to report on.
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
This is custom documentation. For more information, please visit SAP Help Portal. 285

6/8/26, 6:04 AM
 Note
Drop ship warehouses are not considered in inventory reports and are therefore not included in the consignment quantity. You
can use a script to calculate the total consignation quantity of an item. For more information, see SAP Note 1773671 .
Available
The total available quantity of the item in all the company warehouses. The calculation is based on the following formula:
Qty in Stock + Qty Ordered – Qty Committed
Change To
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
Sales Analysis
The Sales Analysis report provides detailed information about the sales volume achieved with your customers. Specifying the
duration of the report can help you identify problem areas. In addition, a graphical display facilitates information analysis. The
report assists you in determining the following:
Which customers have paid the highest prices for your products
Which customers are the most profitable for your business
Which of your products are the most successful on the market
Which of your sales employees attain the best sales results
More Information
Sales Analysis Report Detailed
Sales Analysis Report - Selection Criteria
Use this window to specify selection criteria for the Sales Analysis report. The window contains three tabs:
Customers
This is custom documentation. For more information, please visit SAP Help Portal. 286

6/8/26, 6:04 AM
Analyze the sales volume for each customer or for customer groups. See Sales Analysis Report: Customers Tab.
Items
Analyze the sales volume either per item or per item group. See Sales Analysis Report: Items Tab.
Sales Employee
Analyze the sales volume per sales employee. See Sales Analysis Report: Sales Employee Tab.
Each tab displays different selection parameters and generates reports that provide different aspects of the sales volume in your
company.
To open the window, choose Sales – A/R Sales Reports Sales Analysis . Alternatively, open it from the Reports module.
Sales Analysis Report: Customers Tab
Use this tab to specify selection criteria for the Sales Analysis by Customer report. When you run the report, SAP Business One
creates a corresponding sales volume analysis for each customer.
To access the tab, choose Sales – A/R Sales Reports Sales Analysis Customers . Alternatively, access it from the Reports
module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Customers Tab Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want the report to reflect results for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio button, the total for the year is also displayed. In addition, if you
select one of these options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
Invoices, Orders, Delivery Notes
Select the document type on which you want to base the sales analysis.
 Note
If you base an A/R credit memo on an A/R down payment invoice, that A/R credit memo does not appear in the report.
Cancelled sales orders do not appear in the report.
Returns are displayed as part of delivery notes and they decrease the sales amount.
Individual Display
Displays the report for individual customers.
Group Display
Displays the report for customer groups, with each customer group appearing in a separate row. To display the sales for each
customer in a customer group, double-click the row number of the respective customer group.
This is custom documentation. For more information, please visit SAP Help Portal. 287

6/8/26, 6:04 AM
Total by Customer
Choose how to group the report data.
Total by Blanket Agreement
Choose how to group the report data.
Properties
Choose Properties to include customer properties in the report.
Display Amounts in System Currency
Displays the amounts in system currency.
Related Information
Sales Analysis
Sales Analysis Report: Items Tab
Use this tab to specify selection criteria for the Sales Analysis by Item report, which analyzes sales either per item, or per item
group. SAP Business One creates a sales volume analysis for each item.
To access the tab, choose Sales – A/R Sales Reports Sales Analysis Items.
Alternatively, access it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Analysis Items Tab Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want the report to reflect results for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio button, the total for the year is also displayed. In addition, if you
select one of these options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
Invoices, Orders, Delivery Notes
Select the document type on which you want to base the sales analysis.
 Note
If you base an A/R credit memo on an A/R down payment invoice, that A/R credit memo does not appear in the report.
Cancelled sales orders do not appear in the report.
Returns are displayed as part of delivery notes and they decrease the sales amount.
As the report displays open quantities only, sales orders and delivery notes are displayed with zero quantities and zero
amounts in the following scenarios:
The sales orders are closed or fully copied to either deliveries or A/R invoices.
This is custom documentation. For more information, please visit SAP Help Portal. 288

6/8/26, 6:04 AM
The delivery notes are closed or fully copied to either A/R invoices or returns.
Sales orders or delivery notes that were partially copied into target documents are listed with remaining open quantities
for deliveries or invoices.
Individual Display
Displays a report for an individual item.
No Totals
Displays one row for each item or item group in the report (this depends on the selections you have made in the Individual Display
and Group Display fields).
Total by Customer
Displays a row for each combination of an item and customer (or items group and customer) in the report.
Total by Sales Employee
Display a row for each combination of an item and sales employee who sold it.
Main Selection
Specify the item range to be included in the report.
Define the item codes range, specify an item group if required, and choose Properties to use the item properties as a selection
criteria.
Secondary Selection
Select to define an additional selection: by customer range, group or properties, by sales employee or both.
Display Amounts in System Currency
Displays the amounts in the system currency in the report.
More Information
Sales Analysis
Related Information
Sales Analysis
Sales Analysis Report: Sales Employee Tab
Use this tab to specify selection criteria for the Sales Analysis by Sales Employee report, which analyzes the sales volume per sales
employee. SAP Business One creates a corresponding sales volume analysis for each sales employee.
To access the tab, choose Sales – A/R Sales Reports Sales Analysis Sales Employee.
Alternatively, access it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 289

6/8/26, 6:04 AM
Sales Employee Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want the report to reflect results for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio button, the total for the year is also displayed. In addition, if you
select one of these options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
Invoices, Orders, Delivery Notes
Select the document type on which you want to base the sales analysis.
 Note
If you base an A/R credit memo on an A/R down payment invoice, that A/R credit memo does not appear in the report.
Cancelled sales orders do not appear in the report.
Returns are displayed as part of delivery notes and they decrease the sales amount.
Related Information
Sales Analysis
Sales Analysis By Different Selection Criteria
This window displays the results of a Sales Analysis by report, whose full name reflects your selections from the following options:
Customer
Item
Sales Employee
The time frame follows in parentheses:
(Annual)
(Monthly)
(Quarterly)
 Example
If the user selected the Annual Report option on the Customers tab, this window is named: Sales Analysis by Customer
(Annual).
The details displayed in this window are determined by your selection criteria. Whenever you choose to display different
information, you see different columns.
However, despite your selection criteria, you can still display the following by using the Go To menu:
Customer code or name
Item code or name
This is custom documentation. For more information, please visit SAP Help Portal. 290

6/8/26, 6:04 AM
Sales employee code or name
To view the detailed information related to each row in the report, double-click the number of the row. A detailed window appears.
To display the report results as a graph, choose . A new window with the graph display of the report appears. Choose the
Settings pushbutton to define the display parameters.
More Information
Sales Analysis Report
Sales Analysis Report: Detailed View
This window displays the details for a specific row of the Sales Analysis report. One section displays a table listing all sales
documents and their details; another contains a diagram of the sales information.
You can select different types of diagrams. To print the diagram when you print the report, select Print Diagram.
More Information
Sales Analysis Report
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
This is custom documentation. For more information, please visit SAP Help Portal. 291

6/8/26, 6:04 AM
Description of the field included in the graph.
Including
Displays the element data in the graph.
Backorder Report - Selection Criteria
Use this window to specify selection criteria for the Backorder report, which displays a list of overdue sales orders or A/R reserve
invoices that cannot be shipped due to stock shortages. The report lets you define priorities and accelerate purchase orders or
production orders.
To open the window, choose Sales - A/R Sales Reports Backorder . Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Backorder Report - Selection Criteria
Properties
Select or ignore item properties for the report.
Warehouses Location
Select the location of a warehouse to include it in the report.
Backorder Report
This report displays a list of overdue sales orders or A/R reserve invoices that cannot be shipped due to inventory shortages. It lets
you define priorities and accelerate purchase orders or production orders.
To access this window, choose Sales - A/R Sales Reports Backorder .
You can run the backorder report daily, weekly, or monthly. It displays all sales orders with an open quantity according to the
selection criteria you specify.
 Note
You have the option to display the quantities for the overdue sales orders or A/R reserve invoices either by Inventory UoM or
Sales UoM. In the Form Settings window on the Document tab choose one of the following:
Sales UoM – All quantities are converted to the Sales UoM as defined in the Sales Order or Reserve Invoice. This is the
default.
Inventory UoM – All quantities are converted to the Inventory UoM as defined in the Item Master Data window on the
Inventory Data tab. Items per Unit is set as 1.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 292

6/8/26, 6:04 AM
Backorder Report Fields
Delivery Date
Date (from the row) of an expected delivery for the item.
Payment Status for A/R Reserve Invoice
Payment status options for the A/R reserve invoice are: Fully Paid, Partially Paid, or Not Paid.
Unit of Measure
Name of the Inventory UoM or Sales UoM as defined in the original document.
Items per Unit
The number of items defined in the original document.
Ordered
Original quantity of the item ordered in a sales order.
Delivered
Quantity of the item that has already been delivered to the customer.
Backorder
Quantity of the item yet to be delivered to the customer.
More Information
Backorder Processing
Go To Menu - Sales and Purchasing Documents
When you process a document from the SAP Business One Sales - A/R or Purchasing - A/P module, the Go To menu contains only
functions that relevant for the specific document you are working on.
 Note
You can display the same options as on the Go To menu through the Context menu by clicking the right mouse button.
Go To Menu Options
Base Document
If rows are created with reference to an existing sales document (for example, an order or a delivery note), use this option to
display the document by positioning the cursor on the appropriate row.
Target Document
If follow-up transactions for a document were created with a reference (for example, a delivery for an order), use this option to
display the document by positioning the cursor on the row.
If more than one delivery note was created for an order row, for example, you can see the delivery note that was created last in each
case. If you want to see all the subsequent documents for an order item, use the functions under the Drag & Relate menu.
List of Business Partners
This is custom documentation. For more information, please visit SAP Help Portal. 293

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 294

6/8/26, 6:04 AM
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
Gross Profit
SAP Business One lets you calculate the gross profit for sales documents according to the method you define during application
configuration. The gross profit for each document row is calculated and then totaled for the entire document. Gross profit can be
calculated for documents of Item type and for documents of Service type.
To calculate the gross profit in a sales document, from the tool bar choose the icon.
Gross profit calculation is available for the following documents:
Sales Quotation
Sales Order
Delivery
Return
A/R Invoice, A/R Reserve Invoice, A/R Invoice + Payment
A/R Correction Invoice and A/R Correction Invoice Reversal
A/R Credit Memo (only if not based on A/R Down Payment Invoice)
 Note
Gross profit calculation is active only if you have selected the Calculate Gross Profit checkbox in Administration System
Initialization Document Settings General .
Gross Profit of [Document Name] Window Fields
The fields and information displayed in the Gross Profit for [Document Name] window vary according to the document type: Item
or Service.
Fields for Document of Item Type
This is custom documentation. For more information, please visit SAP Help Portal. 295

6/8/26, 6:04 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Base Price By
Displays the base price in accordance with the price list.
The default value is defined in Administration System Initialization Document Settings General Calculate Gross Profit
Base Price Origin .
If required, you can choose a different price list.
Other additional prices are:
Last Purchase Price – the item price the last time the item was purchased. If the purchasing price of an item changes from
time to time, the gross profit calculation considers it.
Last Evaluated Price – the price calculated the last time the Inventory Valuation Simulation Report was generated.
 Note
If your company manages non perpetual inventory, the name of this report is Inventory Valuation Report.
Item Cost – the item cost calculated in Item Master Data Inventory Data tab. The item cost may vary from time to
time, depending on the valuation method defined for the item..
 Note
This option is available only in companies who manage perpetual inventory system.
Base Price
The base price of the item as defined (or calculated) in the price list selected in the Base Price By field, multiplied by the Items Per
Unit quantity in the sales document. If you change this value manually, the values in Total Base Price, Gross Profit, Profit %, and
Base Price By fields are updated accordingly.
You can update the base price in all of the sales documents even after the document has been closed. The only exceptions are A/R
correction invoice where the base price is a read-only in the Was table, and A/R correction invoice reversal, in which the base price
is a read-only as well.
Total Base Price
The total amount of the base price for gross profit calculation. If you change this value manually, the values in the Base Price,
Gross Profit, Profit %, and Base Price By fields are updated accordingly.
If the quantity in the document is updated, the total base price is recalculated by multiplying the base price by the updated
quantity.
You can update the total base price in all of the sales documents even after the document has been closed. The only exceptions are
A/R correction invoice where the total base price is a read-only in the Was table, and A/R correction invoice reversal, in which the
total base price is a read-only as well.
 Note
The following rules apply when the base price is by Item Cost:
In sales documents that create inventory posting (such as Delivery), the total base price equals to the amount posted to
the Cost of Goods Sold account.
This is custom documentation. For more information, please visit SAP Help Portal. 296

6/8/26, 6:04 AM
When partially drawing a delivery into A/R Invoice, or a return into A/R Credit Memo, the total base price equals the
relative portion of the total base price in the base document, based on the drawn quantity.
 Example
Delivery with Quantity = 10 and Total Base Price = 33.6 is partially drawn into A/R invoice.
Drawn quantity = 6.28. The total base price in the A/R invoice is calculated as follows:
33.6 * 6.28/10 = 21.1008
Total base price of parent items in Sales BOM for which price and total are displayed for parent item only (defined in
Administration System Initialization Document Settings For a Sales BOM in Documents, Display: section ) and
Assembly BOM is the sum of all of their components' cost. In case the valuation method for the parent item is Standard,
and standard price (different from zero) is defined (in Item Master Data Inventory Data tab Item Cost field ) the
standard cost is used.
For Sales BOM, in case the price for component items is displayed, the Base Price, Total Base Price, and Base Price By
fields are blank and disabled.
When drawing A/R invoice into A/R correction invoice, the total base price equals the amount posted to the Cost of
Goods Sold account by the original A/R invoice.
Gross Profit
SAP Business One calculates the difference between the sales price and the base price for each item in the sales document. If the
result is negative, the row is highlighted in red.
Profit %
SAP Business One calculates the gross profit in percent.
When you configure the application, you can choose between two different calculation methods:
The gross profit can be displayed on the basis of the ratio of the gross profit to the sales price of the item.
The gross profit can be displayed on the basis of the ratio of the gross profit to the cost price of the item.
If you change data in this window, confirm your changes by choosing Update and OK.
 Note
When you configure SAP Business One, you can set it up so that an internal mail is sent automatically to specific users when a
particular gross profit is exceeded.
Base Price By
Indicates the way the base price in the row has been calculated. If you change the value in the Base Price field or the Total Base
Price field, the value in the Base Price By column is set automatically to Manual. When selecting any of the options available in the
dropdown list, the values in the Base Price, Total Base Price, Gross Profit, and Profit % fields in the row, are updated accordingly.
 Note
By default this column does not appear in the Gross Profit window. To display it, select this column in from the Form Settings —
Gross Profit for [document name] Window.
Fields for Document of Service Type
Default Gross Profit %
This is custom documentation. For more information, please visit SAP Help Portal. 297

6/8/26, 6:04 AM
The default gross profit percentage for documents of service type, as defined in: Administration System Initialization
Document Settings General Tab Default Gross Profit % for Service Documents field .
If you change this percentage manually, the Profit % field in the table is updated accordingly, and gross profit of all of the rows
appear in this window is recalculated.
When drawing the document into target document, the percentage defined in this field is drawn to the target document.
When drawing multiple service documents with different Default Gross Profit % values, the percentage appears in the Default
Gross Profit % field in the target document, is taken from Administration System Initialization Document Settings
General Tab Default Gross Profit % for Service Documents field .
Service
The description of the services as appears in the sales document.
Total Base Price
The base price of the service. This value is calculated based on the total amount of the service as entered in the sales document,
and according to the default gross profit percentage defined in Administration System Initialization Document Settings
General tab Default Gross Profit % for Service Documents field .
You can change the total base price manually. The values in the Gross Profit, Profit %, and Base Price By fields in the row are
updated accordingly.
When drawing the document to a target document, the total base price is drawn to the target document. If you have changed
manually the total base price in the base document, the updated value is drawn to the target document. If you draw only part of the
row from the base document, the relative portion of the total base price is drawn to the target document.
The total base price in the target document is calculated as follows:
Target Document Total Base Price = Target Sales Price * Base Document Total Base Price / Base Document Sales Price
 Example
Base Document:
Sales Price = 1000
Total Base Price = 336
Target Document:
Drawn Sales Price = 628
Total Base Price = 211.008 (= 336*628/1000)
Sales Price
The sales price of the service as appears in the sales document, before tax and after discount.
Gross Profit
The gross profit amount calculated by subtracting the Total Base Price from the Sales Price. If you change the Total Base Price
the Gross Profit amount is updated accordingly.
Profit %
The percentage of the gross profit, calculated by dividing the Gross Profit by either the Sales Price or the Base Price, depends on
the calculation method selected in Administration System Initialization Document Settings General Tab .
Base Price By
This is custom documentation. For more information, please visit SAP Help Portal. 298

6/8/26, 6:04 AM
Indicates the way the gross profit in the row has been calculated:
Percentage — the gross profit has been calculated according to the percentage defined in the Default Gross Profit % field.
Manual — indicates that you have manually changed the total base price in the row (the gross profit amount and gross
profit percentage are updated accordingly). To return to the original calculation, select from the dropdown list the option
Percentage.
 Note
By default this column does not appear in the Gross Profit window. To display it, select this column in from the Form Settings —
Gross Profit for [document name] Window.
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
Opens a list of predefined texts. To select more than one item, use the ctrl+shift option. Choose New to add more texts to this list.
More Information
Predefined Text - Setup
Item Availability Check
The item availability check enables you to assess the following:
If a specific item is available
If a specific item is in a particular warehouse
If a specific item quantity is available
If a specific item is available for delivery on the required date
In addition, you can check:
This is custom documentation. For more information, please visit SAP Help Portal. 299

6/8/26, 6:04 AM
The item quantity available on the requested delivery date
The earliest delivery date for the full quantity required in the sales order
A basic Available-to-Promise (ATP) report that provides additional information about item availability, such as the
uncommitted stock and receipts available to satisfy potential customer orders. See Inventory Status Window.
The Item Availability Check window only appears when the quantity of an item required in a sales order is larger than the available
quantity on the delivery date, minus the minimum level. The minimum level is defined at the warehouse level (as defined in the Item
Master Data window).
The quantity is calculated as follows:
Available = In Stock + Ordered – Committed from the current date to the requested delivery date.
If you update an existing sales order (instead of creating a new one), SAP Business One does not take into account the existing
sales order values when calculating available quantity, as it does when you create a new sales order.
 Example
A purchase order was created with a quantity of 10 items.
Sales order 1 was created with a quantity of 6 items.
Sales order 2 was created (this is a new sales order) with a quantity of 5 items, and the available quantity is calculated as
4 items.
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
This is custom documentation. For more information, please visit SAP Help Portal. 300

6/8/26, 6:04 AM
Available Quantity
The quantity of an item that will be available for delivery on the Requested Due Date for the selected warehouse. If the Requested
Due Date is beyond the item's lead time, then the Available Quantity is the requested quantity.
SAP Business One determines the available quantity by checking that the amount in the Available Quantity field is greater than the
minimum level defined at the warehouse level.
 Note
If a Delivery Date is not entered in the sales order the current system date is used.
Earliest Availability
The earliest date on which the requested stock will be available according to ATP logic (see Viewing Detailed Confirmation Status).
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
This is custom documentation. For more information, please visit SAP Help Portal. 301

6/8/26, 6:04 AM
Display Quantities in Other Warehouses – opens a window that displays the quantities of the item in other warehouses.
You can choose a different warehouse if required.
Display Alternative Items – opens the Alternative Items – Selection Criteria window, from which you can choose a
different item for the order.
Delete Row – deletes the item row from the sales order.
More Information
Alternative Items – Selection Criteria
Inventory Status Window
Last Prices Report
This report displays the last purchasing and sales prices of an item, either for a specific business partner or for all business
partners.
To open the report, do one of the following:
From the SAP Business One Main Menu, choose Inventory Inventory Reports Last Prices Report .
From the SAP Business One Main Menu, choose Inventory Item Master Data . Go to the record of an existing item,
right click in the Item Master Data window to open the context menu, and then choose Last Prices.
In a sales or purchasing document, place the cursor in the Unit Price field and press CTRL+TAB . The values are copied
automatically from the document.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Last Prices Report Fields
BP Code
Displays the last prices of an item for a specific business partner.
Deselect to display the last prices of an item for all vendors or all customers.
Display ... Last Prices
Enter the number of previous prices to display.
Special Prices
In addition to last prices, displays the Special Prices defined for the selected item.
This selection is optional.
Date
Enter a date to display Special Prices for that specific date.
Quantity
This is custom documentation. For more information, please visit SAP Help Portal. 302

6/8/26, 6:04 AM
Enter a quantity to display Special Prices for that specific quantity.
To generate the report, enter the necessary information and choose Refresh.
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
This is custom documentation. For more information, please visit SAP Help Portal. 303

6/8/26, 6:04 AM
5. Choose OK.
The document displays only the first row of the added text.
If the text is longer than displayed, double-click the row to view the entire text and edit it as necessary.
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
This is custom documentation. For more information, please visit SAP Help Portal. 304

6/8/26, 6:04 AM
SAP Business One recalculates the subtotal with every change. For example, deleting a row may lead to a change in the
subtotal values.
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
This is custom documentation. For more information, please visit SAP Help Portal. 305

6/8/26, 6:04 AM
250 (row 3) + 310 (row 6) = 560 (row 7)
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
This is custom documentation. For more information, please visit SAP Help Portal. 306

6/8/26, 6:04 AM
Withholding Tax Table Fields
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
Additional Information
With SAP Business One you can:
Define form settings for sales documents
Calculate tax
This is custom documentation. For more information, please visit SAP Help Portal. 307

6/8/26, 6:04 AM
Export sales documents to Microsoft Word
Perform other useful tasks
More Information
Form Settings for Sales Documents
Tax Calculation in Sales Documents
Saving Documents and Reports Exported to Microsoft Word
Adjusting Tax Amount
Context
As a business user, you cannot adjust the tax amounts of sales documents manually in the SAP Business One client.
This task needs to be carried out through the Data Interface API (DI API) by your system administrator or SAP Business One
partners. Before using the DI API, make sure that the following settings are enabled in the SAP Business One client.
Procedure
1. From the SAP Business One Main Menu, choose Administration System Initialization Company Details .
2. On the Accounting Data tab, select the checkbox Allow External Calculation of Tax on AR Documents.
For more information about how to work with the DI API, see the online help for SAP Business One SDK on the product
page.
Related Information
Sales Document: Contents Tab
Adjusting Tax Amount
Form Settings for Sales Documents
When you process a sales document, you can define which fields and columns should be displayed and activated or deactivated in
the documents. This enables you to display frequently used detailed information, so that you can enter data more easily.
On the toolbar, click to display the Form Settings window, in which you define the document settings. The window contains
three tabs:
Document: Maintain data that applies to the entire sales document.
Table Format: Select or deselect fields to display the required fields in the Contents tab table of the sales document.
Row Format: Select or deselect fields to make the required selections in the rows of the Contents tab of the sales
document.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 308

6/8/26, 6:04 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Form Settings Fields - Document Tab, Table Subtab
Sales Employee
Displays the sales employee details. If required, change the entry.
Comm. %
Enter a percentage for the commission granted to the sales employee.
Discount %
Specify a discount that is used for all the document rows. This entry overwrites any previously defined discounts.
G/L Account
Enter a revenue account for the sales document rows. This entry applies to all the rows in the document. If required, change the
entry for a row.
Distr. Rule
Enter a distribution rule for the document rows. This entry applies to all the rows in the document. If required, change the entry for
a row.
Project
Enter a project number for the document rows. This entry applies to all the rows in the document. If required, change the entry for
a row.
Warehouse
Displays the default warehouse code. If required, change the entry.
Delivery Date
Enter the delivery date for the sales document.
Form Settings Fields - Document Tab, General Subtab
Display BP Catalog Number
Displays the business partner catalog number for the sales document.
Tax Calculation in Sales Documents
When you process a sales document, tax is calculated according to the settings made for customers, items, and service. Each row
in the document, either an item or a service, stores a tax group. This group enables the system to calculate the total tax amount of
the document and lets you generate various tax reports, as required.
First, SAP Business One checks the default tax groups defined in the G/L Account Determination window and displays those tax
groups as default.
When you select a customer for the sales document, SAP Business One checks whether this customer is liable for tax or defined as
EU. If the customer is tax liable and has an assigned tax group, this tax group overwrites the default one. If no tax group has been
This is custom documentation. For more information, please visit SAP Help Portal. 309

6/8/26, 6:04 AM
defined for the customer, SAP Business One checks every item you select in the document and uses the default group for the
item’s row in the document.
You may select any tax group for the document rows, regardless of the default groups.
Saving Documents and Reports Exported to Microsoft Word
 Note
The feature described here is applicable when you select the Local Folder radio button in the Export Word and Excel File To
section on the Path tab of the General Settings window.
By default, exported documents and reports are saved on each workstation in the WordDocs folder, located in the SAP Business
One folder.
SAP Business One creates one folder for each company database. This folder has the same name as the database.
In the database folder, SAP Business One creates one folder for each business partner to save their respective exported
documents along with their code. The documents are saved in these folders as Microsoft Word files.
The file names of exported documents include the document name and the document number.
 Example
Sales Quotation 6.doc
The file names of exported reports include the report name and the date on which it was exported.
 Example
Account for Customers (Debt Aging) - 10_25_2004.doc
You can save the exported documents and reports in a different location using the saving options in Microsoft Word.
Related Information
How to Work with SAP Business One Microsoft 365 Integration
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
This is custom documentation. For more information, please visit SAP Help Portal. 310

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 311

6/8/26, 6:04 AM
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
agreement has the status Approved or Terminated. If the status is Terminated, the posting date of the document
must be within the date range of the agreement, that is, between the start date and the termination date.
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
This is custom documentation. For more information, please visit SAP Help Portal. 312

6/8/26, 6:04 AM
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
You can create sales and purchasing documents associated with a blanket agreement only if the blanket
agreement has the status Approved or Terminated. If the status is Terminated, the posting date of the document
must be within the date range of the agreement, that is, between the start date and the termination date.
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
This is custom documentation. For more information, please visit SAP Help Portal. 313

6/8/26, 6:04 AM
2. Open the relevant blanket agreement in Find mode.
3. Set the status of the blanket agreement to Approved and choose Update.
4. To save the changes, choose OK.
 Note
An authorizer can reject a blanket agreement after it has been approved. However, rejection is not possible if the
agreement has linked sales or purchasing documents.
Changing a Blanket Agreement
1. Choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
2. Open the relevant blanket agreement in Find mode.
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
This is custom documentation. For more information, please visit SAP Help Portal. 314

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 315

6/8/26, 6:04 AM
Once you choose a blanket agreement, the Draw Document Wizard (DDW) allows you to either choose Draw All Data or
Customize. If you select Customize, you can select the rows you want to copy.
It is not possible to change the quantity of an item to be copied at this stage. You can change an item´s quantity later in the
Quantity field of the document row. The Remarks field in the target document displays the blanket agreement information.
Displaying Available Blanket Agreements
To see at a glance all blanket agreements that may exist with particular business partners or for certain date ranges, you can
generate a blanket agreement list report.
Procedure
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
This is custom documentation. For more information, please visit SAP Help Portal. 316

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 317

6/8/26, 6:04 AM
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
Total Open Amount
The sum total of Planned Amount - (Cumulative Amount + Ordered Amount) in local currency.
Purchasing Goods Related to a Blanket Agreement
Prerequisites
A blanket agreement exists for the business partner, and the posting date of the purchasing transaction falls into the validity period
of the agreement.
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
This is custom documentation. For more information, please visit SAP Help Portal. 318

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 319

6/8/26, 6:04 AM
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
Increases the cumulative quantity and cumulative amount
Decreases the open quantity and open amount
 Note
If you cancel the sales document later, linked blanket agreements in the cancellation document remain the same, regardless of
whether the posting date of the cancellation document is still within the durations of the agreements. After the cancellation, the
above-mentioned cumulative and open values in all linked agreements are reverted.
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
This is custom documentation. For more information, please visit SAP Help Portal. 320

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 321

6/8/26, 6:04 AM
Descriptive text for the agreement, if required.
Blanket Agreement: General Tab
Use this part of the blanket agreement to specify the general terms of the agreement.
To access this tab, choose Sales – A/R Sales Blanket Agreement or Purchasing – A/P Purchase Blanket Agreement .
General Tab Fields
Agreement Type
The kind of agreement you have made with your business partner:
General
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
This is custom documentation. For more information, please visit SAP Help Portal. 322

6/8/26, 6:04 AM
When you copy multiple blanket agreements to a marketing document, and the payment methods defined in the blanket
agreements are not the same, the document payment method remains unchanged.
When a blanket agreement is linked to the document lines without using the Copy To function, the payment method
defined in the blanket agreement has no impact on the document.
Shipping Type
Define a shipping type for the blanket agreement.
When a blanket agreement is associated with a marketing document, either automatically or manually, the shipping type defined in
the blanket agreement will be taken into the Shipping Type field in the document.
Settlement Probability %
Specify a percentage value to indicate how probable it is that the business partner will pay for the goods.
Status
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
This is custom documentation. For more information, please visit SAP Help Portal. 323

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 324

6/8/26, 6:04 AM
Enter the item prices that you agreed on with the business partner.
Cumulative Committed Quantity
Display the sum of the quantity of the item in the open lines of the sales orders and non-delivered A/R reserve invoices that are
associated with the blanket agreement.
Cumulative Committed Amount
The total monetary value of those items from open lines in sales orders and non-delivered A/R reserve invoices associated with the
blanket agreement. This value is filled in by the system.
Cumulative Ordered Quantity
Display the sum of the quantity of the item in the open lines of the purchase orders and non-delivered A/P reserve invoices that are
associated with the blanket agreement.
Cumulative Ordered Amount
The total monetary value of the items in the open lines of the purchase orders and non-delivered A/P reserve invoices that are
associated with the blanket agreement.
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
This is custom documentation. For more information, please visit SAP Help Portal. 325

6/8/26, 6:04 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 326

6/8/26, 6:04 AM
In the MRP run, the application subtract the item's open quantities in blanket agreements with the type of Specific from the
forecasted quantities.
For more information, see Managing Forecasts.
Activity
To record an activity, such as a phone call or meeting, associated with the blanket agreement, click the yellow arrow and specify the
required information.
More Information
General Settings: Inventory Tab
Blanket Agreement: Documents Tab
Use this tab to view the documents associated with the blanket agreement.
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
This is custom documentation. For more information, please visit SAP Help Portal. 327

6/8/26, 6:04 AM
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
This is custom documentation. For more information, please visit SAP Help Portal. 328

6/8/26, 6:05 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:05:14 GMT+0000
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
Sales - A/R
This module covers the entire sales process, from creating quotations for customers and interested parties, to invoicing, creating
document drafts, and printing. SAP Business One provides an extensive range of sales documents, each of which pertains to a
different stage of the sales process.
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Transaction Processing
Please note that image maps are not interactive in PDF outputs.
Document Customization
Please note that image maps are not interactive in PDF outputs.
Report Management
Please note that image maps are not interactive in PDF outputs.
Other Functions
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:05 AM
Please note that image maps are not interactive in PDF outputs.
Document Printing
Context
Use this function to print batches of documents according to your required selection criteria. You can choose whether to print the
whole list or specific documents.
Procedure
1. From the SAP Business One Main Menu, choose one of the following:
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
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:05 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:05 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:05 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:05 AM
2. On the Per Document tab, in the Document dropdown list, select the required document type.
3. Select Print Document.
4. Enter the required number of copies in Copies (Incl. Original).
 Note
You can configure additional settings for the document. For more information, see Print Preferences: Per Document Tab.
5. Choose Update and OK.
Related Information
Print Preferences
This is custom documentation. For more information, please visit SAP Help Portal. 7