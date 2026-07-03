6/12/26, 12:25 PM
Localization for UK International and
Republic of Ireland
Generated on: 2026-06-12 12:25:55 GMT+0000
SAP Business One | 10.0
Public
Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/c77c8f1a3edb43e6a04c1a17dc75d8cb?locale=en-
US&state=PRODUCTION&version=10.0
Warning
This document has been generated from SAP Help Portal and is an incomplete version of the official SAP product documentation.
The information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be
missing important aspects and/or correlations to other topics. For this reason, it is not for production use.
For more information, please visit https://help.sap.com/docs/disclaimer.
This is custom documentation. For more information, please visit SAP Help Portal. 1

6/12/26, 12:25 PM
Localization for UK International and Republic of Ireland
This documentation describes features and functions in SAP Business One that are specific to the localization for UK International
and Republic of Ireland.
Information about general features and functions that are not localization-specific is available in the online help for SAP Business
One. You can also access the online help and localization-specific information directly in SAP Business One ( Help
Documentation Online Help and Help Documentation Country/Region Specific Information ).
Setup and Administration: UK International and Republic of
Ireland
This section describes the settings and definitions related to functions that are specific to the localization for UK International and
Republic of Ireland. For information about the localization for the United Kingdom of Great Britain and Northen Ireland, please see
the separate dedicated localization-specific information.
Information about settings and definitions related to general functions is available in the general online help file, under: Help
Documentation Online Help .
Company Details
Accounting Data tab
Use Deferred Tax
Select if you want to recognize tax when the payment takes place and not when the invoice is created.
Extended Tax Reporting
Generates and saves tax reports for the tax authorities through BAS reporting.
Making Tax Digital
Activates functionality to interact with the United Kingdom tax authorities HMRC through Making Tax Digital processes.
See the section Making Tax Digital in localization-specific information for the United Kingdom of Great Britain and Northen Ireland
for more information.
Period Type for Report Generation
Related to Extended Tax Reporting. Specify the period type for report generation.
Enable Automatic Adjustment of Payment with Cash Discount
Enables automatic creation of correctional posting for payments with a cash discount. If you select this checkbox, the Automatic
Adjustment of Payment with Cash Discount checkbox on business partner master data is selected for each new business partner
by default.
Basic Initialization tab
Enable Intrastat
Select the checkbox to initialize the Intrastat declaration function. After you have installed Intrastat, this checkbox becomes
uneditable. For more information, see Initializing the Intrastat Declaration Function.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/12/26, 12:25 PM
 Note
Default templates for the Asset History Sheet are available for companies who use predefined chart of accounts. When using
user-defined chart of accounts these default templates are not available. The chart of accounts is defined here:
Administration System Initialization Company Details Basic Initialization tab Chart of Accounts Template
Tax-Related Definitions
To set tax-related definitions choose: Administration Setup Financials Tax The following settings are available:
Tax Groups
Tax Code Determination
Withholding Tax Codes
Tax Declaration Boxes - Setup Window
Tax Groups (Tax Codes)
SAP Business One provides predefined tax groups (tax codes under English UK settings) for supported localizations to be used by
your company for purchasing, sales, and payments.
Tax Groups (Tax Codes) - Setup Window
Use this window to define your company's tax groups (tax codes under English UK settings).
To open this window, choose Administration Setup Financials Tax Tax Groups .
Tax Groups – Setup Window
Code, Name
Specify a code and name for the tax group.
Inactive
Select to indicate that the tax group is inactive. Once the tax group is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
Category
Select one of the two tax groups:
Output Tax – tax groups for A/R documents
Input Tax – tax groups for A/P documents
EU
Select this option if the tax group is used for transactions with European Union countries (relevant only for Output Tax groups).
Triangular Deal, Goods Shipment, Service Supply
Select Goods Shipment, Triangular Deal, or Service Supply. These three fields are mutually exclusive.
Acquisition/Reverse
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/12/26, 12:25 PM
This column is relevant only for Input Tax groups (A/P). Select this option to define the tax group as pertaining to Acquisition /
Reverse.
Specifying the acquisition tax is a procedure used when you record goods purchased from EU countries. Tax is not calculated in the
document, but the correct amount is recorded in the journal entry and affects the tax report. In this case, the tax amount in the
rows and in the total of the A/P invoice would be 0.
Effective from, Rate %
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can create additional entries by double-clicking the row number of the
tax group and defining them in the Tax Definition window.
 Note
The tax amounts in the documents are calculated according to the tax group's effective date.
Non Deduct. %
The rate of tax that was paid but not allowed as a deduction. The calculation of the non-deductible amount is based on the tax
amount. Relevant only for Input tax groups (A/P).
 Example
Rate of input tax group: 16%
Rate of non-deductible: 4%.
When creating an A/P invoice for total amount of 100, the amount of total tax is 16 from which 0.64 (=4%*16) is the non-
deductible amount and 15.36 is deductible.
When using a tax group defined as non-deductible, the total amount of tax is divided between the tax account and the non-
deductible tax account.
Non Deduct. Acct
Specify the account to which you want to post the non-deductible tax amounts.
Tax Account
Specify a G/L account to use in journal entries containing this tax group.
Acquisition Tax Account
Specify a G/L account to use in journal entries containing an acquisition tax.
Deferred Tax Account
Specify the account to which you want to post deferred tax amounts.
Group Description
Use this informative field to enter values, which could be used later as parameters in user queries.
Cash Discount Account
Specify the account to which you want to post cash discount amounts.
Tax Definition - Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/12/26, 12:25 PM
Use this window to specify tax information for a specific group or code.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Groups .
Select the required tax group and choose the Tax Definition button.
Tax Definition - Setup Window
Effective From, Rate
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can specify new values.
 Note
The tax amounts in the documents are calculated according to the tax group's effective date.
Deferred Tax and Exchange Rate Differences
In a deferred tax system, you report collected or paid tax according to the date the tax is actually paid, and not according to the
date the marketing document is created. If the document has been created using a foreign currency, it is likely that the exchange
rates differ on these dates.
If tax is reported in the local currency at the exchange rate applied when the marketing document is settled, and not at the
exchange rate applied when the document was created, the resulting differences need to be accounted for.
Hence the amount of VAT or any other deferred tax calculated in the original document is only for provisional purposes. It is not
considered as the basis for the amount of tax to be paid or reported to the local tax authorities.
Currency exchange rate differences in documents where deferred tax is applied can be posted to a new G/L account.
 Note
The documents covered by the deferred tax system are: A/R and A/P invoices, A/R and A/P credit memos, A/R and A/P down
payment invoices. Exchange rate differences are not liable to tax.
Prerequisites
The deferred tax method must be in use in SAP Business One and the apply exchange rate on deferred tax function set up for your
company.
Example
An A/R invoice was created in US dollars with an exchange rate of 10 Mexican pesos per US dollar. This is for one transaction row
item of 1000 US dollars and VAT of 15% deferred (150 US dollars is the tax amount liable). The G/L account postings are as follows
on the date the A/R invoice is created:
USD (Foreign Currency) Mexican Pesos (Local Currency)
Customer 1150 11500
A/R 1000 10000
VAT Deferred 150 1500
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/12/26, 12:25 PM
When the A/R invoice is paid, the exchange rate is 11 Mexican pesos per US dollar.
If the apply exchange rate on deferred tax function is not set up for your company, the G/L account postings are as follows:
|               | USD (Foreign Currency) |      | Mexican Pesos (Local Currency) |       |
| ------------- | ---------------------- | ---- | ------------------------------ | ----- |
| Cash          | 1150                   |      | 12650                          |       |
| Customer      |                        | 1150 |                                | 11500 |
| VAT Deferred  | 150                    |      | 1500                           |       |
| VAT Payable   |                        | 150  |                                | 1500  |
| Exchange Rate |                        |      |                                | 1150  |
Gain/Loss
If the apply exchange rate on deferred tax function is set up for your company, the G/L account postings are as follows:
|               | USD (Foreign Currency) |      | Mexican Pesos (Local Currency) |       |
| ------------- | ---------------------- | ---- | ------------------------------ | ----- |
| Cash          | 1150                   |      | 12650                          |       |
| Customer      |                        | 1150 |                                | 11500 |
| VAT Deferred  | 150                    |      | 1500                           |       |
| VAT Payable   |                        | 150  |                                | 1650  |
| Exchange Rate |                        |      |                                | 1150  |
Gain/Loss
| Tax Exchange Rate |     |     | 150 |     |
| ----------------- | --- | --- | --- | --- |
Gain/Loss
Activating Exchange Rate Difference Handling for Deferred Tax
Prerequisites
The deferred tax method is set up as follows:
In  Administration   System Initialization   Company Details   Accounting Data  you have determined whether to
manage a deferred tax system for customers, vendors, or both.
In  Business Partners   Business Partner Master Data   Accounting   Tax  you have defined whether to include each
business partner in the deferred tax system.
Since the reporting according to the deferred tax method is done by using special G/L accounts, in  Administration
 Setup   Financials   Tax   Tax Groups (Tax Codes) , you have set up each tax code you want to include in the deferred tax
system, and in a deferred tax account.
Context
Exchange rate difference handling for deferred tax can be activated at any time, but once it is activated and transactions have been
processed, then it cannot be disabled. It is not activated by default for either an existing or a new company.
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/12/26, 12:25 PM
Procedure
1. From the SAP Business One Main Menu, choose Administration System Initialization Company Details Accounting
Data tab.
2. Select the Apply Exchange Rate on Deferred Tax checkbox.
Results
A new G/L account, Realized Exchange Diff. Gain/Loss on Deferred Tax, is added at company level. Exchange rate differences in
marketing documents where deferred tax is applied are posted to this G/L account.
To see the newly-added account, from the SAP Business One Main Menu, choose Administration Setup Financials G/L
Account Determination .
Related Information
Deferred Tax and Exchange Rate Differences
Deferred Tax Account
For reporting purposes, at the end of a company’s financial period, any invoice posted to the accounts within this period must have
a corresponding tax liability recorded in the same period.
In the localizations where deferred tax is supported, the tax liability crystallizes only when the payment is due. It is common
business practice for there to be a delay between the invoice creation and its associated payment. When the end of the financial
period falls within this delay period, the tax value in respect of the invoice is recorded in the deferred tax account to identify the
matching tax liability for the period. At the end of the financial period, the transactions that make up the value of the accrued tax
liability must be easily auditable.
In SAP Business One, postings to the deferred tax account are automatically reconciled (either fully or partially) when deferred tax
is applied in the following scenarios:
Creating an incoming or outgoing payment based on an AR/AP invoice, AR/AP down payment invoice, AR/AP reserve
invoice, AR/AP credit memo
The deferred tax amount is posted to the deferred tax account when you create the base document. When you create a full
or partial incoming or outgoing payment on the base document, a reversal posting is made to the deferred tax account with
a proportionate amount. As a result, the deferred tax account is reconciled in proportion to the paid tax amount.
Creating a credit/debit memo based on an AR/AP invoice, AR/AP down payment invoice
The deferred tax amount is posted to the deferred tax account when you create the base document. When you create a
credit/debit memo fully or partially on the base document, a reversal posting is made to the deferred tax account with a
proportionate amount. As a result, the deferred tax account is reconciled in proportion to the credited/debited tax amount.
Creating an AR invoice with payment
The deferred tax account is credited and then debited with the deferred tax amount. As a result, the deferred tax account
balance is brought to zero, and the postings to this account are fully reconciled.
Manually reconciling an AR/AP invoice, AR/AP down payment invoice, AR/AP reserve invoice with an AR/AP credit memo,
incoming or outgoing payment on account
When you manually reconcile an invoice with a credit memo or payment, an internal reconciliation applies for the BP
account. At the same time, a separate reconciliation applies automatically for a G/L account, the deferred tax account.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/12/26, 12:25 PM
If the payment, or the reconciliation of the BP account is cancelled, the reconciliation of the deferred tax account is also
cancelled automatically.
However, in the above scenarios, if the deferred tax account has been involved in a manual reconciliation before the automatic
system reconciliation takes place, SAP Business One does not perform the system reconciliation.
  Example
1. You create an A/R invoice for item B01 using deferred tax as follows:
| Item No. Quantity |     | Unit Price | Total | Tax | Item Cost |     |     |
| ----------------- | --- | ---------- | ----- | --- | --------- | --- | --- |
| B01 5             |     | 20         | 100   | 14  | 10        |     |     |
The corresponding journal entry posting is as below:
| Account                    |     | Debit |     |     | Credit |     |     |
| -------------------------- | --- | ----- | --- | --- | ------ | --- | --- |
| BP Account                 |     |       |     |     |        |     |     |
| Deferred Tax Account       |     |       |     |     | 14     |     |     |
| Revenue Account            |     |       |     |     | 100    |     |     |
| Inventory Account          |     |       |     |     | 50     |     |     |
| Cost of Goods Sold Account |     | 50    |     |     |        |     |     |
2. You create a partial incoming payment based on the A/R invoice as follows:
| Total | Total Payment |     | Payment Means |     |     |     |     |
| ----- | ------------- | --- | ------------- | --- | --- | --- | --- |
| 114   | 38            |     | Cash          |     |     |     |     |
The corresponding journal entry posting is as below:
| Account                  |     | Debit |     | Credit |     |     |     |
| ------------------------ | --- | ----- | --- | ------ | --- | --- | --- |
| Cash on Hand             |     | 38    |     |        |     |     |     |
| BP Account               |     |       |     |        |     |     |     |
| VAT Payable (Output Tax) |     |       |     | 4.67   |     |     |     |
| Deferred Tax Account     |     | 4.67  |     |        |     |     |     |
SAP Business One automatically reconciles the postings to the deferred tax account as follows:
| Account              | Debit |     | Credit |     |     | Reconciliation Amount | Balance Due |
| -------------------- | ----- | --- | ------ | --- | --- | --------------------- | ----------- |
| Deferred Tax Account | 4.67  |     | 14     |     |     | 4.67                  | 9.33        |
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/12/26, 12:25 PM
In this case, the deferred tax account is reconciled in accordance with the paid tax amount. As a result, the deferred tax account
balance due is 9.33.
Tax Code Determination
In sales and purchasing documents, you must specify a tax code for items and services that are liable for taxes. SAP Business One
proposes a tax code by default, which depends on the localization you are using.
You can set up tax code determination rules that take precedence over the tax information in the business partner or item master
data, and G/L account determination. When you create a sales or purchasing document, the application proposes a tax code for
each item line based on the rules you defined, but you can overwrite this proposal.
In tax code determination, you can do the following:
Define tax code determination rules
Update tax code determination rules
Delete tax code determination rules
Change the order of tax code determination rules
Define tax code determination rules for freight charges
For more information, see Working with Tax Code Determination Rules.
If you do not define tax code determination rules, the tax code is determined as follows:
Item type documents Service type documents
1. Default tax code in business partner master data 1. Default tax code in business partner master data
2. Default tax code in item master data 2. Default tax code in account details
3. Default tax code in freight setup 3. Default tax code in freight setup
4. Default tax code in G/L account determination 4. Default tax code in G/L account determination
Working with Tax Code Determination Rules
You define tax code determination rules to determine how the application proposes tax codes in sales and purchasing documents.
 Caution
If several superusers are connected to the same company database and add a tax code determination rule at the same position
in the hierarchy, the database may become inconsistent.
Procedure
Defining Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/12/26, 12:25 PM
The Tax Code Determination Rule Setup window appears.
2. Specify at least the following mandatory data:
Document Type
Business Area
Condition
You can specify up to five conditions, for example, ship-to address, item, or user-defined field (UDF), and their values
per rule.
 Note
If you create several rules with the same conditions, the application cannot apply the rule, because it is not
unique. For example, rule 1 has the condition Ship-To Address, and rule 2 also has the condition Ship-To Address.
Value
If you do not manage freight in documents: Line Tax Code.
If you manage freight in documents: Line Freight Tax or Header Freight Tax. In this case, specifying a line tax code is
optional.
Filling in the other columns is optional. For more information, see Tax Code Determination – Setup Window.
 Recommendation
Specify the data in the order given here, that is, first the document type, then the business area, and so on.
3. If you selected UDF as a condition, the User-Defined Fields Selection window appears. In this window, select the relevant
UDF.
4. Repeat step 2 for all tax code determination rules that you want to define. Note that you can copy, cut and delete several
rows at the same time by choosing CTRL plus the relevant option from the right-click menu.
5. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
6. To confirm the change, choose Yes.
Updating Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Change the relevant data.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Deleting Tax Code Determination Rules
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/12/26, 12:25 PM
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Select the line of the rule that you want to delete, right-click, and choose Delete Row. To delete several rules at the same
time, hold the CTRL key when clicking the tax code determination rule lines.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Changing the Order of Tax Code Determination Rules
Changing the order of tax code determination rules affects the process of tax code proposals in sales and purchasing documents.
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Select the tax code determination rule that you want to move. You can move only one rule at a time.
3. Drag and drop the rule to the desired location in the hierarchy.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Defining Tax Code Determination Rules for Freight Charges
You can define tax code determination rules for freight charges only if the Manage Freight in Documents field is selected in
Administration System Initialization Document Settings .
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Specify the data as described above in Defining Tax Code Determination Rules. In addition, enter the following data:
Line Freight Tax
Header Freight Tax
3. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
4. To confirm the change, choose Yes.
More Information
Tax Code Determination
Tax Code Determination – Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/12/26, 12:25 PM
Tax Code Determination - Setup Window
Use this window to define tax code determination rules, according to which the application proposes tax codes in sales and
purchasing document lines.
Tax Code Determination – Setup Window Fields
Determination Order
The position of the tax code determination rule within the hierarchy of tax code determination rules. When determining the tax
code proposal in a sales or purchasing document, the application works its way through the rules starting at the highest position.
Document Type
Specify for which type of document, for example, item, service, or both, the tax code determination rule is relevant. This field is
mandatory.
Business Area
Specify whether the tax code determination rule is relevant for sales or purchasing, or both. This field is mandatory.
Condition
Select a condition based upon which the tax code is determined. The conditions that you can select depend on the localization you
are using. You can specify up to five conditions, for example, business partner, item, ship-to address, or user-defined fields.
If you select more than one condition, all conditions must be met for the tax code determination rule to be applied.
This field is mandatory.
Value
Specify a value for the condition you selected in the Condition column. This field is mandatory.
Depending on the condition you selected, you can either select a value from a list or enter a value. The value itself also depends on
the condition selected.
 Example
Condition Value or Action
Federal Tax ID Filled-in
Empty
Business Partner Select the relevant business partner code.
Ship-to Address Select the ship-to address defined in the business partner master
data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Description
If necessary, enter an additional explanation for the tax code determination rule.
Line Tax Code
Specify the tax code that should be proposed in sales or purchasing documents, if the tax code determination rule applies. Use one
of the tax codes defined in the application or create a new one. Depending on the business area you specified, you can only select a
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/12/26, 12:25 PM
tax code relevant for that business area. For example, if you selected Sales as a business area, the application only displays sales
tax codes.
In the sales or purchasing document, you can change the tax code that is proposed by the tax code determination rule.
Line Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document lines.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
Header Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document headers.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
More Information
Working with Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
When defining tax code determination rules, you specify conditions and values that must apply for the application to propose a tax
code on sales and purchasing documents. The conditions and values you can specify depend on the localization of SAP Business
One that you are using as well as on the document type and business area. The table below lists the conditions and values that are
available for the different localizations.
You can specify values by using the dropdown list or, for some values, by entering free text. For some of the conditions and values, if
you have specified them once, you can select the value that was used last for the condition from the dropdown list.
Conditions and Values for Tax Code Determination Rules
Condition Value
Federal Tax ID
Filled in: The Federal Tax ID field on the sales or purchasing
document must contain a value.
Empty: The Federal Tax ID field on the sales or purchasing
document must be empty.
Ship-To Address Choose: Select the ship-to address defined in the business partner
master data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Ship-To Street / PO Box
Choose: Select a ship-to street / PO box defined in the
business partner master data.
Filled in: The Street / PO Box field in the ship-to address of
the sales or purchasing document must contain a value.
Not defined: The Street / PO Box field in the ship-to
address of the sales or purchasing document must not
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/12/26, 12:25 PM
Condition Value
contain a value.
Ship-To City
Choose: Select a ship-to city defined in the business
partner master data.
Filled in: The City field in the ship-to address of the sales or
purchasing document must contain a value.
Not defined: The City field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Zip Code
Choose: Specify a ship-to zip code.
Filled in: The Zip Code field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The Zip Code field in the ship-to address of
the sales or purchasing document must not contain a value.
Ship-To County
Choose: Select a ship-to county defined in the business
partner master data.
Filled in: The County field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The County field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To State
Choose: Select a ship-to state defined in the application.
Filled in: The State field in the ship-to address of the sales
or purchasing document must contain a value.
Not defined: The State field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Country/Region
Choose: Select a ship-to country/region defined under
Administration Setup Business Partners
Countries/Regions .
EU: The item is shipped to a member state of the European
Union.
Non-EU: The item is shipped to a country/region outside of
the European Union.
Item Choose: Select an item code from the list.
Item Group Choose: Select an item group from the list.
Business Partner Choose: Select a business partner from the list.
Customer Group Choose: Select the customer group the customer must be
associated with from the list.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/12/26, 12:25 PM
Condition Value
Vendor Group Choose: Select the vendor group the vendor must be associated
with from the list.
Warehouse
Choose: Select a warehouse that the item must be shipped
from or to.
Filled in: The Warehouse field on the sales or purchasing
document must contain a value.
Not defined: The Warehouse field on the sales or
purchasing document must not contain a value.
G/L Account Choose: Select the G/L account that must be used on the sales or
purchasing document for the rule to apply.
Tax Status
Liable: The tax status field in the business partner master
data must contain the value Liable.
Exempt: The tax status field in the business partner master
data must contain the value Exempt.
EU/Acquisition: The tax status field in the business partner
master data must contain the value EU or Acquisition.
Freight Choose: Select a type of freight from the list.
UDF Choose: Select a user-defined field that you use on the sales or
purchasing document, business partner or item master data, for
warehouses, or item groups.
More Information
Tax Code Determination
Working with Tax Code Determination Rules
Tax Code Determination - Setup Window
Example: Tax Code Determination Rules Applied on Marketing
Docs
The following examples illustrate how the tax code determination (TCD) rules are applied when you create a sales or purchasing
document.
Tax code determination rule with line and header freight tax conditions defined
TCD rule definition Master data
Line Tax Code Line Freight Tax Header Freight Tax BP Item
A1 A4 A5 A2 A3
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/12/26, 12:25 PM
TCD rule definition Master data
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A4                    | A5                      |     |     |     |
Tax code determination rule without line tax code defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| Not defined   | A2               | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A2            | A2                    | A2                      |     |     |     |
Tax code determination rule with one condition for header freight
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | A5                 | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A5                      |     |     |     |
Tax code determination rule without freight tax conditions defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A2                      |     |     |     |
Tax code determination rule without freight tax conditions defined – freight tax code defined in freight setup
| TCD rule definition |     |     | Master data |     | Freight Setup |
| ------------------- | --- | --- | ----------- | --- | ------------- |
Line Tax Code Line Freight Tax Header Freight Tax BP Item Freight Tax Code
| A1  | Not defined | Not defined | Not defined | Not defined | A6  |
| --- | ----------- | ----------- | ----------- | ----------- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/12/26, 12:25 PM
TCD rule definition Master data Freight Setup
Tax code proposed on document
Item Tax Code Line Freight Tax Header Freight Tax
Code Code
A1 A6 A6
More Information
Tax Code Determination
Defining BAS Codes
Define the BAS codes you need for your business activity statement reporting. You can add or remove BAS codes, for example if
there are any changes in tax regulations.
Procedure
Adding New BAS Codes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Specify the following data:
Code
Name
Type
Summary field
Debit/credit
Formula syntax
3. Choose the BAS Code Definitions - Rows button and set additional parameters for the BAS code.
 Note
The BAS Code Definitions - Rows button is available for BAS codes of types VAT Group (VAT Code under English UK
language settings), Account, and Single Choice.
4. Choose Update and OK.
Modifying BAS Codes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Change the data in the table, for example, the debit/credit data or the formula syntax. For more information about these
fields, see BAS Code Definitions Window.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/12/26, 12:25 PM
 Note
Depending on the type of tax code, you can only change certain items of information. For account type tax codes for
example, you can only change the debit/credit information, but not the summary field. The items that you cannot
change are grayed out as inactive.
Removing BAS Codes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Place your cursor in a row and choose Data Remove from the menu bar.
3. Choose Update and OK.
The BAS code is removed.
Related Information
Business Activity Statement Reporting
BAS Code Definitions Window
In this window, you review the BAS codes used for business activity statement (BAS) reporting, modify or remove BAS codes, or
add new ones.
To open this window, choose Administration Setup Financials Tax BAS Code Definitions .
BAS Code Definitions Window
Code
Code of the tax category to be used in business activity statement reporting.
Name
Description of the tax category to be used in business activity statement reporting.
Type
Indicates how tax is calculated.
VAT Group (VAT Code under English UK language settings): Use this type to report, group, and filter transactions by tax
codes. You can combine tax codes and/or constants in a formula using mathematical operations.
If you include a tax code of type Acquisition/Reverse in the formula, you can define the Acquisition/Reverse Tax Type of
the tax code to report only the input tax part (debit side), the output tax part (credit side), or both the input and output tax
parts (both debit and credit sides) of the transactions. To do so, double-click the BAS code row to define the details.
Account: Use this type to report, group, and filter transactions by G/L accounts. You can assign each account to only one
BAS code. This means, after you select an account for a BAS code, it is not displayed for another code selection. We
recommend that you select the Display only accts with postings checkbox in the Select accounts for group: <group
name> window to filter unused accounts.
Manual Input: Use this type if you want to manually enter an amount or a percentage rate, for example, as an adjustment to
a BAS code, in the BAS Report - Generation window.
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/12/26, 12:25 PM
If you enter a percentage rate, you can use decimals. However, if you enter an amount as an adjustment to a particular BAS
code, you can use decimals only if they are allowed for this BAS code.
Formula: Use this type if you want to combine the existing BAS codes and/or constants in a formula using mathematical
operations.
When you include BAS codes in a formula, use brackets “[]”as placeholders for each BAS code.
 Note
You cannot include a BAS code of type Single Choice in a formula.
 Example
G1, G2, G3, G4, G5, G6, and G7 are BAS codes; S1 and S2 are tax codes.
Among the BAS codes, G5, G6, and G7 are of type Formula.
[G5] = [G2] + [G3] + [G4]
[G6] = [G1] – [G5]
[G7] = [G2] /11
G1 is of type VAT Code.
[G1] = [S1]+ [S2]
Single Choice: With this type, you can provide background information or additional remarks for certain BAS codes
according to legal regulations. You can specify a few legally valid options as reason codes and select only one of them for
reporting purposes.
 Example
1. You create the following BAS codes of type Manual Input:
F1: Varied fringe benefits tax installment, FBT code
F2: Estimated total fringe benefits tax payable, FBT code
2. To provide background information for F1 and F2, you create a BAS code F3 of type Single Choice, as follows:
F3: Reason for fringe benefits tax variation, FBT code
Reason Code 01: Benefits ceased/reduced and salary increased
Reason Code 02: Benefits ceased/reduced and no compensation to employees
Reason Code 03: Fewer employees
Reason Code 04: Increase in employee contribution
...
Summary Field
Select an option to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount
Non-Deductible Amount
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/12/26, 12:25 PM
Debit/Credit
Determines which parts of the transactions that are calculated are added: for example, only the debit amount, only the credit
amount, or both.
Formula Syntax
Indicates the formula syntax to calculate the tax amount.
Sort Order
Indicates the position of the tax code in the BAS statement.
Absolute Value
Displays the absolute amount for the relevant tax code in the report.
Position in Report
Displays the position of BAS codes in the report.
Related Information
Defining BAS Codes
Withholding Tax Codes - Setup Window
Use this window to define withholding tax codes for your company.
To open the window, choose Administration Setup Financials Tax Withholding Tax .
Withholding Tax Codes - Setup Fields
WT Code
Specify a code for the withholding tax.
Inactive
Select to indicate the withholding tax is inactive. Once the withholding tax is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
WT Name
Enter a description for the withholding tax code.
Category
Choose one of the following from the dropdown list:
Invoice – the withholding tax calculation appears in the invoice and is recorded in the journal entry when the invoice is
added.
Payment – the withholding tax calculation appears in the invoice, but is recorded in the journal entry when it is created by
the incoming payment based on that invoice.
Effective From
Enter the date from which a tax group rate (%) is effective.
Rate
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/12/26, 12:25 PM
Enter the rate of tax to be calculated from the date defined in the Effective From field.
Base Type
Choose either Gross (includes VAT) or Net from the drop-down list to determine from which amount the withholding tax will be
calculated.
% Base Amount
Specify the percentage of the base amount that is subject to withholding tax. The default value is 100%.
Official Code
Specify the official code to be reported in the withholding tax report.
Account
Choose the G/L account code to be recorded in journal entries relevant for this withholding tax code.
Withholding Tax Definition
Choose this button to open the Withholding Tax Definition - Setup: <XXX> window, in which you can define the Effective From
date and the tax percentage for the selected withholding tax code.
Minimum Taxable Amount
Specify the minimum taxable amount for the withholding tax to take effect.
More Information
Tax Definition - <XXX> Window
Tax Declaration Boxes - Setup Window
Use this window to define selection criteria for the tax declaration boxes appearing in the tax declaration box report.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax
Declaration Boxes .
Tax Declaration Boxes - Setup Window
Effective From
Enables you to set up groups of tax declaration boxes, with each group sharing one effective period. Proceed as follows:
1. Specify the date from which the group of tax declaration boxes you want to create is effective. From the Effective From
dropdown list, select one of the following:
01.01.1900
01.01.2024: This date is displayed by default.
Define New: If you want to specify a date other than 01.01.1990 or 01.01.2024, define a new one.
Once you define a new date, the tax declaration group that has the default Effective From date 01.01.2024 is copied
to the new group.
Similarly, every time you define a new date, the existing tax declaration box group that has the chronologically latest
Effective From date is copied to the new group.
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/12/26, 12:25 PM
 Note
The chronologically later Effective From date of one tax declaration box group automatically becomes the "Effective To”
date for the group with the early Effective From date.
For example, you only create two groups of tax declaration boxes, group A and group B. The Effective From dates of
group A and B are set as 01.01.2009 and 01.01.2010, respectively. Therefore, 01.01.2010 automatically becomes the
”Effective To” date of group A, that is, the effective period of group A is from 01.01.2009 to 01.01.2010.
2. If required, define the individual tax declaration boxes within the group you create.
For each group, you can define different numbers of tax declaration boxes, and each tax declaration box within the group
can have individual settings.
Code, Name
Enter a code and relevant description for the box.
Inactive
Select to indicate the tax declaration box is inactive. Once the tax declaration box is set as inactive, you cannot include it in the tax
declaration box report. By default, the checkbox is not selected.
Type
Choose one of the following options:
Vat Group – summarizes VAT groups in the box
Box – summarizes several boxes in this box
Summary Field
Choose to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount – the actual tax amount
Non-Deductible Amount
Debit/Credit
Choose one of the following options to determine what to add of the transactions that will be calculated in the box:
Debit Side – only the debit amount
Credit Side – only the credit amount
Debit Side + Credit Side – both the credit and debit amount
Formula Syntax
The calculation formula of the box (the tax groups and the relations between them). For more information on the formula, go here.
Sort Order
Define the display order of the boxes in the report by entering their successive numbers. By default, the next successive number is
entered when you update the Tax Declaration Boxes - Setup window.
Absolute Value
Displays the absolute box amount in the report.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/12/26, 12:25 PM
Box Definition - Rows
Opens the Box Definition – Rows window, in which you can define a formula for the selected box.
Box Definition - Rows - Setup Window
Use this window to define formulas for selected VAT groups or boxes.
To access this window, choose Administration Setup Financials Tax Tax Declaration Boxes . Double-click the relevant
box row.
Box Definition - Rows - Setup Window
VAT Group
Click the dropdown list and select the VAT group or box to include in the box.
Formula Sign
Click the dropdown list and select the arithmetic operation (+ or -) to define the relation between this VAT group or box, and the
one below it.
Choose Update to move to the next row.
After you have finished defining all VAT groups or boxes for the formula, choose Update to save your changes.
VAT Calculation, EU
The following procedure provides a working method by which the VAT is automatically calculated in manual journal entries
(including those created through recurring postings, postings templates and journal vouchers).
Prerequisites
The following preliminary definitions should be made in order to have the VAT calculated automatically.
You have gone to Financials Chart of Accounts and chosen the Account Details button. In the displayed G/L Account
Details window, you defined the relevant default tax group for each account and whether or not to allow changing the
chosen VAT group in transactions.
You have gone to Administration System Initialization Document Settings Per Document tab. From the drop-
down menu, you chose Journal Entry and defined whether or not to use automatic VAT calculation.
 Note
In order to create a one time journal entry without having the VAT calculated automatically, go to the Form Settings - Journal
Entry window and clear the Auto VAT checkbox.
Procedure
1. Choose a “base” account.
The default VAT group defined for this account appears in the Tax Group field in a journal entry, and in the Tax Code
field in a service document.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/12/26, 12:25 PM
In a manual journal entry, a row for the account defined as a tax account for the chosen tax group automatically
appears in gray. This tax account row is filled automatically and is not editable.
2. If changing VAT groups is allowed, the VAT Group and VAT Code fields are activated. You can choose a different VAT group.
3. Enter a debit or credit amount for the chosen account.
The tax amount is calculated according to the VAT amount and entered in the Tax Amount field.
 Note
To avoid calculating the credit or debit amount in advance, you can enter the total amount including VAT in the Gross
Value field and SAP Business One automatically calculates the debit or credit amount and the VAT amount. Note that
the gross value can be entered in local currency only.
4. Complete the journal entry, and add it.
The behavior described above for manual journal entries is relevant for journal entries created through posting templates,
recurring postings, and journal vouchers, as well.
 Note
SAP Business One can calculate the VAT according to the sign at the amount in the transaction and not only according
to the side it appears on. For example, a VAT amount on the debit side with a minus sign is considered as a VAT amount
on the credit side.
When creating an invoice for a service and no VAT group is defined for the selected account, SAP Business One uses the
default VAT group defined in Administration Setup Financials G/L Account Determination .
When you create a payment and apply a cash discount (prompt payment discount, PPD), the application posts a VAT
proportional to the discounted price on the invoice.You can enable the automatic adjustment of payment with cash
discount feature in Administration System Initialization Company Details Accounting . For more information,
see SAP Note 2132412 .
Intrastat
If your company is registered for VAT in a European Union (EU) member state and conducts business related to the trading of
goods (tangible, manufactured commodities such as fabrics, tools, oil, and so on) between member states with a trade value above
the exemption threshold, you must file monthly or, in Italy in some cases, quarterly Intrastat (Intra-EU Trade Statistics System)
declarations with the competent national authority. An Intrastat declaration is not used to collect data on services, except where
the service is an integral part of the contract for the supply of such goods, for example, freight and insurance charges that are
included in the price of the goods.
 Note
The Intrastat setup is available only if you have activated it in your system.
After initializing the Intrastat declaration function, you can use the Intrastat declaration wizard to prepare Intrastat declarations if
your company is based in one of the following countries/regions:
 Note
Some countries/regions do not have corresponding localizations in SAP Business One, for example, Bulgaria and Lithuania.
Nevertheless, you can still make Intrastat declarations if your company is based in one of these countries/regions.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/12/26, 12:25 PM
AT – Austria
BE – Belgium
BG – Bulgaria
CY – Cyprus
CZ – Czech Republic
DE – Germany
DK – Denmark
EE – Estonia
ES – Spain
FI – Finland
FR – France
GB – UK International / Republic of Ireland
 Note
Due to the UK’s departure from the European Union (EU) in a process known as Brexit, the SAP Business One
localization United Kingdom of Great Britain and Northern Ireland (UK) is available for UK customers to stay compliant
with reporting requirements following Brexit.
GR – Greece
 Note
SAP Business One supports the ISO country/region code “EL” for Greece instead of “GR”. When generating output files
for your Intrastat declarations, the system converts the country/region code from “EL” to “GR”.
HU – Hungary
IE – Irish Republic
IT – Italy
LT – Lithuania
LU – Luxembourg
LV – Latvia
MT – Malta
NL – Netherlands
PL – Poland
PT – Portugal
SE – Sweden
SI – Slovenia
SK – Slovakia
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/12/26, 12:25 PM
Before using the Intrastat declaration wizard to generate Intrastat declarations, you must make some additional settings. For more
information, see Configuring Intrastat Settings.
Initializing the Intrastat Declaration Function
Procedure
 Note
If your company database is upgraded from SAP Business One 8.82 or lower and you have already installed the Intrastat add-on
on it, you do not have to initialize the Intrastat declaration function manually; the system automatically enables the function
and the Enable Intrastat checkbox becomes uneditable.
1. From the SAP Business One Main Menu, choose Administration System Initialization Company Details .
2. On the Basic Initialization tab, select the Enable Intrastat checkbox.
A system message appears to remind you that initializing this function is irreversible,
3. After confirming that you want to continue with the initialization, choose the Update button in the Company Details
window.
Result
You can do the following:
Configure Intrastat settings for your company, business partners, and items. For more information, see Configuring
Intrastat Settings.
Make Intrastat declarations and create output files.
Upgrade of Intrastat Add-On
If you created your company in SAP Business One 8.82 or lower, and have installed the Intrastat add-on, the upgrade process has
the following effects or results:
During the upgrade, the wizard checks whether the following values of each Intrastat-relevant business partner are the
same:
Customer/Supplier VAT Reg. No. in the Business Partner Intrastat Setting window of the Intrastat add-on
Federal Tax ID in the general area – of the default ship-to address as well – in the Business Partner Master Data
window
If these two values are different, a new ship-to address is created for the business partner. For more information, see SAP
Note 1720067 .
The Enable Intrastat checkbox in the Company Details window is selected, which means that the Intrastat functionality is
automatically enabled for the upgraded company. For more information, see Initializing the Intrastat Declaration Function.
The old Intrastat data and settings are retained in the upgraded company as follows:
The data in the Business Partner Intrastat Setting window is moved to the Intrastat Settings tab of the
corresponding business partner master data. The exception is the old Customer/Supplier VAT Reg. No. field, which
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/12/26, 12:25 PM
is merged into a ship-to address of the business partner during the upgrade.
The data in the Item Intrastat Setting window is moved to the Intrastat Settings tab of the corresponding item
master data.
The data in the Configuration Tool window is moved to the Intrastat Configuration window.
The data in the old user-defined windows (for example, country/region-specific fields) is moved to the Intrastat
Configuration window.
Both open and closed declaration runs are saved in the Intrastat declaration wizard with the status Archived. However,
they serve only as a reference; you cannot reopen, overwrite, or correct any declaration run with the status Archived.
The marketing document has two pairs of Incoterms and Transport Mode fields. However, only one pair is used for Intrastat
declaration. We recommend that you hide the old add-on fields using the Form Settings tool.
To identify the add-on fields, choose View System Information . Their information is listed in the table below:
Field Field Name
Incoterms U-BNIncTrm
Transport Mode U-BNTrnMod
Configuring Intrastat Settings
Prerequisites
You have initialized the Intrastat declaration function. For more information, see Initializing Intrastat Declaration Function.
You have verified which Intrastat data and SAP Business One source fields are mandatory for your reporting country/region.
We recommend that you refer to the Intrastat Fields tab in the Intrastat Configuration window for verification. For more
information, see Intrastat Configuration: Intrastat Fields Tab
Context
To generate Intrastat declarations, you must configure Intrastat settings for your company, business partners, and items.
Procedure
1. In the Company Details window, define some general company information, for example, the company name and address.
2. In the Intrastat Configuration window, perform the following tasks:
On the General tab, specify some additional Intrastat-specific information. For more information, see Intrastat
Configuration: General Tab.
On the Intrastat Fields tab, specify data that need validation during the Intrastat declaration run. For more
information, see Intrastat Configuration: Intrastat Fields Tab.
On the other tabs, import or specify Intrastat codes, for example, Incoterms. For more information about code
import, see Intrastat Configuration Window.
3. Configure the Intrastat-relevant settings of your business partners and items. For more information, see Configuring
Business Partner and Item Intrastat Settings.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/12/26, 12:25 PM
4. Upload the electronic file formats that you use to create output files for your declarations. For more information, see Setting
Up Generic and Special-Purpose Electronic File Formats.
5. Specify the file path for saving the generated Intrastat declaration files. On the Path tab of the General Settings window,
choose XML File Folder and select an appropriate directory. This path is provided as default when you generate Intrastat
declaration files, but you can change it in the Intrastat declaration wizard.
Intrastat Configuration Window
Use this window to specify information required for making Intrastat declarations.
All tabs – except for the General and Intrastat Fields tabs – store various codes that are used for statistical purposes in
documents.
 Note
For some codes, you can specify one default value for import and one for export. When you select the Default for Export or the
Default for Import checkbox of one code, the original default code remains valid for export or import.
You can filter the data on all the tabs except for the General tab. For more information, see the page Filtering Data in SAP
Business One in the general online help file.
Tabs
General
On this tab, you specify some company information that is used in Intrastat declarations. For more information, see Intrastat
Configuration: General Tab.
Commodity Codes
Import or specify commodity codes laid down in the Combined Nomenclature to classify traded goods. You must assign a
commodity code to each item that should be declared. You can enter up to 10 characters for a commodity code in SAP Business
One, but only commodity codes of 8 or 10 characters are declared. For example, 01 represents live animals; 0101 represents live
horses, asses, mules and hinnies; and 01012100 represents pure-bred breeding animals.
The last two characters of a ten-character-long commodity code are a two-digit TARIC code. TARIC codes represent various rules
applied to specific products when imported into the EU, for example, tariff suspensions, tariff quotas, and tariff preferences.
You can also specify the following information for the appropriate commodity code:
A supplementary unit: The options in the Supplementary Units dropdown list are defined on the Suppl. Units tab.
A validity period: To define the validity period, specify the Valid From and Valid To dates. As commodity codes may change
over time, limiting their validity periods restricts the commodity codes, and therefore related transactions, from being
declared in invalid periods of time.
(Czech localization) A two-digit statistical code
In the Italy localization, you assign commodity codes to items whose Intrastat type is defined as Item.
Service Codes
Relevant to Italy only. You assign service codes to items whose Intrastat type is defined as Service.
Import or specify service codes that are to be assigned to services. Service codes are used to classify services for statistical
reporting needs.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/12/26, 12:25 PM
Define the validity period of each service code by specifying the Valid From and Valid To dates. As service codes may change over
time, limiting their validity periods restricts the service codes, therefore related transactions, from being reported in invalid periods
of time.
Regions
Import or specify the administrative regions – states, counties, provinces – in your country/region and partner countries/regions.
The regions can be used as the import destinations and export origins of items.
You need to indicate whether these regions are valid for import and export. Default regions must also be valid, and the default
regions for import and export can be the same ones.
Incoterms
Incoterms is a codification of delivery terms used in foreign trade contracts that is maintained by the International Chamber of
Commerce, such as FOB (Free On Board) and CIF (Cost, Insurance and Freight).
Specify a percentage statistical value for each Incoterm. The percentage is used to calculate the statistical value of a transaction.
Calculation of the statistical values depends on your setting of the Simplified Procedure checkbox on the General tab of the
Intrastat Configuration window.
Customs Procs
Import or specify customs procedures established by the Community Customs Code to identify goods subject to customs control.
For example, release for free circulation, transit, customs warehousing, inward processing, processing under customs control,
temporary importation, outward processing, and exportation.
You need to indicate whether these customs procedures are valid for import and export. Default customs procedures must also be
valid, and the default customs procedures for import and export can be the same ones.
Nature of Trans
Import or specify types of transactions, for example, straightforward sale or purchase, free-of-charge goods, goods sent for
processing, goods returned following processing, and so on.
You need to indicate whether these nature of transaction codes are valid for import and export. Default nature of transaction codes
must also be valid, and the default codes for import and export can be the same ones.
Statistical Procs
Import or specify codes for the statistical procedures that are defined with respect to customs procedures (Commission
Regulations (EEC): 54/77 and 3678/87), for example, after outward processing, after economic outward processing for textiles,
and so on.
Trans. Modes
Import or specify different transport modes by which the goods leave or enter the statistical territory of dispatch or arrival. Indicate
the default transport modes for export and import – they can be the same modes.
Ports of Entry/Exit
Import or specify ports of shipment or destination. You need to indicate whether these ports are valid for import and export.
Default ports must also be valid, and the default ports can be the same ones.
Suppl. Units
Import or specify supplementary units that are required for certain commodity codes. The supplementary units are used to
measure goods in other ways than net mass.
Intrastat Fields
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/12/26, 12:25 PM
This tab lets you specify which data to validate during a declaration run for the selected country/region. Different
countries/regions have different requirements for Intrastat declaration; the same country/region may also have different
requirements for import and export data.
The Required For columns indicate which fields are mandatory for declaration in the selected country/region. These columns are
by default hidden.
For more information, see Intrastat Configuration: Intrastat Fields Tab.
Import Button
The Import button is available for certain tabs. You can import the following codes from external files into SAP Business One:
Commodity codes
Service codes
 Note
Service codes are relevant only to the Italy localization.
Regions
Incoterms
Customs procedures
Nature of transactions
Statistical procedures
Transport modes
Ports of entry or exit
Supplementary units
 Recommendation
Import codes as follows:
1. On the tab of codes you want to import, export the table to a Microsoft Excel (or txt) file by clicking in the toolbar.
2. Fill out the Excel file with codes and other relevant data.
3. Import the Excel file back into SAP Business One by choosing the Import button on the appropriate tab of the Intrastat
Configuration window.
If you need to define supplementary units for some commodity codes, ensure that the supplementary units have already been
defined on the Suppl. Units tab before you import the commodity code file. Otherwise, the supplementary units will not be
imported.
Intrastat Configuration: General Tab
Use this tab to specify some Intrastat-specific information for your company.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/12/26, 12:25 PM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab Fields
VAT Reg. No. of Trader
Enter your PSI (provider of statistical information) VAT registration number if you have one. Otherwise, enter your VAT registration
number.
 Note
No default value is available for Austria (AT). You must specify a value manually.
VAT Reg. No. Extension
If your company is a branch company or a subsidiary, specify the VAT registration number extension.
Company Declaration ID
Your company's official identifier obtained from local authorities. In Germany (DE), this ID is used to automatically name
declaration files.
Degree of Obligation
Used in France. Your degree of obligation is based on your EU trade volume in the previous calendar year. If you exceed the
thresholds of arrival and dispatch within the current year, your degree of obligation changes as of the month during which the
thresholds are exceeded.
Intrastat Declaration Office
Office name where you file your Intrastat declarations. Generally you file your Intrastat declarations at your local statistical office.
Specify the value of this field according to the actual requirements.
Federal State of Tax Office
The default value comes from the State field on the General tab of the Company Details window.
Declaring Department
The department in your company that makes the declaration.
Validation Key Identification
Your company-specific identification of the key which has been used to validate the sent message, in this case the Intrastat
declaration.
Require All Data
Select this checkbox to force declaration of all necessary Intrastat field data. “Necessary Intrastat fields” refer to those specified as
required for import or export on the Intrastat Fields tab.
Intrastat declarations are generated only if all necessary Intrastat fields have values. If any necessary data is missing, the Intrastat
declaration wizard cannot proceed with the declaration.
For more information, see Intrastat Configuration: Intrastat Fields Tab.
Display Always Net Mass Value
Select this checkbox to display in the Intrastat declaration an item's net mass, even if the item's mass in the supplementary unit is
not zero.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/12/26, 12:25 PM
Track Country of Origin for Items
Select this checkbox to track item country of origin and allow the production of Intrastat reports with country of origin data.
Cannot be deselected or reversed after selection. Country of origin information in Item Master Data is used by default, unless
changes are made in Country of Origin Assignment for transactions
Simplified Procedure
To use document values as statistical values, select the Simplified Procedure checkbox. If you do not select this checkbox, the
statistical value equals the document line total multiplied by the Incoterms statistical percentage of the document line total.
Document Handling Section
To exclude ineligible document rows from your Intrastat declarations, select the following checkboxes and specify the thresholds if
possible:
Exclude Document Row with Quantity Less Than
Exclude Document Row with Total Amount Less Than
Note that you can specify negative amounts for both checkboxes. For the second checkbox, the currency is always the local
currency.
Exclude Document Row Marked as Without Qty Posting: Once selected, Intrastat declarations will exclude the credit
memo rows marked as Without Qty Posting. The checkbox is selected by default.
Electronic File Format
Choose from the list in Electronic File Manager. The chosen electronic file format is uploaded by default to Electronic File Format
in step 7 of the Intrastat Wizard. If Electronic File Format is changed while on step 7 Generating the Declaration File of the
Intrastat Wizard, then there is an option to update this field in Intrastat Configuration: General Tab with the change.
Intrastat Configuration: Intrastat Fields Tab
Use this tab to specify which fields to validate during a declaration run for a selected country/region. This tab also indicates which
fields are mandatory for import or export declaration.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Intrastat Fields Tab Fields
Country/Region
From the dropdown list, select a EU country/region. Different countries/regions have different fields for you to define and also
different mandatory fields.
If you need to include a country/region in the list or exclude a country/region from the list, select or deselect the EU checkbox of
the country/region in the Countries/Regions - Setup window. To open this window, choose Administration Setup Business
Partners Countries/Regions .
Field Source
Displays fields in which you need to specify Intrastat information and their locations. These field values are taken as the default
declaration values or, in some cases, the default values of some fields in the Intrastat Configuration window. The primary field
source takes priority over the secondary field source.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/12/26, 12:25 PM
The places that include source fields are listed below:
Company Details window
Intrastat Configuration window
Business partner master data
Item master data
Marketing documents that are eligible for Intrastat declaration
Field Location
Displays the steps in which the fields appear in the Intrastat declaration wizard or the target fields in the Intrastat Configuration
window.
Validation For
Select the Import or Export checkbox to specify the field will be validated during the declaration run for import or export.
 Note
The Validation For checkboxes are independent of the setting of the Require All Data checkbox on the General tab. For
example, if you deselect the Require All Data checkbox while selecting the Validation For checkbox for import, the field is still
validated during the import declaration run.
Required For
Uneditable. Indicates whether the field is mandatory for import or export declaration in the selected country/region. However, you
need to select the Require All Data checkbox on the General tab to force declaration of selected fields.
Import, Export
To indicate that a field requires validation or is mandatory for import or export declaration, select the corresponding Import or
Export checkbox, and choose the Update button.
Configuring Business Partner and Item Intrastat Settings
Configure Business Partner Intrastat Settings
1. From the SAP Business One Main Menu, choose Business Partners Business Partner Master Data .
2. In the Business Partner Master Data window, find the business partner you want to define or add a new business partner.
3. Define a default ship-to address that is in a EU country/region.
4. If the business partner is of type company, specify a federal tax ID for the default ship-to address.
 Caution
A valid federal tax ID must start with the appropriate country/region code; otherwise, the business partner is not
declared. For example, it must start with GB if the ship-to address is in the UK.
 Note
If the business partner is of type private , you do not need to specify a federal tax ID.
5. In the general area, select the Intrastat Relevant checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/12/26, 12:25 PM
The Intrastat Settings tab becomes available.
6. On the Intrastat Settings tab, specify the Intrastat settings of the business partner. For more information, see Business
Partner Master Data: Intrastat Tab.
7. To save the changes, choose the Update pushbutton.
Configure Item Intrastat Settings
1. From the SAP Business One Main Menu, choose Inventory Item Master Data .
2. In the Item Master Data window, find the item you want to define or add a new item.
3. In the general area, select the Intrastat Relevant checkbox.
The Intrastat Settings tab becomes available.
4. On the Intrastat Settings tab, specify the Intrastat settings of the item. For more information, see Item Master Data:
Intrastat Tab.
5. To save the changes, choose the Update pushbutton.
Business Partner Master Data: Intrastat Settings Tab
Use this tab to specify your business partners' Intrastat settings.
To display this tab, select the Intrastat Relevant checkbox on the General tab.
For the dropdown boxes, the list options are taken from the corresponding tabs in the Intrastat Configuration window. To open this
window, from the SAP Business One Main Menu, choose Administration Setup Financials Intrastat Intrastat
Configuration .
Intrastat Settings Tab Fields
Nature of Transactions
Select the major type of transactions you deal in with this business partner, for example, part of a sale or a hire transaction.
Statistical Procedure
Select a statistical procedure that represents when the goods cross the border, for example, after outward processing.
Incoterms
Select the major delivery terms you adopt when dealing with the business partner. The specified value is declared by default for the
business partner unless you specify otherwise in the marketing documents.
Transport Mode
Specify how the goods leave the statistical territory of dispatch or enter the statistical territory of arrival. The specified value is
declared by default for the business partner unless you specify otherwise in the marketing documents.
Port of Entry or Exit
Select the major port or airport used when the goods are delivered by water or air.
Customs Procedure
Select the major customs procedure for the goods delivered to or from the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/12/26, 12:25 PM
Item Master Data: Intrastat Settings Tab
Use this tab to specify the Intrastat settings of your items.
To display this tab, select the Intrastat Relevant checkbox on the General tab.
For the dropdown boxes, the list options are taken from the corresponding tabs in the Intrastat Configuration window. To open this
window, from the SAP Business One Main Menu, choose Administration Setup Financials Intrastat Intrastat
Configuration .
Intrastat Settings Tab Fields
 Note
In the Italy localization, the following fields appear only when you have selected Item from the Type dropdown list:
Commodity Code
Supplementary Unit
Factor of Supplementary Unit
Commodity Code
Specify the appropriate commodity code for the item. The commodity code is mandatory for making Intrastat declarations.
Supplementary Unit
Select a supplementary unit for the item.
The supplementary unit depends on the specified commodity code. When you change the commodity code, the supplementary
unit specified for the new commodity code in the Intrastat Configuration window is automatically selected.
Factor of Supplementary Unit
Specify a conversion factor of the specified supplementary unit. This factor is used to calculate the item's mass in supplementary
units.
Use Weight in Calculation of Mass in Supplementary Units
Select this checkbox to take weight into account when calculating the item's mass in supplementary unit. If you do not select this
checkbox, the item weight is not counted for when calculating the item's mass in supplementary unit.
Destination Region for Import, Region of Origin for Export
Select the default country/region and state – or county/region, province, region – in which goods arrive, and the default
country/region and state – or county/region, province, region – from which goods are dispatched.
Nature of Transactions
Select the option that best describes the shipment type of the items imported or exported.
Statistical Procedure
Select the default statistical procedure that represents when the materials cross the border.
Country/Region of Origin
Select the country/region where the goods are manufactured, produced or grown, or in which the goods originate. The specified
value is declared by default for the item unless you specify otherwise in the marketing documents.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/12/26, 12:25 PM
Working with Intrastat Declarations
Context
The Intrastat declaration wizard helps you collect and edit data for creating Intrastat declarations. You can then generate an import
or export declaration file that you submit to the local authorities.
 Caution
If you change the Intrastat settings of your company, business partners, items, or transactions after a declaration run, the
changes are not included automatically in the Intrastat declaration report. To include such changes, run the declaration wizard
again.
 Note
For a new company or an upgraded company without the Intrastat add-on, if you have added some business documents before
you initialize the Intrastat declaration function, the processed transactions can be declared when the following requirements
are met:
The business partner is Intrastat–relevant, has a default ship-to address in an EU country/region, and has a federal tax
ID.
The item is Intrastat–relevant.
For sales documents, the ship-to address on the document is in an EU country/region other than the declaration
country/region.
For an upgraded company with the Intrastat add-on, the system automatically enables the Intrastat declaration function during
upgrade.
With the Intrastat declaration wizard, you can perform the following tasks:
Create Intrastat declarations
View and correct executed declarations
Generate declaration files
Capture country of origin information for the tracking and tracing of goods and cargo
You can create the following types of Intrastat declarations:
New declaration: “Normal” monthly or quarterly Intrastat declaration
Nil declaration: “Empty” Intrastat declaration that you file when you have no EU trade to declare for a particular month or
quarter. Even if it is not mandatory, creating a nil declaration helps you avoid unnecessary queries from authorities.
Correction declaration: Changes to a declaration that you have submitted if you discover that you have understated or
overstated your Intrastat trade. For monthly declaration in some countries/regions, if the variations are within a certain
range, you do not need to create a correction declaration for the particular declaration month, but you should include the
missing transactions in your next declaration.
 Note
Some countries/regions do not allow nil declarations; some countries/regions do not allow correction declarations. For these
countries/regions, the Nil Declaration or Correction Declaration option is not provided as a declaration type.
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/12/26, 12:25 PM
Before creating an import or export declaration file, the Intrastat declaration wizard validates the data in your declaration based on
the following settings:
On the General tab of the Intrastat Configuration window, if you have selected the Require All Data checkbox, the wizard
validates all Intrastat fields for which the Required For checkbox is selected for import or export.
On the Intrastat Fields tab of the Intrastat Configuration window, if you have selected the Validation For checkbox for
import or export for a field, the wizard validates the field for import or export.
The Intrastat declaration wizard saves the declaration with one of the following statuses:
O (Open): You have saved the declaration run but have not created a declaration file.
C (Closed): You have executed the declaration run and generated a declaration file.
A (Add-on Run): The declaration run was saved in SAP Business One 8.82 or lower before the company was upgraded to
9.0.
 Note
The declaration runs with the status Archived serve only as a reference. You cannot reopen, overwrite, or correct any of
them. In addition, the link arrows in step 6 (Transactions) of these declaration runs do not work.
Creating a New Declaration
Prerequisites
You have configured the Intrastat settings for your company in the Intrastat Configuration window.
You have configured the Intrastat settings for your business partners and items.
You have imported an appropriate EFM format for creating the declaration file to the Electronic File Manager window.
For more information, see Configuring Intrastat Settings.
Procedure
1. To start the Intrastat declaration wizard, from the SAP Business One Main Menu, choose Financials Financial Reports
Intrastat Intrastat Declaration Wizard or Reports Financials Intrastat Intrastat Declaration Wizard .
2. In step 1 of the wizard (Wizard Options), select the Create New Declaration radio button and choose the Next pushbutton.
3. In step 2 (General Information)), select the declaration type New Declaration, specify the other information, and choose
the Next pushbutton.
4. If applicable, specify the additional information required by the declaration country/region in step 3 (Country/Region-
Specific Fields – <Declaration Country/Region>)and choose the Next pushbutton. If the declaration country/region does
not require any additional information, the wizard goes directly to step 4.
5. In step 4 (Business Partners), edit the Intrastat data of relevant business partners as follows:
a. Update the fields as necessary.
b. To save the changes to the business partner Intrastat settings, choose the Save BP Settings pushbutton.
c. Choose the Next pushbutton.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/12/26, 12:25 PM
To ensure that all relevant business partners are displayed, the business partners must meet the following requirements:
On the General tab of the Business Partner Master Data window, you have selected the Intrastat Relevant
checkbox.
The business partner has a default ship-to address in a country/region other than the declaration country/region.
The business partner has a federal tax ID.
6. In step 5 (Items), edit the Intrastat data of relevant items as follows:
a. Update the fields as necessary.
b. To save the changes to the item Intrastat settings, choose the Save Item Settings pushbutton.
c. Choose the Next pushbutton.
To ensure that all relevant items are displayed, on the General tab of the Item Master Data window, select the Intrastat
Relevant checkbox.
7. In step 6 (Transactions), select transactions to declare and edit the Intrastat data of the transactions as follows:
a. Update the fields as necessary.
b. Choose the Next pushbutton.
For more information, see Data Collection Rules: Calculations.
8. In step 7 (Declaration Generation), generate your declaration file by proceeding as follows:
a. Select the Generate Declaration File radio button.
b. Select an electronic file format for the declaration file.
c. Specify the declaration file name and choose the button to specify its storage path.
d. Choose the Next pushbutton.
 Note
To save the Intrastat declaration instead of generating the declaration file immediately, select the Save Declaration Run
radio button and then choose the Finish pushbutton to exit the wizard. The status of the saved declaration is Open.
The wizard saves the executed declaration run and sets its status as Closed . For correcting executed declarations, see Correcting
an Executed Declaration.
Related Information
Intrastat Declaration Wizard: Step 1 - Starting or Loading a Declaration
Intrastat Declaration Wizard: Step 2 - Specifying Data Required for All Countries/Regions
Intrastat Declaration Wizard: Step 3 - Specifying Country/Region-Specific Fields
Intrastat Declaration Wizard: Step 4 - Updating Business Partner Intrastat Data
Intrastat Declaration Wizard: Step 5 - Updating Item Intrastat Data
Intrastat Declaration Wizard: Step 6 - Editing Transactional Data
Intrastat Declaration Wizard: Step 7 - Generating the Declaration File
Correcting an Executed Declaration
If you have executed an Intrastat declaration and created a declaration file, the status of the declaration is set to Closed.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/12/26, 12:25 PM
You can correct an executed declaration in one of the following ways:
For countries/regions that allow correction declarations, create a correction declaration to correct the executed
declaration.
 Note
You can create a correction declaration based only on a new declaration, but not on a nil declaration.
For countries/regions that do not allow correction declarations, reopen the executed declaration to make necessary
changes or create another declaration to overwrite the reopened declaration.
For countries/regions that allow correction declarations, you can correct a correction declaration by doing either of the following:
Reopen the correction declaration to make necessary changes.
Create a new correction declaration.
Countries/regions that allow correction declarations are listed below:
BE – Belgium
CZ – Czech Republic
ES – Spain
IT – Italy
NL – Netherlands
If you correct an executed declaration by reopening it and creating another declaration to overwrite it, you need to fill in the same
“set of fields” so that the system recognizes that you are correcting an existing declaration. Depending on your declaration
country/region, the “set of fields” differs as listed in the “Set of Fields” table below.
If you correct an executed declaration by creating a correction declaration, you also need to fill in the same “set of fields” except for
the Declaration Type field.
Set of Fields
Country/Region Austria, France, United Italy Portugal, Sweden Finland and Others
Kingdom, Ireland, Spain
Set of Fields Declaration Type Declaration Type Declaration Type Declaration Type
Flow of Goods Flow of Goods Flow of Goods Flow of Goods
Reporting Period Reporting Period Reporting Period Reporting Period
Declaration Declaration Declaration Declaration
Country/Region Country/Region Country/Region Country/Region
VAT Reg. No. of Trader VAT Reg. No. of Trader VAT Reg. No. of Trader VAT Reg. No. of Trader
VAT Reg. No. Extension VAT Reg. No. Extension VAT Reg. No. Extension VAT Reg. No. Extension
Declaration Number Declaration Number in Declaration Number
Period
Declaration Number in
Period
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/12/26, 12:25 PM
Procedure
Creating a Correction Declaration to Correct an Executed Declaration
 Note
For Italy, the correction declaration information is appended to the original declaration file. You must select the correct
declaration file to overwrite it.
For other countries/regions, you must generate a new correction file to replace the declaration file you want to correct.
1. To start the Intrastat declaration wizard, choose Financials Financial Reports Intrastat Intrastat Declaration Wizard
or Reports Financials Intrastat Intrastat Declaration Wizard .
2. In step 1 of the wizard (Wizard Options), select the Create New Declaration radio button and choose the Next pushbutton.
3. In step 2 (General Information), proceed as follows:
a. Select the declaration type Correction Declaration.
b. Specify the “set of fields” specific to your declaration country/region.
c. Specify the other information.
d. Choose the Next pushbutton.
4. Proceed with steps 3, 4, 5, 6, as if you were creating a new declaration.
5. In step 7 (Declaration Generation), save the declaration run or generate a declaration file.
Reopening an Executed Declaration for Correction
1. To start the Intrastat declaration wizard, choose Financials Financial Reports Intrastat Intrastat Declaration Wizard
or Reports Financials Intrastat Intrastat Declaration Wizard .
2. Select the Load Saved Declaration radio button, select the executed declaration you want to correct, and choose the Next
pushbutton.
3. Keep choosing the Next pushbutton until step 6 (Transactions) and then choose the Reopen pushbutton. Steps 4 and 5 are
skipped.
The declaration is reopened.
4. Make any necessary changes, and then choose the Next pushbutton in step 6.
5. In step 7 (Declaration Generation), save the declaration run or generate a declaration file.
Related Information
Intrastat Declaration Wizard: Step 1 - Starting or Loading a Declaration
Intrastat Declaration Wizard: Step 2 - Specifying Data Required for All Countries/Regions
Intrastat Declaration Wizard: Step 3 - Specifying Country/Region-Specific Fields
Intrastat Declaration Wizard: Step 4 - Updating Business Partner Intrastat Data
Intrastat Declaration Wizard: Step 5 - Updating Item Intrastat Data
Intrastat Declaration Wizard: Step 6 - Editing Transactional Data
Intrastat Declaration Wizard: Step 7 - Generating the Declaration File
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/12/26, 12:25 PM
Generating a File for a Saved Declaration
Prerequisites
You have appropriate GEP electronic file formats stored in the Electronic File Manager window.
Context
You can generate an Intrastat file for a saved declaration, whether executed or not.
Procedure
1. To start the Intrastat wizard, from the SAP Business One Main Menu, choose Financials Financial Reports Intrastat
Intrastat Declaration Wizard or Reports Financials Intrastat Intrastat Declaration Wizard .
2. In step 1 of the wizard, select the Load Saved Declarations radio button, select the declaration for which you want to
generate a file, and do either of the following:
Keep choosing the Next pushbutton till step 7. Note that, for saved but not executed declarations, you can change
the transaction details.
Choose the Finish pushbutton to go directly to step 7.
3. In step 7, generate your declaration file by proceeding as follows:
a. Select the Generate Declaration File radio button.
b. Select an electronic file format for the declaration file.
c. Specify the declaration file name and choose the button to specify its storage path.
d. Choose the Next or Finish pushbutton.
For more information, see Intrastat Declaration Wizard: Step 7 # Generating the Declaratio.
Using the Intrastat Declaration Wizard
The Intrastat declaration wizard helps you generate Intrastat declarations. You can do the following:
Collect and edit trade data
Create Intrastat declarations
Correct Intrastat declarations
Generate declaration files
To start the Intrastat declaration wizard, from the SAP Business One Main Menu, choose Financials Financial Reports
Intrastat Intrastat Declaration Wizard or Reports Financials Intrastat Intrastat Declaration Wizard .
Related Information
Intrastat Declaration Wizard: Step 1 - Starting or Loading a Declaration
Intrastat Declaration Wizard: Step 2 - Specifying Data Required for All Countries/Regions
Intrastat Declaration Wizard: Step 3 - Specifying Country/Region-Specific Fields
Intrastat Declaration Wizard: Step 4 - Updating Business Partner Intrastat Data
Intrastat Declaration Wizard: Step 5 - Updating Item Intrastat Data
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/12/26, 12:25 PM
Intrastat Declaration Wizard: Step 6 - Editing Transactional Data
Intrastat Declaration Wizard: Step 7 - Generating the Declaration File
Intrastat Declaration Wizard: Step 8 - Reviewing the File Generation Result
Intrastat Declaration Wizard: Step 1 - Starting or Loading a
Declaration
In the Wizard Options window, you start a new declaration or load a saved one.
For the saved declarations, you can do either of the following:
If the declaration is closed, you can view the declaration or generate a declaration file.
If the declaration is still open, you can change the declaration details and execute the declaration to generate a declaration
file.
Create New Declaration
Creates a new Intrastat declaration.
In the next step, you select one of the following declaration types:
New declaration if you have EU trade to declare for a particular period
Nil declaration if you have no EU trade to declare for a particular period. Nil declarations are available only for a few
countries/regions. For more information, see Creating a Nil Declaration.
Correction declaration if you understated or overstated your trade for a particular period and you need to make a new
declaration to correct the mistake. If your declaration country/region does not allow correction declarations, you need to
reopen the erroneous declaration and correct it. For more information, see Correcting an Executed Declaration.
Load Saved Declarations
Select this radio button to display previously saved declarations, including executed declarations. You can do the following things:
Filter the declarations
Select a declaration to view its details
Select a declaration to reopen it for correction. For more information, see Correcting an Executed Declaration.
Select a declaration to generate a declaration file
Load Saved Declarations Fields
Status
Status of a saved declaration:
Open: You have saved the declaration run but have not created a declaration file.
Closed : You have executed the declaration run and generated a declaration file.
Archived : The declaration run was saved in SAP Business One 8.82 or lower before the company was upgraded to 9.0.
 Note
The declaration runs with the status Archived serve only as a reference. You cannot reopen, overwrite, or correct them.
In addition, the link arrows in step 6 (Transactions) of these declaration runs do not work.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/12/26, 12:25 PM
The status of a declaration may change in the following situations:
The initial value of Open is set to Closed after you choose to execute the declaration and create a declaration file in step 7
of the wizard.
A closed declaration is set to Open if you reopen it in step 6 of the wizard.
No.
Sequential number that the system assigns automatically to each saved declaration.
Execution Date
Date when the declaration is executed or saved.
Declaration Type
Includes the following types:
New Declaration: Includes EU trade data for a particular period
Nil Declaration: Includes no EU trade data for a particular period; created and submitted so that the authorities do not pose
unnecessary queries
Correction Declaration: Created if you understated or overstated in a declaration file and need to make a new declaration
 Note
Nil or correction declarations are available only for a few countries/regions. For more information, see Creating a Nil Declaration
and Correcting an Executed Declaration.
Flow of Goods
Direction of the merchandise: I for import and E for export.
Declaration Country/Region Code
Code of the country/region in which you conduct transactions and which requires you to submit Intrastat declarations.
Period From
Starting day of the declaration period.
Period To
Ending day of the declaration period.
VAT Reg. No. of Trader
VAT registration number of the trader.
VAT Reg. No. Extension
VAT registration number extension.
Decl. Sequential No.
Specific to Finland. A separate declaration number assigned to each company by the local authorities.
No. of Declarations in Period
Indicates how many times you execute declarations during the declaration period.
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/12/26, 12:25 PM
Total Value
Total trade value of the Intrastat declaration.
No. of Declared Docs
Total number of documents included in the declaration.
Description
Description of the Intrastat declaration.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 2 - Specifying Data Required
for All Countries/Regions
In the General Information window, you specify data for the common fields that are required for all EU countries/regions.
Left-Side Fields
Declaration Type
Select one of the following declaration types according to your needs:
New Declaration
Nil Declaration
Correction Declaration
 Note
Nil or correction declarations are available only for a few countries/regions. For more information, see Creating a Nil Declaration
and Correcting an Executed Declaration.
Flow of Goods
Select either Import or Export depending upon whether you want to report import or export of goods.
Reporting Period From ... To ...
Specify the start and end dates covered by the declaration. Note that the start date must be the first day of each period and the
end date must be the last day of the period.
The values of these two fields are dependent on the Declaration Period field.
Description
Describe the Intrastat declaration (maximum length of 200 characters).
Declaration Country/Region
Select the appropriate country/region for your declaration.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/12/26, 12:25 PM
SAP Business One supports the ISO country/region code “EL” for Greece instead of “GR”. When generating output files for your
Intrastat declarations, the system converts the country/region code from “EL” to “GR”.
Declaration Period
Specify whether you are making a monthly or quarterly declaration.
To declare quarterly, select Quarterly and specify the declaration period in the Reporting Period From ... To ... fields as follows:
The first quarter is from January to March.
The second quarter is from April to June.
The third quarter is from July to September.
The fourth quarter is from October to December.
Declare Credit Memos and Returns Based on Flow of Goods
Select this checkbox if you want to declare the following documents based on the actual transport direction of the goods:
A/R credit memo
A/P credit memo
Return
Goods return
As a result, the values of the documents are presented in the opposite sign.
 Example
If you declare export data and select this checkbox, all relevant A/P credit memos and goods returns are collected. If the values
are positive in these documents, they are presented as positive values in the declaration. On the contrary, if you do not select
this checkbox, you declare A/R credit memos and returns with the negative sign.
Include Documents Not Declared in Previous Period
Available for monthly declarations only.
Select if you want the wizard to include the documents that you did not declare in the previous month. You either created these
documents after you had filed your declaration or erroneously excluded them from your declaration.
 Example
It is October currently.
Your declaration month is October. After you select this checkbox, all the documents that you missed declaring in
September are included.
Your declaration month is September. After you select this checkbox, all the documents that you missed declaring in
August are included.
You declaration month is November. After you select this checkbox, all the documents that you missed declaring in
October are included.
If you understated or overstated your trade volume in your October declaration, you can pre-run a November declaration
and select this checkbox to see whether the variation is within the acceptable range. If not, you need to create a
correction declaration or reopen the October declaration to correct it.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/12/26, 12:25 PM
Include All Goods Receipt POs or All Deliveries from the Previous Reporting Period
Select this checkbox if you want the wizard to include the Goods Receipt POs and the Deliverables from the previous reporting
period. This checkbox is selected by default.
Right-Side Fields
Contact Person
Specify the contact person at your company.
Default: First name and last name from the employee master data of the currently logged-on user
Phone
Specify the phone number of the contact person.
Default: Office Phone field from the employee master data of the currently logged-on user
Fax
Specify the fax number of the contact person.
Default: Fax field from the employee master data of the currently logged-on user
E-Mail
Specify the e-mail address of the contact person.
Default: E-Mail field from the employee master data of the currently logged-on user
Company Name
Specify the name of the declaring company.
Default: Company Name field in the Company Details window
Street
Specify the street where the declaring company is located.
Default: Street / PO Box field in the Company Details window
City
Specify the city where the declaring company is located.
Default: City field in the Company Details window
Zip Code
Specify the zip code of the declaring company.
Default: Zip Code field in the Company Details window
Company Declaration ID
Specify the identifier of the declaring company.
Default: Company Declaration ID field in the Intrastat Configuration window
VAT Reg. No. of Trader
Specify the VAT registration number of the declaring company.
Default: VAT Reg. No. of Trader field in the Intrastat Configuration window
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/12/26, 12:25 PM
VAT Reg. No. Extension
Specify the VAT registration extension number of the declaring company.
Default: VAT Reg. No. Extension field in the Intrastat Configuration window
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 3 - Specifying
Country/Region-Specific Fields
In the Country/Region-Specific Fields – <Declaration Country/Region> window, you specify the data for country/region-specific
fields. This step is relevant only for part of the EU countries/regions; if your declaration country/region does not require any
additional fields, the wizard proceeds from step 2 directly to step 4.
Declaration No. in Period
Required by: Italy, Poland, Portugal, Sweden
Specify a declaration identifier, if you are allowed to file more than one declaration per period.
Box1: Periodicity
Required by: Italy
Do one of the following:
If you specified the first month of a quarter in step 2 of this procedure, select First Month of Quarter.
If you specified the first two months of a quarter in step 2 of this procedure, select First and Second Months of Quarter.
If you specified a different month or a different combination of months for a quarter, select None of the Other Cases.
Box 2: Company Activity
Required by: Italy
Select one of the following:
0: None of the Other Cases
Default value
7: First Declaration
8: Stop Activity / Change of Federal Tax ID
9: First Declaration After Federal Tax ID Change
Customs Office Name
Required by: Finland
Specify the name of the customs office where the declaration is to be filed.
Customs Office ID
Required by: Finland, Portugal
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/12/26, 12:25 PM
Specify the corresponding ID of the customs office where the declaration is to be filed.
Declaration Serial Number
Required by: Finland
Specify a serial number to identify the sequence of your declarations.
Interchange Control Reference
Required by: Finland, Ireland, United Kingdom
Specify a unique interchange reference number.
Tax Code Extension
Required by: France
Specify the tax code extension.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 4 - Updating Business Partner
Intrastat Data
This step collects data about the business partners that have documents you must declare for a specific period. By default, all
values except for Business Partner Federal Tax ID come from the Intrastat settings of the business partner master data.
 Note
This step is available only in new declarations.
In the Business Partners window, you can update the values of certain fields. Among these editable fields, the specified values in
the following fields for each business partner are drawn to step 6 of the wizard as the default values for the transactions with the
business partner:
Nature of Transactions
Statistical Procedure
Customs Procedure
Domestic/Foreign Identifier
Port of Entry or Exit
For the following editable fields, if you have not specified a value in a transaction, the specified value in this step for the business
partner is taken as the default value for the transaction in step 6 of the wizard:
Transport Mode
Incoterms
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/12/26, 12:25 PM
The updated values affect only the Intrastat declaration that you are creating. To save the updated values to the Intrastat
settings of the business partners, choose the Save BP Settings pushbutton.
BP Code
Business partner code. Click to view the business partner master data.
BP Name
Displays the name of the business partner.
Nature of Transactions
Select the major type of transactions you deal in with the business partner.
Statistical Procedure
Select a statistical procedure that represents when the goods that you purchase from or sell to the business partner cross the
border.
Customs Procedure
Select the major customs procedure for the goods delivered to or from the business partner.
Transport Mode
Select a mode indicating how goods are shipped from or to the business partner.
Incoterms
Select the Incoterms for shipping goods from or to the business partner.
Business Partner Federal Tax ID
This value is taken from the Federal Tax ID field in the general area of the business partner master data.
Domestic/Foreign Identifier
Specify an appropriate identifier.
Port of Entry or Exit
Specify the location at which goods enter or exit the country/region.
Save BP Settings
Choose to save the changes into the business partners' Intrastat settings.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 5 - Updating Item Intrastat
Data
This step collects data about the items that are included in the transactions that you must declare for a specific period. By default,
all values come from the Intrastat settings of the item master data.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/12/26, 12:25 PM
This step is only available in new declarations.
In the Items window, you can update the values of all fields except the Item Code and Item Description fields. The Item Type field
in the Italy localization and the Statistical Code field in the Czech Republic localization cannot be updated, as well. The specified
values for each item are drawn to step 6 of the wizard as the default values for the transactions of the item.
 Note
The updated values affect only the Intrastat declaration that you are creating. To save the updated values relating to the
Intrastat settings of the items, choose the Save Item Settings pushbutton.
 Note
In the Italy localization, the following fields are irrelevant if the item is of the Service type:
Commodity Code
Supplementary Unit
Factor of Supplementary Unit
Item Code
Item code. Click to view the item master data.
Item Description
Displays the item description.
Commodity Code
Specify the commodity code of the item.
Supplementary Unit
If applicable, select a supplementary unit for the item.
Factor of Supplementary Unit
Specify the factor to calculate the item mass in supplementary unit. For more information, see Data Collection Rules: Calculations.
Country/Region of Origin
Select the country/region of origin of the item. Country of Origin Assignment only updates document rows for country of origin if
no values are present.
Destination Country/Region for Import
Select the destination country/region for import. The default value comes from the country/region value of the Destination Region
for Import field in the item master data.
Destination Region for Import
Select the destination region for import. The default value comes from the region value of the Destination Region for Import field
in the item master data.
Country/Region of Origin for Export
Select the country/region of origin for export. The default value comes from the country/region value of the Region of Origin for
Export field in the item master data.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/12/26, 12:25 PM
Region of Origin for Export
Select the region of origin for export. The default value comes from the region value of the Region of Origin for Export field in the
item master data.
Save Item Settings
Choose to save the changes into the Intrastat setting of the items.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 6 - Editing Transactional Data
A transaction (document row) is collected for Intrastat declaration if it meets the following requirements:
The business partner is eligible for Intrastat declaration. For more information, see the business partner section of
Configuring Business Partner and Item Intrastat Settings.
The item is eligible for Intrastat declaration. For more information, see the item section of Configuring Business Partner and
Item Intrastat Settings.
The Ship to field on the Logistics tab of the business document meets the following requirements:
The field is not blank.
The address is in an EU country/region different from the declaration country/region and defined as an EU
country/region under Administration Setup Business Partners Countries/Regions .
In the Transactions window, you can carry out the following activities:
For a new declaration or an open saved declaration, you can select/deselect transactions to include/not include them in the
declaration; and you can edit many data, for example, net mass and the transactional value.
You can reopen an executed declaration to edit transactional data.
Some of the default values of the editable fields are drawn from relevant fields according to the following priority table:
Priority Table
Priority Document
1 (Highest) Step 4 (Business Partners) or step 5 (Items) of the declaration wizard
2 Business document
3 Business partner Intrastat setting
4 Item Intrastat setting
General Area Fields
Group Documents By
Select one of the following ways to group transactions (document rows):
Business partner
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/12/26, 12:25 PM
Commodity code
Service code
Only available for Italy.
Expand
Displays all the detail rows of the declaration.
Collapse
Hides all the detail rows of the declaration.
Reopen
Reopens an executed declaration. The declaration status is changed from Closed to Open.
Declaration Fields
BP Code
Business partner code.
Deselect the Include checkbox of a business partner to exclude all the business partner's transactions from the declaration.
Document No.
Combination of the transaction type abbreviation and the number of the document, for example, PU-1. For information about
transaction type abbreviations, see Transaction Type Abbreviations Legend.
Deselect the Include checkbox of a document to exclude all its transactions (document rows) from the declaration.
Include
The Include checkbox is selected for each line by default.
If you deselect the Include checkbox of a transaction, the transaction is excluded from the declaration file.
If you deselect the Include checkbox of a document, all the transactions in the document are excluded from the declaration
file.
If you deselect the Include checkbox of a business partner, all the business partner's transactions (document rows) are
excluded from the declaration file.
If you group the documents by the commodity code or the service code, and deselect the Include checkbox of a commodity
code or a service code, all transactions of the item with the commodity code or the service code are excluded from the
declaration file.
Declaration Row No.
Line number of each transaction in the respective section of the declaration file.
Document Row No.
The row number of the transaction in the business document.
Posting Date
Posting date of the business document.
Business Partner Country/Region
Default value:
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/12/26, 12:25 PM
Purchasing – A/P transactions: From the default ship-to address of the business partner
Sales – A/R transactions: From the ship-to address of the business document
Destination Country/Region for Import
Default value: drawn according to the priority table above.
Destination Region for Import
Default value: drawn according to the priority table above.
Country/Region of Origin for Export
Default value: drawn according to the priority table above.
Region of Origin for Export
Default value: drawn according to the priority table above.
Incoterms
Default value: drawn according to the priority table above.
Nature of Transactions
Default value: drawn according to the priority table above.
Statistical Procedure
Default value: drawn according to the priority table above.
Customs Procedure
Default value: drawn according to the priority table above.
Triangular Deals for France Localization only:
Specific customs procedure codes for triangular deals are available in the Administration Setup Financials
Intrastat Intrastat Configuration Customs Procedures tab:
21 Livraison exoneree
11 Acquisitions intra-communautaires
31 Facturations dans le cadre d’opérations triangulaires
In this field, the customs procedure is filled in automatically according to the following rules:
If the business partner country/region is not equal to the code of the state where payment is made for the A/R
Invoice, the customs procedure with triangular deal type 11 is selected.
If a drop-ship warehouse is used in the A/R Invoice then the customs procedure with triangular deal type 21 is
selected.
If the business partner country/region is not equal to the code of the state where payment is made for the A/P
Invoice, the customs procedure with triangular deal type 31 is selected.
You can change the customs procedure, if needed.
Transport Mode
Default value: drawn according to the priority table above
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/12/26, 12:25 PM
Port of Entry or Exit
Default value: drawn according to the priority table above.
Commodity Code
Default value: drawn according to the priority table above.
Statistical Code
Relevant to the Czech Republic only.
Default value: drawn according to the priority table above.
Service Code
Relevant to Italy only.
Default value: drawn according to the priority table.
Country/Region of Origin
Default value: drawn according to the priority table above.
Tax Code Extension
Relevant to France only.
Default value: drawn from step 3 of the wizard.
Net Mass Sign
Specify whether the value in the Net Mass field is negative or positive. By default, if a transaction is in the same direction as the
declaration, the sign is positive; if a transaction is in the opposite direction of the declaration, for example, a goods return in an
import declaration, the sign is negative.
Net Mass
Value calculated according to the calculation rules of data collection. For more information, see Data Collection Rules: Calculations.
 Note
In this step, the item weight is automatically converted to kilograms when calculating the item's net mass and mass in
supplementary unit. The conversion does not affect the original values of the Weight fields in the relevant business documents
or item master data.
Net Mass Unit
Specify the unit of measurement of the net mass.
Default value: kg
Sign for Mass in Supplementary Unit
Specify whether the value in the Mass in Supplementary Unit field is negative or positive. By default, if a transaction is in the same
direction as the declaration, the sign is positive; if a transaction is in the opposite direction of the declaration, for example, a goods
return in an import declaration, the sign is negative.
Mass in Supplementary Unit
Value calculated according to the calculation rules of data collection. For more information, see Data Collection Rules: Calculations.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/12/26, 12:25 PM
In this step, the item weight is automatically converted to kilograms when calculating the item's net mass and mass in
supplementary unit. The conversion does not affect the original values of the Weight fields in the relevant business documents
or item master data.
Supplementary Unit
Default value: drawn according to the priority table above.
Value Sign
Specify whether the value in the Value field is negative or positive. By default, if a transaction is in the same direction as the
declaration, the sign is positive; if a transaction is in the opposite direction of the declaration, for example, a goods return in an
import declaration, the sign is negative.
Value
Transaction value that is to be declared. For information about its calculation rules, see Data Collection Rules: Calculations.
Value in Foreign Currency
If the transaction is recorded in a foreign currency, the value in foreign currency is drawn from the Total (Doc) field of the business
document row. Otherwise, it is zero.
Foreign Currency
If the transaction is recorded in a foreign currency, the field displays by default the foreign currency; otherwise, it displays the local
currency.
Statistical Value Sign
Specify whether the value in Statistical Value is negative or positive. By default, if a transaction is in the same direction as the
declaration, the sign is positive; if a transaction is in the opposite direction of the declaration, for example, a goods return in an
import declaration, the sign is negative.
Statistical Value
Value calculated according to the calculation rules of data collection. For more information, see Data Collection Rules: Calculations.
Domestic/Foreign Identifier
Specify the appropriate identifier.
Return Identifier
Specify the return identifier.
Referenced Month, Referenced Year, Referenced Document No., Referenced Item No.
Displays the information of the base transactions.
Relevant to the following documents:
A/R credit memo based on A/R invoices
A/P credit memo based on A/P invoices
For non-based A/P Credit Notes, A/R Credit Notes, Goodes Returns, Returns and Correction Invoices, the Referenced Month and
Referenced Year are taken automatically from the referenced document information under marketing document Accounting
tab Referenced Document Document Referenced To Date .
This referenced information can be filled out while generating the credit document. It is meant for cases when the base document
is not documented in SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/12/26, 12:25 PM
Ref. Year of Summary to Correct
Relevant to Italy only. Used in the correction section.
Displays the declaration year of the document's base transactions if the document is used to rectify other documents.
Business Partner Federal Tax ID
If the federal tax ID in the business document is different from that in the business partner master data, which is drawn to step 4 of
the wizard, the default value of the Business Partner Federal Tax ID field is the federal tax ID in the business document.
Manual Change Indicator
If you manually change the value in one of the following fields in this step, the manual change indicator changes from N to Y:
Net Mass Sign
Net Mass
Sign for Mass in Supplementary Unit
Mass in Supplementary Unit
Value Sign
Value
Value in Foreign Currency
Foreign Currency
Statistical Value Sign
Statistical Value
Changed Data Record ID
Specify a record ID for the data change.
Changed By
Default value: the SAP Business One user who makes the data change.
Time Stamp for Change
Specify the date on which the data was changed.
Delete Indicator
Indicates whether this transaction is included or not in the declaration file.
Service Supply Method
Default value: drawn from step 5.
Service Payment Method
Default value: drawn from step 5.
Code of the State Where the Payment is Made
Specify the code of the state where the payment is made.
Default value: drawn from the Pay to/Bill to address of the relevant document.
No. of Declaration to Correct
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/12/26, 12:25 PM
Displays the number of the declaration (executed) that includes the corrected document.
Row No. Inside Section 3 to Correct
Default value: drawn from the original document.
Warehouse Postal Code
Relevant for France only.
The Warehouse Postal Code is used in the Region field in the Intrastat file.
In the case of A/R Invoice (export) or A/P Invoice (import), the zip code of the warehouse used in the invoice lines is taken.
In the case of a drop ship warehouse, the zip code from the default Ship To address of the document's vendor is taken.
If no zip code is filled then the region will be taken from the Intrastat definitions.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 7 - Generating the Declaration
File
In the Declaration Generation window, you can perform the following activities:
Save the declaration run without generating a declaration file
Generate an Intrastat declaration file for the declaration run
Save Declaration Run
If you intend to generate the declaration file later, select this radio button to save the declaration run with the status Open.
Generate Declaration File
Select this radio button to generate a declaration file based on the data collected in the previous steps.
Electronic File Format
The default choice is taken from Electronic File Format on Intrastat Configuration: General Tab. If you change the selected
Electronic File Format in the wizard, then there is an option to update Electronic File Format in Intrastat Configuration: General
Tab with the change. Electronic file formats that are available in the list must be imported to Electronic File Manager. For more
information, see Setting Up Generic and Special-Purpose Electronic File Formats.
Declaration File Name
Choose the button to specify the storage location and name of the declaration file.
More Information
Working with Intrastat Declarations
Intrastat Declaration Wizard: Step 8 - Reviewing the File
Generation Result
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/12/26, 12:25 PM
The Summary and Error Report window displays the following information:
How many documents were processed in the declaration run
How many items were processed in the declaration run
How many transactional rows were excluded from declaration
In addition, a hyperlink to the location where the file is stored is provided. You can click the link to access the file location.
More Information
Working with Intrastat Declarations
Data Collection Rules
When you use the Intrastat declaration wizard to prepare an Intrastat declaration, your data collection process is subject to rules
pertaining to such issues as which business documents are data sources, how to collect specific data, how to calculate certain
statistics, and so on.
 Note
In the Italy localization, you can declare both service and item transactions between European countries. However, you must
create item master data for each service declared and create item documents to record the transactions of the service item. In
other words, a service document is never included in an Intrastat declaration.
More Information
Data Collection Rules: Intrastat Business Documents
Data Collection Rules: Calculations
Data Collection Rules: Declaration Month
Data Collection Rules: Sale BOM Structured Items
Data Collection Rules: Triangular Deal Transactions
Data Collection Rules: Intrastat Business Documents
The following business documents are used in the creation of an Intrastat declaration. The transaction rows in these documents
constitute the data to declare.
Intrastat Business Documents
Sales Document Purchasing Document Others
Delivery Goods receipt PO Inventory transfer
Return Goods return
A/R invoice A/P invoice
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/12/26, 12:25 PM
Sales Document Purchasing Document Others
A/R credit memo A/P credit memo
A/R reserve invoice A/P reserve invoice
A/R correction invoice A/P correction invoice
Correction invoices are available only for four Intrastat–relevant localizations: Czech Republic, Hungary, Poland, and Slovakia.
Declaration of correction invoices follow the rules below:
If a correction invoice increases the trade value of a transaction (an invoice or another correction invoice), the increased
value adds to the value of the declaration with the same transactional direction as the invoice.
If a correction invoice decreases the trade value of a transaction (an invoice or another correction invoice), the correction
invoice is handled like a credit memo.
If a correction invoice is reversed in the same declaration period, neither the correction invoice nor the correction invoice
reversal is declared.
If a correction invoice is reversed in a later declaration period, the correction invoice and the correction invoice reversal are
declared in respective periods.
 Example
An A/R correction invoice contains two item rows
The first row increases the value of its base transaction. As a result, this row is included in the export declaration, though
with only the increased value.
The second row decreases the value of its base transaction. As a result, this row is included in the import declaration if
you declare your trade based on the actual flow of goods.
An inventory transfer is declared under the following conditions:
The “From” and “To” warehouses are located in two different EU countries/regions and each has a federal tax ID.
Either the “From” warehouse or the “To” warehouse is located in the same country/region as the declaration
country/region.
The inventory transfer involves a business partner that is located in the same country/region as the “From” warehouse.
Standalone and Paired Intrastat Documents
Intrastat-relevant documents exist as standalone or paired, as explained below:
A standalone document has no relationship to any other Intrastat document.
All Intrastat documents can be declared as standalone documents.
A paired document is coupled with another Intrastat document. The target document has priority over the base document.
As long as there is no more than one period's difference between the posting dates of the two documents, the target
document is the one you declare.
Paired Intrastat Documents
Base Document Target Document
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/12/26, 12:25 PM
Base Document Target Document
Delivery A/R invoice
Return A/R credit memo
A/R reserve invoice Delivery
Goods receipt PO A/P invoice
Goods return A/P credit memo
A/P reserve invoice Goods receipt PO
 Note
The following pairs of Intrastat documents also have dependency between themselves, but the target document does
not have priority over the base document. Both documents are included in the Intrastat declaration.
Base Document Target Document
Delivery Return
A/R invoice A/R credit memo
A/R invoice A/R correction invoice
Goods receipt PO Goods return
A/P invoice A/P credit memo
A/P invoice A/P correction invoice
 Example
A delivery is copied to an A/R invoice; the A/R invoice is then copied to an A/R credit memo. The A/R invoice has
declaration priority over the delivery while both the A/R invoice and the A/R credit memo are declared.
More Information
Data Collection Rules: Declaration Date
Data Collection Rules: Canceled Documents and Cancellation
Documents
You can cancel all Intrastat business documents except for inventory transfers and correction invoices. Each canceled document is
coupled with a cancellation document. The declaration of canceled documents and cancellation documents follows the rules
described in the table below:
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/12/26, 12:25 PM
Scenario Canceled Document Cancellation
Document
The canceled document and cancellation document are posted in the same declaration Not declared Not declared
period.
The cancellation document is posted in an earlier declaration period than the canceled Not declared Not declared
document.
 Note
This scenario is possible only when you have activated future posting.
The cancellation document is canceled in The canceled document records or Declared in the Declared in the
a later declaration period than the reflects goods movement, for example, respective period respective period
canceled document. deliveries and A/P invoices not based on
goods receipt POs.
The canceled document does not record Declared in the Not declared
or reflect goods movement, for example, respective period
A/P invoices based on goods receipt POs.
More Information
Canceling Sales and Purchasing Documents
Data Collection Rules: Declaration Period
Data Collection Rules: Declaration Period
Consider the following rules when specifying your reporting period:
You must file a declaration every month or quarter, whether a new or nil declaration.
For paired documents, the maximum permitted delay between the base and target documents is one month or quarter. For
more information, see Data Collection Rules: Business Documents
The posting date of a business document determines the reporting period in which the document is declared.
 Note
A transaction that should be declared in June does not appear automatically in the July declaration if you forget to declare it in
June.
Declaration Period for Paired Intrastat Documents
 Note
The following table outlines how the system processes paired documents when target documents are fully based on base
documents. For partly reconciled paired documents, consider their declaration as a combination of fully reconciled paired
documents and standalone documents.
Scenario Declaration Period Example (Monthly)
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/12/26, 12:25 PM
Scenario Declaration Period Example (Monthly)
The base and target documents are posted Declare the target document in its posting Base document = July
in the same month or quarter. month or quarter.
Target document = July
Declaration month = July
The target document is posted in the next Declare the target document in its posting Base document = July
month or quarter of the base document. month or quarter.
Target document = August
Declaration month = August
The posting month of the target document Declare the base document in the next Base document = July
is more than one month or quarter later month or quarter.
Target document = September
than that of the base document.
The target document is not declared.
Declaration month for base document =
August
Declaration month for target document =
None
 Example
Your company makes monthly Intrastat declarations.
1. Create a delivery as follows:
Posting date = Oct. 1, 2012
Quantity = 10
2. Create an A/R invoice based on the delivery, as follows:
Posting date = Nov. 1, 2012
Quantity = 5
3. Create export Intrastat declarations for October and November. The results are as below:
October: Neither the delivery nor the A/R invoice is declared.
November: The A/R invoice is declared, and the uninvoiced part of the delivery is also declared.
For more information, see Data Collection Rules: Calculations.
Declaration Period for Standalone Intrastat Documents
Intrastat Document Declaration Period Example (Monthly)
Delivery and goods receipt PO One month or quarter later than the Posting month = July
delivery of goods
Declaration month = August
A/R invoice and A/P invoice The invoice month or quarter Posting month = July
Declaration month = July
Return and goods return One month or quarter later than the return Posting month = July
of goods
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/12/26, 12:25 PM
Intrastat Document Declaration Period Example (Monthly)
Declaration month = August
A/R credit memo and A/P credit memo The credit memo month or quarter Posting month = July
Declaration month = July
A/R reserve invoice and A/P reserve invoice One month or quarter later than the invoice Posting month = July
month
Declaration month = August
Inventory transfer The month or quarter when the goods Posting month = July
movement occurs
Declaration month = July
Data Collection Rules: Calculations
Rules are used to calculate net mass, mass in supplementary unit, statistical values, and the total value of collected transactions.
Net Mass
Net mass is drawn from the Weight field of the document row. If the Weight field is blank, but you have defined the sales weight
and the purchase weight for the item later, net mass is calculated as shown in the table below:
Transactional Type Net Mass
Sales – A/R Net Mass = Sales Weight * Quantity
Purchasing – A/P Net Mass = Purchase Weight * Quantity
 Note
The sales weight and the purchase weight are drawn from the item master data. Rounding applies only to net mass, not to the
sales weight or purchase weight of single items.
Mass in Supplementary Unit
Mass in supplementary unit is calculated for items to which you have assigned a supplementary unit.
 Note
If you want an item's mass in supplementary unit calculated, you must define a factor of supplementary unit in the item's
Intrastat settings.
The weight value used in the calculation comes by default from the Weight field in the document. If the Weight field is blank, the
weight value comes from the sales weight or the purchase weight in the item master data. Your setting of the Use Weight in
Calculation of Mass in Supplementary Unit checkbox on the Intrastat Settings tab of the item master data also has an impact on
the calculation.
The mass in supplementary unit is calculated in one of the following ways:
If you use weight in the calculation, Mass in Supplementary Unit = Quantity × Factor of Supplementary Unit × Weight
If you do not use weight in the calculation, Mass in Supplementary Unit = Quantity × Factor of Supplementary Unit
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/12/26, 12:25 PM
 Example
Calculation Examples of Mass in Supplementary Unit
Supplementary Quantity Factor Weight (kg) Use Weight in Formula/Result
Unit Calculation
Ton 5 0.001 10 Yes Mass = 5 × 0.001 ×
10 = 0.05
No Mass = 5 × 0.001 =
0.005
0 Yes Mass = 5 × 0.001 ×
0 = 0
No Mass = 5 × 0.001 =
0.005
Statistical Value
The statistical value of each transaction row depends on your setting of the Simplified Procedure checkbox on the General tab of
the Intrastat Configuration window.
Calculation Rule for Statistical Values
Simplified Procedure checkbox Calculation Rule
Not selected Statistical Value = Row Total × Percentage Statistical Value of the
Incoterms
Not selected and the document row is not assigned an Incoterms Statistical Value = Row Total
Selected
Transaction Value and Total Declaration Value
The value of each declared transaction row is collected according to the following rules:
By default, it is drawn from the Total (LC) field of each row, or the Total (Doc) field if the transaction is recorded in a foreign
currency.
If you have defined a discount for the document, the transaction value is the discounted row total.
If a delivery or goods receipt PO is fully invoiced, the invoiced value is declared.
If a partly invoiced delivery or goods receipt PO is included in a declaration, only its uninvoiced value is declared
The total declaration value is the sum of all collected transaction values. Depending on its value sign, a transaction value is
deducted from or added to the total value.
Data Collection Rules: Sales BOM Structured Items
If an item is used as a sales bill of material (BOM), declaration of the item is determined by the setting of the For a Sales BOM in
Documents, Display: field on the General tab of the Document Settings window.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/12/26, 12:25 PM
Collection Rules
For a Sales BOM in Documents, Parent Item Component Item Intrastat Declaration
Display:
Price and Total for Parent Item Displayed Displayed The transaction rows of the
| Only |     |     |     |     | parent item and the component |
| ---- | --- | --- | --- | --- | ----------------------------- |
items are all declared in an
export report.
Price for Component Items Not displayed Displayed Only the transaction rows of the
component items are declared
in an export report.
  Note
If you have selected the Price for Component Items radio button, you must define the component items as Intrastat-relevant to
display them in the Intrastat declaration wizard.
Example
This example illustrates how a sales BOM “P001” is declared depending on your setting of the For a Sales BOM in Documents,
Display: checkbox:
| Item No. | Parent Item / Component Item |     | Quantity |     | Unit Price |
| -------- | ---------------------------- | --- | -------- | --- | ---------- |
| P001     | Parent Item                  |     | 1        |     | EUR 50     |
| I002     | Component Item               |     | 1        |     | EUR 10     |
| I003     | Component Item               |     | 2        |     | EUR 15     |
1. In the Document Settings window, select Price and Total for Parent Item Only.
2. Create an A/R invoice with the following data:
| Row Number | Item No. | Quantity | Unit Price | Total (LC) |     |
| ---------- | -------- | -------- | ---------- | ---------- | --- |
| 1          | P001     | 1        | EUR 50     | EUR 50     |     |
| 2          | I002     | /        | /          | /          |     |
| 3          | I003     | /        | /          | /          |     |
3. Run the Intrastat declaration wizard, and rows 1 to 3 in the A/R invoice are all declared, with values presented in line with
the parent item only.
4. In the Document Settings window, select Price for Component Items.
5. Run the Intrastat declaration wizard again, and only rows 2 to 3 in the A/R invoice are declared.
Data Collection Rules: Triangular Deal Transactions
A triangular deal transaction involves two companies. For example, company X, which is located in country/region A, sells some
goods to its business partner, company Y, which is located in country/region B. However, the goods are shipped to country/region B
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/12/26, 12:25 PM
from company X's warehouse in country/region C.
 Note
You must set up tax codes for triangular deal transactions and assign the correct tax code to business documents. Otherwise,
irrelevant triangular deal transactions appear in your declarations.
To set up tax codes for triangular deal transactions, proceed as follows:
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Groups .
2. In the Triangular Deal field for the tax code, select a non empty value.
Declaration rules for triangular deal transactions
For a triangular deal transaction to be included in an Intrastat declaration, the following requirements must be met:
You have specified a triangular deal tax code for the transaction.
The declaration country/region is the same as the warehouse country/region in the business document.
For import: The warehouse and the default ship-to address of the business partner are in different countries/regions.
For export: The warehouse and the ship-to address in the business document are in different countries/regions.
If the warehouse in the business document is located in a different country/region from the declaration country/region, a
triangular deal transaction (identified by a triangular deal tax code) is not declared properly.
Declaration rules for paired business documents relevant to triangular deal transactions
The tax code of the target document determines the declaration when one of the following occurs:
The posting dates of the base document and the target document are within the same month.
The posting date of the target document is one month later than the posting date of the base document.
The tax code of the base document determines the declaration when the posting date of the target document is more than one
month later than the posting date of the base document. The triangular deal is declared only when the determining tax code is not
empty.
More Information
Data Collection Rules: Intrastat Business Documents
Creating a Nil Declaration
You create a nil declaration when you have no EU trade to declare for the particular month or quarter.
Countries/Regions that allow nil declarations are listed below:
AT – Austria
BE – Belgium
CZ – Czech Republic
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/12/26, 12:25 PM
DK – Denmark
ES – Spain
GB – United Kingdom
HU – Hungary
NL – Netherlands
PL – Poland
SK – Slovakia
Procedure
1. To start the Intrastat declaration wizard, from the SAP Business One Main Menu, choose Financials Financial Reports
Intrastat Intrastat Declaration Wizard or Reports Financials Intrastat Intrastat Declaration Wizard .
2. In step 1 of the wizard (Wizard Options), select the Create New Declaration radio button and choose the Next pushbutton.
3. In step 2 (General Information), select the declaration type Nil Declaration, specify the other information, and choose the
Next pushbutton.
4. If applicable, specify the additional information required by the declaration country/region in step 3 (Country/Region-
Specific Fields – <Declaration Country/Region>) and choose the Next pushbutton. If the declaration country/region does
not require any additional information, the wizard goes directly to step 7 (Declaration Generation).
5. To generate your declaration file, proceed as follows:
a. Select the Generate Declaration File radio button.
b. Select an electronic file format for the declaration file.
c. Specify the declaration file name and choose the button to specify its storage path.
d. Choose the Next or Finishpushbutton.
The wizard saves the executed declaration run and sets its status as Closed. For information about correcting executed
declarations, see Correcting an Executed Declaration.
Related Information
Intrastat Declaration Wizard: Step 1 - Starting or Loading a Declaration
Intrastat Declaration Wizard: Step 2 - Specifying Data Required for All Countries/Regions
Intrastat Declaration Wizard: Step 3 - Specifying Country/Region-Specific Fields
Intrastat Declaration Wizard: Step 7 - Generating the Declaration File
Transfer Posting Correction Wizard
The Transfer Posting Correction Wizard enables you to post corrections resulting from VAT changes, for amounts transferred from
revenue or expense accounts to new accounts.
This wizard guides you in defining parameters required to generate these postings.
To access the wizard, from the SAP Business One Main Menu, choose Administration Utilities Transfer Posting Correction
Wizard .
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/12/26, 12:25 PM
 Note
Ensure that you execute the wizard only once for the selected period and the selected accounts.
 Note
All documents that you post after executing the wizard and that are valid for this period, must be transferred manually. To
transfer the posting manually, create a journal entry.
More Information
Transfer Posting Correction Wizard - Selection Criteria
Transfer Posting Correction Wizard - Transaction Selection
Transfer Posting Correction Wizard - Transaction Confirmation
Transfer Posting Correction Wizard - Summary
Transfer Posting Correction Wizard - Selection Criteria Window
Use this window to specify the selection criteria for the wizard run.
Selection Criteria Fields
Date From... To...
Specify the date range for the wizard run. By default, the transactions within the posting date range are selected.
 Caution
There should be no overlap of the date ranges specified in different wizard runs; otherwise, you could correct the same posting
twice.
Doc. Date
Selects documents within the document date range.
 Caution
Always use the selected option during the rest of the period; otherwise, you could correct the same posting twice.
Tax Rate
Specify the tax rate of the transaction – 16% or 19% – that the wizard uses to select documents.
Code
Tax group code
Name
Tax group name
Display
Deselect the tax group that you do not need in the wizard run.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/12/26, 12:25 PM
 Note
Only those tax groups with the tax rate of 16% or 19% are valid for the wizard.
G/L Accounts
Limits the selection to specific G/L accounts only. Click to open the Accounts - Selection Criteria window where you can
select the needed G/L accounts.
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard: Transaction Selection
Window
Use this window to select the transactions that you want to include in the wizard run.
 Recommendation
After selecting the needed transactions, you should print the screen or export it to Excel; you may use it for future verification.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Selection Fields
App
Select the posting that you want to correct
G/L Account
The revenue or expense account relevant to a transaction
Tax Code
The tax group code associated with a transaction
Tax %
The tax rate that was effective for the tax code at the time the transaction was posted
Doc. No.
The document number in SAP Business One
Debit, Credit (FC, SC)
The debit or credit tax amount (in terms of foreign currency or system currency)
More Information
Transfer Posting Correction Wizard
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/12/26, 12:25 PM
Transfer Posting Correction Wizard: Transac. Confirmation
Window
Use this window to confirm the amount, accounts, and tax codes for which correction posting will be created.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Confirmation Fields
Interim Account
Specify the clearing account to be used during the correction posting process.
Expense Account
Specify the account to which the expense is posted.
Revenue Account
Specify the account to which the revenue is posted.
Input Tax Group
Specify the input tax group to be used in the correction posting.
Non-Deductible Tax Group
Specify the non-deductible tax group to be used in the correction posting.
Output Tax Group
Specify the output tax group to be used in the correction posting.
Deferred Tax Group (Input)
Specify the tax code which belongs to the input tax group and has a deferred tax account defined in the Tax Groups – Setup
window.
Deferred Tax Group (Output)
Specify the tax code which belongs to the output tax group and has a deferred tax account defined in the List of Tax Definitions
window.
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard - Summary Window
In this window, you can see how many journal entries have been made during the correction process. The number appearing is
twice the number of the corrected transactions because it includes the entries on both the debit and credit sides.
You can view the transactions created by the wizard in the Journal Entry window of the Financials module.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/12/26, 12:25 PM
Transfer Posting Correction Wizard
Tax Reports: UK International and Republic of Ireland
Following is information about tax reports required in the localization for UK International and Republic of Ireland and additional
information related to tax handling in SAP Business One:
Tax Report Generation
Tax Report
EU Sales Report
Withholding Tax Report
Tax Reconciliation Report
Tax Declaration Box Report
To generate the reports choose: Financials Financial Reports Accounting Tax , or Reports Financial Accounting
Tax
Generating EU Sales Report
Follow the steps below to generate the EU sales report as electronic report.
Prerequisites
You have imported the electronic format for the EU Sales Report using the electronic format manager.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Electronic Reports EU Sales Report
. Alternatively, choose it from the Reports module.
The EU Sales Report window appears. In each step, you can choose an appropriate button, as follows:
Next: proceed to the next step
Back: return to the previous step
Cancel: quit the process
Preview: preview a report based on the parameters that you have specified
2. In Step 1 of 4, specify the general parameters as follows, and choose Next.
Date
Generates the report according to either the posting date range or the document date range that you specify.
Year
Specify the fiscal year for which to generate the report
Month/Quarter
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/12/26, 12:25 PM
Specify the month or quarter for which to generate the report.
Code
The codes of the EU tax groups, as defined in Administration Setup Financials Tax Tax Groups .
 Note
To be included in the EU Sales Report window, all documents with EU tax codes must have a Federal Tax ID specified.
3. In Step 2 of 4, specify the contact information of the person in the company who submits the EU sales report, and choose
Next.
4. In Step 3 of 4, specify the destination file path for the generated EU sales report, and choose Next.
5. In Step 4 of 4, do the following:
To view the system log, choose the View Log button.
To open the generated EU sales report, click the hyperlink.
To close the wizard, choose the Finish button.
 Note
The EU Sales Report is generated in the ELMA5 file format. For more information, see SAP Note 1806782 .
EU Sales Report - General Parameters
In this step (Step 1 of 4), you specify the general parameters for generating the EU sales report.
Date
Generates the report according to either the posting date range or the document date range that you specify.
Year
Specify the fiscal year for which to generate the report
Month/Quarter
Specify the month or quarter for which to generate the report.
Code
The codes of the EU tax groups, as defined in Administration Setup Financials Tax Tax Groups .
 Note
To be included in the EU Sales Report window, all documents with EU tax codes must have a Federal Tax ID specified.
Include Service Documents
Select this checkbox to include sales documents of type Service in the report.
More Information
Generating EU Sales Report
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/12/26, 12:25 PM
Generating Extended Tax Reports
Prerequisites
You have activated extended tax reporting.
 Note
You can deactivate extended tax reporting at any time. If you reactivate extended tax reporting afterwards, previously saved
reports will still be in the system.
To activate extended tax reporting, follow the steps below:
Choose Administration System Initialization Company Details , and on the Accounting Data tab, select the Extended Tax
Reporting checkbox.
Context
You can generate and save extended tax reports to be submitted to the tax authorities. Extended tax reporting enables you to mark
reported transactions and thus prevent duplicate transaction reporting.
 Recommendation
We recommend that, before starting to use extended tax reporting, you save a mock report with previously reported
transactions from earlier periods. This prevents irrelevant documents being offered by SAP Business One for reporting.
Extended tax reporting lets you do the following:
Track which items were claimed from or paid to the tax authorities in specified periods
Claim from, or pay to, tax authorities any items missing from the original report for the specified period and added later
Post tax liabilities and receivables to G/L accounts
Depending on your company setup, you can generate up to three different types of reports:
Original - a new tax report
Adjusted - an existing report updated with missing items
Replacement - an existing report updated with changes
 Note
Extended tax reporting does not affect the following reports:
Withholding tax report – the report relates to income tax (not VAT).
EU sales report – the report relates to EU statistical purposes (relevant for sales total amounts).
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting Tax Tax Report
Generation . Alternatively, choose it from the Reports module.
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/12/26, 12:25 PM
2. In the Tax Report Generation - Selection Criteria window, specify parameters for generating a tax report for a given period,
and choose the OK button.
3. In the Tax Report - Generation window, specify parameters for generating a tax report for given tax codes and tax groups,
and choose the Add button.
  Note
To see any errors in tax calculation, choose the Error Report button.
4. Choose  Financials    Financial Reports    Accounting    Tax    Tax Report . Alternatively, choose it from the Reports
module.
5. In the Tax Report - Selection Criteria window, specify parameters for generating a tax report for the given period and tax
codes, and choose the OK button.
Results
The tax report is displayed according to your selection criteria in the Tax Report window.
Example
In January 2009, you entered the following transactions into SAP Business One:
Document Posting Date Net Amount Tax Amount Tax Group/Tax Account
| IN1   | 5/1/2009 | 100 | 10  | A1/111 |
| ----- | -------- | --- | --- | ------ |
| IN2   | 6/1/2009 | 150 | 15  | A2/112 |
| PU1   | 6/1/2009 | -50 | -5  | B1/211 |
| Total |          | 200 | 20  |        |
You prepared and submitted a tax report to the tax authorities for January 2009. Since you are obliged to pay 20 to the tax
authorities, you posted the following from the tax account to the liability account:
| Account              | Debit | Credit |     |     |
| -------------------- | ----- | ------ | --- | --- |
| 111                  | 10    |        |     |     |
| 112                  | 15    |        |     |     |
| 333 (tax payable)    |       | 25     |     |     |
| 211                  |       | 5      |     |     |
| 444 (tax receivable) | 5     |        |     |     |
In February 2009, you entered the following transactions:
Document Posting Date Net Amount Tax Amount Tax Group/Tax Account
| IN3 | 5/2/2009  | 1000 | 100 | A1/111 |
| --- | --------- | ---- | --- | ------ |
| IN4 | 10/1/2009 | 500  | 50  | A2/112 |
| PU2 | 1/2/2009  | -900 | -90 | B1/211 |
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/12/26, 12:25 PM
Document Posting Date Net Amount Tax Amount Tax Group/Tax Account
Total 600 60
Although your total liability in February 2009 is 60, IN4 should be submitted in January 2009 (the invoice has been posted in
February 2009 with a January 2009 posting date). You have the following options:
Create a Replacement type report for January 2009 including all items with a January 2009 posting date.
Create an Adjusted type report, containing only items with a January 2009 posting date that were not included in the
January 2009 report
Create a Original type report for February 2009 including all items posted in February 2009, even if they contain posting
dates earlier than February 2009.
Related Information
Tax Report Generation - Selection Criteria Window
Tax Report
Tax Declaration Box Report
Tax Report Generation
Use this function to generate and save the report to be submitted to tax authorities.
Prerequisites
You have enabled the Extended Tax Report function.
Choose Administration System Initialization Company Details , and on the Accounting Data tab, select the Extended Tax
Reporting checkbox.
Tax Report Generation - Selection Criteria Window
Use this window to specify selection criteria for generating tax reports.
To open this window, choose Financials Financial Reports Accounting Tax Tax Report Generation . Alternatively, open
it from the Reports module.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Selection Criteria
Tax Declaration Type
Select one of the following report types to generate:
Original: new tax report
Replacement: existing report updated with changes
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/12/26, 12:25 PM
Adjusted: existing report updated with missing items
Tax Declaration Name
Select the period for a report.
Adjustment
Select the adjusted version of a report.
Tax Settlement Account (Liability)
Select the account to which the paid tax is re-posted from the VAT account.
Tax Settlement Account (Claim)
Select the account to which the claimed tax is re-posted from the VAT account.
Date
Generate the report according to either the posting or the document date type.
Date From...To...
Define a date range for the report.
Combined with your selection in the Tax Declaration Type field, the tax report displays all the documents whose posting date or
document date falls into the selected range:
Original: Displays the documents that are not saved to any period and match the selected date range.
Replacement: Displays the documents that are saved to the period of the tax report that you selected in the Tax
Declaration Name field and the documents that are not saved to any period and match the selected date range.
Adjusted: Displays the documents that are not saved to any period and match the selected date range.
If you do not specify the date range, all the periods are taken as the default date range for the tax report.
Series
Enables you to filter the transactions to be included in the tax report by series. Proceed as follows:
1. Select the radio button.
2. In the Series - Filter window, specify the required series. To open the window, click next to the radio button.
Transaction Type
Enables you to filter the transactions to be included in the tax report by transaction type. Proceed as follows:
1. Select the radio button.
2. In the Document Type window, specify the relevant document types. To open the window, click next to the radio
button.
Tax Report - Generation
Use this window to generate tax reports to submit to local tax authorities.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/12/26, 12:25 PM
This topic includes explanations of some of the fields and other elements in this window.
Tax Report - Generation Window
Confirmed
Select the documents required by the tax authorities and save them with this report.
Already Approved
Shows whether this document has already been saved in previous reports.
 Note
The documents that were saved before you enable the Extended Tax Reporting function are still shown as unchecked in this
column.
Tax Code
Displays the code of a specific tax group.
Click to display the transactions associated with the tax code.
EU
Indicates whether a tax code is relevant to the European Union.
Tax %
Tax rate of a tax code, displayed as a percentage.
Doc. No.
The document number in the system and its type
For example, an A/P invoice with the number 110007 is displayed as PU 110007 in this column.
Base Amount
Total amount of a document before tax
Tax Amount
Amount calculated for a document by Total Tax minus Non-Deductible
Total Tax
All the tax calculated for a document
Non-Deductible
Tax amount that cannot be deducted for a document
Doc. No.
The document number in the system and its type
For example, an A/P invoice with the number 110007 is displayed as PU 110007 in this column.
Vendor Ref. No.
Vendor reference number in a document
Error Report
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/12/26, 12:25 PM
Displays error messages pertaining to the report
More Information
Tax Report Generation — Selection Criteria
Tax Report
Use this report to display documents and manual journal entries that include tax amounts sorted by tax code. Tax reports can be
produced in an electronic format by choosing an electronic reporting option in Output Mode. The report includes the following
documents:
A/R and A/P invoices and credit memos
Inventory transfer documents – The inventory transfer transactions are displayed only in order to report the transactions in
the report because the tax percentage is 0.
Manual journal entries
Incoming payments and payments to vendors that are not based on invoices
Incoming payments and payments to vendors that include cash discounts
 Note
When printing the report, you can print the selection criteria on a separate page.
Use this window to specify selection criteria for the Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report . Alternatively, open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Selection Criteria Name
Criteria by which the report is created. Choose for a list of existing selection criteria, or press CTRL + A and specify new
selection criteria.
Date From...To..
Choose whether to generate the report according to Posting Date or Document Date or VAT Date or System Date, and specify the
date range for the report.
 Example
A/R invoice no. 15 was created with a posting date 25.3.19 and a document date 1.4.19. Generating the report according to
Posting Date and defining the date range as 1.1.19 – 31.3.19, includes A/R invoice no. 15 in the report. However, generating the
report according to Document Date and defining the same date range of 1.1.19 – 31.3.19, excludes A/R invoice no. 15, as the
Document Date assigned to it is not in the range.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/12/26, 12:25 PM
Round Amount
Rounds the total amounts calculated in the report.
Series
Generates the report for documents created according to specific numbering series. After selecting, choose the ... button to open
the Series – Filter window in which you can define the required numbering series.
Transact.
Generates a report for specific document types.
After selecting, choose the ... button to open the Document Type window in which you can define the document types to include in
the report.
Output
This table displays all the tax groups defined as output tax groups ( Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report
- to change the order of the tax groups, highlight a group and click the arrows to position it
Input
This table displays all the tax groups defined as input tax groups (see Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report.
Button Up and Button Down - to change the order of the tax groups, highlight a group and click the arrows to position it.
Display Credit Memos in a Separate Column
The credit memos that were based on invoices from previous periods (previous to the range of dates defined in the Selection
Criteria window) appear in a separate section, at the end of the report.
Hide Tax Codes without Transactions
Excludes from the report those tax codes with no transactions related during the defined period.
Output Mode
Choose the type of report that you want to produce. You can choose an electronic tax report output here.
Only Display Documents with Externally Calculated Sales Tax
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/12/26, 12:25 PM
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Only includes in the report documents with an externally calculated tax amount on at least one row.
 Note
If you select this checkbox, the Externally Calculated Tax field is displayed in the tax report window.
Update/ OK
When you change the preferences in the Tax Report – Selection Criteria window, the OK option changes to the Update mode.
Choose Update to save the report under the name you entered in the Report Name field.
The preferences chosen for the report are saved.
Tax Report - Declaration
The following table describes the fields appearing in the Tax Report - Declaration window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Tax Declaration
option, set the other required parameters in the Tax Report - Selection Criteria window, then choose OK. Alternatively, open it
from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report - Declaration
Tax Code
Displays the code and the tax codes selected for the report.
Choose the icon to display a list of transactions involving that tax code.
EU
Indicates whether the tax code is EU relevant.
Tax %
Displays the tax rate as a percentage, as defined for the tax code.
Doc. No.
Displays the internal number of the document and its type. For example A/P invoice number 110007 is displayed as PU 110007.
Posting Date
Displays the posting date of the documents. If the Tax Date option is selected in the Selection Criteria window, this column
displays the tax date of the documents.
Base Amount
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/12/26, 12:25 PM
Total amount of the document before taxes, summarized for each tax code.
Tax Amount
Tax amount calculated for the tax group: Total Tax field minus Non Deductible field.
Total Tax
Displays the amount of the tax.
Non Deductible
The amount which cannot be deducted.
Account
Displays the control account in which the journal entry of the document is posted.
Vendor Ref. No.
Displays the vendor’s reference number from the document, if defined.
Error Report
Choose to display error messages regarding the displayed report.
More Information
Tax Report
Tax Report - Register Book
The following table describes the fields appear in the Tax Report - Register Book window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Register Book
option and set the other required parameters in the Tax Report - Selection Criteria window, and then choose OK. Alternatively,
open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Register Book
Reg. No.
Displays the successive number of the records, beginning with the value defined in the Selection Criteria window.
Date
Displays either the posting date of the documents, or, if the Tax Date option is selected in the Selection Criteria window, the tax
date.
Doc. No.
Displays the internal number of the document and its type. For example, A/P invoice number 110007 is displayed as PU 110007.
Base Amount
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/12/26, 12:25 PM
Total amount of the document before taxes.
Tax %
The tax rate defined for the tax code, as a percentage.
Tax
Displays the amount of the tax in the document.
Non-Deductible
The amount of the non-deductible tax in the document, calculated according to the tax code definition.
Total Amount (LC)
Displays the total amount of the document in local currency.
More Information
Tax Report
EU Sales Report
This report can list goods and services sold by a company to customers in the European Union, grouped by the country/region and
tax ID of the customers.
This report can also list inventory transfers that occur between foreign European Union countries/regions and your company's
home country/region or other foreign European Union countries/regions. Inventory transfers from warehouses in your company's
home country/region to warehouses in your company's home country/region are not reported.
The report can include transactions that result from the following document types:
A/R Invoice
A/R Invoice + Payment
A/R Reserve Invoice
A/R Down Payment Invoice
Manual journal entries that are specified as relevant for the report
Inventory Transfers
The report does not include A/R Down Payment Requests (even if paid).
 Note
When printing the report, you can print the selection criteria on a separate page.
More Information
EU Sales Report - Selection Criteria
EU Sales Report Window
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/12/26, 12:25 PM
EU Sales Report - Selection Criteria
Use this window to specify selection criteria for the EU Sales report.
To open the window, choose Financials Financial Reports Accounting Tax EU Sales Report . Alternatively, open it from
the Reports module.
After defining the report, you can view it in the EU Sales Report window.
Selection Criteria
Selection Criteria Name
Specify selection criteria from a predefined set or press CTRL + A to specify a new criterion.
Date
Generates the report according to either a posting date or a document date or a VAT date or a system date range that you specify.
Interval
Generates the report for a calendar month, quarter, or year:
Month– specify the month for which you want to create the report.
Quarter – specify the quarter for which you want to create the report.
Year – generates the report for the entire calendar year.
 Note
Since the month, quarter, and year date ranges are calendar values, they do not necessarily match the posting periods defined
for the company.
Round Amounts
Report displays rounded amounts.
Summary Layout
Displays the report results grouped by countries.
Display Credit Memos in Separate Section
Displays credit memos separated from the other documents included in the report.
Group by Sales Code
Select to group all transactions with the same federal tax ID and the same transactions type (Goods Shipment / Triangular Deal /
Service Supply) and the same sales code under one node.
Include Service Documents
Select this checkbox to include Service type sales and purchasing documents in the report.
Output
All tax groups marked as EU:
Code – tax group code
Name – tax group name
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/12/26, 12:25 PM
Display – select the tax groups you want to include in the report
Amount – select the tax groups for which you want to display a summary in the report.
Include Inventory Transfers
Select this checkbox to include the following three types of Inventory Transfers in the report:
"Call-off Inventory Transfer" when inventory transfers are from warehouses in your company's home country/region to
warehouses in foreign EU countries/regions.
"Call-off Inventory Return" when inventory transfers are from warehouses in foreign EU countries/regions to warehouses in
your company's home country/region.
"Inventory Transfer" when inventory transfers are from warehouses in foreign EU countries/regions to warehouses in
foreign EU countries/regions.
Inventory transfers from warehouses in your company's home country/region to warehouses in your company's home
country/region are not reported.
Include Down Payment Documents
Select this checkbox to include down payment documents in the report.
Save
Save your selection criteria for future use.
More Information
EU Sales Report: Europe
EU Sales Report Window
This window displays the EU Sales report according to your defined selection criteria.
EU Sales Report Window
Country/Region
The first two characters of the federal tax ID found in the shipping address of the document.
Tax No.
Tax number saved in the sales document, without the first two characters, according to the customer’s shipping address.
Customer Code
Displays the code for the business partner.
Customer Name
Displays the name of the customer.
All EU Sales, Code
Values derived from the tax groups.
Doc. No.
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/12/26, 12:25 PM
In an expanded display, the document number and symbol.
 Example
IN 43222 stands for invoice number 43222.
Posting Date, Period, Posting Year
Document date, relevant period number and posting year, in which the document was created.
Document Date
Displays the document date defined for the document or transaction.
VAT Date
Displays the VAT date defined for the document or transaction.
Value
Total sales amount not including tax per document.
If the document includes freight (on row level and/or document level), to which EU tax groups have been defined, the value of these
freight is added here.
Inventory Transfers
If the Include Inventory Transfers checkbox is selected in the report selection criteria, then three types of inventory transfers are
reported in separate categories:
"Call-off Inventory Transfer" is reported in the EU Sales field when inventory transfers are from warehouses in your
company's home country/region to warehouses in foreign EU countries/regions.
"Call-off Inventory Return" is reported in the EU Sales field when inventory transfers are from warehouses in foreign EU
countries/regions to warehouses in your company's home country/region.
"Inventory Transfer" is reported in the EU Sales field when inventory transfers are from warehouses in foreign EU
countries/regions to warehouses in foreign EU countries/regions.
Inventory transfers from warehouses in your company's home country/region to warehouses in your company's home
country/region are not reported.
Withholding Tax Report
This report displays the withholding tax amounts collected and paid during specific periods.
 Note
If a payment on account with withholding tax has been fully reconciled (that is, the reconciled amount equals the payment
amount), the withholding tax report does not include the payment information.
 Note
When you print the report, you can print the selection criteria on a separate page.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/12/26, 12:25 PM
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner
Vendor Mode – Detailed Format Window
Withholding Tax Report by WTax Code
Withholding Tax Report - Selection Criteria
Use this window to specify selection criteria for the Withholding Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Withholding Tax Report. Alternatively, open
it from the Reports module.
New requirements for the Tax Summary Report and layouts are occasionally introduced by the authorities for different taxation
periods. Variations in selection criteria may exist for different taxation periods which result in different outputs.
After defining the report, you can view it in the Withholding Tax Report by Business Partner Window or the Withholding Tax Report
by WTax Code Window.
Selection Criteria
Selection Criteria Name
Specify the previously saved selection criteria you want to apply for the report, or press CTRL + A to specify new ones.
Date From...To...
Choose whether to include documents based on document date or posting date and specify the date range of the current year.
Declared Period
Specify the required declaration period.
Declaration Type
Specify the type of declaration:
Original: The report includes all documents within the specified date range. When you approve the report, these documents
will be marked as printed.
Substitute: The report includes all documents within the specified date range, including documents already marked.
Complementary: The report includes only unmarked documents within the specified date range.
Vendors
Opens the Vendor Selection window, where you can select the vendors to include in the report.
Customers
Opens the Customer Selection window, where you can choose the customers to include in the report.
Doc. Type
Opens the Document Type window, where you can select the documents to include in the report.
Withholding Tax
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/12/26, 12:25 PM
Codes and names of all tax codes relevant for the report. Deselect tax codes that should be excluded.
 Note
To clear the entire column, click the column header.
To display subtotals for tax codes, select the relevant tax codes in the Amount column.
[Arrow Up/Down]
Determines the order of appearance of the tax codes in the report display and print layout.
Output Mode
Choose the required layout of the report.
The following display the report related to purchasing documents:
WTax Code Layout-Purchasing: grouped by tax codes
Vendor Layout-Purchasing: grouped by vendors
The following display the report related to sales documents:
WTax Code Layout-Sales: grouped by tax codes
Customer Layout-Sales: grouped by customers
Exceptional Event
Exceptional Event options are available for Withholding Tax Reports.
Save
Saves your selection criteria for future use.
Withholding Tax Report by Business Partner Window
This window displays the withholding tax report by business partners according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Report by Business Partner Window Fields
#
Double-click a row to open the Vendor Mode – Detailed Format window for detailed information about the relevant business
partner, grouped by document numbers.
BP Name
Displays the name of the business partner. Choose the icon to open the Business Partner Master Data window.
Federal Tax ID
Displays the federal tax ID of the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/12/26, 12:25 PM
Document Amount
Displays the total document amount of the business partner.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Subject Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
Vendor Mode - Detailed Format Window
Withholding Tax Table
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/12/26, 12:25 PM
Vendor Mode - Detailed Format Window
This window displays detailed information about the relevant business partner, grouped by document numbers.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Vendor Mode – Detailed Format Window Fields
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Example
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see the Transaction
Type Abbreviation Legend page in the general online help.
Date
Displays the posting date of the reconciled transaction or payment.
WTax Code, WTax %, Official Code
Displays the code, rate, and official code of the withholding tax that is included in the reconciled transaction or payment.
Invoice Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Date
Displays the posting date of the payment.
Non-Subject Amount
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/12/26, 12:25 PM
Displays the following result: the base amount - the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
More Information
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner Window
Withholding Tax Table
Withholding Tax Report by WTax Code Window
This window displays the withholding tax report by withholding tax codes according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Report by WTax Code Window Fields
WTax Code, WTax Name, WTax %
Displays the code, name, and rate of the withholding tax defined in the Withholding Tax Codes – Setup window according to your
selection criteria.
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Note
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see Transaction Type
Abbreviations Legend in the general online help, under: Help Documentation Online Help .
Document Date
Displays the posting date of the document.
Payment Date
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/12/26, 12:25 PM
Displays the posting date of the payment.
Document Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Sbj. Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/12/26, 12:25 PM
Withholding Tax Table
Withholding Tax Table
You can check the details and break up of the withholding tax types involved in the document and also edit the withholding tax
information as needed. To open this window, in the relevant A/P or A/R transaction window, click beside the WTax Amount field.
WT Tax Category
Displays the withholding tax category from the business partner withholding tax setup.
Details
Specify any detailed information you want to put for the withholding tax.
Code
Display the code defined in the Withholding Tax Codes - Setup window and also selected for the business partner.
Name
Display the code description you have defined in the Withholding Tax Codes - Setup window.
Rate
Display the Effective Rate which is based on the rate defined in the Withholding Tax Codes - Setup window.
Base Amount
Display the base amount depending on the amount in the transaction.
Taxable Amount
Display the taxable amount in the transaction.
WTax Amount
Display the withholding tax amount which is calculated based on the taxable amount and the rate.
Category
Displays the document category.
Base Type
Displays the base type which you have defined in the Withholding Tax Codes - Setup window.
Criteria
Displays the criteria which you have defined for the business partner.
More Information
Withholding Tax Codes - Setup Window
Tax Reconciliation Report
This report enables you to track the tax amounts that were posted in sales and purchasing documents and in manual transactions.
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/12/26, 12:25 PM
The report displays the G/L accounts involved in these transactions and calculates the tax amounts that should have been paid,
based on the tax codes defined for each transaction.
The report covers the following transactions:
A/P and A/R invoices
A/P and A/R credit memos
Manual journal entries
A/P and A/R down payment invoices
Incoming and outgoing payments
 Note
When saving a journal entry, if you deselect the Automatic Tax option in the Journal Entry window, you cannot view the journal
entry in this report.
 Note
When printing the report, you can print the selection criteria on a separate page.
 Note
Accounts are only displayed when there is at least one posting with a VAT code on the accounts within the respective period.
More Information
Tax Reconciliation Report - Selection Criteria
Accounts - Selection Criteria
Tax Report - Reconciliation Window
Tax Reconciliation Report - Selection Criteria
Use this window to specify selection criteria for the Tax Reconciliation report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Reconciliation Report . Alternatively,
open it from the Reports module.
After creating the report, you can view it in the Tax Report - Reconciliation window.
 Note
Only G/L accounts that have VAT transaction postings are considered in this report. Accounts are only subsequently displayed
in the report when there is at least one posting with a VAT code on the accounts within the respective period.
Selection Criteria
Selection Criteria Name
Click to select previously saved report selection criteria and use them to generate the report.
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/12/26, 12:25 PM
To save new selection criteria, press CTRL + A and enter a name in this field.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting Data tab of the Company
Details window Administration System Initialization Company Details ).
Opening Balance, Non-VAT Transactions
The report displays transactions grouped by G/L accounts and divided by tax codes, including non-tax transactions. This display
lets you crosscheck between the tax report, tax and tax based account balances, and the balance of the connected G/L account in
the system.
In addition, the report displays the opening balance of the specified tax based accounts, additional non-tax transactions that were
posted to this account, the document date, and the journal amount.
Select the Non-VAT Transactions checkbox to include the non-VAT transactions posted to the relevant G/L accounts in the report.
Date From...To
Define a date range for the report. By default, these fields display the start and end dates of the current fiscal year.
Document Date
Generates the report according to document, not posting date.
Round Amount
Report rounds off its amounts.
Series
Choose to select the series, for example, products, services, regions or brands, to include in the report.
Doc. Type
Choose to select the types of documents to include in the report.
Output
Codes and names of all the tax codes defined as output tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
Use the Amount column to select the tax codes for which you want to display subtotals.
Input
Codes and names of all the tax codes that are defined as input tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/12/26, 12:25 PM
Use the Amount column to select the tax codes for which you want to display subtotals.
[Arrow Up/Down]
Use these buttons to determine the appearance order of the selected tax codes in the report display and in the printed report.
G/L Accounts
Choose to open the Accounts – Selection Criteria window, in which you choose the G/L accounts to include in the report.
Save
Choose to save your report selection criteria for future use.
Related Information
Accounts - Selection Criteria
Accounts - Selection Criteria
Use this window to specify selection criteria for the current report.
To open this window, choose the button in the G/L Accounts field, in the Selection Criteria window of the relevant report.
Selection Criteria
Find
Opens the G/L Accounts window for selecting the G/L accounts to be displayed in the report. Selected accounts are marked with
an X.
Level
Choose the Level of the account display in the table.
Choosing Level 1 displays the highest level titles for the accounts. When you select a row in the table, you select all the accounts
that appear under this title.
Level
This column shows which accounts or titles have been selected.
If a row is marked with X, the specific account or group of accounts appears in the report.
To select an account, click in the selected row.
To cancel a selection, clear its X.
To clear all selections/select all accounts in the table, click the X in the column header.
Account
This column displays the codes and names of the accounts.
To view details of each account, use the arrow that appears next to the code and name.
More Information
Tax Reconciliation Report
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/12/26, 12:25 PM
Tax Report - Reconciliation Window
This window displays the Tax Reconciliation report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Reconciliation Window
#
Choose to expand or collapse the display of each account.
Tax Code
Displays the tax codes involved in the transactions included in the report, for each G/L account.
Click to display a list of the transactions involving that tax code.
Tax %
Displays the tax rate of the tax code.
Posting Date
Displays the posting date of the document/journal entry.
If Tax Date is selected in the Selection Criteria window, this column displays the tax date of the document/journal entry.
Tax Base Amount
Displays the amount that is the basis for the tax calculation and was posted to the G/L account.
Tax Amount
Tax amount calculated for the report.
Deferred Tax Document
Indicates whether the document contains deferred tax.
Tax Declaration Box Report
This tax report should be generated monthly or quarterly. It includes transactions that involve tax and pertain to tax codes. The
following documents and transactions are covered in the report:
A/R and A/P invoices
A/R and A/P credit memos
Incoming payments and outgoing payments
Manual journal entries
Down payments
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/12/26, 12:25 PM
When printing the report, you can print the selection criteria on a separate page.
More Information
Tax Declaration Box Report - Selection Criteria
Tax Report - Declaration Window
Tax Declaration Box - Selection Criteria
Use this window to specify selection criteria for the Tax Declaration Box report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Declaration Box Report . Alternatively,
open it from the Reports module.
After creating the report you can view it in the Tax Report-Declaration window.
Selection Criteria
Selection Criteria Name
Click to select previously saved report selection criteria and use them to generate the report. To save new selection criteria,
press CTRL + A and enter a name.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting tab of the Company
Details window ( Administration System Initialization Company Details ).
Adjustment
Select the adjusted version of a report.
Date From... To
Specify a range of posting dates or document dates or VAT dates or system dates to include specific transactions in the report. By
default, the From and To fields display the start and end dates of the current fiscal year.
If the specified From date falls into the effective period range of a tax declaration box group, all the tax declaration boxes within this
group are automatically displayed in the Tax Declaration Boxes table. For more information about the effective period of a tax
declaration box group, see the Effective From field in Tax Declaration Boxes - Setup window.
Round Amount
Report rounds off its displayed amounts.
Tax Declaration Boxes
This table displays the tax declaration boxes according to the specified From date. It includes the following columns:
Code – displays the code of the box
Name – displays the name of the box
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/12/26, 12:25 PM
Opening Balance - you can manually enter the opening balance relevant for each box
Display – all the checkboxes in this column are selected by default. Deselect the checkboxes of the boxes you want to
exclude from the report.
Save
Choose to save the Report Selection Criteria for future use.
More Information
Tax Declaration Box Report
Tax Report - Declaration Window
This window displays the Tax Declaration Box report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Declaration Window
Box Code
Displays the box code and a drill-down option to display the tax group or boxes that are combined to calculate the value for this
box.
Box Component Code
Displays the code of the component included in the box, and provides a drill-down icon that enables you to display the tax codes
included in each component.
Tax Code
This column displays tax codes only in expanded view mode.
Use the drill-down icon next to the tax code to display a list of documents which use that tax code.
Tax %
Displays the rate of each tax group.
Posting Date
Displays the posting date of each document.
Doc. Date
Displays the document date of each document.
VAT Date
Displays the VAT date of each document.
Credit Amount, Debit Amount
In a collapsed view mode, the credit column displays the cumulative amounts of both the credit and debit sides. A negative amount
indicates a greater debit side, and vice versa.
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/12/26, 12:25 PM
In an expanded view mode, these columns display the credit or debit amounts per row in the transaction created by each
document.
Summary Field
Displays the summary criteria defined in the Define Tax Declaration Box window.
Debit/Credit
Displays the choice made in the Credit/Debit column of the Define Tax Declaration Box window.
More Information
Tax Declaration Box Report
Business Activity Statement Reporting
Business activity statement (BAS) reporting is used by businesses in different countries for various purposes.
Usually, BAS reporting is done on a monthly, quarterly, or annual basis. However, it is also possible to report transactions, the dates
of which are beyond the range of the reported month, quarter, or year.
Prerequisites
Initializing the BAS Reporting Function
To initialize the BAS reporting function, you have done the following:
1. You have selected the Extended Tax Reporting checkbox in Administration System Initialization Company Details
Accounting Data .
2. You have defined the period type for BAS reporting at the same location.
Related Information
Defining BAS Codes
Generating BAS Reports
Retrieving BAS Reports and Saving Report Data
Generating BAS Reports
Procedure
1. Choose Financials Financial Reports Accounting Tax BAS Report Generation .
The BAS Report Generation - Selection Criteria window appears.
2. Specify the tax declaration type (VAT declaration type under English UK language settings):
Original: To save the report for the first time in a given period.
Replacement: To correct a report that has already been saved.
Adjusted: To show only documents that have not yet been included in any previous report for a given period.
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/12/26, 12:25 PM
3. Specify the tax declaration name (VAT declaration name under English UK language settings) by selecting the appropriate
year and period. For a replacement declaration, also select the desired adjustment number.
4. Choose the date and date range according to which transactions should be included in the report, and choose OK.
The BAS Report - Generation window appears.
5. In this window, select the documents and transactions that you want to include in the report. The documents and
transactions are grouped by BAS code. You can change the values in the report for manual BAS codes and select one option
from “Single Choice” type codes.
6. To save the report, choose Add and OK.
Related Information
Business Activity Statement Reporting
Retrieving BAS Reports and Saving Report Data
Prerequisites
You have generated the BAS report for the desired reporting period.
Context
You can retrieve BAS reports for review and, depending on the localization, save the report data to be submitted to the tax
authorities.
To retrieve and save the BAS reports, use the BAS report retrieval function. Proceed as follows:
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting Tax BAS Report
Retrieval .
The BAS Report Retrieval - Selection Criteria window appears.
2. Select the tax declaration name and the BAS codes you want to display, and choose OK.
The BAS Report - Retrieval window appears. It shows all documents included in the report, grouped by BAS code. To
display the individual transactions, click the down arrow for a BAS Code or choose Expand to display all documents.
3. To export the BAS amounts, choose Export. The BAS Report Export window appears. It displays the BAS codes and the
corresponding tax amount.
4. To export the values to Microsoft Excel, choose File Export MS-EXCEL . You can then open the file in Microsoft Excel,
fill in the electronic or paper form of the business activity statement and submit it to the tax authorities.
Related Information
Business Activity Statement Reporting
Generating BAS Reports
Banking
This section describes the features and functions under the Banking module that are specific to the localization for UK
International and Republic of Ireland only.
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/12/26, 12:25 PM
Information about general features and functions in the Banking module is available in the general online help file provided with
SAP Business One, under Help Documentation Online Help
Postdated Check Deposit
Use this function to transfer to the cash account checks that were deposited as postdated.
To deposit postdated checks, choose Banking Deposits Postdated Check Deposit .
More Information
Postdated Checks Deposit Window
Depositing Postdated Checks
Procedure
1. Choose Banking Deposits Postdated Check Deposit .
2. In the general area of the window, fill in the fields so that the table displays the checks you want to deposit.
3. Specify the account to which the amount of the selected postdated checks should be transferred.
 Note
Only checks deposited as postdated checks in the Deposit window can be deposited from the Postdated Check Deposit
window.
4. Select the checks to be deposited.
5. To record the deposit in the database, choose Add.
Results
A journal entry transferring the deposited checks from the postdated checks account to the cash checks account is created. The
status of the checks is updated from Deposited as Deferred to Deposited as Cash.
Postdated Check Deposit Window
To open the Postdated Check Deposit window, choose Banking Deposits Postdated Check Deposit .
Postdated Check Deposit Window
Key
Successive number, starting from 1, for each postdated check deposit document.
Deposit Currency
To display only checks created with one currency, specify this currency. If you choose a foreign currency, a field displaying the
exchange rate appears. You can change the exchange rate if required.
Bank Account
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/12/26, 12:25 PM
Specify the account code to which the checks should be transferred.
Date
Due date of the checks. This is the current date by default. Change the date if required.
Display Until
Specify a date to display all checks that have reached their value date by this date.
Find Check No.
To trace a specific check, specify its number. SAP Business One marks the required check.
Date, Account Code, Check, Bank, Branch, Acct No., BP/Account Code, BP/Account Name, Check Amount, Incoming Payment
Information about the postdated checks.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
Total for Deposit
Total amount of all checks selected for deposit.
No. of Checks
Number of checks selected for deposit.
Remarks
Remarks about this document.
Reconcile Amounts After Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Check Deposit
Postdated Credit Voucher Deposit
Use this function to transfer to the cash account credit card vouchers deposited to the deferred account.
To deposit postdated credit card vouchers, choose Banking Deposits Postdated Credit Voucher Deposit .
More Information
Postdated Credit Voucher Deposit Window
Depositing Postdated Credit Card Vouchers
Depositing Postdated Credit Vouchers
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/12/26, 12:25 PM
Context
Follow this procedure to deposit vouchers that were deposited as postdated to the cash account credit card.
Procedure
1. Choose Banking Deposits Postdated Credit Voucher Deposit .
2. In the general area of the window, specify the relevant parameters to display in the table the credit card vouchers to be
deposited.
3. Select the credit card vouchers you want to deposit.
4. If a commission is involved in the deposit, choose next to Total Commissions.
5. In the Commission window, specify the commission details and choose Update.
6. To record the deposit in the database, choose Add.
Results
A journal entry that transfers the postdated credit card vouchers from the deferred account to the cash account is created. If the
deposit involves a commission, this is reflected in the journal entry.
Related Information
Postdated Credit Voucher Deposit Window
Postdated Credit Voucher Deposit Window
To open the Postdated Credit Voucher Deposit window, choose Banking Deposits Postdated Credit Voucher Deposit .
Postdated Credit Voucher Deposit Window
Key No.
Successive number, starting from 1, for each deposit of a postdated credit card voucher or postdated check.
Deposit Currency
To display credit card vouchers created with a particular currency, specify this currency.
No. of Vouchers
Number of vouchers selected for deposit.
Display Until
To display all credit card vouchers that have reached their value date by a certain date, specify this date.
Date
By default, the current date. You can change this date if necessary.
Find Voucher No
To find a credit card voucher by its number, sort the Doc. No. column and then specify the required number here. SAP Business
One places this voucher at the beginning of the list.
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/12/26, 12:25 PM
Date, Acct Code, Doc. No., Card Name, Ref., Payment Method, BP/Account Code, BP/Account Name, # Pymts, of, Total,
Incoming Payment
Information about the postdated credit card vouchers displayed.
Journal Remarks
Add any comments about the deposit.
Trans. No.
Number of the journal entry created by this document and a link to it. The number appears after you have added the document.
Total Commissions
Opens the Commission window where you can enter the amount of commission to be paid for the deposit.
Reconcile Amounts after Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Credit Vouchers Deposit
Commission Window
Manually Reconciling Bank Statements
 Recommendation
When you use this function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do not
simultaneously use the external bank statement processing function (see Recording Transactions from External Statements in
the general online help file provided with SAP Business One) and the standard function for manually performing an external
reconciliation (see Manually Performing External Reconciliations in the general online help file provided with SAP Business One)
for the same bank account. In addition, we recommend that you use exclusively either this function or the standard function for
manually reconciling bank statements.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
The External Bank Reconciliation - Selection Criteria window appears.
2. In the Account Code field, select an account code.
As a result, Account Name and Currency are displayed automatically in the respective fields. If the account currency is
defined as All Currencies, the local currency is displayed and is the reconciliation currency. You cannot edit the Currency
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/12/26, 12:25 PM
and the Last Balance fields. In addition, the Last Balance field automatically displays the updated balance from the
previous reconciliation.
In the Ending Balance field, specify the current balance received from the bank; in the End Date field specify the date to
which the current balance is updated.
3. Choose OK.
The Reconciliation Bank Statement window appears.
SAP Business One displays all the open deposits and payments in which the selected account is involved. View and specify
the information displayed.
4. Select the transactions to be cleared.
When you select a transaction, SAP Business One recalculates the value in the Difference field. Reconciliation is performed
only if the difference equals zero.
5. If the value in the Difference field is not zero, do one of the following:
Create an adjustment.
For more information, see Creating Adjustments.
Save your selection for future processing.
Choose the Save button. The next time you choose the same account in the External Bank Reconciliation -
Selection Criteria window, the Reconciliation Bank Statement window displays the saved selection.
6. To perform the reconciliation, choose the Reconcile button.
 Note
You cannot re-create reconciliations created in the Reconciliation Bank Statement window.
Result
SAP Business One reconciles the selected transactions and sets the reconciliation type for this reconciliation to Manual.
More Information
Example: Manual Reconciliation of External Bank Statements
Creating Adjustments
To reflect transactions that are already in the bank statement but are not yet posted in SAP Business One, you can create a
balancing transaction or document.
 Recommendation
When you use this localized function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do
not simultaneously use the external bank statement processing function (see the Recording Transactions from External
Statements page in the general online help provided with SAP Business One) and the standard function for manually
performing an external reconciliation (see the Manually Performing External Reconciliations page in the general online help
provided with SAP Business One) for the same bank account. In addition, we recommend that you use exclusively either this
function or the standard function for manually reconciling bank statements.
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/12/26, 12:25 PM
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
After you make the required adjustments, the difference between the ending balance in the bank statement and the account
balance in the books equals zero, and you can now reconcile the selected transactions.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
2. In the External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
3. In the Reconciliation Bank Statement window, make the required selections and choose Adjustments.
The Adjustments window appears.
4. Select one of the following types of transactions you want to create and choose OK:
Journal entry
Incoming payment
Outgoing payment
Check for payment
Deposit
The window of the selected transaction type appears.
5. Create the required transaction and choose Add.
As a result, the created transaction is added to the table of the Reconciliation Bank Statement window, and it is also
selected. The value in the Difference field is updated accordingly.
6. To perform the reconciliation, choose the Reconcile button.
More Information
Manually Reconciling Bank Statements
Example: Manual Reconciliation of External Bank Statements
External Bank Reconciliation - Selection Criteria Window
Reconciliation Bank Statement Window
Example: Manual Reconciliation of External Bank Statements
On December 1, 2009, you decide to perform a reconciliation for your bank account. The last balance of this account was 100, and
the ending balance of this bank account for this date is 250.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/12/26, 12:25 PM
The Reconciliation Bank Statement window displays 2 deposits that you can clear:
Date Transaction Number Deposit Amount
November 10, 2009 927 45
November 24, 2009 929 100
You need to reconcile transactions to match the value of the cleared book balance to the ending balance of this bank account. In
this case, you need to reconcile transactions with a total amount of 150 = 250 minus 100.
You select both transactions, but the total amount of the open transactions is 145 = 45 + 100.
You create a manual journal entry as an adjustment, debiting the bank account by the amount of 5.
As a result, an additional row is added to the list of transactions you want to clear. The difference between the cleared book balance
and the statement ending balance is now zero, enabling you to complete the reconciliation.
More Information
Creating Adjustments
External Bank Reconciliation - Selection Criteria Window
Use this window to define the selection criteria for manually reconciling bank statements.
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation .
External Bank Reconciliation – Selection Criteria Window Fields
Account Code, Account Name, Currency
Select the relevant account code.
After you select an account code, the account name and currency are displayed automatically in the respective fields. If the
account is defined as All Currencies, the local currency is displayed and is the reconciliation currency.
 Note
You cannot edit the Currency field (described above) and the Last Balance field (described below).
Bank Statement
This section contains the following fields:
Last Balance – Automatically displays the updated balance from the previous reconciliation.
Ending Balance – Specify the current balance received from the bank.
End Date – Specify the date to which the current balance is updated.
More Information
Reconciliation Bank Statement Window
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/12/26, 12:25 PM
Manually Reconciling Bank Statements
Reconciliation Bank Statement Window
This window displays all the open deposits and payments in which the account you chose in the External Bank Reconciliation -
Selection Criteria window is involved.
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation . In the
External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
General Area
Account Code
Displays the account code selected in the External Bank Reconciliation – Selection Criteria window.
Display
Determines what transactions are displayed. Select one of the following display options:
All – Both cleared and uncleared transactions
Cleared – Only cleared transactions
Uncleared – Only uncleared transactions
Find
Enables you to find a specific transaction in a sorted column.
 Example
To find a transaction according to its number, sort the Trans. No. column. Then in the Find field, specify the relevant number.
SAP Business One highlights the first transaction that matches the value entered.
 Note
By default, the Date column is sorted.
Statement No.
Specify the number of the statement you received. This number is unique for each account. This means you can assign the same
number to statements created for different accounts; however, you can assign the same number only to one statement in each
account. You can create a statement without a number.
 Note
If a reconciliation is canceled, its statement number becomes available again and can be used for a new reconciliation.
Last Statement Balance
Displays the balance of the previous statement.
Payment, Deposit: Total No., Total Amount
The Total No. field displays the total number of selected transactions on the debit side (Payment) and on the credit side (Deposit).
The Total Amount field displays the cumulative debit amount and credit amount.
Cleared Book Balance
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/12/26, 12:25 PM
Displays the total cleared amount, considering the selected transactions.
Statement Ending Balance
Displays the value entered in the Ending Balance field in the External Bank Reconciliation – Selection Criteria window.
Difference
Displays the difference between the Cleared Book Balance and the Statement Ending Balance. This value depends on the
selected transactions.
Save
Saves the current reconciliation so that you can continue working on it later. The next time you choose the same account in the
External Bank Reconciliation – Selection Criteria window, the Reconciliation Bank Statement window displays the saved
selection.
Adjustments
Enables you to create any required bank adjustments by opening the Adjustments window. For more information, see Creating
Adjustments .
Table Area
Cleared
Select to indicate that the transaction has been cleared.
Type
Displays the transaction type:
PS – represents payments, that is, transactions in which the selected account is credited
DP – represents deposits, that is, transactions in which the selected account is debited
Date
Displays the posting date of the transactions.
Trans. No.
Displays the number of the transaction and provides a link to the journal entry.
Reference No.
Displays the reference number as it appears in the Ref. 1 field in the Journal Entry window.
Payment
Displays the amount on the debit side in the transaction.
Deposit
Displays the amount on the credit side in the transaction.
Cleared Amount
After you select the transaction, the amount in the Payment/Deposit column is displayed here.
More Information
External Bank Reconciliation - Selection Criteria Window
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/12/26, 12:25 PM
Manually Reconciling Bank Statements
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
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/12/26, 12:25 PM
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
Goods receipt P/O based Goods return based on Inventory Allocation Negative Adjustment
| on goods return |     | goods receipt P/O |     | Account, Price |
| --------------- | --- | ----------------- | --- | -------------- |
Differences Account
Goods return based on Goods receipt P/O based Inventory Allocation Negative Adjustment
| goods receipt P/O |     | on goods return |     | Account, Price |
| ----------------- | --- | --------------- | --- | -------------- |
Differences Account
| A/P invoice based on |     | Credit memo based on | No inventory transaction |     |
| -------------------- | --- | -------------------- | ------------------------ | --- |
| goods receipt P/O    |     | goods return         |                          |     |
A/P credit memo based A/P invoice based on Vendor, Allocation Price Differences
| on goods return |     | goods receipt P/O |     | Account, Negative |
| --------------- | --- | ----------------- | --- | ----------------- |
Adjustment Account
A/P credit memo based Invoice based on credit Inventory Vendor Negative Adjustment
| on A/P invoice |     | memo |     | Account, Price |
| -------------- | --- | ---- | --- | -------------- |
Differences Account
Delivery based on return Delivery based on return Inventory COGS Negative Adjustment
Account
Return based on delivery Return based on delivery Sales Return COGS Negative Adjustment
Account, Price
Differences Account
| A/R invoice based on  |     | Credit memo based on | No inventory transaction |     |
| --------------------- | --- | -------------------- | ------------------------ | --- |
| delivery              |     | return               |                          |     |
| A/R credit memo based |     | A/R invoice based on | No inventory transaction |     |
| on return             |     | delivery             |                          |     |
A/R credit memo based A/R invoice based on Sales Return COGS Negative Adjustment
| on invoice |     | credit memo |     | Account, Price |
| ---------- | --- | ----------- | --- | -------------- |
Differences Account
Updating and Deleting Posted Purchasing Documents
Some purchasing documents such as A/P invoices or goods receipt POs are legally binding. Therefore, you cannot delete them or
make any changes that affect inventory entries or journal entries after you created these documents in SAP Business One.
However, you can change data that is not relevant for inventory or journal entries. For example, if you wish to postpone the
payment date of an invoice or the payment method.
Prerequisites
You have full authorization to modify posted A/P documents (check under  Administration   System Initialization
|  Authorizations  |  Purchasing | ).  |     |     |
| ---------------- | ----------- | --- | --- | --- |
Activities
You can modify the following data in A/P invoices, A/P down payment requests, A/P down payment invoices, A/P reserve invoices,
and A/P credit memos after posting them in SAP Business One:
Due date (if the document was not partially or fully copied into another document, or partially or fully paid)
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/12/26, 12:25 PM
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
Updating and Deleting Posted Sales Documents
After you have posted a sales document, you can no longer delete the document or make any changes that affect inventory entries
or journal entries. For example, you cannot change or delete deliveries or invoices for legal reasons. You must either reject or
reverse them by means of a clearing posting.
You cannot change or delete the rows in a sales document once follow-on documents have been created with reference to the rows
in the sales document.
For some localizations however, you can change certain data on posted sales documents. For example, if your customer calls and
wishes to postpone the payment date of an invoice or change the payment method.
Prerequisites
You have full authorization to modify posted A/R documents (check under Administration System Initialization
Authorizations Sales ).
Activities
You can modify the following data in A/R invoices, A/R down payment requests, A/R down payment invoices, A/R reserve invoices,
and A/R credit memos after posting them in SAP Business One:
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/12/26, 12:25 PM
Due date (if the document was not partially or fully copied into another document, or partially or fully paid)
Payment method (if the document was not partially or fully copied into another document, or partially or fully paid)
Pay-to data (if the document was not partially or fully copied into another document, or partially or fully paid)
Sales employee (can be changed anytime)
Buyer (can be changed anytime)
Owner (can be changed anytime)
Lines of text (can be changed anytime)
Furthermore, it is possible to modify data in deliveries and returns. You can change the following data:
Payment terms (if the document was not partially or fully copied into another document, or partially or fully paid)
Payment method (if the document was not partially or fully copied into another document, or partially or fully paid)
Pay-to data (if the document was not partially or fully copied into another document, or partially or fully paid)
Sales employee (can be changed anytime)
Buyer (can be changed anytime)
Owner (can be changed anytime)
Lines of text (can be changed anytime)
You can also change the due date of any open installments (unreconciled, not yet fully or partially paid installments) in A/R
invoices and A/R reserve invoices.
The changes you make are tracked in the SAP Business One change log. When you print an already posted sales or purchasing
document after you made some changes to it, the printout includes all modifications and the title “Amended”.
Updating Existing Purchasing Documents
The following table describes which changes can be made in existing goods receipt POs, goods returns, A/P invoices, A/P down
payment requests and invoices, A/P reserve invoices, and A/P credit memos:
| Field    | Changes possible after   | Changes possible after    | Comments                  |
| -------- | ------------------------ | ------------------------- | ------------------------- |
|          | document has been added? | document has been closed? |                           |
| Due Date | Yes                      | No                        | If there is more than one |
installment in the A/P invoice,
the Due Date field is disabled.
| Sales Employee | Yes | Yes |     |
| -------------- | --- | --- | --- |
| Owner          | Yes | Yes |     |
| Pay to         | Yes | No  |     |
| Text           | Yes | Yes |     |
Message Documentation
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/12/26, 12:25 PM
Message documentation aims to provide you with the information you need to respond to system or error messages that may
appear in SAP Business One.
410000063
Message
File path does not exist; enter valid file path
Diagnosis
You have attempted to generate an electronic report in a target path that does not exist.
Procedure
In Step 3 of 4 of the EU sales report, specify an existing file path for the generated EU sales report.
More Information
Generating EU Sales Report
10000397
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the Output
Tax Group field empty.
Procedure
In step no. 4, specify the required tax group in Output Tax Group field, and choose Run.
10000398
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run, but you have left the Input Tax
Group field empty.
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/12/26, 12:25 PM
Procedure
In step no. 4, in the Input Tax Group field, specify the required tax group and choose Run.
10000399
Message
Enter valid acquisition tax group
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step 4, the Transaction Confirmation window, you have chosen
the Run button. However, the Acquisition Tax Group field is either empty or contains an invalid tax group.
Procedure
In step 4, the Transaction Confirmation window, in the Acquisition Tax Group field, specify the required tax group, and choose the
Run button.
More Information
Transfer Posting Correction Wizard - Transaction Confirmation Window
10000400
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the Non—
Deductible Tax Group field empty.
Procedure
In step no. 4, specify the required tax group in Non-Deducible Tax Group field, and choose Run.
10000401
Message
Missing or invalid account
Diagnosis
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/12/26, 12:25 PM
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the Interim
Account field empty.
Procedure
In step no. 4, specify the required G/L account in the Interim Account field, and choose Run.
10000402
Message
Missing or invalid account
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the
Revenue Account field empty.
Procedure
In step no. 4, specify the required G/L account in Revenue Account field, and choose Run.
10000403
Message
Missing or invalid account
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the
Expense Account field empty.
Procedure
In step no. 4, specify the required G/L account in Expense Account field, and choose Run.
10000979
Message
In “From” and “To” fields, enter dates
Diagnosis
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/12/26, 12:25 PM
You have opened the Transfer Posting Correction Wizard — Selection Criteria window, and have chosen the Next button, but you
have not specified dates in the From and To fields. To continue to the next step, you must specify a valid date range since SAP
Business One retrieves data in ascending order from the earliest date to the latest date.
Procedure
In the Transfer Posting Correction Wizard — Selection Criteria window, specify dates in the From and To fields.
More Information
Transfer Posting Correction Wizard - Selection Criteria Window
10000982
Message
In “Tax Rate” field, enter number greater than zero
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step 2, the Selection Criteria window, you have chosen the Next
button. However, the Tax Rate contains a negative value.
Procedure
In step 2, the Selection Criteria window, enter a number greater than zero in the Tax Rate field, and choose the Next button.
 Note
Only tax groups with a tax rate of 16% or 19% are valid for the wizard.
More Information
Transfer Posting Correction Wizard - Selection Criteria Window
10000054
Message
Create VAT rows automatically
Diagnosis
In the Recurring Postings window, you have either created a new or updated an existing recurring posting template:
1. You have selected the Automatic Tax checkbox
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/12/26, 12:25 PM
2. In one of the table rows, you have specified in the G/L Acct/BP Code column the code of G/L account that is defined as a
tax account of a tax group (in Administration Setup Financials Tax Tax Groups Tax Groups— Setup window
Tax Account )
3. You have tried to exit the G/L Acct/BP Code column in the Recurring Postings window
Procedure
When the Automatic Tax checkbox is selected, you may create transaction rows only for G/L accounts that are not defined as tax
accounts.
More Information
Recurring Posting Window
10000424
Message
Create VAT rows automatically
Diagnosis
You have created new posting template.
1. In the Posting Templates window you have entered a code and description for the new template. You have selected the
Automatic VAT checkbox.
2. In the table area, in the G/L Acct/BP Code column, you have specified a code of G/L account that is used as tax account (in
Administration Setup Financials Tax Tax Groups ) and tried to exit this field.
Procedure
When creating posting template with the Automatic VAT checkbox selected, G/L accounts used as tax accounts cannot be
specified. To know which G/L accounts are available, open the List of G/L Accounts window. The window lists only the G/L
accounts that can be assigned to the template.
10000488
Message
Enter G/L account not defined as tax account
Diagnosis
In the Journal Entry window, you have tried to created a journal entry manually:
1. You have selected the Automatic Tax checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/12/26, 12:25 PM
2. In one of the table rows, you have specified in the G/L Acct/BP Code column the code of G/L account that is defined as a
tax account of a tax group (in Administration Setup Financials Tax Tax Groups Tax Groups— Setup window
Tax Account ).
3. You have tried to exit the G/L Acct/BP Code column in the Journal Entry window.
Procedure
When the Automatic Tax checkbox is selected, you can only create transaction rows for G/L accounts that are not defined as tax
accounts.
More Information
Creating Journal Entries Manually
10000492
Message
You cannot add document; tax account is missing
Diagnosis
You have tried to add a sales or purchasing document containing one or more items linked to a tax code, but your company has not
set up the tax code correctly.
Procedure
 Note
Ask your superuser to follow the steps below.
1. Choose Administration Setup Financials Tax Tax Groups .
2. In the Tax Account field, specify a valid G/L account number.
More Information
Tax Groups - Setup Window
10000586
Message
Invalid VAT Group
Diagnosis
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/12/26, 12:25 PM
In G/L Account Determination window Purchasing tab Tax sub tab you have specified in the Purchased Tax Group (Items)
field or in the Purchase Tax Group (Services) field the required tax group. By the time you have chosen Update the selected tax
group was deleted from SAP Business One.
Procedure
In the Purchased Tax Group (Items) field or in the Purchase Tax Group (Services) field specify a tax group that appears in
Administration Setup Financials Tax Tax Groups .
10000800
Message
You cannot add correction tax group to invoice
Diagnosis
You have opened an A/R or A/P invoice, and have clicked in the Freight field. The Freight Charges window is displayed. This
window shows the freight defined in the Freight - Setup window.
In the Tax Group column, you have tried to specify the tax group related to the freight. This tax group is wrongly defined as a
correction tax group in SAP Business One.
Procedure
 Note
Ask your superuser to follow the steps below.
1. Choose Administration Setup Financials Tax Tax Groups . The Tax Groups — Setup window displays with the
list of your company's tax groups.
2. Deselect the Corrections checkbox for the required tax group.
10001388
Message
Define effective date
Diagnosis
In the Tax Groups - Setup window, you have tried to define a new tax group, and you have chosen the Update button. However, the
Effective from field is empty. To continue, you need to define a starting date for which the new tax group is effective.
Procedure
1. Do one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/12/26, 12:25 PM
Double-click the row containing the new tax group.
Select the row containing the new tax group, and then choose the Tax Definition button.
The Tax Definition - Setup: <XXX> window opens.
2. In the Effective from field, specify a starting date for which the new tax group is effective.
3. Choose the Update button, and then the OK button to return to the Tax Groups - Setup window.
More Information
Tax Groups - Setup Window
Tax Definition - <XXX> Window
1250000104
Message
You cannot use a correction tax group for the freight tax group
Diagnosis
You have done the followings:
1. Choose Sales - A/R A/R Invoice .
2. In the A/R Invoice window, add a customer.
3. To open Form Settings window, click the icon.
4. In the Form Settings window, select the Table Format tab, select the Visible checkbox for the fields: Freight X, Freight
X(LC), and Freight X Tax Group, and choose the OK button.
5. Add one item and in the Freight X Tax Group column, select the newly created tax group.
6. You change the tax group that you have selected for the Freight X Tax Group column as correction.
 Example
a. Choose Administration Setup Finance Tax Tax Group .
b. In the Tax Groups - Setup window, select the tax group you have selected for the Freight X Tax Group column
and select the Correction checkbox.
7. In the A/R Invoice window, specify the other information and choose the Add button.
Procedure
In the Freight X Tax Group field in the A/R Invoice window, select a non-correction tax group.
This is custom documentation. For more information, please visit SAP Help Portal. 121