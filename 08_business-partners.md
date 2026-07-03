6/8/26, 6:06 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:06:44 GMT+0000
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

6/8/26, 6:06 AM
Business Partners
The Business Partners module manages all the information relevant for your relationships with customers, vendors, and leads
(interested parties), as well as performing and reviewing internal reconciliations for business partners.
 Example
Typical information includes contact persons, addresses, payment terms, and financial and logistic information.
Business Partners and Accounts
SAP Business One differentiates between business partners and G/L accounts:
Business partners are all your company customers, vendors, and leads.
G/L accounts are all the entities defined in your company's Chart of Accounts, such as expenses, revenues, assets, and
liabilities.
SAP Business One connects between business partners and G/L accounts through control accounts that are defined during
system initialization, and which may vary for different business partners.
All sales and purchasing transactions are posted to the appropriate control accounts, allowing you to access the overall balance,
the balance for customers, and the balance for vendors in one G/L account. In addition, you can access the balance of a specific
customer or vendor.
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Please note that image maps are not interactive in PDF outputs.
Related Information
Verifying VAT Numbers for Business Partners
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:06 AM
Business Partner Master Data
Use the business partner master data to record and retrieve business partner (customers, vendors, and leads) information and
schedule business partner activities. Business partner information typically includes:
Company details, including addresses and telephone numbers
Business partner contact persons, including telephone numbers and E-mail addresses
Logistic details
Tax information
Accounting information
Details of payment terms
The master data forms the basis for all sales and purchasing documents, and activities involving a business partner. You can also
use the data to analyze your business partner relationships in detail.
This image is interactive. Hover over each area for a description. Choose the highlighted areas for more information.
Please note that image maps are not interactive in PDF outputs.
Managing Business Partner Master Data
Context
When you process business partner master data, you can perform the following actions:
Add new business partners
Display and update existing business partners
Delete business partners for which there are no related transactions
When a business partner is both a vendor and a customer, connect vendor with customer on the General tab of the
Accounting tab on Business Partner Master Data. Consider connnections between customer and vendor in step 3 of the
the Dunning Wizard before sending dunning letters. See the relevant sections of these help pages for more information
about the fields Connected Vendor, Connected Customer and Consider Connected Vendors.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:06 AM
Removing Business Partners
1. Find and display the relevant business partner.
 Note
For more information, see Displaying and Updating Business Partners
2. Do one of the following:
From the menu bar, choose Data Remove business partner .
Right-click the Business Partner Master Data window and choose Remove business partner.
3. In the Business Partner Master Data system message, do one of the following:
To permanently delete the business partner, choose the OK button.
To keep the business partner and return to the Business Partner Master Data window, choose the Cancel button.
 Note
You can remove a business partner master record only if the following conditions are met:
Business partner balance is zero.
Business partner is not defined as a consolidation business partner.
Business partner is not connected to any document.
Displaying and Updating Business Partners
Procedure
1. From the SAP Business One Main Menu, choose Business Partners Business Partner Master Data .
The Business Partner Master Data window appears in Find mode.
2. Enter your search criteria in one or several fields. The searchable fields are highlighted in yellow.
You can limit your search to a specific business partner type. You can also specify search criteria on the various tabs of the
window.
 Note
You must first define the business partner type before you are able to define the numbering series.
3. Choose Find.
A list of the business partners that match your search criteria appears.
4. Select the business partner you want to display and choose the Choose button.
Alternatively, you can browse through existing business partners, using the icons in the toolbar:
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:06 AM
5. To edit data, modify the required fields.
6. To save your changes, choose Update.
 Note
You can change the code, type, or currency of the business partner only if the following conditions are met:
Business partner balance is zero.
Business partner is not defined as a consolidation business partner.
Business partner is not connected to any document.
The following are the exceptions to the above rules:
If the business partner is connected to a sales opportunity, sales order, sales quotation, or activity, you can change the
business partner code and business partner type.
If the business partner is connected to a sales opportunity, sales order, sales quotation, activity, item, or draft, you can
change the business partner currency to another currency. You can set the business partner currency to All Currencies,
irrespective of the object to which the business partner is connected.
 Note
When changing the business partner’s name, you can choose whether to update the name in the business partner’s open
documents, as per the list below.
Open Documents for Customers:
Sales - A/R: Open Sales Order
Sales Opportunities: Open Sales Opportunity
Service: Service Call with the status: Open, Pending and every new status you defined
Service: Customer Equipment Card: with the status Active, Returned and In Repair Lab
Service: All Service Contracts
All open Draft Documents (including Payment Drafts)
Open Documents for Leads:
Sales Opportunities: Open Sales Opportunity
Open Documents for Vendors:
Purchasing - A/P: Open Purchase Quotation
Purchasing - A/P: Open Purchase Order
All Open Draft Documents (including Payment Drafts)
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:06 AM
More Information
Business Partner Master Data Window
Activity Window
Adding New Business Partners
Context
Use this procedure to add new business partners to SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Business Partners Business Partner Master Data .
The Business Partner Master Data window appears.
2. To switch to Add mode, choose .
3. In the field to the right of the Code field, select the business partner type.
 Note
If a vendor is also one of your customers, you must create two different master data records (one customer record and
one vendor record) containing the same data, but with different codes.
 Note
When a business partner defined as Lead becomes a customer, change the business partner type to Customer.
4. Enter other required data in the relevant fields of the window, see Business Partner Master Data Window.
5. Choose Add.
Related Information
Displaying and Updating Business Partners
Business Partner Master Data Window
Use this window to add new business partners, display and edit business partner records.
To open the window, choose Business Partners Business Partner Master Data .
By default, the window opens in Find mode, which lets you search for business partners. The following tabs appear:
General
Payment Terms
Payment Run
Accounting
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:06 AM
Remarks
In Add and Update modes, the following additional tabs appear:
Contact Persons
Addresses
Properties
 Note
When a business partner record is displayed, choose Go to in the menu bar to view related data, such as:
Special Prices for Business Partners
Business Partner Catalog Numbers Window: BP Tab
Inventory Posting List by BP
Dunning History Report
Inventory Status Report
 Note
The Inventory status report is generated directly from the Business Partner Master Data window for preferred vendors
only (as defined on the Purchasing Data tab in the Item Master Data window). The selection criteria for the report is
automatic; you cannot change it.
More Information
Business Partner Master Data: General Area
Adding New Business Partners
Displaying and Updating Business Partners
Business Partner Master Data: General Area
Use this area to enter general information about a business partner.
To open the window, choose Business Partners Business Partner Master Data .
General Area Fields
Code
Specify a unique code for the business partner. You can specify any alphanumeric string up to 15 characters.
 Note
You cannot specify a code if this code already exists for a G/L account defined in the chart of accounts or for an existing
business partner.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:06 AM
If a customer is also one of your vendors, create two business partners with two different codes.
Type
Select the business partner type from the list to the right of the Code field. The type determines the transactions you can perform
with this business partner:
Customer - You can carry out sales transactions, activities, enter sales opportunities and service calls.
Vendor - You can carry out purchasing transactions and activities.
Lead - You can enter sales opportunities, sales quotations, sales orders, and activities.
Name
Specify the business partner’s full name.
Foreign Name
Specify the business partner's foreign name, which can be up to 100 characters. The foreign name as entered here will be printed
in documents when a print layout in foreign language is selected.
Group
Select a predefined group by which you want to classify the business partner.
 Note
If you do not select a group, the business partner is automatically assigned to the first group in the list.
Currency
Select the currency in which you carry out transactions with the business partner.
If you selected All Currencies for the business partner, you can choose the ellipsis button to open the Currencies form. In this
form, you can do the following for the specific business partner:
To set default currency select the required currency row and choose Set as Default button. The default currency will be set
in new marketing documents and payments of this business partner. If required, you can change the currency in the
document itself.
To define which currencies will be hidden for the specific business partner’s documents, deselect the check box in the
Include column for each currency you wish to hide for this business partner. Based on this definition, you will only see the
included currencies in the specific business partner marketing documents and payments documents.
 Note
These settings only effect the currencies appearances in the business partner’s marketing and payments documents and can
be changed at any time.
 Note
Changing the currency assigned to the business partner is only allowed in the following cases:
No transactions were posted to the business partner master data yet.
If transactions are already posted to the business partner master data, and the assigned currency is other than All
Currencies, you can change the current currency to All Currencies. This change is irreversible.
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:06 AM
 Note
Assigning All Currencies to a business partner, enables you to carry out transactions with all currencies defined in SAP
Business One. For such business partners, all reports and reconciliations are calculated and displayed in the local currency
only.
 Note
Combining Business Partners assigned All Currencies with Business Partners assigned a local currency in a joint delivery
document is possible by using the Document Generation Wizard.
Federal Tax ID
Specify the Federal Tax ID of the business partner. This number is transferred to the documents.
 Note
Some countries have specific rules for defining the Federal Tax ID. If you specify an incorrect number, a message appears with
relevant information on how to specify the number.
Owner
Specify the employee who is the owner of the business partner.
When you manage data ownership by Business Partner Only or Business Partner and Document , the business partner owner will
be automatically drawn to the documents that are created for this business partner. By default, the business partner owner
becomes the document owner.
[Local Currency/System Currency/BP Currency]
Select the display currency for the amounts in the fields, Account Balance, Deliveries, Orders, and Opportunities.
The last three fields are not relevant for business partner master data of type vendor.
 Note
If the currency assigned to the business partner is either the local currency or All Currencies, you can choose between Local
Currency and System Currency. If you assigned a foreign currency to the business partner the option BP Currency is available
as well.
Account Balance
Bookkeeping balance of the customer or vendor account. SAP Business One updates the value automatically whenever an amount
is posted to the business partner’s account. Click to open the Account Balance window that displays the transactions resulting
in the displayed balance.
To display the account balance as a graph, choose . A window with the graph display of the account balance appears.
 Note
Not relevant for leads.
Deliveries
The value of open deliveries that are not yet fully copied into A/R invoices, returns, or closed. SAP Business One updates the value
automatically whenever a new delivery is added or the status of existing deliveries is changed. Click to open the Delivery
Balance window that displays the list of deliveries that brake down the value displayed in this field.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:06 AM
Relevant for customers only.
Orders
The value of open sales orders that are not yet delivered, canceled or closed. SAP Business One updates the value whenever a
sales order is created or if a delivery or an invoice is created on the basis of a sales order. Click to open the Sales Order Balance
window that displays the list of open sales orders created for the customer.
To display the orders as a graph, choose . A new window with the graph display of the orders appears.
 Note
Not relevant for vendors.
Goods Receipt PO
Displays the value of the open goods receipts POs and goods returns created for the given vendor. Click to open the Goods
Receipt PO Balance window, where the list of open documents is displayed.
 Note
This field is not relevant for customers or leads.
Opportunities
The number of open opportunities entered for the business partner. Lost and won opportunities are not counted. SAP Business
One updates the value automatically whenever an opportunity is added or the opportunity status changes. Click to open
Opportunities Report window that displays the list of open opportunities created for that business partner.
Purchase Orders
Displays the value of the open purchase orders created for the given vendor. Click to open the Purchase Order Balance window,
where the open documents are displayed.
 Note
This field is not relevant for customers and leads.
Checks
Displays the value of the open checks that are not yet deposited, endorsed or canceled. Click to open the Check Balance
window, where all the checks are displayed.
 Note
Relevant for customers only.
You Can Also
Select whether to view service calls, activities, opportunities, recurring transactions, blanket agreements, or service contracts
related to the business partner. In addition, you can create a new activity, service call, opportunity, quotation, order, invoice, or
credit memo.
More Information
Business Partner Master Data Window
Activity Window
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:06 AM
Activities Management
Activities Overview Report
Account Balance Window
Use this window to view the transactions posted to a G/L account or a business partner. According to the transactions, the balance
of the account or the business partner is calculated.
To access the window, proceed as one of the following:
To open the Account Balance Window for a G/L account, from SAP Business One Main Menu, choose Financials Chart
of Accounts , select the account, and click in the Balance field.
To open the Account Balance Window for a business partner, from SAP Business One Main Menu, choose Business
Partners Business Partner Master Data , and click in the Account Balance field.
Account Balance Window
Posting Date
Posting date of each transaction entry.
Trans. No.
Transaction number of each entry.
Origin
Original document type of a transaction entry.
Origin No.
Document number of each transaction entry.
Offset Account
Offset account of each transaction entry.
Details
Details of each transaction entry.
C/D (LC)
Credit or debit amount in local currency.
Cumulative Balance (LC)
Displays the account's total balance, recorded cumulatively with each posting, in local currency.
This field takes the amounts from the C/D (LC) field and not the Balance Due (LC) field. Therefore, the total of the Balance Due
(LC) is not the same as the Cumulative Balance (LC).
In addition, the Cumulative Balance (LC) field only shows the cumulative balance of the transactions displayed on the screen.
Therefore, the Cumulative Balance (LC) can differ when the option Display Unreconciled Trans. Only is selected or unselected.
Hence, this field should not be used to view the current balance of a business partner.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:06 AM
1. Go to Sales - A/R A/R Invoice and add an invoice with a total amount of 100.00.
2. Go to Banking Incoming Payments and add a partial payment of 40.00 against the A/R invoice.
3. Go to Business Partners Business Partner Master Data , you will find that the Account Balance is 60.00
Choose the Account Balance link arrow to open the Account Balance window, you will find that the Cumulative
Balance (LC) is 100.00.
Cumulative Balance Due (FC)
Displays in foreign currency the account's total balance, recorded cumulatively with each posting.
Balance Due (LC)
Balance due amount in local currency
Debit (LC)
Debit amount in local currency.
Credit (LC)
Credit amount in local currency.
Project
Displays the project specified in the corresponding journal entry of each transaction.
Distr. Rule
Displays the distribution rule specified in the corresponding journal entry of each transaction.
View by Control Account
To view the account balance categorized by control account, choose this button to open the Account Balance by Control Account
window.
Aging Report
To proceed with the aging report, choose this button to open the Vendor Liabilities Aging - Selection Criteria window.
Internal Reconciliation
To proceed with internal reconciliation, choose this button to open the Internal Reconciliation window.
More Information
Business Partner Master Data Window
BP Account Balance by Control Account
Context
You can display the account balance by business partner and by control account.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:06 AM
1. From the SAP Business One Main Menu, choose Business Partners Business Partner Master Data .
2. In the Business Partner Master Data window, open a business partner master record.
3. Click the arrow next to the Account Balance field.
The Account Balance – XXX window appears, where XXX stands for the selected business partner.
4. In this window, select View by Control Account.
The Account Balance by Control Account window appears, displaying totals by control account.
5. To see the detailed transactions, double-click one row.
Related Information
Business Partner Master Data: General Area
Business Partner Master Data: General Tab
Use this tab to enter general information about a business partner.
To access the tab, choose Business Partners Business Partner Master Data General .
General Tab Fields
Tel 1, Tel 2, Mobile Phone, Fax, E-Mail, Web Site
Specify the communication details of the business partner.
 Note
If you have Microsoft’s automatic phone dialer installed, you can press CTRL+TAB to automatically dial the numbers in the
telephone fields.
Shipping Type
Specify a shipping type for the business partner.
 Note
When you are creating a marketing document for a business partner, the shipping type on the Logistics tab will be the one
assigned to the business partner, while the shipping type in the item line will be the one assigned to the item. If no shipping type
is assigned to the item, the business partner's shipping type appears in the item line. However, you can always manuallly
update the shipping type on the line level and document level.
Password
Specify a password for e-commerce applications that integrate with SAP Business One.
Factoring Indicator
If required, assign a factoring indicator (both code and name) for the business partner. The indicator is automatically inserted as
the default value in invoices and can be displayed in the account statements.
BP Project
Select a project to associate with the business partner.
Type of Business
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:06 AM
Choose from Company, Private, Government and Employee. Use Private to represent sole proprietors. Use Employee to represent
an employee for use in expenses reimbursement under A/P Invoices and A/P Credit Memos.
Contact Person
Name of the default contact person specified on the Contact Persons tab.
ID No. 2
Specify any additional identification number for the business partner.
Unified Federal Tax ID
An ID to be used in case the company is part of group of companies or a child company connected to a parent company.
Company Reg. no. (CRN)
Type here the company registration number of the business partner. This number is used as a means of identification in contacts
with government authorities and other organizations.
Remarks
Specify any additional information related to the business partner.
Sales Employee/Buyer
For customers, select the default sales employee. For vendors, select the default buyer.
Commission Group
Specify a commission for the sales employee, either by entering a commission percentage for User-Defined Commission or by
selecting a predefined commission group. This field appears only if the option Set Commission by Customers is selected on the
BP tab in Administration System Initialization General Settings .
 Note
To define commission groups, choose Administration Setup General Commission Groups .
BP Channel Code
Specify a business partner serving as the channel partner of this customer. The channel partner will be automatically displayed in
documents created for the customer.
 Note
Relevant for customers only.
Technician
Specify a default technician (employee) for the customer.
 Note
Relevant for customers only.
Territory
Specify the territory to which this business partner belongs.
Personal Data Protection
For more information, see Personal Data Protection Management.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:06 AM
Natural Person: This setting can be selected when creating and adding data subjects to the system or through the
Personal Data Management Wizard.
Status: Updated depending on which data protection actions have been performed.
GLN (Global Location Number)
Represents an address or business partner. This field is alphanumeric and 50 characters long.
The GLN displayed in this form is retrieved from the Company Details window.
EDI Message
Specify the trading partner details by adding Sender and Recipient IDs.
Sender ID
The company or business partner sending the document. This field is alphanumeric and 50 characters long.
Recipient ID
The company or business partner receiving the document from the sender. This field is alphanumeric and 50 characters long.
Language
If the business partner is located abroad and you want to print documents in his local language, specify the required language. By
default, the company language is displayed.
 Note
Before you print documents for foreign business partners, ensure that the foreign language fields have been translated.
 Note
The field is only displayed if you have selected Multi-Language Support on the Company Details: Basic Initialization tab.
Generated from Campaign
Displays the no. of the campaign from which this business partner is generated.
To view the campaign, choose the icon.
Active
Displays additional fields that allow you to define a period in which the business partner is active.
 Note
When a business partner exceeds its active period, you can no longer post sales or purchasing documents for this business
partner. However, you can create draft documents.
Inactive
Displays additional fields that allow you to lock the business partner for a specified period.
 Caution
You cannot post sales or purchasing documents for a locked business partner.
Branch Assignment
Choose to open the Branch Assignment window to assign business partners to branches.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:06 AM
 Note
This field is available only if you have enabled multiple branches. For more information, see Working with Multiple Branches.
More Information
Business Partner Master Data Window
Business Partner Master Data: Contact Persons Tab
General Settings: BP Tab
Issuing Documents in the Customer's Language
Agents - Setup Window
Business Partner Master Data: Contact Persons Tab
Use this tab to add and update details about business partner contact persons.
To access the tab, choose Business Partners Business Partner Master Data Contact Persons .
The list of contact persons defined for this business partner is displayed on the left side of the tab. The details of the selected
contact person are displayed in the respective fields on the right side.
To add a new contact person, select the Define New row and enter the relevant information in the different fields.
To update an existing contact person, select the relevant contact ID row and update the relevant information in the different fields.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Contact Persons Tab Fields
E-Mail Group
When you assign an e-mail group to the given contact person, whenever an e-mail is sent to the selected e-mail group, this contact
person receives the e-mail.
To define a new e-mail group, choose the Define New option.
Remarks 1- 2
Specify any additional information about the contact person.
Password
Specify a password for connecting to e-commerce applications.
Place of Birth, Date of Birth, Gender, Profession
Specify personal information about the contact person.
Connected Address
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:06 AM
With the dropdown list, you can link the business partner’s existing Bill to, Pay to or Ship to address to the selected contact
person.
When you select a connected address, the address fields for the contact person will be replaced with the selected address
information, and become uneditable. When you update the connected address on the Addresses tab, it will be updated
automatically on the Contact Persons tab.
El. Doc. Recipient
Select this checkbox if the person should receive electronic documents. Make sure you specify the e-mail address of this contact
person.
Personal Data Protection
For more information, see Personal Data Protection Management.
Natural Person: This setting can be selected when creating and adding data subjects to the system or through the
Personal Data Management Wizard.
Status: Updated depending on which data protection actions have been performed.
Set as Default
Sets the selected contact person as default for the business partner.
 Note
The default contact person name is displayed on the General tab and is automatically assigned to all documents created for
the business partner.
 Note
To permanently delete a contact person, do one of the following:
Right-click on the Contact Persons tab and choose Remove Contact person
In the toolbar, choose Data Remove Contact Person
More Information
Business Partner Master Data Window
Business Partner Master Data: Addresses Tab
Use this tab to define business partner addresses, which are used as the default billing/paying and shipping addresses for the
various documents in SAP Business One.
To access the tab, choose Business Partners Business Partner Master Data Addresses .
To add a new address, under Bill to, Pay to, or Ship to, choose Define New.
For vendors, you can define as many Pay to and Ship to addresses as required.
For customers, you can define as many Bill to and Ship to addresses as required.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:06 AM
To delete an address, do one of the following:
In the address list on the left, select an address name on the left, and in the menu bar, choose Data Remove Address .
On the Addresses tab, right-click and select the Remove Address option.
Addresses Tab Fields
Address Related Fields
Specify the Address ID first, and then enter all address details.
GLN (Global Location Number)
Represents an address or a business partner. This field is alphanumeric and 50 characters long.
The GLN displayed on this tab is retrieved by default from the Company Details window.
Country/Region
The country/region selected when the company was created.
You can specify a different country/region. When specifying a Bill to/Pay to country/region other than the one defined for your
company, the following message appears: Change accounts receivable/payable?
Select Yes to change the control account of this business partner to the EU Accounts Receivable/Payable or the Foreign
Accounts Receivable/Payable defined in the G/L Account Determination window.
Select No to leave the Domestic Accounts Receivable/Payable as the control account for this business partner.
 Note
You can change the default country/region in the Pay to or Bill to address only under one of the following circumstances:
Business partner is connected to a sales opportunity, sales order, sales quotation, activity, or item.
Business partner is not connected to any document.
Set as Default
Sets the selected address as the default address for this business partner in all sales and purchasing documents or in incoming
and outgoing payments.
You can set one default Bill to/Pay to address and one Ship to address.
Default addresses are displayed in bold letters.
Show Location in Web Browser
Opens a Web browser and displays the business partner's location in a Web map with the browser. For more information, see
Working with Map Services.
Active
Set a business partner address as inactive by deselecting this checkbox. Inactive addresses will not appear in any address
dropdown lists.
Allow Changes in Address Components
If you deselect this checkbox, editing the address in the business partner master data will no longer be possible.
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:06 AM
More Information
Business Partner Master Data Window
G/L Account Determination
Business Partner Master Data: Payment Terms Tab
Use this tab to specify the business partner payment terms, which determine the due date of invoices related to the business
partner.
To access the tab, choose Business Partners Business Partner Master Data Payment Terms .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Payment Terms Fields
Payment Terms
Select the preferred payment terms, or define new ones.
 Note
If you change the payment terms displayed here, the following message appears:
Overwrite the BP's existing payment terms
To update existing fields according to the new selected payment terms, choose Yes.
To leave the data in the existing field although new payment terms were specified, choose No.
Interest on Arrears %
For information purposes, this specifies the interest rate for delayed customer payments.
Price Mode
This only appears if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Determine a default price mode for the business partner, which will be carried over to the sales or purchasing document that is
created for this business partner.
In order to add or update the business partner successfully, the selected mode must agree with the price mode of the price list
selected in the Price List field on this tab.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Price List
A price list linked to the selected payment terms or set as default in Administration System Initialization General Settings
BP tab. If required, select a different price list.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:06 AM
If you have selected the checkbox Enable Separate Net and Gross Price Mode in the Administration System Initialization
Company Details Basic Initialization tab, in order to add or update the business partner successfully, the price mode of the
selected price list must agree with the mode you have defined in the Price Mode field on this tab.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
 Note
Item prices in sales and purchasing documents are automatically taken from the price list selected in this field. Therefore, when
you link a certain price list to a business partner, make sure that the item prices are defined in this price list. Otherwise, no price
is displayed for the item in documents related to the business partner.
For more information, see Working with Item Prices in Sales and Purchasing Documents.
Total Discount %
The total discount linked to the selected payment terms. If required, you can enter a different value.
 Note
The discount is automatically calculated as a general discount in all sales or purchasing documents for this business partner.
Credit Limit
The credit limit linked to the selected payment terms. If required, you can enter a different value.
Commitment Limit
The commitment limit linked to the selected payment terms. If required, you can enter a different value.
Dunning Term
Select a predefined dunning term or add a new term in the Dunning Terms - Setup window.
 Note
Relevant for customers only.
Automatic Posting
This field only appears if you selected dunning terms for the business partner. The value is taken from the Dunning Terms – Setup
window.
Specify whether to automatically post interest and fee, interest only, or fee only when creating a dunning letter for a customer. If
you choose to automatically post interest and/or fee, a service invoice is created in the dunning run that posts the interest and/or
fee. To enable this, accounts for posting interest and fee must be specified. The default accounts are taken from the dunning
terms,. however you can change this setting by choosing the icon and specifying different accounts.
You can also choose not to post any interest or fee automatically.
Effective Discount Groups
Select one of the options for the discount calculation whenever there is more than one discount defined for the business partner in
the Discount Groups window.
Select one of the following:
Lowest Discount - The lowest available discount is taken (default).
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:06 AM
Highest Discount - The highest available discount is taken.
Average - The average of all available discounts is taken.
Total - The sum of all available discounts is taken.
Discount Multiples - The multiple of all available discounts is taken.
By default, when an effective discount is selected in the business partner group, it is displayed in this field. You can always change
the value in this field.
 Note
This field is only available when the Do Not Apply Discount Groups checkbox is not selected.
Effective Price
Define how to determine the price source in sales and purchasing documents when more than one price exists for the same item.
By default, the Default Priority option is displayed.
 Note
If there is a blanket agreement that is linked to the sales or purchasing document, the item price will be taken from that blanket
agreement, regardless of what option you select in this field.
Default Priority - the price will be taken from the sources in the following priority order:
1. Special Prices for Business Partners
The item price will be taken from the Special Prices for Business Partner window when the following conditions are
met:
The business partner and the line item in the document match the business partner and item defined in the
Special Prices for Business Partner window.
The document posting date falls within the validity period of the defined special prices.
2. Price defined in the Period and Volume Discounts window
The item price will be taken from the Period and Volume Discounts window when the following conditions are met:
The line item and the price list selected in the Form Settings window of the document match the item and
price list defined in the Period and Volume Discounts window.
The document posting date falls within the validity period of the defined discounted prices.
3. Price List Selected in the Document
The item price will be taken from the price list defined or selected in the Form Settings window of the document.
Lowest Price - SAP Business One calculates prices from all available price sources, and the lowest price will be taken.
Highest Price - SAP Business One calculates prices from all available price sources, and the highest price will be taken.
 Note
Discounts are taken into account in the determination of effective price.
If you have defined discount groups, the discount defined in the Discount Groups window applies to price source No.2 – the
Period and Volume Discounts window and price source No.3 – the Price List in Document; if you have not defined any discount
groups, the discount defined in source No.2 – the Period and Volume Discounts window, takes effect.
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:06 AM
For more information, see Working with Item Prices in Sales and Purchasing Documents.
Effective Price Considers All Price Sources
Select this checkbox to consider all price sources when calculating the effective price, no matter whether you have defined a
discount in the Discount Groups window or not. For more information, see How to Determine the Prices in Sales and Purchasing
Documents.
This checkbox is selectable when the Effective Price option is Highest Price or Lowest Price.
When this checkbox becomes selectable, it will take the value of the Effective Price Considers All Price Sources on the Pricing tab
of the General Settings window.
Business Partner Bank
Click and specify the business partner bank account in the Business Partner Bank Accounts – Setup window.
The bank account you specify:
Will be used for payments created by the payment wizard
Will be the default bank account for checks in incoming payments
Credit Card Type
Select the appropriate credit card type.
 Note
Relevant for customers only.
ID Number
Specify the identification number of the credit card holder.
Average Delay
Specify the average delay in days for payments from customers or to vendors. The specified value is taken into account in the cash
flow analysis and the expected payments are corrected accordingly in the analysis.
Priority
Specify the business partner priority in sales orders.
 Note
Priorities can be used as selection criteria in the Pick and Pack process.
Default IBAN
Specify the International Bank Account Number for domestic and foreign payment transactions.
If the default IBAN is specified, that value will be taken during bank file generation. If the default IBAN is not specified, the IBAN of
the selected business partner bank account on this tab will be taken during bank file generation.
Holidays
Select a predefined holiday schedule.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:06 AM
The schedule indicates dates when the business partner does not trade, thus affecting the due date of related sales or
purchasing documents.
Payment Dates
Opens the Payment Dates window in which you define the dates when the business partner receives (vendor) or makes
(customer) payments.
 Note
The dates affect the due date of the invoice and payment documents.
Allow Partial Delivery of Sales Order
Allows partial copying of rows from a sales order to a target document:
When selected, every new sales order you process for this business partner is automatically marked as Allow Partial
Delivery.
 Example
If a sales order contains five item rows, you can only copy three of the rows to a delivery document.
When deselected, you must copy the complete sales order to a target document.
 Note
Not relevant for vendors.
Allow Partial Delivery per Row
Allows partial copying of quantity from a sales order to a target document.
 Example
If a sales order contains a quantity of five in a certain item row, you can copy three of the items to a delivery document.
When deselected, you must copy all items in a row from a sales order to a target document.
 Note
The field is only displayed for customers and leads, and when Allow Partial Delivery of Sales Order is selected.
Do Not Apply Discount Groups
Defines whether the business partner is submitted to discounts definitions.
If you select the checkbox, the discount groups defined for this business partner are considered in his document, by default.
 Note
The discount in the document's header is not affected by the selection in this field.
When this checkbox is not selected, you can still define discounts manually in the document's rows and header.
When copying a document to a target document, the discounts from the base document are copied to the target
document regardless of what is defined in the Do Not Apply Discount Groups checkbox.
Endorsable Checks from This BP
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:06 AM
Select this checkbox to indicate that checks from this business partner can be endorsed. When this checkbox is selected, in the
payments created for this business partner, on the Check tab of the Payment Means window, the Endors. column is set to Yes by
default. This allows you to endorse this check using manual journal entries or directly in outgoing payments. However, you can
always change the Endors. status on the Check tab of the Payment Means window before adding the payment.
This checkbox is selected by default.
For more information about endorsing checks using manual journal entries, see Endorsing Checks Using Manual Journal Entry.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This checkbox is available for most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
This BP Accepts Endorsed Checks
Select this checkbox to enable using endorsable checks in outgoing payments to this business partner. When this checkbox is
selected, in the outgoing payments created for this business partner, on the Check tab of the Payment Means window, the
Endorse checkbox is available. Selecting the Endorse checkbox enables the Endorsable Check No. column, thus you can select
endorsable checks as a payment means.
This checkbox is deselected by default.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This checkbox is available for most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
More Information
Business Partner Master Data Window
Defining Payment Terms
Dunning Terms - Setup Window
Pick and Pack
Payment Dates
Business Partner Bank Accounts - Setup Window
In this window, you maintain bank information of the business partner.
To open the window, choose Business Partners Business Partner Master Data Payment Terms Bank Country Region
Country/Region
Displays the country/region code of the bank. The value is automatically displayed once you enter the bank code.
Bank Code
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:06 AM
Enter the code of the bank or choose one from the list.
Account No.
Enter the account number.
IBAN
International Bank Account Number
Specify the code to be used for banking transactions across international borders or for SEPA (Single Euro Payment Area)
transactions.
BIC/SWIFT Code
Specify the BIC/SWIFT code to be used in transactions and messages between banks. The default is taken from the Banks - Setup
window of the selected bank code.
Bank Account Name
Specify the name of the bank account.
Mandate ID
Specify the code to identify the direct debit mandate between the business partner and the company. Mandate ID must contain a
unique number; you cannot enter an already existing mandate ID.
Date of Signature
Specify the date on which the mandate is signed.
Branch No.
Enter the branch number of the bank.
Address Fields
Enter address details for each bank.
Control Key
Enter an additional control value.
User No. 1 - 4
Enter up to four user numbers or passwords to identify a payment file for a certain account.
Set as Default
Select the bank and choose the command pushbutton to define the bank as the default.
SEPA Seq. Type
SEPA Seq. Type (Single Euro Payment Area Sequence Type) is the sequence type of a direct debit mandate. SEPA Seq. Type is
copied to step 6 Recommendation Report of the Payment Wizard. SEPA Seq. Type can be edited directly in the payment wizard.
The options for SEPA Seq. Type include:
FRST: first
FNAL: final
OOFF: one-off
RCUR: recurring
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:06 AM
If two or more payments of the same mandate are arranged, the first payment needs to be marked as FRST and the next payment
needs to be marked as RCUR or FNAL. You cannot change SEPA Seq. Type from FRST to RCUR in Business Partner Bank
Accounts - Setup. SEPA Seq. Type is applicable to SEPA-relevant localizations only.
Payment Dates
Use this window to define the days each month when your customer usually pays the open invoices, or the days each month that
your company pays its vendors.
To open the window, choose Business Partners Business Partner Master Data Payment Terms Payment Dates .
Structure
In the Payment Dates window, enter the payment dates of the business partner.
Example
When 10 and 20 are defined for a certain customer, the invoice due dates are calculated as follows:
If the posting date is between the 1st and the 10th of the month, the due date of the invoice is the 10th of the same month.
If the posting date is between the 10th and the 20th of the month, the due date of the invoice is the 20th of the same
month.
If the posting date is after the 21st of the month, the due date of the invoice is the 10th of the next month.
 Note
If payment dates are defined in the Business Partner Master Data window, the invoice due date is determined by these
payment dates and not by the payment dates defined in the payment terms.
More Information
Business Partner Master Data: Payment Terms Tab
Business Partner Master Data: Payment Run Tab
Use this tab to specify options to be used in the Working with the Payment Wizard for the business partner.
To access the tab, choose Business Partners Business Partner Master Data Payment Run .
Payment Run Tab Fields
House Bank (Country/Region, Bank, Account, Branch, IBAN, BIC/SWIFT Code, Control No.)
From the dropdown lists, select the house bank account linking the offset account in journal entries created by the payment
wizard. Alternatively, click , and in the Choose Bank window, select the house bank account.
You can choose the button near the Bank or Account fields to open the Banks – Setup or the House Bank Accounts – Setup
windows respectively.
DME Identification, Instruction Key
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:06 AM
Relevant for the creation of the OPEX file by the Payment Engine add-on.
 Note
Relevant for European countries/regions, vendors only.
Reference Details
Designated for exporting bank transfer files and relevant for the OPEX file created by the payment wizard.
 Note
Relevant for European countries/regions only.
Payment Block
To define the business partner as blocked and exclude it from payment, select this checkbox and the proper payment block
reason.
 Note
All documents created for the business partner will be automatically defined as blocked from payment.
Single Payment
Defines that the payment wizard is to create a separate payment for each invoice.
When deselected, the payment wizard summarizes all open invoices of the business partner into one payment document, per
payment method.
Collection Authorization
Defines that the customer authorizes an automatic collection from his/her bank account. This field is also relevant for the OPEX
file created by the payment wizard.
 Note
When selected, the customer is not included in the dunning wizard.
 Note
Relevant for customers only.
Bank Charges Allocation Code
Select the required bank charges allocation code to be assigned to the business partner. SAP Business One saves the selected
code in the OPEX file that is processed by Payment Engine, and it is used for sorting and filtering.
Auto. Calculate Bank Charge for Incoming Payment
Select the checkbox to automatically calculate the difference between the transaction balance due and the total amount in the
Payment Means window as bank charges when you choose the Add in Sequence button in the Incoming Payments window.
 Note
Relevant for customers only.
Payment Methods
Customers can see all incoming payment methods. Vendors can see all outgoing payment methods.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:06 AM
If the Enable Negative Payment for Payment Wizard checkbox on the General tab of the Document Settings window is selected,
the list changes to the following:
For customers, the following appear in the table:
All incoming payment methods
All outgoing payment methods whose payment means is bank transfer
For vendors, the following appear in the table:
All outgoing payment methods
All incoming payment methods whose payment means is bank transfer
In this situation, you can only include the negative payment method by including its linked payment method, and only exclude the
negative payment method by excluding its linked payment method. For more information, see Payment Methods - Setup and
Paying Negative Totals Using the Payment Wizard.
 Note
To use the payment wizard for this business partner, you must set at least one active payment method as available. To do this,
select Include for the preferred active payment method.
 Note
To define new payment methods, from the SAP Business One Main Menu, choose Administration Setup Banking
Payment Methods .
Clear Default
Cancels the selection of a payment method as the default.
Set as Default
Sets the payment method selected in the table as the default method in all documents for the business partner.
 Note
On the General Settings: BP tab, you can select a default payment method for all business partners.
More Information
Business Partner Master Data Window
Defining Payment Blocks
General Settings: BP Tab
Defining Payment Blocks
Context
If you use the payment wizard to automatically issue and create incoming and outgoing payments, there might be cases where you
would want to exclude a specific business partner from the payment run. For this purpose you assign a payment block that
indicates the reason for the exclusion.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:06 AM
Use the procedure to define the payment blocks.
Procedure
1. From the SAP Business One Main Menu, choose Business Partner Business Partner Master Data Payment Run .
2. Select Payment Blocks.
3. In the field on the right, choose Define New.
The Payment Blocks – Setup window appears.
4. In the Payment Block field, enter a description of the payment block reason.
5. Choose Update.
 Note
The list is updated after each row entry.
Related Information
Business Partner Master Data: Payment Run Tab
Payment Blocks - Setup Window
Payment Blocks - Setup Window
Use this window to specify descriptions of payment blocks, which appear as options in the Payment Block field on the Business
Partner Master Data: Payment Run Tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Payment Blocks Fields
Payment Block
Specify a reason for the payment block.
More Information
Defining Payment Blocks
Business Partner Master Data Accounting Tab, General
Use this subtab to set accounting properties for business partners.
To access the tab, choose Business Partners Business Partner Master Data Accounting General .
General Tab Fields
Consolidating Business Partner
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:06 AM
There may be cases where you will need/want to consolidate the business activities carried out with several business partners to
specific business partner.
 Example
You have a customer who is chain store. Each branch is a separate business partner with whom you do business (receive
orders, issue deliveries, etc.) but the payments for the goods you deliver to the different branches are received from the main
office of the chain store. In this scenario, the consolidating business partner is the business partner master data record that
represents the main office, and the consolidation method will be Payment Consolidation. As a result, the A/R invoices you
issue for the different branches, will be assigned to the main office business partner to pay.
Specify here the business partner to consolidate the transactions of this business partner.
Payment Consolidation
Select to display invoices of business partners that are linked to the same consolidating business partner in the Incoming or
Outgoing Payments window.
When the head office pays for all invoices sent for its branches. In a specific payment document, you can select the branch
business partner directly.
Delivery Consolidation
Select to display deliveries of business partners that are linked to the same consolidating business partner in the Invoice window.
When the head office is invoiced for all deliveries shipped to its branches. In a specific Invoice document, you can select the branch
business partner directly.
Control Account
Opens the Control Accounts window where you set default control accounts for Assets, Open Debts, and in certain localizations
also Down Payments.
Accounts Receivable/Accounts Payable
Accounts Receivable - The control account to be recorded in all journal entries posted for a customer.
Accounts Payable - The control account to be recorded in all journal entries posted for a vendor.
The default control accounts are defined in the G/L Account Determination window.
Planning Group
If required, specify the planning group for use in the B1iSN integration scenario Liquidity Forecasting. The planning group is used
to process the liquidity forecasting report in SAP ERP.
Block Dunning Letters
Blocks the issuing of dunning letters for the customer.
Relevant for customers only.
Dunning Level
The highest dunning level for the customer.
If the customer is related to an invoice for which level 2 and level 3 dunning letters were sent, the value 3 is displayed.
Relevant for customers only.
Dunning Date
The last date when a dunning letter was issued.
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:06 AM
Relevant for customers only.
Use Shipped Goods Account
Available for customers only. Select this checkbox to post the delivery of the inventory to the shipped goods account instead of the
COGS account, when the delivery of inventory and the issue of the invoice occur in different posting periods.
Once you have selected the Use Shipped Goods Account for Customer checkbox on the Business Partner tab of the General
Settings window, the current checkbox will be selected by default for newly added customers.
 Note
This checkbox is available for perpetual inventory companies only.
Connected Vendor
This field is available only when the Type of a business partner is Customer.
If the business partner is also a vendor, you can create a new business partner with the Type of Vendor, and then enter the vendor
code in this field to connect these two types of business partners.
Connecting two types of business partners for one business partner enables you to view open transactions from both the vendor
and the customer side in the aging report and dunning wizard. It also enables you to reconcile open A/R transactions with open
A/P transactions.
Connected Customer
This field is available only when the Type of a business partner is Vendor.
If the business partner is also a customer, you can create a new business partner with the Type of Customer, and then enter the
customer code in this field to connect these two types of business partners.
Connecting these two types of business partners for one business partner enables you to view open transactions from both the
vendor and the customer side in the aging report and dunning wizard. It also enables you to reconcile open A/R transactions with
open A/P transactions.
 Note
If one business partner is connected to another, SAP Business One automatically creates an opposite connection. Thus, if the
current business partner is a customer, the connected business partner is a vendor, and vice versa. If you change the business
partner type of the current business partner, the connected business partner type changes accordingly.
More Information
Business Partner Master Data Window
Business Partner Master Data: Accounting Tab, Tax
Business Partner Master Data: Accounting Tab, Tax
Use this tab to specify tax information for business partners. To access the tab, choose Business Partners Business Partner
Master Data Accounting Tax .
Accounting Tab, Tax Fields
Tax Status
Select a tax status for the business partner:
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:06 AM
Liable - The business partner's transactions include tax calculations.
Exempt - The business partner's transactions do not include tax calculations.
EU - The customer's transactions include only tax groups defined as EU. Relevant only for Europe.
Acquisition - The vendor's transactions include only tax groups defined as Acquisition/Reverse. Relevant only for Europe.
 Note
The options can vary from one country/region to another.
Exempt No.
Specify the number of the exemption certificate.
 Note
Only relevant for customers whose Tax Status is Exempt.
Subject to Withholding Tax
Indicates that the vendor is subject to withholding tax.
 Note
Only available for vendors and if you have selected Withholding Tax on the Tax subtab of the Purchasing or Sales tab in the
G/L Account Determination window.
 Note
When Subject to Withholding Tax is selected, additional fields appear. Relevant only for some countries/region.
Certificate No./(UTR)
Specify the ID number of the withholding tax certificate:
For vendors, type the vendor's certificate number
For customers, type your company certificate number.
Expiration Date
Specify the date until which the credit card is valid. Up to 5 characters are allowed, use the format MM/YY for the date as shown
on the credit card, such as 04/10 for April 2010.
NI Number.
Specify the national insurance number.
WTax Codes Allowed
Opens the WTax Codes Allowed window where you select the withholding tax codes that can be used with the business partner.
 Note
You can set a default withholding tax code to be selected automatically in all documents created for the business partner.
Accrual / Cash
For information purposes, select the withholding tax report type.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:06 AM
Type for WTax Rpt
Select the type of report to be generated.
More Information
Business Partner Master Data Accounting Tab, General
G/L Account Determination: Purchase Tab
G/L Account Determination: Sales Tab
WTax Codes Allowed
Tax Exemption Letter
WTax Codes Allowed
Use this window to specify the withholding tax codes you want to make available for a specific business partner.
 Note
To add codes or modify existing ones, choose Administration Setup Financials Tax Withholding Tax.
WTax Codes Allowed Fields
Code
Withholding tax code, as defined in the Withholding Tax Codes – Setup window.
Description
Description ( WTaxName) of the withholding tax code, as defined in the Withholding Tax Codes – Setup window.
Choose
Select the withholding tax codes you want to allow for the business partner.
Set as Default
Sets the selected withholding tax code as default in all documents created for the business partner.
More Information
Withholding Tax Codes – Setup Window
Business Partner Master Data: Properties Tab
Use this tab to assign predefined properties to the business partner. You can use the properties as selection criteria for your
business partner reports.
To access the tab, choose Business Partners Business Partner Master Data Properties .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:06 AM
Defining Business Partner Properties
Business Partner Master Data Window
Business Partner Master Data: Remarks Tab
Use this tab to add descriptions, comments, notes, and images regarding the business partner.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
To access the tab, choose Business Partners Business Partner Master Data Remarks .
More Information
Business Partner Master Data Window
Activities Management
Activities refer to interactions you have with business partners, such as phone calls, meetings, tasks, or other types of activities.
You are able to manage a one-time activity, or recurring activities.
All activities, except the Email type, are automatically recorded in your calendar and in activity reports, which you can use to:
Plan your day, week, and month.
Analyze your communications with business partners, both currently open activities and activities that have been closed.
Monitor the progress of your sales and purchasing opportunities and the service calls of business partners.
All the images in this topic are interactive. Hover over each area for a description. Choose the highlighted areas for more
information.
The following image contains information about creating and managing activities.
Please note that image maps are not interactive in PDF outputs.
The following image contains information about activity management related windows.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:06 AM
Please note that image maps are not interactive in PDF outputs.
Activity Window
Use this window to add or update one-time, or recurring activities that you have pertaining to your business partners, such as
meetings, phones calls, notes and tasks, as well as to your private activities. All activities, except the Email type, are displayed in
the calendar.
To open the window, choose Business Partners Activity .
To perform different activities, select an activity from the Activity dropdown list.
Related Information
Activity: General Area
Activity: General Tab, Phone Call
Activity: General Tab, Meeting
Activity: General Tab, Task
Activity: General Tab, Email
Activity: General Tab, Note
Activity: General Tab, Other
Activity: Content Tab
Activity: Linked Document Tab
Activity: Attachments Tab
Activity: General Area
Use this area to enter the main information about an activity.
To access the area, choose Business Partners Activity .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area Fields
Activity
Specify a suitable type for your activity.
Type
Select a more detailed classification of the activity.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:06 AM
 Example
You can classify Meeting as First Meeting, Presentation, and Follow-Up.
 Note
You can activate or deactivate an activity type. From the Type dropdown list, choose Define New, and in the Activity Types -
Setup window, select the checkbox to activate an activity type, or deselect to deactivate it. Deactivated types are not displayed
in the dropdown list.
Subject
Select another detailed classification of the activity.
 Example
Typical subjects are products, business area and so on.
 Note
You can activate or deactivate an activity subject. From the Subject dropdown list, choose Define New, and in the Activity
Subjects - Setup window, select the checkbox to activate an activity subject, or deselect to deactivate it. Deactivated subjects
are not displayed in the dropdown list.
Assigned To
From predefined lists of users and employees in your company or a self-defined recipient list, select the user or employee, or a
combination of users, employees and recipient lists that are handling the activity. By default, the user who created the activity is
displayed.
 Note
Employees that are linked to users are only displayed as users in the user list. When all employees are linked to users or there is
no employee, you can assign the activity to a user only.
When an employee is linked to a user, the activities originally assigned to the employee are automatically assigned to the user
instead of the employee.
A self-defined recipient list can contain one or more users, employees, and existing recipient lists.
To add recipients to the activity with the Recipient List function, follow the steps below:
1. In the Assigned To field of the Activity window, choose Recipient List. All the recipient lists can be found in the field on the
right.
2. At the bottom of the list of recipient lists, choose Define New. The Add Recipient window appears.
3. The displayed window has Users, Employees, and Recipient Lists tabs. (The Employees tab is displayed only if there are
employees that are not linked to any user.) On these tabs, select the checkboxes of the users and existing recipient lists to
which you want to assign this activity.
If you choose:
a. a single user or a single recipient list, and then choose OK – the user or the recipient list name is displayed in the
field
b. multiple users, or multiple recipient lists, or a combination of users and recipient lists, and then choose OK –
Multiple is displayed in the field
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:06 AM
c. multiple users, or multiple recipient lists, or a combination of users and recipient lists, and then choose Save as
Recipient List – you will need to give the new recipient list a name, and then this name is displayed in the field
To activate or deactivate a recipient list, follow these steps:
1. In the Assigned To field of the Activity window, choose Recipient List. A list of recipient lists can be found in the field on the
right.
2. At the bottom of the list of recipient lists, choose Define New. The Add Recipient window appears.
3. On the Recipient Lists tab of the displayed window, select the checkbox before Active to activate a recipient list, or, vice
versa, deselect the checkbox to deactivate it.
To remove members from a specific recipient list, following these steps:
1. In the Assigned To field of the Activity window, choose Recipient List. A list of recipient lists can be found in the field on the
right.
2. In the list of recipient lists, choose the recipient list that you want to edit.
3. Choose the link arrow to display the window of the specific recipient list.
4. Select the number before a user or a recipient name, and then choose Remove.
5. Choose Update to finish editing.
 Note
You can only remove a recipient list that has not been linked to any activity.
Personal
Indicates that the activity is of a personal nature.
 Note
Although an activity is defined as Personal, other users can see it.
Number
Unique activity number that is automatically assigned to each new activity.
BP Code, Type
Select a business partner code to relate to the activity. The type of the business partner is automatically displayed in the field on
the right.
 Note
If you create the activity through a document/window in which a specific business partner appears, this business partner is
automatically selected in the Activity window.
 Note
If Personal is selected, or Purchase Request is selected as the document type on the Linked Document tab, you do not have to
select a business partner code.
Contact Person
Default contact person defined for the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:06 AM
 Note
If several contact persons are defined for the business partner, you can select a different contact person. You can also leave the
field blank.
Telephone No.
Phone number of the selected contact person.
 Note
If a phone number is not defined for this person, the business partner's phone number is displayed.
More Information
Creating and Updating Activities
Activity Statuses - Setup
Use this window to define various activity statuses.
Status Name
Enter a status name as you want.
Status Description
Specify the description of the activity status you defined.
More Information
Activity Window
Activity: General Tab, Phone Call
Use this tab to enter general information about a phone call.
To view the fields for phone calls, choose Business Partners Activity, and select Phone Call as the activity.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab, Phone Call Fields
Remarks
Shortly, describe the phone call.
Start Time
Specify the date and time for the start of the phone call. By default, the system date and time are displayed.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:06 AM
 Note
When you define an activity as a recurring activity, the date of the Start Time and the value in the Repeat on section are
interdependent.
End Time
Specify the time for the conclusion of the phone call. By default, the end time is set to fifteen minutes past the start time.
 Caution
You cannot set the end time to a time earlier than the start time.
Duration
Specify the length of time you expect the phone call to take. By default, the duration is set to fifteen minutes. If you change it, the
end time is updated accordingly.
 Note
To specify minutes, enter the number of minutes followed by the letter M. To specify hours, enter the number of hours followed
by the letter H. To specify days, enter the number of days followed by the letter D.
Recurrence
Used for setting recurring activities. It is only available for Phone Call, Meeting, or Task.
The default value is None that stands for non-recurring activities. Select from the dropdown list to define the frequency of the
recurring activity. You can define a daily, weekly, monthly, or annually activity.
Repeat Every
Use it to define the frequency for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For daily activities, to schedule the activity on every working day, select the radio button Every Weekday. Alternatively,
1. Select the first radio button.
2. Specify the daily frequency. The value should be a number between 1 and 6.
For weekly, monthly, or annually activities, specify the frequency that the activity takes place. The value should be a number
between 1 and 4.
For weekly activities, specify a number between 1 and 4.
For monthly activities, specify a number between 1 and 12.
For annually activities, specify a number between 1 and 10.
Repeat on
Use it to define the date when the activity recurs. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For weekly activities, select the days when the activity recurs. You can select multiple days.
For monthly activities, select from the two radio buttons to define the date when the activity recurs. The value of the first
radio button cannot exceed the number of days of the month specified in the Start Time field above.
For annual activities, select from the two radio buttons to define the date when the activity recurs.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:06 AM
 Note
For the second dropdown list of the second radio button for both monthly and annual activities, the ranges of weekdays and
weekends are decided by the values specified in the Weekend From ... To ... field in the Holiday Dates window. For more
information, see Holiday Dates Window.
Range
Use it to define the range for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
Select from the three radio buttons and specify the end date for the activity. You can:
Leave the end date open.
End the activity after certain occurrences.
End the activity by a certain date.
Specify the date in the mm/dd/yy format.
Reminder
Displays a reminder in the Messages/Alert Overview window prior to the time set for the phone call.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
 Note
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Inactive
Inactivates the activity and removes it from your calendar. You can still update and reactivate it.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
Follow Up
Opens a new Activity window where you can enter a follow-up activity.
No follow up is available for recurring activities.
 Note
To enter a follow-up activity, you must first add the current activity.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:06 AM
Creating and Updating Activities
General Settings: Services Tab
Activity: General Tab, Meeting
Use this tab to enter general information about a meeting you want to view in the calendar, such as a meeting with a business
partner, or a personal meeting.
To view the fields for meetings, choose Business Partners Activity, and select Meeting as the activity.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab, Meeting Fields
Remarks
Shortly, describe the meeting.
Start Time
Specify the date and time for the start of the meeting. By default, the system date and time are displayed.
 Note
When you define an activity as a recurring activity, the date of the Start Time and the value in the Repeat on section are
interdependent.
End Time
Specify the time for the conclusion of the meeting. By default, the end time is set to fifteen minutes past the start time.
 Caution
You cannot set the end time to a time earlier than the start time.
Duration
Specify the length of time you expect the meeting to take. By default, the duration is set to fifteen minutes. If you change it, the
end time is updated accordingly.
 Note
To specify minutes, enter the number of minutes followed by the letter M. To specify hours, enter the number of hours followed
by the letter H. To specify days, enter the number of days followed by the letter D.
Address
Specify the address details of the meeting location.
 Note
To automatically specify a business partner’s address, select Business Partner Address in the Meeting Location field and
select an address ID in the Address ID field. The details of the business partner's default (or first, if no default address is
specified) Ship to address are automatically applied.
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:06 AM
Manually editing the meeting location address details in the Activity window does not change the business partner's address
information.
Recurrence
Used for setting recurring activities. It is only available for Phone Call, Meeting, or Task.
The default value is None that stands for non-recurring activities. Select from the dropdown list to define the frequency of the
recurring activity. You can define a daily, weekly, monthly, or annually activity.
Repeat Every
Use it to define the frequency for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For daily activities, to schedule the activity on every working day, select the radio button Every Weekday. Alternatively,
1. Select the first radio button.
2. Specify the daily frequency. The value should be a number between 1 and 6.
For weekly, monthly, or annually activities, specify the frequency that the activity takes place. The value should be a number
between 1 and 4.
For weekly activities, specify a number between 1 and 4.
For monthly activities, specify a number between 1 and 12.
For annually activities, specify a number between 1 and 10.
Repeat on
Use it to define the date when the activity recurs. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For weekly activities, select the days when the activity recurs. You can select multiple days.
For monthly activities, select from the two radio buttons to define the date when the activity recurs. The value of the first
radio button cannot exceed the number of days of the month specified in the Start Time field above.
For annual activities, select from the two radio buttons to define the date when the activity recurs.
 Note
For the second dropdown list of the second radio button for both monthly and annual activities, the ranges of weekdays and
weekends are decided by the values specified in the Weekend From ... To ... field in the Holiday Dates window. For more
information, see Holiday Dates Window.
Range
Use it to define the range for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
Select from the three radio buttons and specify the end date for the activity. You can:
Leave the end date open.
End the activity after certain occurrences.
End the activity by a certain date.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:06 AM
Specify the date in the mm/dd/yy format.
Reminder
Select to display a reminder in the Messages/Alert Overview window prior to the time set for the meeting.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
 Note
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Tentative
Indicates that you are not certain the meeting will occur.
Inactive
Inactivates the activity and removes it from your calendar. You can still update and reactivate it.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
Follow Up
Opens a new Activity window where you can enter a follow-up activity.
No follow up is available for recurring activities.
 Note
To enter a follow-up activity, you must first add the current activity.
More Information
Creating and Updating Activities
General Settings: Services Tab
Activity: General Tab, Task
Use this tab to enter general information about a task.
To view the fields for tasks, choose Business Partners Activity, and select Task as the activity.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:06 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab, Task Fields
Remarks
Shortly, describe the task.
Start Time
Specify the date and time for the start of the task. By default, the system date and time are displayed.
 Note
When you define an activity as a recurring activity, the date of the Start Time and the value in the Repeat on section are
interdependent.
End Time
Specify the date and time for the conclusion of the task. By default, the end time is set to fifteen minutes past the start time.
 Note
When you define the activity as a recurring activity, the starting date is determined by the value you select in the Repeat on
field.
Recurrence
Used for setting recurring activities. It is only available for Phone Call, Meeting, or Task.
The default value is None that stands for non-recurring activities. Select from the dropdown list to define the frequency of the
recurring activity. You can define a daily, weekly, monthly, or annually activity.
Repeat Every
Use it to define the frequency for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For daily activities, to schedule the activity on every working day, select the radio button Every Weekday. Alternatively,
1. Select the first radio button.
2. Specify the daily frequency. The value should be a number between 1 and 6.
For weekly, monthly, or annually activities, specify the frequency that the activity takes place. The value should be a number
between 1 and 4.
For weekly activities, specify a number between 1 and 4.
For monthly activities, specify a number between 1 and 12.
For annually activities, specify a number between 1 and 10.
Repeat on
Use it to define the date when the activity recurs. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
For weekly activities, select the days when the activity recurs. You can select multiple days.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:06 AM
For monthly activities, select from the two radio buttons to define the date when the activity recurs. The value of the first
radio button cannot exceed the number of days of the month specified in the Start Time field above.
For annual activities, select from the two radio buttons to define the date when the activity recurs.
 Note
For the second dropdown list of the second radio button for both monthly and annual activities, the ranges of weekdays and
weekends are decided by the values specified in the Weekend From ... To ... field in the Holiday Dates window. For more
information, see Holiday Dates Window.
Range
Use it to define the range for the recurring activity. It is only available for Phone Call, Meeting, or Task, when the value of
Recurrence is not None.
Select from the three radio buttons and specify the end date for the activity. You can:
Leave the end date open.
End the activity after certain occurrences.
End the activity by a certain date.
Specify the date in the mm/dd/yy format.
Reminder
Select to display a reminder in the Messages/Alert Overview window prior to the time set for the meeting.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
 Note
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Inactive
Inactivates the activity and removes it from your calendar. You can still update and reactivate it.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
More Information
Creating and Updating Activities
General Settings: Services Tab
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:06 AM
Activity: General Tab, Email
Use this tab to enter general information about an activity of the Email type.
To email all specified recipients, open the activity, and choose Send in the Send Message window ( File Send SAP Business
One Mailer ). The email will use the activity remarks as the subject and the activity content as the body. You can make any further
changes in the Send Message window, but these changes will not be saved back to the activity. Once you choose Send, the
Emailed checkbox in the activity will then be selected, and further edits to this activity will not be possible. You can check the sent
email in the Messages/Alerts Overview window.
 Note
This type of activities does not appear in the calendar.
To view the fields for activities of the Email type, choose Business Partners Activity , and select Email as the activity.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab, Email Fields
Remarks
Define the email subject.
Time
Specify a date and time related to the activity. By default, the system date is displayed.
Priority
Set the email priority.
Email Recipients
Choose recipients from users, employees, contact persons, distribution lists, or enter email addresses manually. Employees linked
to users will only appear as users in the user list.
Reminder
Displays a reminder in the Messages/Alert Overview window prior to the time set for the activity.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
 Note
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Emailed
This checkbox is automatically selected when you choose Send in the Send Message window ( File Send SAP Business One
Mailer ).
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:06 AM
 Caution
You cannot modify an emailed activity.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
Follow Up
Opens a new Activity window where you can enter a follow-up activity.
 Note
To add a follow-up activity, you must first add the current activity.
Activity: General Tab, Note
Use this tab to enter general information about a note.
To view the fields for notes, choose Business Partners Activity, and select Note as the activity.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab, Note Fields
Remarks
Shortly, describe the note.
Time
Specify a date and time related to the note. By default, the system date is displayed.
Reminder
Displays a reminder in the Messages/Alert Overview window prior to the time set for the note.
Specify the reminder in minutes or hours. To enter hours, type the number of hours followed by the letter H.
 Note
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Inactive
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:06 AM
Inactivates the activity and removes it from your calendar. You can still update and reactivate it.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
More Information
Creating and Updating Activities
General Settings: Services Tab
Activity: General Tab, Other
Use this tab to enter general information about an activity that you cannot fit into any of the predefined activity types.
To view the fields for other activities, choose Business Partners Activity, and select Other as the activity.
General Tab, Other Fields
Remarks
Shortly, describe the activity.
Start Time
Specify the date and time for the start of the activity. By default, the system date is displayed.
End Time
Specify the time for the conclusion of the activity. By default, the end time is set to fifteen minutes past the start time.
 Caution
You cannot set the end time to a time earlier than the start time.
Duration
Specify the length of time you expect the activity to take. By default, the duration is set to fifteen minutes. If you change it, the end
time is updated accordingly.
 Note
To specify minutes, enter the number of minutes followed by the letter M. To specify hours, enter the number of hours followed
by the letter H. To specify days, enter the number of days followed by the letter D.
Reminder
Displays a reminder in the Messages/Alert Overview window prior to the time set for the activity.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:06 AM
The reminder is displayed according to the settings on the Services tab in Administration System Initialization General
Settings .
 Note
When you assign an activity to an employee, the Reminder checkbox is not available.
Inactive
Inactivates the activity and removes it from your calendar. You can still update and reactivate it.
Closed
Closes the activity.
 Note
You cannot modify a closed activity. To reopen a closed activity, right-click it and choose Reopen in the context menu.
Follow Up
Opens a new Activity window where you can enter a follow-up activity.
 Note
To enter a follow-up activity, you must first add the current activity.
More Information
Creating and Updating Activities
General Settings: Services Tab
Activity: Content Tab
Use this tab to briefly describe the meeting, phone call, or any other event that took place during the activity.
To access the tab, choose Business Partners Activity Content .
 Note
For activities of the Email type, the activity content will be used as the email body.
More Information
Creating and Updating Activities
Activity: Linked Document Tab
Use this tab to:
Link a document to an activity
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:06 AM
View the linked opportunity or service call from which an activity was created
View the base activity, if an activity is a follow-up
 Example
If you make a phone call regarding a certain sales order, you can link the relevant order.
To access the tab, choose Business Partners Activity Linked Document .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Linked Document Tab Fields
Document Number
Specify the number of the linked document.
 Note
You can only specify documents matching the selected document type.
Show Documents Related to the BP
Filters the selection of documents so that only documents related to the selected business partner appear in the list of documents
for selection.
 Note
This checkbox will be not available if you have selected the linked document type to be Purchase Request, Deposits, Journal
Entries, or Campaign Management.
Source Object Type
Indicates if the activity was created from a service call or a sales or purchasing opportunity.
Source Object No.
Service call or opportunity number from which the activity was created.
Previous Activity
Number of the base activity, if the activity is a follow-up.
More Information
Creating and Updating Activities
Activity: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:06 AM
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
Creating and Updating Activities
General Settings: Path Tab
Creating and Updating Activities
Use the procedures to manage a one time activity, or recurring activities.
Procedure
Creating Activities
1. From the SAP Business One Main Menu, choose Business Partners Activity .
The Activity window opens.
2. In the Activity field at the top, select the type of activity you want to create.
3. Do one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:06 AM
If the activity is related to a business partner, specify the partner in the BP Code field.
If the activity relates only to yourself, select Personal.
4. Enter any other required information about the activity. For more information, see Activity Window.
5. To save the activity, choose Add.
 Note
By duplicating an existing activity, you can also create a new activity. For more information, see Duplicating Activities.
Updating Activities
1. From the SAP Business One Main Menu, choose Business Partners Activity .
The Activity window opens.
2. Display the required activity using standard search functions.
3. Modify the activity information, as required.
4. Choose Update.
More Information
Business Partner Reports
Duplicating Activities
Context
An activity can be duplicated with values in certain fields copied to the new activity. The number of the new activity is the next
available number.
Procedure
1. From the SAP Business One Main Menu, choose Business Partners Activity .
2. In the Activity window, display the required activity using standard search functions.
3. Duplicate the activity using one of the following three methods:
Right-click anywhere in the Activity window, except for the Attachments table, and choose Duplicate.
Press Ctrl + D .
Choose Data Duplicate .
4. The new activity opens in Add mode with values in the following fields or areas copied from the existing activity:
General Area: Activity, Type, Subject, Assigned To, Personal checkbox.
General Tab: Remarks
Content Tab
Fields whose values are not copied are filled with default values, if any.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:06 AM
Related Information
Creating and Updating Activities
Closing, Disabling, and Deleting Activities
Use these procedures to:
Disable one-time or recurring activities so that they do not appear in the calendar or in reports
Close one-time or recurring activities that are no longer relevant
Delete one-time or recurring activities, even if they are related to service calls, opportunities, or activity-related reports
Procedure
Disabling Activities
1. From the SAP Business One Main Menu, choose Business Partners Activity .
2. In the Activity window, display the required activity using standard search functions.
3. On the General tab, select Inactive.
 Note
To reactivate an activity, deselect Inactive.
 Note
For activities of the Email type, there is no Inactive checkbox.
4. Choose Update.
Closing Activities
1. From the SAP Business One Main Menu, choose Business Partners Activity .
2. Display the required activity using standard search functions.
3. Select Closed and choose Update.
4. To confirm, choose Yes in the system message.
 Note
Closed activities can be reopened. In the Closed Activity window, right-click and choose Reopen.
Deleting Activities
1. From the SAP Business One Main Menu, choose Business Partners Activity .
2. Display the required activity using standard search functions.
3. From the menu bar choose Data Remove .
4. To confirm, choose Yes in the system message.
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:06 AM
 Note
When you remove recurring activities, the system asks you:
Would you like to remove only this event, only unchanged events of this recurrence or all
events of this recurrence?
Select one of the following radio buttons: Only this event, Remove only unchanged events, or Remove all events and choose
OK.
 Note
To remove a closed activity, display the required activity, right-click, and choose Remove.
More Information
Adding and Updating Activities
Creating Activities in the Calendar Window
Procedure
1. From the menu bar, choose Window Calendar .
Alternatively, click the icon in the tool bar.
The Calendar window appears.
2. In the calendar, double-click a cell to open the Activity Window.
 Note
To create an activity with a time period of more than one cell, select the relevant cells for the time period and press
Enter . The activity's Start Time and End Time correspond to the time of the selected cell(s).
3. Enter the required data for the activity.
4. Choose Add.
Related Information
Calendar Window
Calendar Window
Use the calendar to view, add, or update meetings, phone calls, task activities, and other activities.
To open the calendar, from the menu bar, choose Window Calendar , or alternatively click the icon in the tool bar.
To view the activities, absences, and education information of employees that are not linked to users, you must have made the
following selections in the Calendar Settings window:
On the Work Week tab, you have selected the Apply Employee Absence and Education checkbox.
On the Users tab, you have selected the employee whose information you want to view and made relevant selections.
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:06 AM
 Note
You can reschedule activities using drag and drop. Depending on the calendar settings (see Defining Calendar Settings)
the activity is either opened or automatically placed in its new location.
Note activities are not displayed.
More... appearing in a column header of the calendar indicates that more than three activities are entered at a specific
time of a day. To view a list of all the activities of the day, double-click More... in the column header.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Calendar Fields
Date
Date displayed in the calendar. By default, the current date is displayed.
Go
Applies the specified date in the calendar.
Today
Applies the current date in the calendar.
Week
Displays a regular week in the calendar.
 Note
You can set the first day of the week on the Work Week tab in the Calendar Settings window.
Work Week
Displays the working days of a week in the calendar.
 Note
You can set working days on the Work Week tab in the Calendar Settings window. The work week considers company holidays.
Group View
Groups activities, absences, education, and service calls information of users and employees specified on the Users tab in the
Calendar Settings window, by each user or employee.
Enables viewing activities, absences, and education information of up to seven users and employees for a certain day.
 Note
Available in the Day view only.
Show Activities
Select activities to display or hide in the calendar.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:06 AM
More Information
Activity Window
Calendar Settings: Work Week Tab
Calendar Settings: Users Tab
Creating Activities in the Calendar Window
Procedure
1. From the menu bar, choose Window Calendar .
Alternatively, click the icon in the tool bar.
The Calendar window appears.
2. In the calendar, double-click a cell to open the Activity Window.
 Note
To create an activity with a time period of more than one cell, select the relevant cells for the time period and press
Enter . The activity's Start Time and End Time correspond to the time of the selected cell(s).
3. Enter the required data for the activity.
4. Choose Add.
Related Information
Calendar Window
Defining Calendar Settings
Procedure
1. From the menu bar, choose Window Calendar .
Alternatively, click the icon in the tool bar.
The Calendar window appears.
2. To open the Calendar Settings window, choose .
On the Calendar Settings – General Tab, define color schemes and general display settings.
On the Calendar Settings – Work Week Tab, define working days and working hours.
On the Calendar Settings – Users Tab, define display settings for users and employees.
3. Choose Update, then OK.
Related Information
Calendar Window
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:06 AM
Calendar Settings: General Tab
Use this tab to define general display settings for the calendar.
To access the tab, choose , then .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Calendar Settings, General Tab Fields
Automatically confirm when dragging an activity
If deselected - When dragging an activity to a new time and/or date, the Activity window opens, in which you can view the
activity details before confirming the rescheduling.
If selected - When dragging an activity to a new time and date, the activity is automatically confirmed and rescheduled.
Automatically confirm when dragging a service call
If deselected - When dragging a service call to a new time and/or date, the Service Call window opens, in which you can
view the service call details before confirming the rescheduling.
If selected - When dragging a service call to a new time and date, the service call is automatically confirmed and
rescheduled.
Show Personal Activities
Displays activities defined as Personal.
 Note
The icon representing personal activities is slightly different from regular activities.
Minutes per Row
Select to divide the rows into intervals of 15, 30, 60 or 120 minutes.
Color Rows
By double-clicking the color bars, you can define different colors for different calendar items, including working hours, non working
hours, activities, service calls, and employee absence and education information.
More Information
Defining Calendar Settings
Activities Management
Calendar Settings: Work Week Tab
Use this tab to define the beginning and end of the work week, and to apply holidays, employee absences, and employee education
information to the calendar.
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:06 AM
To access the tab, choose , then .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Work Week Tab Fields
Display
Selected days are displayed as working days in the calendar.
 Note
The Work Week view displays only the selected working days. In other views, the working days have a different color than the
non-working days.
Start of Day, End of Day
Sets a range of working hours, which are displayed in a separate color in any view showing hours.
Apply Holidays
Applies a predefined set of holidays to the calendar.
 Note
The holidays definition here does not affect forecasts and MRP calculation. To define proper holidays to be considered by MRP
calculation and forecasts, see the Holiday Dates Window.
Apply Employee Absence and Education
Enables viewing employee absences and education information in the calendar. However, if an employee is linked to a user, the
absence and education information of the employee is applied to the user instead.
More Information
Defining Calendar Settings
Activities Management
Company Details: Accounting Data Tab
Calendar Settings: Users Tab
Use this tab to specify users or employees whose activities you would like to view.
To access the tab, choose , then .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Calendar Settings, Users Tab Fields
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:06 AM
Display Employees
Enables viewing employee activities, absence, and education information. However, employees that are already linked to users are
not displayed in this list; instead, they are displayed as users in the upper user list.
 Note
If you deselect this checkbox, any selections made for the employees are not saved.
Period View
Select to display the user's or employee’s activities, absences, education, and service calls information in Month, Week, Work
Week, and Day views.
Group View
Select to display the user or employee's activities, absences, education, and service calls information in the Group View.
 Note
No more than seven users and employees can be displayed in the Group View simultaneously.
Color
Opens a color palette from which you can choose a color for each user's or employee's activities, as well as absences and
education information.
More Information
Defining Calendar Settings
Activities Management
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
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:06 AM
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
latter, see Displaying Available Blanket Agreements.
4. When the planned quantity of the agreement has been reached, you issue a credit memo for your customer, or, if you are
the buyer, receive a credit memo from your vendor. To record this in the system, create an A/R credit memo or A/P credit
memo without inventory movement.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:06 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:06 AM
Business partner code or name
Start date of the agreement
End date of the agreement
3. Optional: In the Description field, enter a short description of the blanket agreement.
4. On the General tab, select the agreement type Specific and do the following:
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
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:06 AM
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
The agreement status changes to Terminated and further sales or purchases associated with this agreement can only be
made if the posting date of the sales or purchasing document lies between the start date and the termination date of the
agreement.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:06 AM
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
Once you choose a blanket agreement, the Draw Document Wizard (DDW) allows you to either choose Draw All Data or
Customize. If you select Customize, you can select the rows you want to copy.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:06 AM
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
You can change the date when no document is linked to the blanket agreement, and the status of the blanket agreement is On
Hold.
End Date
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:06 AM
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
The monetary value of those items that are included in sales or purchasing transactions associated with the blanket agreement.
This value is filled in by the system.
Open Amount
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:06 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:06 AM
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
SAP Business One checks whether a blanket agreement for this customer exists that is valid at the specified posting date
and covers the desired items. If there is such an agreement, it enters the blanket agreement number into the Blanket
Agreement column for each item. It also inserts the unit prices agreed upon in the blanket agreement. If the Ignore Prices
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:06 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:06 AM
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
Descriptive text for the agreement, if required.
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:06 AM
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
When you copy multiple blanket agreements to a marketing document, and the payment methods defined in the
blanket agreements are not the same, the document payment method remains unchanged.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:06 AM
When a blanket agreement is linked to the document lines without using the Copy To function, the payment method
defined in the blanket agreement has no impact on the document.
Shipping Type
Define a shipping type for the blanket agreement.
When a blanket agreement is associated with a marketing document, either automatically or manually, the shipping type defined
in the blanket agreement will be taken into the Shipping Type field in the document.
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
Appears only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:06 AM
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
Enter the item prices that you agreed on with the business partner.
Cumulative Committed Quantity
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:06 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:06 AM
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
In the MRP run, the application subtract the item's open quantities in blanket agreements with the type of Specific from the
forecasted quantities.
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:06 AM
For more information, see Managing Forecasts.
Activity
To record an activity, such as a phone call or meeting, associated with the blanket agreement, click the yellow arrow and specify
the required information.
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
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:06 AM
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
Internal Reconciliations
As a part of the bookkeeping process, internal reconciliation is about matching and clearing transactions for business partners or
for G/L accounts. In SAP Business One, part of the internal reconciliation process is done automatically by the application, and
part of it can be done manually.
Most of the time, internal reconciliation takes place automatically, for example, when you create incoming or outgoing payments
linked to invoices. In this case, SAP Business One automatically reconciles payments with the linked invoices. However, a
standalone transaction, such as a payment on account, is unable to be automatically reconciled, as SAP Business One cannot
know to which open invoices the payment relates. Therefore, you need to decide to which invoice the payment is to be applied and
perform the reconciliation manually.
For both the automatic system reconciliations and the manually performed reconciliations, SAP Business One enables you to view
the reconciliation details, and if necessary, cancel previous reconciliations in some cases.
More Information
Automatic System Reconciliation
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:06 AM
Reconciliation
Manage Previous Reconciliations
Automatic System Reconciliation
In SAP Business One, automatic system reconciliation applies in various scenarios where it is possible to match the debit and
credit postings of certain transactions, or where manual reconciliation is difficult to carry out.
The automatic system reconciliation can be full or partial depending on the different cases. It facilitates the internal reconciliation
and the auditing processes.
More Information
Internal Reconciliations
Interim Accounts
Interim Accounts
An interim account is an account used to temporarily hold a transaction before it is transferred to a permanent account. It is
common business practice to use an interim account when a business transaction is split into two steps due to timing of the
activity.
In SAP Business One, a number of interim accounts are used to record an interim financial position until the close of a set of
transactions. For auditing purposes, these interim accounts are automatically reconciled. They are as follows:
Allocation Account, Expense Clearing Account, Stock in Transit Account
WIP Inventory Account
Down Payment Interim Account, Down Payment Clearing Account
 Note
SAP Business One lets you view a backdated breakdown of the transactions which make up the value of the interim accounts.
To do this, use the general ledger report with the Consider Reconciliation Date checkbox selected.
For more information, see General Ledger.
More Information
Automatic System Reconciliation
Allocation Acct, Expense Clearing Acct, Stock in Transit Acct.
For reporting purposes, at the end of a company’s financial period, any inventory posted to the accounts within the period must
have a corresponding vendor liability which is recorded in the same period.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:06 AM
It is common business practice for there to be a delay between inventory receipt and receipt of its associated vendor invoice. When
the end of the financial period falls within the delay period, the posted inventory value in respect of these receipts does not have a
corresponding vendor invoice. Instead, liability accounts, such as the allocation account and expense clearing account, hold the
posted inventory value on a temporary basis until the vendor invoice is received. At the end of the financial period, the transactions
which make up the value of these special liability accounts must be easily auditable.
In SAP Business One, certain postings to the following accounts are automatically reconciled to facilitate the auditing process:
Allocation Account
The account records the offsetting amount for the change in inventory value due to actual inventory received or issued via
the goods receipt PO or A/P returns documents.
Expense Clearing Account
The account records the offsetting amount for the change in inventory value due to expenses directly incurred in the
receipt or issue of inventory through the goods receipt PO or A/P returns documents, for example, freight.
Stock in Transit Account
The account records the offsetting amount for the change in inventory value due to both actual inventory and expenses
directly incurred through the reserve invoice documents.
The full or partial automatic system reconciliation of the postings to these three accounts occurs in the following scenarios:
Creating an A/P invoice based on a goods receipt PO
Creating an A/P credit memo based on an A/P goods return
Closing a goods receipt PO which is not copied, or not fully copied to an A/P invoice or a goods return
Closing an A/P goods return which is not copied, or not fully copied to an A/P credit memo or a goods receipt PO
Creating an A/P goods return based on a goods receipt PO
Creating a goods receipt PO based on an A/P goods return
Creating a goods receipt PO based on an A/P reserve invoice
Creating an A/P credit memo based on an A/P reserve invoice
However, in the above scenarios, if any of the three accounts has been involved in a manual reconciliation before the automatic
system reconciliation takes place, SAP Business One does not perform the system reconciliation.
 Note
You can cancel the automatic system reconciliation only if the document that triggers the reconciliation is cancelled.
 Example
1. You create a goods receipt PO for item A01 as follows:
Item No. Quantity Unit Price Freight 1 Freight 1 Inventory Tax
A01 100 1 10 Yes 19.25
The corresponding journal entry posting is as below:
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:06 AM
| Account                  |     | Debit |     | Credit |     |     |
| ------------------------ | --- | ----- | --- | ------ | --- | --- |
| Allocation Account       |     |       |     | 100    |     |     |
| Expense Clearing Account |     |       |     | 10     |     |     |
| Inventory Account        |     | 110   |     |        |     |     |
2. You create an A/P invoice partially based on the goods receipt PO as follows:
Item No. Quantity Unit Price Freight 1 Freight 1 Inventory Tax
| A01 | 40  | 1   |     | 4   | Yes | 7.70 |
| --- | --- | --- | --- | --- | --- | ---- |
The corresponding journal entry posting is as below:
| Account                    |     | Debit |     | Credit |     |     |
| -------------------------- | --- | ----- | --- | ------ | --- | --- |
| BP Account                 |     |       |     | 51.70  |     |     |
| VAT Receivable (Input Tax) |     | 7.70  |     |        |     |     |
| Allocation Account         |     | 40    |     |        |     |     |
| Expense Clearing Account   |     | 4     |     |        |     |     |
SAP Business One automatically reconciles the allocation account and expense clearing account as follows:
| Account            | Debit |     | Credit |     | Reconciliation Amount | Balance Due |
| ------------------ | ----- | --- | ------ | --- | --------------------- | ----------- |
| Allocation Account | 40    |     | 100    |     | 40                    | 60          |
| Expense Clearing   | 4     |     | 10     |     | 4                     | 6           |
Account
More Information
Interim Accounts
WIP Inventory Account
In manufacturing companies, it is common business practice for there to be a time interval between production commencement
and completion. During this period, the inventory value of the in-process products is usually posted to a work-in-progress account,
for example, WIP inventory account. At the end of the company’s financial period, the transactions that make up the value of the
WIP account must be easily auditable.
In SAP Business One, the postings to the WIP inventory account are automatically reconciled as follows to facilitate the accounting
process:
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:06 AM
In the case of a standard or special type of production order with the “Manual” issue method, the reconciliation process is
as follows:
When you create the “Issue for Production” document, the WIP inventory account is debited with the total cost of
issued components.
When you create the “Receipt from Production” document, the WIP inventory account is credited with the cost of
the finished product.
If there is a variance in the WIP inventory account postings between the component cost and the product cost, the variance
is posted when the production order is closed. As a result, the overall WIP inventory account balance in respect of the
production order postings is brought to zero, and these WIP inventory account postings are fully reconciled.
The WIP inventory account of a production component is cleared against the WIP variance account of the parent item, even
if you have defined WIP variance accounts for component items.
In the case of a standard or special type of production order with the “Backflush” issue method, the reconciliation process
is as follows:
The components for production are issued automatically.
When you create the “Receipt from Production” document, the WIP inventory account is debited with the total cost
of issued components, and credited with the cost of the finished product.
If there is a variance in the WIP inventory account postings between the component cost and the product cost, the variance
is posted when the production order is closed. If there is no variance in the WIP inventory account when the production
order is closed, a zero value posting is still made. The overall WIP inventory account balance in respect of all the production
order postings is, therefore, zero following production order closure, and these WIP inventory account postings are
automatically fully reconciled.
In the case of a disassembly type of production order with either “Manual” or “Backflush” issue method, the reconciliation
process is similar to the above two cases, except that the WIP inventory account is debited with the cost of the product and
credited with the cost of the disassembled components.
The postings to the WIP inventory account are automatically fully reconciled only after the corresponding production order is
closed, no matter if the production order is completed with several rounds of issue and receipt, or if an issue or a receipt is related
to more than one production order.
The WIP inventory account of a production component is cleared against the WIP variance account of the parent item, even if you
have defined WIP variance accounts for component items.
However, in the above cases, if the WIP inventory account has been fully, manually reconciled before the automatic system
reconciliation takes place, SAP Business One does not perform the system reconciliation.
 Example
1. You create a standard production order as follows and release it:
Product: Tool Kit
Planned Quantity: 1
Item Base Quantity Planned Quantity Issue Method Item Cost
Hammer 1 1 Backflush 20
Screw Driver 2 2 Backflush 10
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:06 AM
2. You create a “Receipt from Production” document based on the production order as follows:
| Item     | Item Cost | Planned |     | Completed |     |     |
| -------- | --------- | ------- | --- | --------- | --- | --- |
| Tool Kit | 50        | 1       |     | 1         |     |     |
The corresponding journal entry posting is as below:
| Account               |     | Debit |     | Credit |     |     |
| --------------------- | --- | ----- | --- | ------ | --- | --- |
| WIP Inventory Account |     |       |     | 50     |     |     |
| Inventory Account     |     | 50    |     |        |     |     |
| Inventory Account     |     |       |     | 40     |     |     |
| WIP Inventory Account |     | 40    |     |        |     |     |
3. You close the production order, and the corresponding journal entry posting is as follows:
| Account                        |     |     | Debit |     | Credit |     |
| ------------------------------ | --- | --- | ----- | --- | ------ | --- |
| WIP Inventory Account          |     |     | 10    |     |        |     |
| WIP Inventory Variance Account |     |     |       |     | 10     |     |
SAP Business One automatically reconciles the WIP inventory account as follows:
| Account               | Debit |     |     | Credit | Reconciliation Amount | Balance Due |
| --------------------- | ----- | --- | --- | ------ | --------------------- | ----------- |
| WIP Inventory Account |       |     |     | 50     | 50                    | 0           |
| WIP Inventory Account | 40    |     |     |        |                       |             |
| WIP Inventory Account | 10    |     |     |        |                       |             |
More Information
Interim Accounts
Down Payment Interim Account, Down Payment Clearing
Account
When a company receives or makes a down payment, the payment amount is recorded in an interim account before it’s deducted
from the final transaction. For period end auditing purposes, the transactions that make up the value of the interim accounts must
be easily auditable.
In SAP Business One, postings are made to the following two interim accounts in the down payment process:
Down payment clearing account
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:06 AM
Down payment interim account
The postings to these two accounts are automatically reconciled as follows:
Down Payment Request Process
When you create a payment for an A/R or A/P down payment request, the down payment interim account is debited or
credited with the payment amount, and the down payment clearing account is credited or debited with the payment
amount excluding tax.
When you fully or partially draw the down payment to the final A/R or A/P invoice, the down payment interim account is
credited or debited with the drawn amount, and the down payment clearing account is debited or credited with the drawn
amount excluding tax.
As a result, the postings to the down payment interim account and the down payment clearing account are fully or partially
reconciled accordingly.
Down Payment Invoice Process
When you create a full or partial payment for an A/R or A/P down payment invoice, the down payment clearing account is
credited or debited with the invoice amount excluding tax.
When you fully or partially draw the down payment to the final A/R or A/P invoice, the down payment clearing account is
debited or credited with the drawn amount excluding tax.
As a result, the postings to the down payment clearing account are fully or partially reconciled accordingly.
In the above two processes, if the final A/R or A/P invoice is then fully or partially drawn to a credit memo, the postings to the two
accounts generated by the A/R or A/P invoice are proportionately reversed and reconciled.
However, if either of the two accounts has been fully, manually reconciled before the automatic system reconciliation takes place,
SAP Business One does not perform the system reconciliation.
 Note
You can cancel the automatic system reconciliation only if the document that triggers the reconciliation is cancelled.
 Example
1. You create a sales order as follows:
Item No. Quantity Unit Price Total Tax
A01 50 1 50 8.75
2. You create an A/R down payment request based on the sales order and create an incoming payment for it as follows:
Item No. Quantity Unit Price Total Tax Down Payment Total Payment Payment
Made Means
A01 10 1 10 1.75 10 11.75 Cash
The corresponding journal entry posting is as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:06 AM
| Account                       |     | Debit | Credit |     |
| ----------------------------- | --- | ----- | ------ | --- |
| Cash on Hand                  |     | 11.75 |        |     |
| BP Account                    |     |       | 11.75  |     |
| Down Payment Interim Account  |     | 11.75 |        |     |
| VAT Payable (Output Tax)      |     |       | 1.75   |     |
| Down Payment Clearing Account |     |       | 10     |     |
3. You create a final A/R invoice based on the sales order and partially draw the down payment to it as follows:
Item No. Quantity Unit Total Tax Net Amount to Tax Amount to Draw Gross Amount to Draw
Price Draw
| A01 50 | 1   | 50 8.75 4 | 0.7 | 4.7 |
| ------ | --- | --------- | --- | --- |
The corresponding journal entry posting is as below:
| Account                       |     | Debit | Credit |     |
| ----------------------------- | --- | ----- | ------ | --- |
| BP Account                    |     | 58.75 |        |     |
| Down Payment Interim Account  |     |       | 4.7    |     |
| Down Payment Clearing Account |     | 4     |        |     |
| VAT Payable (Output Tax)      |     |       | 8.75   |     |
| VAT Payable (Output Tax)      |     | 0.7   |        |     |
| Revenue Account               |     |       | 50     |     |
| Inventory Account             |     | 50    |        |     |
| Cost of Goods Sold Account    |     |       | 50     |     |
SAP Business One automatically reconciles the postings to the down payment interim account and down payment clearing
account as follows:
| Account              | Debit | Credit | Reconciliation Amount | Balance Due |
| -------------------- | ----- | ------ | --------------------- | ----------- |
| Down Payment Interim | 11.75 | 4.7    | 4.7                   | 7.05        |
Account
| Down Payment Clearing | 4   | 10  | 4   | 6   |
| --------------------- | --- | --- | --- | --- |
Account
Related Information
Interim Accounts
A/R Down Payment Documents: Accounting Tab
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:06 AM
A/P Down Payment Document: Accounting Tab
Reconciliation
Use this function to internally reconcile transactions posted to business partners. You can perform either partial or full
reconciliation, for specific business partner or for multiple business partners. Choose the appropriate reconciliation type for the
amount of transactions to be reconciled, while referring to whether partial reconciliation or reconciliation of multiple business
partners is required:
Type Used to reconcile...
Manual A small number of transactions, cases where partial reconciliations are required, or
transactions posted to more than one business partner
Automatic A large number of transactions, or a range of business partners, based on user-defined
parameters and priorities.
 Note
When performing automatic reconciliation for a range of business partners, the
reconciliation is done separately for each business partner successively and not between
transactions posted to different business partners.
 Note
You can select the Ignore Ordered Transactions checkbox to exclude transactions in
payment order runs from this automatic internal reconciliation. Otherwise, all transactions
are taken into consideration. The checkbox is selected by default.
Semi-Automatic Manually, based on recommendations provided by SAP Business One.
 Note
Transactions representing documents with cash discounts are not handled by this
reconciliation type.
To access this function, choose Business Partners ->Internal Reconciliations-> Reconciliation.
More Information
BP Internal Reconciliation - Selection Criteria: Manual
Internal Reconciliation Window
Reconciliation Window
BP Internal Reconciliation - Selection Criteria: Manual
The following fields appears in this window when selecting the Manual reconciliation type.
To open the window, choose Business Partners Internal Reconciliations Reconciliation .
Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:06 AM
Multiple BPs
Appears only when the Manual reconciliation mode is selected. This option enables the transactions of more than one business
partner to be reconciled.
 Example
If a specific business partner is a customer as well as a vendor and therefore has two business partner master data records,
you can reconcile the transactions created against both business partner master data records.
Business Partner
Specify the business partner whose transactions you want to reconcile.
BP Code
Appears only when Multiple BPs is selected under the Manual reconciliation type. Specify the codes of the business partners
whose transactions you want to reconcile.
BP Currency
Displays the code of the currency assigned to the business partner. The sign ## indicates that the option All Currencies was
assigned to this business partner.
Balance Due (LC)
The current balance of the business partner in the local currency. A positive amount indicates a credit balance, and a negative
amount indicates a debit balance. If Display Credit Balance in Negative Sign was selected in Administration System
Initialization- Company Details Basic Initialization tab, a positive amount indicates a debit balance while a negative amount
indicates a credit balance.
Balance Due (FC)
The current balance of the business partner in the foreign currency. A value appears in this field only if a specific foreign currency
was assigned to the business partner. If the currency of the business partner is either the local currency or All Currencies, this
field remains empty. A positive amount indicates a credit balance, and a negative amount indicates debit balance. If Display Credit
Balance in Negative Sign was selected in Administration System Initialization Company Details Basic Initialization tab,
a positive amount indicates a debit balance while a negative amount indicates a credit balance.
Reconcile
Performs the reconciliation according to the parameters you defined. If you selected the Manual or Semi-Automatic mode, choose
this button to open the Internal Reconciliation or Reconciliation window.
More Information
Manage Previous Internal Reconciliations Window
Internal Reconciliation Printing Preferences
When performing internal reconciliation manually, it is possible to print the reconciliations. Use this window to set the printing
preferences for the manual internal reconciliations you are about to perform.
To open the window, choose the Print Settings button at the Internal Reconciliation window.
Internal Reconciliation Printing Preferences
Print Reconciliations
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:06 AM
Prints reconciliations. When you select this option, the following options appear:
New Reconciliations Only – Prints only the reconciliation that the system is about to perform.
New and Old Reconciliations – Prints reconciliations that were created in the past as well as the ones the system is about to
perform. When you select this option, additional fields appear that enable you to define the reconciliation number range.
Unreconciled Transactions
Prints unreconciled transactions. When you select this option, the following fields appear:
Sorting 1
Sorting 2
Use these fields to define the sorting order of the unreconciled transactions for the purpose of printing. Click in each field to select
the values according to which sorting is to be performed.
More Information
Manage Previous Internal Reconciliations - Selection Criteria
Internal Reconciliation Window
This window lists the transactions for reconciliation that match the selection criteria you specified in the BP Internal
Reconciliation – Selection Criteria window.
General Area Fields
BP
The code of the business partner. Appears only when a single business partner was specified in the BP Internal Reconciliation –
Selection Criteria window.
Display SC-Only Transactions
Select the checkbox to display any additional transaction that has a balance due in system currency only.
 Note
This checkbox is available only if the currency of the selected BP or G/L account is Local Currency or All Currencies.
Display LC/SC-Only Transactions
Select the checkbox to display any additional transaction that has a balance due in the following currencies:
Local currency only
System currency only
Both local currency and system currency
 Note
This checkbox is available only if the currency of the selected BP or G/L account is a foreign currency.
Reconciliation Currency
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:06 AM
If the currency of the specified business partner(s) is local currency or all currencies, the reconciliation currency is the local
currency. If one of the foreign currencies was specified for the business partner(s), the reconciliation currency is this foreign
currency. This field is in read-only mode.
Reconciliation Date
The date on which reconciliation takes place. By default, the current date is displayed. SAP Business One uses the reconciliation
date when generating exchange rate differences.
Adjustments
Opens a window in which you can create a journal entry or document that is required to complete reconciliation. If, after you have
selected all the required transactions, the amount at the bottom of the Amount to Reconcile column is different than zero, you
cannot perform reconciliation. In this case, you balance this difference by creating an adjustment.
Print Settings
Opens the External Reconciliation Printing Preference window, in which you can define your preferences for printing
reconciliations.
Reconcile
Reconciles the selected transaction rows.
Table Area Fields
Selected
Select the transactions you want to reconcile.
Origin
Indicates the document or transaction type that initiated the posting of each transaction. For example, IN represents a transaction
resulting from the creation of an A/R invoice. For a complete list of origins, see Transaction Type Abbreviations Legend.
Origin No.
The number of the document that initiated the creation of the transaction. For example the number of the A/R Invoice.
Posting Date
The posting date of the business partner row in the transaction.
Amount
The original amount posted in the specific row of the transaction. This field is disabled. Amounts in brackets indicate debits, unless
the option Display Credit Balance in Negative Sign is selected (in Administration System Initialization Company Details
Basic Initialization tab ) in which case it indicates credits.
Balance Due
The unreconciled amount. If this amount is smaller than the value appears in the Amount field, it indicates that this row in the
transaction was already partially reconciled internally. This field is disabled. Amounts in brackets indicate debits, unless the option
Display Credit Balance in Negative Sign is selected (in Administration System Initialization Company Details Basic
Initialization tab ), in which case it indicates credits.
Amount to Reconcile
Specify the amount of this transaction row you want to reconcile. The amount to reconcile must be greater than zero and smaller
or equal to the Balance Due amount. By default, the Amount to Reconcile equals the Balance Due. At the bottom of this column
you can see the accumulated balance of the selected transactions. A zero amount indicates balanced reconciliation.
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:06 AM
Payment Order Run
If the checkbox is selected, it indicates that this document is included in a payment order run.
Reconciliation Window
This window lists the transaction rows to be reconciled on the debit and credit sides, together with the reconciliation
recommendations generated according to the selection criteria and parameters defined in the BP Internal Reconciliation –
Selection Criteria window for Semi-Automatic reconciliation
Reconciliation Window
BP
The business partner for whom the reconciliation is performed.
Reconciliation Currency
If the currency of the specified business partner is either local currency or all currencies, the reconciliation currency is the local
currency. If one of the foreign currencies was specified for the business partner, the reconciliation currency is the foreign currency.
This field is in read-only mode.
Open Transactions on Debit Side
List of transactions with unreconciled amounts greater than zero on the debit side.
Trans. No.
The journal entry number as it appears in the field Trans. No. in the Journal Entry window.
Posting/Due/Document Date
The posting date, due date, or document date of this transaction row, depending on which value you specified in the BP Internal
Reconciliation – Selection Criteria window
Ref. 1/Ref. 2/Ref. 3
Reference 1, 2, or 3, of the transaction row displayed, depends on the reference specified in the BP Internal Reconciliation –
Selection Criteria window.
Balance Due
The amount still to be reconciled. If the transaction was partially reconciled previously, this amount is smaller than the original
amount posted in the transaction.
Open Transactions on Credit Side
List of transactions with unreconciled amounts greater than zero on the credit side.
Trans. No.
The journal entry number as it appears in the field Trans. No. in the Journal Entry window.
Posting/Due/Document Date
The posting date, due date, or document date of this transaction row, depending on which value you specified in the BP Internal
Reconciliation – Selection Criteria window
Ref. 1/Ref. 2/Ref. 3
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:06 AM
Reference 1, 2, or 3, of the transaction row displayed, depends on the reference specified in the BP Internal Reconciliation –
Selection Criteria window.
Balance Due
The amount still to be reconciled. If the transaction was partially reconciled previously, this amount is smaller than the original
amount posted in the transaction.
Payment Order Run
If the checkbox is selected, it indicates that this document is included in a payment order run.
Ignore Negative Amounts
When selected, it is impossible to display recommendations for transactions with negative amounts, and once you double click
such transaction, the error message “Negative row can not be selected” is displayed.
Manual
Enables you to manually reconcile the transactions of the selected business partner by opening the Internal Reconciliation
window with the business partner’s data.
Manage Previous Reconciliations
This function enables you to display, cancel and recreate external or internal reconciliations created for a specified range of
business partners or G/L accounts. This function does not deal with reconciliations created by SAP Business One.
To manage previous reconciliations, choose Banking Bank Statements and Reconciliations Manage Previous
Reconciliations .
More Information
Manage Previous Reconciliations Window
Manage Previous Internal Reconciliations - Selection Criteria
Use this window to specify the parameters according to which previous internal reconciliations are displayed.
To open the window, choose Business Partners Reconciliations Manage Previous Reconciliations .
Selection Criteria
Previous Reconciliation for
Specify whether to display previous internal reconciliations for business partners or G/L accounts.
G/L Acct/BP Code From...To...
Define a range of business partners or G/L accounts (depends on your choice in the previous field).
Date From...To...
Specify dates to display the previous internal reconciliations performed within a particular date range.
Reconciliation No. From...To...
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:06 AM
Define a range of reconciliation numbers for which the system should display reconciliations.
Manage Previous Internal Reconciliations Window
This window lists the previous internal reconciliations that match the selection criteria you specified in the Manage Previous
Internal Reconciliations – Selection Criteria window.
This window has two sections:
Reconciliation History – lists the previous reconciliations.
Reconciliation Details – lists the transaction rows associated with the selected reconciliation from the Reconciliation
History section
Reconciliation History
Recon. No.
The reconciliation number assigned to the internal reconciliation by SAP Business One when the reconciliation took place.
Recon. Amount
The total amount of the reconciliation.
Recon. Type
Indicates the type of reconciliation, based on whether the reconciliation is a result of document creation or user initiation:
Deposit - Reconciliation is the result of creating a deposit document for check(s), cash, credit card voucher(s), or bill(s) of
exchange (the latter is supported only by the SAP Business One software versions of the relevant localizations. Details are
available in the localization-specific online help file under Help Documentation Country/Region Specific
Information ).
Automatic - Reconciliation was performed by selecting the Automatic option in the BP Internal Reconciliation - Selection
Criteria window.
Bank Statement Processing - Reconciliation was performed by the bank statement processing functionality, according to
the user-defined matching rules.
Cancellation - Reconciliation was cancelled by using the Cancel Reconciliation button in this window.
Payment - Reconciliation is the result of creating an incoming or outgoing payment for specific documents/transactions.
Credit Memo Reconciliation is the result of copying an A/P or A/R invoice to an A/P or A/R credit memo.
Manual - Reconciliation was performed manually.
Semi-Automatic - Reconciliation was performed by selecting a transaction from the Reconciliation recommendations
window that opens if you selected the Semi-Automatic option in the BP Internal Reconciliation - Selection Criteria
window.
Period Closing - Reconciliation was automatically performed when a period-end closing adjustment was created at the year
end.
Reconciliation Date
The date on which reconciliation took place. For manual reconciliation, this is the date specified in the Reconciliation Date field in
the Internal Reconciliation window. For reconciliations resulting from document creation (payments, credit memos), the
reconciliation date is the posting date of the latest document to be included in the reconciliation.
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:06 AM
 Example
An incoming payment is created for two different A/R invoices that were created a week ago and two days ago. The posting
date of the incoming payment is the current date. This is considered as the reconciliation date in this case.
Canceling/Cancelled Reconciliation Number
If reconciliation is the result of cancelling a former reconciliation and then re-reconciling, the number of the former reconciliation is
displayed.
Reconciliation Details
Origin
Indicates the document or transaction type that initiated the posting of each transaction. For example, IN represents a transaction
resulting from the creation of an A/R invoice. For a complete list of origins, see XX in the online help.
Origin No.
The number of the document that initiated the creation of the transaction, for example, the number of the A/R invoice.
G/L Acct/BP Code
The code of the G/L account or business partner to which the reconciled transaction row was posted.
Ref. 1
The value in the field Ref. 1 in the reconciled transaction.
Due Date
The due date specified in the reconciled transaction row.
Amount
The original amount of the reconciled transaction row. Amounts in brackets reflect negative amounts. If the option Display Credit
Balance with Negative Sign is selected in Administration System Initialization Company Details Basic Initialization tab
amounts in brackets represent credit amounts.
Applied Amount
The amount from the transaction row that was reconciled in this reconciliation. When the applied amount is different from the
value displayed in the Amount field, it indicates that the transaction row is partially reconciled by this reconciliation.
Cancel Reconciliation
Choose to cancel the marked reconciliation. You cancel one reconciliation at a time.
 Note
Reconciliations resulting from the following scenarios can not be cancelled, and therefore when marking such reconciliation,
the Cancel Reconciliation button is disabled:
Creating incoming or outgoing payments for specific transactions.
Creating A/P or A/R credit memo based on existing document.
Reversing transaction by using the Reverse option in the Journal Entry window.
Cancelling transaction by using the Cancel option in Data menu.
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:06 AM
More Information
BP Internal Reconciliation - Selection Criteria
Business Partner Reports
These reports provide an overview of your interactions with business partners.
 Note
The reports are also available from the Reports module.
My Activities – Shows all the activities assigned to you, by yourself or by other users.
Activities Overview – Provides an overview of the activities throughout SAP Business One.
 Note
You can view activities relating to a specific business partner in the Activity window or the Business Partner Master Data
window by choosing Related Activities after selecting a business partner.
Inactive Customers – Shows all customers who do not appear in any of the selected sales documents.
Dunning History Report – Shows dunning letters and the invoices included in them, per customer.
Aging – Provides a general or detailed overview of the age of unpaid customer debts, the age of unpaid liabilities to the
vendors, and the value of the debts or liabilities.
Internal Reconciliations – Internally reconciles transactions created for business partners or for G/L accounts.
In addition to the reports mentioned above, you can find under this menu entry various system queries relating to business
partners.
My Activities
Activities Overview Report
Inactive Customers
Dunning History Report
Inventory Status Report
Customers Receivables by Customer Cross-Section Report
Customers Credit Limit Deviation
Aging
My Activities
This report lets you view all activities assigned to you, by yourself or by other users.
To create the report, choose Business Partners Business Partner Reports My Activities .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:06 AM
My Activities Fields
Display Only Open Activities
Hides activities that are closed.
Handled by
User to whom the activity is assigned.
Activity
Main type of the activity.
Type
Sub-type of the activity.
 Example
Technical or Service can provide information about the type of meeting, phone call and so on.
Contact Person
Name of the business partner contact person specified for the activity.
Remarks
Text entered in the Remarks field in the Activity window.
Personal
Yes if Personal is selected in the Activity window.
Tentative
Yes if Tentative is selected in the Activity window.
Reminder
Yes if the Reminder is selected in the Activity window.
Reminder Period
Time period for sending a reminder defined in the Activity window.
Sales Employee
Default sales employee of the business partner.
Closed
Yes if the Closed is selected in the Activity window.
Closing Date
Date on which the activity was closed.
Room, Street, City, Country/Region, State
Address details entered for a Meeting type of activity.
Content
Text specified on the Content tab of the activity.
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:06 AM
[Document Icon]
indicates that a document is linked to the activity.
 Note
Double-click the icon to open the linked document.
[Attachment Icon]
indicates that a file is attached to the activity.
 Note
Double-click the icon to open the attached file.
Source Type
Opportunity - If the activity was created from within a sales or purchasing opportunity.
Service Call – If the activity was created from within a service call.
Source Number
Opportunity number or service call number from which the activity was created.
Previous Activity
Original activity number if the activity is a follow-up activity.
System Date, System Time
Date and time when the activity was added.
Related Information
Activities Overview Report
Activities Overview Report
This comprehensive report displays information about all activities recorded in SAP Business One.
 Example
A report can be a manager’s summary of all the activities of his/her employees, or a sales employee’s report showing all the
activities of his/her customers.
Related Information
My Activities
Activities Overview - Selection Criteria
Use this window to specify selection criteria for the Activities Overview Report.
To open the window, choose Reports Business Partners Activities Overview .
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:06 AM
After defining the report, you can view it in the Activities Overview Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Handled by
Specify the ranges of users and employees whose activities are to be included in the report.
 Note
To include all users or employees, leave the fields blank.
 Note
Employees that are linked to users are only displayed as users in the user list.
Contact Person
Select a contact person. The field is only active if one specific business partner is selected in the BP Code From...To... fields.
Properties
Opens the Properties window in which you can select business partner properties.
Remarks
Specify some text as a search criterion.
User-Defined Fields
Select the checkbox and click the ellipsis icon (...) to filter activities by their user-defined fields (UDFs).
You can display and hide the selected UDFs in the Activities Overview and My Activities reports through Form Settings.
Display Scheduled Service Calls
Select the checkbox to display all scheduled service calls in the Activities Overview report.
"Scheduled" means that on the scheduled row level, at least one of the fields (Handled By or Technician) is filled in, and the start
date/time, end date/time are filled in.
Hide Closed Service Calls
Select the checbox to display the service calls that are not closed in the Activities Overview report.
Activities Overview Report Window
This window displays the Activities Overview Report according to your defined selection criteria.
 Note
By default, only some columns are displayed. To display additional columns, choose .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:06 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Activities Overview Report Fields
Display Only Open Activities
Hides activities that are closed.
Handled By
User or employee to whom the activity is assigned.
Activity
Main type of the activity.
Type
Sub-type of the activity.
 Example
Technical or Service can provide information about the type of meeting, phone call and so on.
Contact Person
Name of the business partner contact person specified for the activity.
Remarks
Text entered in the Remarks field in the Activity window.
Personal
Yes if Personal is selected in the Activity window.
Tentative
Yes if Tentative is selected in the Activity window.
Reminder
Yes if Reminder is selected in the Activity window.
Reminder Period
Time period for sending a reminder, as defined in the Activity window.
Sales Employee
Default sales employee of the business partner.
Closed
Yes if Closed is selected in the Activity window.
Telephone
Phone number entered in the Activity window.
Room, Street, City, Country/Region, State
Address details entered for a Meeting type of activity.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:06 AM
Content
Text entered on the Content tab of the activity.
[Document Icon]
indicates that a document is linked to the activity. Double-click the icon to open the linked document.
[Attachment Icon]
indicates that a file is attached to the activity. Double-click the icon to open the attached file.
Source Type
Opportunity - If the activity was created from within a sales or purchasing opportunity.
Service Call – If the activity was created from within a service call.
Source Number
Opportunity or service call number from which the activity was created.
System Date, System Time
Date and time when the activity was added.
Related Information
My Activities
Business Partner Reports
Inactive Customers
This report lists the customers for whom none of the selected sales documents were created, according to the range defined in the
Inactive Customers – Selection Criteria window.
Inactive Customers Fields
Sales Quotations, Orders, Delivery Notes, A/R Invoices, A/R Down Payments
By default, SAP Business One automatically selects all the documents.
To remove a sales document type from the report, deselect it. Choose Refresh each time you change your selection of documents.
Customer Code, BP Name, Telephone 1, Telephone 2
Names and numbers of the inactive customers, along with the main phone numbers from the customer master record.
Related Information
Reports
Business Partners
Inactive Customers - Selection Criteria
The Inactive Customers report indicates whether a customer is inactive by checking whether or not specific sales documents were
created to the customer within a defined period.
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:06 AM
 Example
In your company, if Sales Order was not issued to a customer within the past month, this customer is considered as inactive.
Use this window to specify selection criteria for generating a report that reflects the Inactive Customers in your business.
To open the window, choose Business Partners Business Partner Reports Inactive Customers .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Customer Group
Select a customer group to filter by.
 Note
Applies if the customers have been assigned to groups in the business partner master data.
Dunning History Report
This report displays dunning letters and their included invoices, per customer, according to your selection criteria.
The dunning letters and all other details are taken from the dunning wizard.
Related Information
Dunning
Dunning History Report - Selection Criteria
Use this window to specify selection criteria for the Dunning History Report.
To open the window, choose Business Partners Business Partner Reports Dunning History Report .
After defining the report, you can view it in the Dunning History Summary Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Properties
Opens the Properties window, where you can set properties as selection criteria.
Due Date From...To...
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:06 AM
Specify a due date range to include documents that contain due dates within the range in the report.
AR Invoice No. From...To...
Specify a range for the A/R Invoice number to be included in the report.
Down Payment No. From...To...
Specify a range for the Down Payment document number to be included in the report.
Include Deselected Invoices
Includes invoices displayed in the dunning run but which are not included in dunning letters.
Dunning Level
Specify a specific dunning level, to display only invoices and letters related to it, or specify all dunning levels.
Related Information
Dunning
Properties
Dunning History Summary Report
Use this report to view the invoices included in each dunning letter, per dunning level, per customer.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Dunning History Summary Report Fields
Find
To find specific letters in the report, specify the first character of a required name. SAP Business One locates the first dunning
letter containing the specified characters.
Dunning Name
Wizard’s name as defined in step no. 2 of the dunning wizard.
Doc. No.
Internal number of the document included in the dunning run.
Dunning Address
Address to which the dunning letter should be sent. The default value is the Pay To address from the invoice. If required, specify
another address.
Due Date
Due date as defined in the document.
Last Dunning Date
Last dunning date, in case the document was dunned previously.
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:06 AM
Document Sum, Open Sum
Total of the document and amount that is not credited or paid yet.
Interest Days
Difference between dunning run date and due date of the invoice.
Interest %, Interest Amount
Interest rate and amount defined and calculated during the dunning run.
Total
Summary of all the open sums from the dunned invoices plus the interest calculated.
Fee
Fee amounts, as appear in the recommendation report.
Sum
Total of debt amount plus interest and fees. The values cannot be edited.
Inventory Status Report
You can use this report to check the planned inventory transactions for a specific item, according to the defined selection criteria.
The report lists the available quantities for the requested items.
Planned inventory transactions include:
Inventory that is to be shipped to customers or used for production
Inventory that has been ordered from vendors or production and is to be received into the warehouse
The Inventory Status report can be generated in Normal or Available-to-Promise (ATP) layout (see Inventory Status Window
(Normal) and Viewing Detailed Confirmation Status).
 Note
The Inventory Status report is generated directly from the:
Item Master Data window for Inventory Items only.
Business Partner Master Data window for Preferred Vendors only.
Inventory Status - Selection Criteria
To open the Inventory Status window, choose Inventory Inventory Reports Inventory Status , specify the selection criteria,
and choose the OK button.
 Note
To generate the Inventory Status report directly, right-click on the window and choose Inventory Status as follows on the:
Item Master Data window for inventory items only.
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:06 AM
Business Partner Master Data window for preferred vendors only.
The report is generated using the current inventory item or vendor as the selection criteria. If there are no transactions based
on your current selection, the report is not generated.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Status – Selection Criteria Fields
Hide Items with No Quantity in Stock
Do not display items with zero quantities from the In Stock, Committed, and Ordered columns.
By Location tab
Specify the selection criteria for the report according to the warehouse's location. Select or deselect the locations to be included
in, or excluded from, the report.
 Note
The default is to include all warehouses and locations in the report.
By Warehouse tab
Specify a range of warehouses to include in the report. You can exclude warehouses within a range of included warehouses. For
example, if you include warehouses 01 to 10 and exclude warehouses 06 to 08, only warehouses 01 through 05 and warehouses
09 and 10 are considered in the report. The default value is no selection, namely all warehouses and locations are included in the
report.
Select Including and specify a range of warehouses to include in the report.
Select Excluding and specify a range of warehouses to exclude from the report.
 Note
The default is to include all warehouses and locations in the report.
Inventory Status Window
The Inventory Status window displays a list of items and their current inventory status based on the defined selection criteria.
To open this window, choose Inventory Inventory Reports Inventory Status from the SAP Business One Main Menu. In the
Inventory Status - Selection Criteria window, choose OK.
 Note
You can also generate the Inventory Status report directly by right-clicking and choosing Inventory Status report in the:
Item Master Data window for inventory items only.
Business Partner Master Data window for preferred vendors only.
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:06 AM
The report is generated using the current Inventory Item or Vendor as the selection criteria. If there are no transactions based
on your selection, a report is not generated.
You can also display the Inventory Status report in Normal or Available-to Promise layout (see Inventory Status Window
(Normal) and Viewing Detailed Confirmation Status). The Available-to-Promise (ATP) report provides additional information
about item availability, such as the uncommitted stock and receipts available to satisfy potential customer orders.
General Area Fields
Item No.
To find an item, enter the item number in the Item No. field. The cursor moves to that item in the list.
Double-click row number to open following report
You can display the Inventory Status report according to the following layout types:
Normal displays the Inventory Status report in Normal layout (see Inventory Status Window (Normal)), or
Available-to-Promise displays the Inventory Status report in a basic Available-to-Promise layout (see Viewing Detailed
Confirmation Status).
Table Area Fields
Item No.
The number of the item, as defined in the Item Master Data window.
Item Description
The description of the item, as defined in the Item Master Data window.
In Stock
The current stock level of the item.
This is the quantity physically in the warehouse.
Committed
The quantity of an item reserved from the inventory for the following document types:
Sales orders
Production orders (the quantity used for producing a parent item)
A/R reserve invoices
 Note
In various localizations there might be differences in this functionality. For complete information, refer to the localized online
help file provided with SAP Business One by choosing: Help Document Localization Specific Info .
Ordered
The quantity of an item already purchased or produced, but not yet received. The following document types contribute to the
quantity displayed in this field:
Purchase orders
Production orders (the quantity you plan to receive from production)
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:06 AM
A/P reserve invoices
 Note
In various localizations there might be few differences in this functionality. For complete information, refer to the localized
online help file provided with SAP Business One by choosing: Help Document Localization Specific Info .
Available
The quantity of an item that will be available when the Committed stock is issued from the warehouse and the Ordered stock is
received by the warehouse.
The quantity is calculated as follows:
Available = In Stock + Ordered – Committed
If the available stock for an item is negative, the value appears in red.
 Note
The Available to Promise report lets you view and reserve invoices from specific warehouses. To access this report, from the
SAP Business One Main Menu, choose Inventory Item Master Data . Right-click Item and choose Available to Promise
Report.
 Note
The values in the following three fields always show the total quantity in all warehouses, regardless of the selection criteria
chosen for the report. For example, a specific warehouse.
By default, these fields are hidden. To make them visible, use Form Settings.
Required Level
The total Required Inventory Level quantity for the item, as specified in the Item Master Data window.
Minimum Inventory Level
The total Minimum Inventory quantity for the item, as specified in the Item Master Data window.
Maximum Level
The total Maximum Inventory quantity for the item, as specified in the Item Master Data window.
Inventory UoM
The item's inventory UoM, if specified in the Item Master Data window.
More Information
Inventory Status Window (Normal and ATP Layout)
Customers Receivables by Customer Cross-Section Report
You can use this window to generate the customer receivables by customer cross-section report. To do it.
To open the window, choose one of the following from the SAP Business One Main Menu:
Business Partners Business Partner Reports Customers Receivables by Customer Cross-Section
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:06 AM
Reports Business Partner Reports Customers Receivables by Customer Cross-Section
After defining the BP Code in the Query - Selection Criteria window, you can view the report in the Customers Receivables by
Customer Cross-Section Report window.
Query - Selection Criteria
BP Code
Specify a business partner code in the field.
 Note
Only a customer code is valid here.
Customers Receivables by Customer Cross-Section Report
Window
This window displays the Customers Receivables by Customer Cross-Section report according to the defined selection criteria.
 Note
This window displays only if the account balance of the selected customer is minus.
Telephone 1
Displays the customer telephone number of the customer.
Account Balance
Displays the balance due of the selected customer.
Open Checks Balance
Displays the undeposited checks of the selected customer.
Payable Limit
Displays the commitment limit of the customer.
Credit Balance
Displays the credit balance of the selected customer. Credit balance equals to the result amount of account balance minus open
checks balance.
Customers Credit Limit Deviation
Use this report to check the customers credit limit deviation details.
To access this window, from SAP Business One Main Menu, choose one of the followings:
Business Partners Business Partner Reports Customers Credit Limit Deviation
Reports Business Partner Reports Customers Credit Limit Deviation
The following are displayed for the customers credit limit deviation details.
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:06 AM
CardCode
Displays the code number of a business partner.
CardName
Displays the name of a business partner.
CreditLine
Displays the credit limit of a business partner.
Balance
Displays the balance of a business partner.
Deviation
Displays the credit limit deviation amount of a business partner.
 Note
The amount can be displayed as negative if you have select the Displays Credit Balance with Negative Sign checkbox in the
Company Details window.
Aging
Aging reports can give you a general or detailed overview of the age of unpaid customer debts, the age of unpaid liabilities to the
vendors, and the value of the debts or liabilities.
To create aging reports, choose one of the following:
Financials Financial Reports Accounting Aging
Business Partners Business Partner Reports Aging
Alternatively, create them from the Reports module.
Related Information
Customer Receivables Aging
Vendor Liabilities Aging
Customer Receivables Aging
This report lists all open customer receivables, sorted by age, and provides an analysis of each customer receivable owed to you.
Use this window to specify selection criteria for the Customer Receivables Aging report (see the topic Customer Receivables
Aging Report).
To open the window, choose one of the following:
Financials Financial Reports Accounting Aging Customer Receivables Aging
Business Partners Business Partner Reports Aging Customer Receivables Aging
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:06 AM
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Customer Receivables Aging Selection Criteria Fields
Group By
Specify whether to group the report by customer or by sales employee.
Customer Group
From the dropdown list, select the group from which to display business partners. To include all customers in the selection criteria,
select All.
Properties
Opens the Properties window, where you can specify customer properties.
Control Accounts
Select the checkbox and click to show only the transactions and balances for selected control accounts.
Select All
Includes all customers in the report
Aging Date
The age of a receivable is determined using this date. Usually, this is the current date, which, therefore, is set as the default. You
can change the default if, for example, you want to display all receivables that are due for payment during the following week.
Interval
Specify a time interval for grouping receivables.
From the dropdown list, select Days, Months, or Periods. If you choose Days, four new fields appear for you to specify the duration
of each time interval. You do not have to specify all four fields, but you must specify at least the first field. The default values for the
four fields are: 30, 60, 90, and 120.
 Example
In the first two fields, specifying 20, 50 days as the interval subdivides the receivables as follows:
Up to 20 days old
21 to 50 days old
51 days or older
Translate Leading Currency at Aging Date
For documents created in foreign currencies, selecting this checkbox will display the local currency and system currency that are
converted from the document currency using the exchange rate on the aging date; deselecting this checkbox will display the local
currency and system currency that were posted in the journal entry from the document.
For documents created in local currency, selecting this checkbox will display the system currency that is converted from the
document currency using the exchange rate on the aging date; deselecting this checkbox will display the system currency that was
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:06 AM
posted in the journal entry from the document. The report will display the foreign currency what was posted in the journal entry
from the document, no matter whether the checkbox is selected or not.
Display Customers with Zero Balance
Includes customers with a zero balance in the report
Display Reconciled Transactions
Displays reconciled journal entries of the accounting documents generated for the customers
Ignore Future Remit
Hides the Future Remit column in the report and excludes transactions that have a value in this field
Display in Pages
Select this checkbox to display the report in pages and with navigation buttons.
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
Customer Receivables Aging Report
 Note
This topic contains an SAP Note that explains additional information.
SAP Business One displays the results of this report according to your selection criteria (see the topic Customer Receivables
Aging).
It displays documents together with the respective receivables. The report provides the value of the debt the customer has
acquired and the length of time that the debt has remained unpaid.
For an All Currencies business partner with a foreign currency as the displayed currency, the values in this report are converted
based on the current exchange rate and not on the original transaction exchange rate. This is because when the currency of a
business partner is set as All Currencies, the operative currency is the local currency, and related foreign currency transactions
are therefore not managed for the account.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Customer Receivables Aging Report
Currency
Specify the currency for displaying the report results.
Aging Date
The aging date specified in the selection criteria window
Age By
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:06 AM
Specify by which date to calculate the age of the receivables: due date, posting date, or document date of the document/journal
entry. For more information about how to print posting date, document date, or due date of the documents on Detailed Receivable
Aging Report, see SAP Note 1260740 .
Type
Displays the document type and provides a link to the document window
Installment No.
Displays the successive number of the installment
 Example
If a document contains three installments, each installment is displayed in a separate row, and this field displays the value 1, 2,
or 3, accordingly.
BP Ref. No.
Displays the business partner reference number
Number of Days Outstanding
The number of days between the due date and the aging date
Original Account
Displays the original document total, the original total of the installment, or the total value of a manual journal entry line
Balance Due
Displays the total open amount of debt
Figures in brackets indicate the payments received from customers that have not been applied for the period.
Future Remit
Displays all open receivables owed by the customer according to the date selected in the Age By field and for which the date
specified in the Aging Date field has not yet been reached
 Example
The customer has an open A/R invoice for USD100, due on May 1st.
In the Age By field, Due Date is selected.
The Aging Date field is set to April 28th.
Since the invoice is due after the aging date, the invoice amount is displayed in the Future Remit column.
Interest
Displays the amount of interest that should be paid. It is calculated according to the dunning term defined on the Payment Terms
tab of this customer.
Project Code
Displays the code of the project to which the document's journal entry is assigned
Payment Method Code
Displays the code of the default payment method assigned to the business partner on the Payment Run tab of the Business
Partner Master Data window
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:06 AM
[Time Intervals]
SAP Business One displays the relevant open receivables in columns representing the specifications you made in the Interval field
in the selection criteria window.
The amount of future remit is first subtracted from the total sum of receivables.
Days – Each column represents the number of days entered in the selection criteria window, starting from the aging date
and moving back.
Months – Each column represents one month, starting from the aging date month and moving back.
Periods – Each column represents one period, as defined in Administration System Initialization Posting Periods ,
starting from the aging date period and moving back.
Dunning Level
Displays the dunning level assigned to the debt
Dunning Letter
Select the checkbox in this column to create a dunning letter for that document.
Doubtful Debt
Displays any existing doubtful debt amount
The calculation for this field depends on the definitions in the Doubtful Debts - Setup window. The sum of the invoices for each
range of days is multiplied by the percentage defined for this range of days.
In this report you are able to issue a journal entry to credit the customer for the doubtful debt. To create a journal entry for a
doubtful debt, proceed as follows:
1. Highlight the customer / invoice row including the doubtful debt.
2. Right-click the row and choose Journal Entry. Alternatively, from the menu bar, choose Go To Journal Entry .
A Journal Entry window opens. The first row in the journal entry includes the customer code, the customer name, and the
amount of the doubtful debt to be cleared in the Credit column.
3. Enter the account code for the second row.
4. Change the amounts in the rows or proceed to the end of the second row to complete the amount in the Debit column in
order to balance the journal entry.
 Note
The entry will be recorded in both the customer amount and the control account that was set for the customer in the business
partner master data.
[Top Total Row]
Displays the sum of amounts listed in one column
[Bottom Total Row]
Displays the percentage of open receivables for each time interval
Go to Page
Enter a page number and press Tab to display the data in this page.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:06 AM
The input number must be a number between 1 and the maximum page number.
 Note
This field is available when you select the Display in Pages checkbox in the Customer Receivables Aging – Selection Criteria
window.
Display <Number> Rows
From the dropdown list, select a number of rows that you want to display in the table as one page.
 Note
The number that you select decides the row number shown in the following four buttons:
First <Number> Rows – Choose this button to display the data in the first page of the table. This button is disabled if
the current display is the first page.
Previous <Number> Rows – Choose this button to display the data in the previous page of the table. This button is
disabled if the current display is the first page.
Next <Number> Rows – Choose this button to display the data in the next page of the table. This button is disabled if
the current display is the last page.
Last <Number> Rows – Choose this button to display the data in the last page of the table. This button is disabled if the
current display is the last page.
 Note
This dropdown list is available when you select the Display in Pages checkbox in the Customer Receivables Aging – Selection
Criteria window.
View
Select the appropriate view to display the data:
Summary – Select the Summary option to display each item's data consolidated in one row in the table including the basic
information. Note that this option is selected by default.
Detailed – Select the Detailed option to display detailed transactional data for each item.
 Note
This dropdown list is available when you select the Display in Pages checkbox in the Customer Receivables Aging – Selection
Criteria window.
Vendor Liabilities Aging
This report analyzes vendor liabilities, sorted by age.
Use this window to specify selection criteria for the Vendor Liabilities Aging report (see the topic Vendor Liabilities Aging Report).
To open the window, choose one of the following options:
Financials Financials Reports Accounting Aging Vendor Liabilities Aging
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:06 AM
Business Partners Business Partner Reports Aging Vendor Liabilities Aging
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Vendor Liabilities Aging Selection Criteria Fields
Group By
Specify whether to group the report by vendor or buyer.
Code From ... To
Specify a range for the business partner number.
Vendor Group
Specify a vendor group as a selection criterion.
Properties
Opens the Properties window, in which you can select the vendor properties.
Control Accounts
Select the checkbox and click to show only the transactions and balances for selected control accounts.
Select All
Report includes all vendors
Aging Date
Used to determine a liability age
The current date is the default setting.
You can change the default if, for example, you want to display all liabilities that are due for payment during the following week.
Interval
Specify a time interval for grouping liabilities.
From the dropdown list, select Days, Months, or Periods. If you choose Days, four new fields appear for you to specify the duration
of each time interval. You do not have to specify all four fields, but you must specify at least the first field. The default values for the
four fields are 30, 60, 90, and 120.
 Example
In the first two fields, specifying 20, 50 days as the interval subdivides the liabilities as follows:
Up to 20 days old
21 to 50 days old
51 days or older
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:06 AM
Translate Leading Currency at Aging Date
For documents created in foreign currencies, selecting this checkbox will display the local currency and system currency that are
converted from the document currency using the exchange rate on the aging date; deselecting this checkbox will display the local
currency and system currency that were posted in the journal entry from the document.
For documents created in local currency, selecting this checkbox will display the system currency that is converted from the
document currency using the exchange rate on the aging date; deselecting this checkbox will display the system currency that was
posted in the journal entry from the document. The report will display the foreign currency what was posted in the journal entry
from the document, no matter whether the checkbox is selected or not.
Display Vendors with Zero Balance
Report includes vendors with a zero balance
Display Reconciled Transactions
Displays reconciled journal entries according to their reconciliation date, rather than the journal entry dates
Ignore Future Remit
Hides the Future Remit column in the report and excludes transactions that have a value in this field
Vendor Liabilities Aging Report
SAP Business One displays the results of the report according to your selection criteria (see the topic Vendor Liabilities Aging).
It displays documents together with the respective liabilities. The report provides the size of the vendor liability and the time that
the debt has remained unpaid.
For an All Currencies business partner with a foreign currency as the displayed currency, the values in this report are converted
based on the current exchange rate and not on the original transaction exchange rate. This is because when the currency of a
business partner is set as All Currencies, the operative currency is the local currency, and related foreign currency transactions
are therefore not managed for the account.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Vendor Liabilities Aging Report
Currency
Specify the currency for displaying the report results.
Aging Date
Displays the aging date entered in the selection criteria window
Age By
Specify by which date to calculate the age of the liabilities: due date, posting date, or document date of the document/journal
entry.
Vendor Code
Displays the vendor code as defined in the business partner master data
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:06 AM
Vendor Name
Displays the name of the vendor, as defined in the business partner master data
Type
Displays the document type and provides a link to the document window
Installment No.
Displays the successive number of the installment
 Example
If a document contains three installments, each installment is displayed in a separate row, and this field displays the value 1, 2,
or 3, accordingly.
BP Ref. No.
Displays the business partner reference number
Number of Days Outstanding
The number of days between the due date and the aging date
Original Account
Displays the original document total, the original total of the installment, or the total value of a manual journal entry line
Future Remit
Displays all open liabilities owed to vendors according to the date selected in the Age By field and for which the date specified in
the Aging Date field has not yet been reached.
 Example
You have an open A/P invoice for USD100, due on May 1st.
Due Date is selected in the Age By field.
The Aging Date field is set to April 28th.
Since the invoice is due after the aging date, the invoice amount is displayed in the Future Remit column.
Project Code
Displays the code of the project to which the document's journal entry is assigned
Payment Method Code
Displays the code of the default payment method assigned to the business partner on the Accounting tab of the Business Partner
Master Data window.
[Time Intervals]
SAP Business One displays the relevant open liabilities in columns representing the specifications you made in the Interval field in
the selection criteria window.
The amount of future remit is first subtracted from the total sum of the liabilities.
The last column in each category includes open liabilities for the respective category prior to the first columns.
Days – Each column represents the number of days entered in the selection criteria window, moving back from the aging
date.
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:06 AM
Months – Each column represents one month, moving back from the aging date month.
Periods – Each column represents one period as defined in Administration System Initialization Posting Periods ,
moving back from the aging date period.
[Top Total Row]
Displays the sum of amounts listed in one column
[Bottom Total Row]
Displays the percentage of open receivables for each time interval
Campaign Management
SAP Business One lets you create, maintain, and analyze your marketing event information using the campaign management
feature. Managing a promotional campaign typically involves the steps outlined below:
Creating and Maintaining a Target Group
Creating a Campaign Using the Campaign Generation Wizard
Managing the Campaign Data
Viewing and Maintaining the Data
Generating Opportunities from a Campaign
Filtering Campaign Response E-Mails
Viewing the Campaign List Report
Creating and Maintaining a Target Group
Procedure
A target group is a list of prospects. You can create a target group and then define a promotional campaign targeting this group.
You can add prospects either from existing customers and leads, or from an external Microsoft Excel file.
 Note
To use the Target Group window, you require correct authorization for the window.
System administrators can assign Full Authorization, Read Only authorization, and No Authorization of this window to users.
To assign to users the authorization for the Target Group window, from the SAP Business One Main Menu, choose
Administration System Initialization Authorizations General Authorizations . In the General Authorizations window,
choose Administration Setup Business Partners Target Group .
To create a target group, proceed as follows:
1. From the SAP Business One Main Menu, choose Administration Set Up Business Partners Target Group .
2. In the Target Group – Set Up window, specify the Target Group Code and the Target Group Name for the new group and
choose Update.
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:06 AM
3. In the # column, double-click the gray sequence number area corresponding to the target group you created in step 2.
The Target Group Details window appears.
To use this window to define potential customers or leads for the target group, do one of the following:
Add Prospects from BP Master Data
In the Target Group Details window, add a business partner by specifying either the BP Code or the BP Name.
To add a group of business partners, choose Selection Criteria. In the Business Partners window, filter business
partners by their codes, groups, and properties.
Add Prospects from External Lists
To add prospects from external lists, do one of the following:
 Note
All the prospects that do not exist in the Business Partner Master Data are marked as External business
partners.
To add multiple contacts for one external business partner, add multiple entries for this business partner with
different contact information.
In the Target Group window, manually enter the business partner's information.
Import prospects from a Microsoft Excel file.
To do so, proceed as follows:
a. Prepare the list for importing. For more information, see Importing a Microsoft Excel File and
Preparing a Microsoft Excel Import File for Business Partners.
b. In the Target Group Details window, choose Import.
The Import from Excel window appears.
c. Each field in the Import from Excel window represents a column in the Microsoft Excel spreadsheet
to be imported. For each field, select the corresponding field definition in accordance with the column
definition from the Microsoft Excel spreadsheet.
d. Choose OK to save the data and open the file manager.
e. Select the file to be imported and choose Open.
You receive a message that the file is imported successfully.
More Information
Campaign Management
Creating a Campaign Using the Campaign Generation Wizard
Use the Campaign Generation Wizard to create promotional campaigns targeted at your prospects. This wizard guides you step-
by-step through the definition of parameters required to generate campaigns.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:06 AM
From the SAP Business One Main Menu, choose Business Partners Campaign Generation Wizard and follow the steps of the
wizard. In each step, choose Next to continue or Back to return to the previous step.
Please note that image maps are not interactive in PDF outputs.
Campaign Generation Wizard, Step 1: Campaign Generation
Options
Use this window to specify whether to generate a campaign based on an existing campaign or to define a new campaign.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Campaign Generation Options
Create New Campaign
Create a new campaign by following the wizard to define necessary parameters step by step.
Create Campaign Based on Existing Campaign
Load data of an existing campaign. Based on this campaign, you can update parameters as required to create and save a new
campaign.
Load Saved Campaigns
Load the campaigns that were saved but not yet executed.
Include Executed Campaigns
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:06 AM
Available only when you have selected the Load Saved Campaigns checkbox. Select the checkbox to additionally load the
campaigns that have already been executed.
Run an Executed Campaign Again
Choose an executed campaign and run it again.
Start Date From… To…
Specify a date range to display only the campaigns with start dates falling into this range.
Find by Name
Enter the key words in the campaign name to search for or narrow down target campaigns.
Exclude Lines with Business Partner’s Response
This field appears only if you have selected the Run an Executed Campaign Again radio button.
Select this checkbox to exclude the business partners that have already responded to the chosen campaign, that is, to exclude the
campaign lines with the Responsecheckbox selected in the chosen campaign. When you run an existing campaign again with this
checkbox selected, the campaign will not be executed for business partners that have already responded.
Run and Go to Final Step
This button is available when one of the following conditions applies:
You have selected the Load Saved Campaigns Only radio button, and the status of the campaign you selected is Open.
You have selected the Run an Executed Campaign Again radio button, and the status of the campaign you selected is
Open.
Choose this button to run the selected campaign and go directly to the final step of the wizard.
More Information
Creating a Campaign Using the Campaign Generation Wizard
Campaign Generation Wizard, Step 2: Campaign Details
Use this window to specify detailed information about the campaign.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Campaign Details
Campaign Type
Select from the dropdown list the type of the campaign.
You can view the type information of a campaign in the Campaign window. Options include: E-Mail, Mail, Fax, Phone Call, Meeting,
SMS, Web, and Other.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:06 AM
When you select an execution method in step 4 that is different from the campaign type you specify in this step, the wizard
execute campaign as you instruct in step 4. And the Campaign Type information you specified in step 2 is not affected. To view
the campaign information, choose Business Partners Campaign . For example, you create a campaign with the type
ofWeb. In step 4, the application default your choice as Generate URL. However, you choose to Generate External List at last.
An external list is generated, and the campaign data is saved with the campaign type of Web.
Target Group Type
Select the type of the target group for which you create the campaign.
Customer (for customers or leads)
Vendor
Owner
Opens the List of Employees window. Select one employee from the list to take charge of this campaign.
Target Group
Opens the List of Target Groups window. Select one group as the targeting prospects for the campaign.
Items
Opens the Items window.
Specify relevant items for the campaign. To maintain the item master data, choose Inventory Item Master Data .
Partners
Opens the Partners window. Select relevant partners for the campaign.
To maintain the partners data, choose Administration Setup Opportunities Partners .
Campaign Template
Opens the file manager. Select a template file to import to the campaign.
The following list explains the supported template file format for each of type of campaign execution method:
Generating External List: No campaign template format is supported.
Generating E-Mail Using Microsoft Office Outlook: TXT, HTML, JPG, GIF,BMP, PNG, and Word templates.
 Note
The application adds the Word template you specify into the e-mail as an attachment. For templates with other formats,
the application shows the file content directly in the e-mail body.
Generating E-Mail Using SAP Business One Mail: TXT and Word documents.
 Note
The application adds the Word template you specify into the e-mail as an attachment. For TXT templates, the
application shows the file content directly in the e-mail body.
Sending Fax: TXT
Generating URL: HTML
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:06 AM
For HTML templates, we recommend that you specify the template name in English, because template names
that contain non-UTF8 characters are not supported.
Make sure that the HTML template source file does not contain any CDATA statement.
Create Activities for Business Partners
Select to automatically generate an activity for each of the targeting prospect after the campaign is generated.
To view the activities created, choose Business Partners Activity . The campaign is automatically linked to the activity. In the
Linked Document tab, to view the campaign number this activity derives from, from the Document Type dropdown list, choose
Campaign. The Document No. field displays the linked campaign for this activity.
More Information
Creating a Campaign Using the Campaign Generation Wizard
Campaign Generation Wizard, Step 3: Target BPs
Use this window to view and maintain the targeting prospects of the target group you specified in step 2. You can update prospect
information, if necessary.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Business Partners
Find
Choose a column you want to search by double-clicking it; then enter search key words in this field. The first line that matches the
entered texts is highlighted.
If you do not choose any column, BP Code is seen as the default column for the search.
Internal
Shows whether this business partner exists in the Business Partner Master Data or not.
If you add this business partner from theBusiness Partner Master Data, the application selects the chechbox and marks
this business partner as Internal.
If you add this business partner from external lists, the application deselects the checkbox.
Clear
Clears all the business partners and prospects displayed in the table.
Add
Opens the Business Partner window where you can filter business partners by specifying the selection criteria.
Import
Opens the Import from Excel window. You can import an external Microsoft Excel list of prospects into this campaign.
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:06 AM
For more information about how to import an external list, see Add Prospects from External Lists in Creating and Maintaining a
Target Group.
More Information
Creating a Campaign Using the Campaign Generation Wizard
Campaign Generation Wizard, Step 4: Save & Execute Options
Use this window to save campaign data and execute the campaign.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Save & Execute Options
Save Campaign and Exit
This radio button is available only if you have selected the Create New Campaign or the Create Campaign Based on Existing
Campaign option in step 1 of the wizard.
Select to save the campaign data without execute the campaign. Choose the Next button to view the summary report.
To view the saved campaign data, choose Business Partners Campaign .
Save Campaign and Execute
This radio button is available only if you have selected the Create New Campaign or the Create Campaign Based on Existing
Campaign option in step 1 of the wizard.
Select to save the campaign data and execute the campaign with one of the following methods. For more information about how to
use campaign templates, see Campaign Generation Wizard, Step 2: Campaign Details.
Generate External List
Choose Next with this option selected, the Save As window appears. Proceed to save the campaign information into an
external communication list.
You receive a message asking you whether to export currency symbols. Choose Yes, to the same column to export
currency symbols and following values in one column; choose Yes, to a separate column to export symbols in a separate
column from the value column; choose No, to ignore the currency symbols to save values only.
Send E-Mail Using Microsoft Office Outlook
Choose Next with this option selected, Microsoft Office Outlook opens and automatically generates a new E-mail. The
subject of the E-mail is the campaign name and all the E-mail addresses of the contacts are copied to the Bcc column.
Send E-Mail Using SAP Business One Mail
Choose Next with this option selected, the Send Message window opens. The window displays all targeting prospects and
their information, with the Mail checkbox selected.
Send Fax
Choose Next with this option selected, the Send Message window opens. The window displays all targeting prospects and
their information, with the Fax checkbox selected.
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:06 AM
Generate URL
Choose Next with this option selected, the application generates a URL for the Web page with the campaign template via
SAP Business One Integration Component.
The summary report displays the URL. Customers are able to use the URL to access the campaign Web page.
Execute Campaign
This radio button is available only if you have selected the Run Existing Campaign radio button in step 1 of the wizard.
Select one of the methods to execute the campaign:
Generate External List
Choose Next with this option selected, the Save As window appears. Proceed to save the campaign information into an
external communication list.
You receive a message asking you whether to export currency symbols. Choose Yes, to the same column to export
currency symbols and following values in one column; choose Yes, to a separate column to export symbols in a separate
column from the value column; choose No, to ignore the currency symbols to save values only.
Send E-Mail Using Microsoft Office Outlook
Choose Next with this option selected, Microsoft Office Outlook opens and automatically generates a new E-mail. The
subject of the E-mail is the campaign name and all the E-mail addresses of the contacts are copied to the Bcc column.
Send E-Mail Using SAP Business One Mail
Choose Next with this option selected, the Send Message window opens. The window displays all targeting prospects and
their information, with the Mail checkbox selected.
Send Fax
Choose Next with this option selected, the Send Message window opens. The window displays all targeting prospects and
their information, with the Fax checkbox selected.
Generate URL
Choose Next with this option selected, the application generates a URL for the Web page with the campaign template via
SAP Business One Integration Component.
The summary report displays the URL. Customers are able to use the URL to access the campaign Web page.
More Information
Creating a Campaign Using the Campaign Generation Wizard
Campaign Generation Wizard, Step 5: Summary Report
Use this window to view the summary information of the campaign you executed. Errors and warning messages are also displayed.
The application automatically allocates a number to the campaign you generate. To view the data of the newly generated
campaign, choose before the campaign number.
More Information
Creating a Campaign Using the Campaign Generation Wizard
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:06 AM
Managing the Campaign Data
Use the Campaign window to manage your marketing events information. You can perform the following tasks:
Viewing and Maintaining the Campaign Data
Generating Opportunities and Leads from a Campaign
 Note
To use the Campaign window, you require correct authorization for the window. System administrators can assign Full
Authorization, Read Only authorization, and No Authorization of this window to users.
To assign authorization for the Target Group window to users, from the SAP Business One Main Menu, choose
Administration System Initialization General Authorizations . In the General Authorizations window, choose
Administration Setup Business Partners Campaign .
Procedure
Viewing and Maintaining the Data
You can create a campaign manually in the Campaign window. After you create and save a campaign using the campaign
generation wizard, the application automatically allocates a campaign number to this campaign. It also creates a document storing
the campaign data you specified in its Campaign window.
To access this window, from the SAP Business One Main Menu, choose Business Partners Campaign . By default, the window
opens in Add mode. The following tabs appear:
Business Partners
Use this tab to view and maintain business partners or prospects imported from an external list.
Items
Use this tab to view and maintain relevant items.
Partners
Use this tab to view and maintain partner companies involved in the campaign.
Attachment
Use this tab to attach relevant files to a campaign. You can attach as many files as needed.
 Note
You must specify an Attachments folder before you attach any file. To define the folder, choose Administration System
Initialization General Settings Path .
User Task User Action and Result
Deleting a Campaign Do one of the following:
In the Campaign window, right-click and choose Remove.
In the SAP Business One menu bar, choose Data
Remove .
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:06 AM
User Task User Action and Result
You receive the message:
Removing a campaign is irreversible. Do you want
to continue?
Choose Yes to remove the campaign.
Choose No to cancel the operation.
Duplicating a Campaign Do one of the following:
In the Campaign window, right-click and choose Duplicate.
In the SAP Business One menu bar, choose Data
Duplicate .
The application duplicates the Campaign Type and Target Group
information of the current campaign to a new campaign.
Canceling a Campaign Do one of the following:
In the Campaign window, right-click and choose Cancel.
In the SAP Business One menu bar, choose Data Cancel
.
You receive the message:
Canceling a campaign is irreversible. Campaign
status will be changed to “Canceled”. Do you
want to continue?
Choose Yes to continue setting the campaign status as Canceled.
Choose No to cancel the operation.
Generating Opportunities and Leads from a Campaign
After you successfully execute a campaign, some of your prospects may show their interest in your products and company. You
may want to generate opportunities and leads from the campaign as a record of the campaign result. To do so, proceed as follows:
1. In the Campaign window, find the campaign you want to work with. The Target BPs tab lets you view all the targeting
prospects involved in this campaign.
2. Find the prospect with an opportunity. In the Document Type column, choose Sales Opportunities. In the Document
Number column, choose to open the List of Opportunity window.
 Note
If the prospect for which you are going to generate an opportunity is not yet a business partner, the application
automatically creates a business partner before you link or generate an opportunity for this prospect.
3. In the List of Opportunity window, do one of the following:
To choose one of the existing opportunities, double-click the row.
The opportunity is linked to the campaign.
To create a new opportunity and link it to this campaign, choose New.
The Opportunity window appears. In the window, specify data as required and choose Add.
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:06 AM
Related Information
Adding Opportunities
Campaign Management
Campaign Window
Campaign Window
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Campaign Information
Target Group Type
Select the type of the target group for which you plan to create the campaign.
Customer (for customers or leads)
Vendor
Campaign No.
Automatically generated number the application assigns to this campaign.
Campaign Type
Select from the dropdown list the type of the campaign.
Default type: E-Mail.
Campaign Name
Specify a name for the campaign.
Target Group
Opens the List of Target Groups window. Select one group of targeting prospects for the campaign.
 Note
When you are trying to change a target group for an existing campaign, you receive a message:
You have specified a new target group. Do you want to replace all existing BPs in the
“Business Partners” tab with the new target group BPs?
Choose Yes to replace all existing business partners with the business partners in the target group. Choose No to change the
target group without changing the business partners in the Business Partners tab.
Status
Status of this campaign. Default status is Open.
Owner
Opens the List of Employees window. Select one employee from the list to take charge of this campaign.
Start Date
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:06 AM
Specify a start date for the campaign.
Default start date is the system date.
End Date
Specify an end date for the campaign.
Created by Campaign Generation Wizard
The checkbox is automatically selected when you are viewing a campaign generated by the campaign generation wizard.
Internal
Shows whether this business partner exists in the Business Partner Master Data or not.
When the checkbox is selected, it means that this business partner exists in the Business Partner Master Data.
When the checkbox is deselected, it means that this business partner is not yet added to the Business Partner Master
Data. You may have added this business partner in the Target Group window or in the Campaign window.
Response
Marks a business partner's response status for this campaign.
Select the checkbox when this business partner responds the campaign.
In the Campaign List report. you can view the total number of business partners who respond to your campaign.
More Information
Managing the Campaign Data
Filtering Campaign Response E-Mails Using the Common
Functions Widget
Prerequisites
1. You have enabled the cockpit function.
2. You have added the Common Functions widget to your cockpit and have added the Campaign item to this widget. For more
information about this widget, see Common Functions
Procedure
1. From Microsoft Office Outlook, select one e-mail to be matched.
 Note
The application matches one e-mail at a time. If you have dragged multiple e-mails to match a campaign, only the last
mail of your selections will be processed.
2. Drag the e-mail to the Campaign item in the Common Functions cockpit.
3. The application searches the sender’s e-mail address in the campaign database.
If the application finds the same e-mail address as in the contact person information of a campaign, the campaign form
appears with the campaign data displayed.
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:06 AM
If the application finds no records of this e-mail address in the campaign database, you receive the message:
No relevant campaign found.
Related Information
Campaign Management
Working with the Cockpit
Viewing the Campaign List Report
To see at a glance all campaigns that exist with particular business partners or for certain date ranges, you can generate a
Campaign List Report.
Procedure
1. From the SAP Business One Main Menu, choose Business Partners Business Partner Reports Campaign List .
Alternatively, open it from the Reports module.
2. In the Campaign List – Selection Criteria window, specify the selection criteria for the report, for example:
Item code
Item group
Target BP Type
Business Partner Code
Business Partner Group
Customer group
Campaign No.
Campaign type
Campaign status
Response Type
Document Types
Campaign start date and end date
3. Choose OK.
Result
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
The campaign list shows the following information:
BP Code
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:06 AM
Displays the code of the business partner of this campaign.
Sales Amount
Available only when the target group type of the campaigns is Customer.
Displays the sales amount of the linked marketing document. When the linked document is a Sales Opportunity, the potential
amount of it is displayed here.
Gross Profit
Available only when the target group type of the campaigns is Customer.
Displays the gross profit of the linked marketing documents. When the linked document is a Sales Opportunities, the gross
profit total of it is displayed here.
Gross Profit %
Available only when the target group type of the campaigns is Customer.
Calculates the gross profit rate of the linked document by dividing the gross profit by either the sales price or the base price,
according to the calculation method of the gross profit defined in the Document Settings window.
Number of BPs Contacted
Displays the number of the business partners you contact in this campaign.
Number of BPs Responded
Displays the number of the business partners who have responded this campaign.
You can mark business partners' response in the Campaign window.
Response %
Displays the BP response rate of the campaign.
The value equals the Number of BPs Responded divided by Number of BPs Contacted.
Number of Leads Generated
Displays the number of the leads generated through the campaign.
Number of Opportunities
Displays the number of opportunities generated in the campaign.
Number of Won Opportunities
Displays the number of the opportunities you have won.
Total Sales Amount
Available only when the target group type of the campaign is Customer.
Displays the total sales amount of the campaign.
Total Gross Profit
Available only when the target group type of the campaign is Customer.
Displays the total gross profit of the campaign.
Total Gross Profit %
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:06 AM
Available only when the target group type of the campaign is Customer.
Calculates the total gross profit rate of the campaign by dividing the gross profit by either the sales price or the base price,
according to the calculation method of the gross profit defined in the Document Settings window.
Opportunities Win Rate
Displays the win rate of the opportunities generated in this campaign.
The win rate equals the number of won opportunities divided by the total number of opportunities generated.
Verifying VAT Numbers for Business Partners
Prerequisites
 Note
This function is only available in the European Union, Norway, Switzerland, and the UK localizations.
You have selected the Verify VAT Numbers for Business Partners and Documents checkbox on the BP tab of the General
Settings window ( Administration System Initialization General Settings ).
You have full authorization for Verify VAT Numbers under Business Partners in the Authorizations window (
Administration System Initialization Authorizations General Authorizations ). This entry only appears after you
select the Verify VAT Numbers for Business Partners and Documents checkbox on the BP tab of the General Settings
window.
Context
You can verify business partners’ VAT identification numbers with VIES in one of the following two ways.
Procedure
To verify VAT numbers for a specific business partner, use the Verify VAT Numbers option in the You Can Also button.
1. From the SAP Business One Main Menu, choose Business Partners Business Partners Master Data .
2. In the Business Partners Master Data window, browse to the business partner for which you want to verify the VAT
identification numbers.
3. Choose the You Can Also button and choose Verify VAT Numbers.
4. In the Business Partners Master Data window, choose Update.
Procedure
To verify VAT numbers for business partners of your choice, use the Verify VAT Numbers window.
1. From the SAP Business One Main Menu, choose Business Partners Verify VAT Numbers .
2. In the Verify VAT Numbers window, specify your selection criteria to locate the business partners for which you want to
verify the VAT identification numbers.
3. Choose the Verify button.
There will be a status bar indicating the verification progress.
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:06 AM
Results
To check the responses from VIES, follow the procedure below:
1. In the Business Partners Master Data window, browse to the business partner for which you have verified the VAT
identification numbers.
2. In the general area, choose the ellipsis button next to the Federal Tax ID field.
3. In the Business Partner VAT Number Verification window, you can find all the VAT numbers for this business partner, and
the respective responses for each of them.
 Note
Response codes are empty for verifications performed after the upgrade to SAP Business One 10.0 FP 2105 and SAP
Business One 10.0 FP2105, version for SAP HANA.
This is custom documentation. For more information, please visit SAP Help Portal. 130