6/12/26, 12:24 PM
Localization for Central MENA
/AE/EG/LB/OM/QA/SA
Generated on: 2026-06-12 12:24:47 GMT+0000
SAP Business One | 10.0
Public
Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/e429e5cb0d1144ecbdad7f550cd70664?locale=en-
US&state=PRODUCTION&version=10.0
Warning
This document has been generated from SAP Help Portal and is an incomplete version of the official SAP product documentation.
The information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be
missing important aspects and/or correlations to other topics. For this reason, it is not for production use.
For more information, please visit https://help.sap.com/docs/disclaimer.
This is custom documentation. For more information, please visit SAP Help Portal. 1

6/12/26, 12:24 PM
Localization for Central MENA/AE/EG/LB/OM/QA/SA
This documentation describes features and functions in SAP Business One that are specific to the localization for Central
MENA/AE/EG/LB/OM/QA/SA (Middle East and North Africa: United Arab Emirates/Egypt/Lebanon/Oman/Qatar/Saudi Arabia).
Information about general features and functions that are not localization-specific is available in the online help for SAP Business
One. You can also access the online help and localization-specific information directly in SAP Business One ( Help
Documentation Online Help and Help Documentation Country/Region Specific Information ).
Setup and Administration: Central
MENA/AE/EG/LB/OM/QA/SA
This section describes the settings and definitions related to functions that are specific to Central MENA /AE/EG/LB/OM/QA/SA.
Information about settings and definitions related to general functions is available in the general online help file, under: Help
Documentation Online Help .
Company Details
Accounting Data tab
Use Deferred Tax
Select if you want to recognize tax when the payment takes place and not when the invoice is created.
Extended Tax Reporting
Generates and saves the tax report for tax authorities.
Selecting this checkbox opens the Period Type for Report Generation dropdown list.
Period Type for Report Generation
Enabled when you select the Extended Tax Reporting checkbox.
Specify the period type for the report generation.
Basic Initialization tab
Use Bill of Exchange
Select to indicate that the company uses bills of exchange (BoE). If not selected, all references to BoE in SAP Business One are
hidden. When a BoE transaction is added, Use Bill of Exchange cannot be disabled.
Tax-Related Definitions
To set tax-related definitions choose: Administration Setup Financials Tax The following settings are available:
Tax Groups
Tax Code Determination
Withholding Tax Codes
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/12/26, 12:24 PM
Defining BAS Codes
Tax Declaration Boxes - Setup Window
Tax Groups - Setup Window
Use this window to define your company's tax groups.
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
This column is relevant only for Input Tax groups (A/P). Select this option to define the tax group as pertaining to Acquisition /
Reverse.
Specifying the acquisition tax is a procedure used when you record goods purchased from EU countries. Tax is not calculated in
the document, but the correct amount is recorded in the journal entry and affects the tax report. In this case, the tax amount in the
rows and in the total of the A/P invoice would be 0.
Effective from, Rate %
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can create additional entries by double-clicking the row number of
the tax group and defining them in the Tax Definition window.
 Note
The tax amounts in the documents are calculated according to the tax group's effective date.
Non Deduct. %
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/12/26, 12:24 PM
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
VAT Exemption Reason
This dropdown field is based on the PEPPOL VATEX code list, and allows you to create or select a reason for VAT exemption in the
Tax Exemption Letter section under Business Partner Master Data Accounting Tax .
Tax Definition - Setup Window
Use this window to specify tax information for a specific group or code.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Groups .
Select the required tax group and choose the Tax Definition button.
Tax Definition - Setup Window
Effective From, Rate
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can specify new values.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/12/26, 12:24 PM
The tax amounts in the documents are calculated according to the tax group's effective date.
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
The Tax Code Determination Rule Setup window appears.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/12/26, 12:24 PM
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
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/12/26, 12:24 PM
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
Specify the tax code that should be proposed in sales or purchasing documents, if the tax code determination rule applies. Use
one of the tax codes defined in the application or create a new one. Depending on the business area you specified, you can only
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/12/26, 12:24 PM
select a tax code relevant for that business area. For example, if you selected Sales as a business area, the application only
displays sales tax codes.
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
You can specify values by using the dropdown list or, for some values, by entering free text. For some of the conditions and values,
if you have specified them once, you can select the value that was used last for the condition from the dropdown list.
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
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/12/26, 12:24 PM
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
the sales or purchasing document must not contain a
value.
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
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/12/26, 12:24 PM
TCD rule definition Master data Freight Setup
Tax code proposed on document
Item Tax Code Line Freight Tax Header Freight Tax
Code Code
A1 A6 A6
More Information
Tax Code Determination
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
Enter the rate of tax to be calculated from the date defined in the Effective From field.
Base Type
Choose either Gross (includes VAT) or Net from the drop-down list to determine from which amount the withholding tax will be
calculated.
% Base Amount
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/12/26, 12:24 PM
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
The BAS Code Definitions - Rows button is available for BAS codes of types VAT Group, Account, and Single Choice.
4. Choose Update and OK.
Modifying BAS Codes
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/12/26, 12:24 PM
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Change the data in the table, for example, the debit/credit data or the formula syntax. For more information about these
fields, see BAS Code Definitions Window.
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
More Information
Business Activity Statement Reporting
BAS Code Definitions Window
In this window, you review the BAS codes used for business activity statement (BAS) reporting, modify or remove BAS codes, or
add new ones.
To open this window, choose Administration Setup Financials Tax BAS Code Definitions .
BAS Code Definitions Window
Effective From
Enables you to set up groups of BAS codes, with each group sharing one effective period. Proceed as follows:
1. Specify the date from which the group of BAS codes you want to create is effective. From the Effective From dropdown list,
select one of the following:
01.01.1900
01.01.2024: This date is displayed by default.
Define New: If you want to specify a date other than 01.01.1990 or 01.01.2024, define a new one.
Once you define a new date, the BAS code group that has the default Effective From date 01.01.2024 is copied to
the new group.
Similarly, every time you define a new date, the existing BAS code group that has the chronologically latest Effective
From date is copied to the new group.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/12/26, 12:24 PM
The chronologically later Effective From date of one BAS code group automatically becomes the "Effective To” date for
the group with the early Effective From date.
For example, you only create two groups of BAS codes, group A and group B. The Effective From dates of group A and B
are set as 01.01.2009 and 01.01.2010, respectively. Therefore, 01.01.2010 automatically becomes the ”Effective To”
date of group A, that is, the effective period of group A is from 01.01.2009 to 01.01.2010.
2. If required, define the individual BAS codes within the group you create.
For each group, you can define different numbers of BAS codes, and each BAS code within the group can have individual
settings.
Code
Code of the tax category to be used in business activity statement reporting.
Name
Description of the tax category to be used in business activity statement reporting.
Type
Indicates how tax is calculated.
VAT Group: Use this type to report, group, and filter transactions by tax codes. You can combine tax groups and/or
constants in a formula using mathematical operations.
If you include a tax group of type Acquisition/Reverse in the formula, you can define the Acquisition/Reverse Tax Type of
the tax group to report only the input tax part (debit side), the output tax part (credit side), or both the input and output tax
parts (both debit and credit sides) of the transactions. To do so, double-click the BAS code row to define the details.
Account: Use this type to report, group, and filter transactions by G/L accounts. You can assign each account to only one
BAS code. This means, after you select an account for a BAS code, it is not displayed for another code selection. We
recommend that you select the Display only accts with postings checkbox in the Select accounts for group: <group
name> window to filter unused accounts.
Manual Input: Use this type if you want to manually enter an amount or a percentage rate, for example, as an adjustment to
a BAS code, in the BAS Report - Generation window.
If you enter a percentage rate, you can use decimals. However, if you enter an amount as an adjustment to a particular BAS
code, you can use decimals only if they are allowed for this BAS code.
Manual Text Input: Use this type if you want to manually enter a text in the BAS Report - Generation window. For this type
of BAS codes, a new column Text Data is available and editable in the BAS Report - Generation window.
Formula: Use this type if you want to combine the existing BAS codes and/or constants in a formula using mathematical
operations.
When you include BAS codes in a formula, use brackets “[]”as placeholders for each BAS code.
 Note
You cannot include a BAS code of type Single Choice in a formula.
 Example
G1, G2, G3, G4, G5, G6, and G7 are BAS codes; S1 and S2 are tax groups.
Among the BAS codes, G5, G6, and G7 are of type Formula.
[G5] = [G2] + [G3] + [G4]
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/12/26, 12:24 PM
[G6] = [G1] – [G5]
[G7] = [G2] /11
G1 is of type VAT Group.
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
Position in Report
Specify the target XML node name.
Summary Field
Select an option to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount
Non-Deductible Amount
Debit/Credit
Determines which parts of the transactions that are calculated are added: for example, only the debit amount, only the credit
amount, or both.
Formula Syntax
Indicates the formula syntax to calculate the tax amount.
Sort Order
Indicates the position of the tax code in the BAS statement.
Absolute Value
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/12/26, 12:24 PM
Displays the absolute amount for the relevant tax code in the report.
More Information
Defining BAS Codes
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
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/12/26, 12:24 PM
Choose Update to move to the next row.
After you have finished defining all VAT groups or boxes for the formula, choose Update to save your changes.
Transfer Posting Correction Wizard
The Transfer Posting Correction Wizard enables you to post corrections resulting from VAT changes, for amounts transferred from
revenue or expense accounts to new accounts.
This wizard guides you in defining parameters required to generate these postings.
To access the wizard, from the SAP Business One Main Menu, choose Administration Utilities Transfer Posting Correction
Wizard .
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
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/12/26, 12:24 PM
Always use the selected option during the rest of the period; otherwise, you could correct the same posting twice.
Tax Rate
Specify the tax rate of the transaction – 16% or 19% – that the wizard uses to select documents.
Code
Tax group code
Name
Tax group name
Display
Deselect the tax group that you do not need in the wizard run.
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
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/12/26, 12:24 PM
Tax %
The tax rate that was effective for the tax code at the time the transaction was posted
Doc. No.
The document number in SAP Business One
Debit, Credit (FC, SC)
The debit or credit tax amount (in terms of foreign currency or system currency)
More Information
Transfer Posting Correction Wizard
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
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/12/26, 12:24 PM
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard - Summary Window
In this window, you can see how many journal entries have been made during the correction process. The number appearing is
twice the number of the corrected transactions because it includes the entries on both the debit and credit sides.
You can view the transactions created by the wizard in the Journal Entry window of the Financials module.
More Information
Transfer Posting Correction Wizard
Folio Number Assignment
Use this function to create legal documents such as invoices and credit memos that include the fiscal document number known as
Folio.
When a company is set up for Chile in Company Details and when printing marketing documents, the settings Obtain Printer
Settings from Default Printing Layout in Document Printing - Selection Criteria and Folio Number Assignment - Selection
Criteria are ignored for the last pages of marketing documents. This ensures that the correct folio number is assigned for
marketing documents during printing and that the folio number of the first page and last page is the same, no matter how many
rows exist in marketing documents.
Documents created with a Folio number have two numbers:
The internal number defined in document numbering (see Administration System Initialization Document
Numbering )
The Folio number that you can define using this function or when you create the document.
 Note
Only documents without folio numbers can be canceled. On the other hand, you cannot assign folio numbers to already
canceled documents and corresponding cancellation documents.
Prerequisites
You have selected the Use Folio Number checkbox on the Basic Initialization tab at Administration System Initialization
Company Details .
More Information
Assigning Folio Numbers
Checking Folio Numbering
Folio Number Assignment - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/12/26, 12:24 PM
Folio Number Assignment: Printed Document Selection
Folio Number Assignment: Folio Number Determination
Assigning Folio Numbers
SAP Business One offers several ways of assigning folio numbers to documents, as described in the table below. If the Folio
Number field is editable in a document, you can take the first and fourth approaches; otherwise, you can take the second, third,
and fourth approaches.
Activities
Activity Procedure
Specifying Folio Number Directly in the Document
1. Display the document to which you want to assign a folio
number.
2. In the header area, enter the folio prefix and number in the
Folio Number field.
3. Choose the Update pushbutton.
Assigning Folio Number for One Document While Printing
1. Display the document to which you want to assign a folio
number.
2. To print the document, choose File Print .
The Print – Document window appears.
3. Select a printer and choose Print.
4. To assign a folio number in the Print – Document window,
choose OK.
If this is the first time you are printing a document of this
type, enter a folio prefix and a number to initialize a series
for this type of document. For example, IN – 000001 for
an A/R invoice. If you have already printed documents of
this type, you can no longer change the folio prefix.
The Folio Number Confirmation window appears, in which
you can confirm the folio number after you have checked
whether your printout was successful. If the printout was
not successful, for example, due to a paper jam, assign a
folio number at a later stage. For more information, see
Assigning Folio Numbers After Documents Are Printed.
5. If the printout was successful, make sure that the number
and prefix are correct and choose OK.
Assigning Folio Number for Many Documents During Printing
1. Choose Sales – A/R Document Printing . Make the
required selection in the Document Printing – Selection
Criteria window and choose OK
2. In the Print Documents window, select the documents you
wish to print and the first folio that will be used. Then
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/12/26, 12:24 PM
Activity Procedure
choose Print.
3. Select the printing format for the documents.
The Folio Number Confirmation – Printed Document
Selection window appears.
4. Select the documents you wish to print and choose Next.
5. The Folio Number Confirmation – Folio Number
Determination window displays the selected documents
and their folio numbers assigned by SAP Business One. Edit
the folio numbers if required and choose Finish.
Assigning Folio Numbers After Documents Are Printed
1. Choose Sales – A/R Folio Number Assignment or
Purchasing – A/P Folio Number Assignment .
2. Make the required selection in the Folio Number
Assignment – Selection Criteria window and choose OK.
The window Folio Number Assignment – Printed
Document Selection appears. This window displays only
documents that have already printed but have no folio
numbers.
3. Select the documents for which you assign folio numbers
and choose Next.
4. The Folio Number Assignment – Folio Number
Determination window displays the selected documents
and their folio numbers assigned by SAP Business One. Edit
the folio numbers if required and choose Finish.
More Information
Document Printing - Selection Criteria
Print Document Window
Folio Number Confirmation: Printed Document Selection
Folio Number Confirmation - Folio Number Determination
Checking Folio Numbering
Prerequisites
Folio numbering has been activated.
Context
You can review which folio numbers have already been used and which numbers are still available.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/12/26, 12:24 PM
Procedure
1. From the SAP Business One Main Menu, choose Administration Utilities Check Folio Numbering .
2. In the Check Folio Numbering window, select the folio numbering range, the date, and the document types you want to
review.
The Document Serial Numbering List window displays the folio numbers per document type that have not been assigned
yet.
Related Information
Folio Number Assignment
Check Folio Numbering
You are enabled to check whether there are duplicated or missing folio numbers for documents created in SAP Business One.
Use the Check Folio Numbering window to define selection criteria for the check. If there are no duplicated or missing folio
numbers, a relevant message appears. If there are missing or duplicated numbers, they are displayed in a separate window.
To display this window, choose Administration Utilities Check Folio Numbering .
Check Folio Numbering Fields
Documents to Review
Select each document type for which you want to run the check.
Folio Number From... To
Define a range of folio numbers to be checked.
Date From... To
Define a range of posting dates to run the check on the documents carrying a posting date within that range.
Select All
Runs the check on all documents with folio numbers.
Clear Selection
Deselects all checkboxes.
Folio Number Assignment - Selection Criteria
Use this window to define the parameters for the documents to which you want to assign folio numbers.
Folio Number Assignment
Document Type
Specify the type of the document to which you want to assign a folio number.
Series
Specify an internal numbering series of the documents to which you want to assign Folio numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/12/26, 12:24 PM
When Batch/Serial No. Exist, Print
Specify what you want to print on the document, when it contains a batch or serial number.
Posting Date From...To
Enter a range of posting dates for the documents to which you want to assign folio numbers.
Internal Number From...To
Enter a range of internal numbers for the documents to which you want to assign folio numbers.
Update Folio
Not selected by default. Documents are selected to update folio numbers.
Select Unprinted Documents
Not selected by default. Only available for selection if Update Folio is selected. When both Update Folio and Select Unprinted
Documents are selected, all (printed and not printed) marketing documents with relevant dates, series, and internal numbers are
displayed in folio number assignment.
More Information
Folio Number Assignment
Folio Number Assignment: Printed Document Selection
This window displays the documents to which folio numbers should be assigned and match the selection criteria you specified.
Printed Document Selection
Selection Column
Select the documents to which you want to assign folio numbers.
Document No., Posting Date, Due Date, BP Code, Total (LC)
General information regarding the documents that match the selection criteria you specified.
More Information
Folio Number Assignment
Folio Number Assignment: Folio Number Determination
This window displays all documents you select in the Folio Number Assignment - Printed Document Selection window.
Folio Number Determination Fields
Document No., Posting Date, Due Date, BP Code, Total (LC)
General information regarding the selected documents. You cannot edit these fields.
Folio Prefix, Folio Number
Enter the Folio Prefix and Folio Number.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/12/26, 12:24 PM
More Information
Folio Number Assignment
Folio Number Confirmation: Folio Number Determination
This window displays all documents selected in the Folio Number Confirmation - Printed Document Selection window, with the
folio numbers assigned to them by SAP Business One.
Change the folio numbers if required.
Folio Number Determination
Document No., Folio Prefix, Folio Number, Posting Date, Value Date, BP Code, Total (LC)
Display general information regarding the selected documents. The values – except for the Folio Prefix and Folio Number – cannot
be edited.
Folio Number Confirmation: Printed Document Selection
This window displays the documents for which folio numbers should be assigned and fit the selection criteria.
Printed Document Selection Fields
Selection Column
Select the documents to which you want to assign folio numbers.
Document No., Posting Date, Value Date, BP Code, Total (LC)
Display general information regarding the documents that fit the selection criteria made by the user.
More Information
Folio Number Assignment
Banking
This section describes the features and functions under the Banking module that are specific to Turkey only.
Information about general features and functions in the Banking module is available in the general online help file provided with
SAP Business One, under Help Documentation Online Help
Postdated Check Deposit
Use this function to transfer to the cash account checks that were deposited as postdated.
To deposit postdated checks, choose Banking Deposits Postdated Check Deposit .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/12/26, 12:24 PM
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
Specify the account code to which the checks should be transferred.
Date
Due date of the checks. This is the current date by default. Change the date if required.
Display Until
Specify a date to display all checks that have reached their value date by this date.
Find Check No.
To trace a specific check, specify its number. SAP Business One marks the required check.
Date, Account Code, Check, Bank, Branch, Acct No., BP/Account Code, BP/Account Name, Check Amount, Incoming Payment
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/12/26, 12:24 PM
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
Context
Follow this procedure to deposit vouchers that were deposited as postdated to the cash account credit card.
Procedure
1. Choose Banking Deposits Postdated Credit Voucher Deposit .
2. In the general area of the window, specify the relevant parameters to display in the table the credit card vouchers to be
deposited.
3. Select the credit card vouchers you want to deposit.
4. If a commission is involved in the deposit, choose next to Total Commissions.
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/12/26, 12:24 PM
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
Date, Acct Code, Doc. No., Card Name, Ref., Payment Method, BP/Account Code, BP/Account Name, # Pymts, of, Total,
Incoming Payment
Information about the postdated credit card vouchers displayed.
Journal Remarks
Add any comments about the deposit.
Trans. No.
Number of the journal entry created by this document and a link to it. The number appears after you have added the document.
Total Commissions
Opens the Commission window where you can enter the amount of commission to be paid for the deposit.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/12/26, 12:24 PM
Reconcile Amounts after Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Credit Vouchers Deposit
Commission Window
Setting Up Bill of Exchange Processing
Context
To activate bill of exchange processing in your company database, follow the steps below:
 Note
You cannot deactivate bill of exchange processing after you have recorded bill of exchange transactions.
Procedure
1. On the Company Details: Basic Initialization tab, select the Use Bill of Exchange checkbox.
2. On the Document Settings: Per Document tab, in the Document field, select Deposit from the dropdown list. Select the Bill
of Exchange Deposit checkbox if you want to split the business partner row in journal entries created by depositing several
bills of exchange in one deposit.
3. On the G/L Account Determination: Sales tab, click next to the Accounts Receivable field to open the Control
Accounts - Accounts Receivable window. Select the default controls accounts for your customers and choose the OK
button
4. On the G/L Account Determination: Purchasing tab, click next to the Accounts Payable field to open the Control
Accounts - Accounts Payable window. Select the default controls accounts for your vendors and choose the OK button
 Note
The control accounts you have defined in the G/L Account Determination window are set as the default for each
new business partner.
Purchasing control accounts should be located in the Liabilities drawer in the Chart of Accounts, and sales
control accounts should be located in the Assets drawer.
Bill of exchange related control accounts function as clearing accounts.
5. In the House Banks Accounts - Setup window, define bill of exchange related parameters.
6. In the Payment Methods - Setup window, define bill of exchange related parameters.
7. In the Business Partner Master Data Window, define bill of exchange related parameters:
On the General tab, in the Agent field, enter the agent code of the business partner. An agent is an employee in your
company who is responsible for bills of exchange (relevant only for Spain and Portugal).
On the Payment Terms tab, enter the bank account details of your business partners.
On the Accounting tab, General tab, click to open the Control Accounts window displaying the default control
accounts. You can change these G/L accounts manually if no journal entry has yet been created with these control
accounts for the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/12/26, 12:24 PM
Results
After you have defined all the necessary settings, you can start processing bills of exchange.
Bill of Exchange Settings
The following fields are relevant for setting up and working with bill if exchange functionality.
Business Partner Master Data Accounting Tab, General
Bill of Exchange Discounted
Specify a G/L account for bill of exchange discounted.
Bill of Exchange on Collection
Specify a G/L account for bill of exchange collection.
Unpaid Bill of Exchange
Specify a G/L account for unpaid bill of exchange.
Bill of Exchange Presentation
Relevant for customers and leads only.
Bank Statement Processing
Working with bank statement processing requires defining internal bank operation codes (as well as additional settings). One of
the related parameters is “Posting Transaction”. The complete information about defining internal bank operation codes in
available in the general online help delivered with SAP Business One. Following bill of exchange specific information related to the
Posting Transaction field in the Internal Bank Operation Codes window.
“Posting Transaction ” is used as one of the criteria to define which transaction should be posted when identified by this internal
code. The specified posting transaction defines the available posting methods for the internal operation code. If the company uses
bills of exchange and a payment means, the following options are available in this field:
Incoming Bill of Exchange
Outgoing Bill of Exchange
They indicate that the internal code refers to transactions resulting either from receiving or from issuing bills of exchange. In both
cases, the applicable posting methods are Bank Interim Account from/to Bank Account and Ignore.
Working with Bills of Exchange
In SAP Business One, your company settings enable use of bills of exchange. A bill of exchange is a means of payment you can use
in incoming and outgoing payments. It is a document addressed by the vendor to the customer requiring the latter to pay a certain
amount on the due date.
A customer buys goods or services and agrees with the vendor that the payment method will be a bill of exchange. On the due
date, the vendor claims payment from the customer or asks the bank to claim it. If the customer pays, the process is completed. If
not, the bank informs the vendor, and the vendor duns the customer.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/12/26, 12:24 PM
The bill of exchange is supported by the payment wizard.
Bills of exchange are reflected in various reports:
Cash Flow
Cash Flow Forecast Dashboard
To access bill of exchange-related functions, choose Banking Bill of Exchange .
More Information
Managing Bills of Exchange
Managing Bills of Exchange
Since paying or collecting bills of exchange is a process which requires several stages, you need to monitor and record the changes
made for each one of your incoming and outgoing bills of exchange.
After you set the required initial definitions, you can start working with the Bill of Exchange function:
You can monitor and record most bill of exchange-related activities in the Bill of Exchange Management window. This
window is designed as a chest of drawers, where each drawer represents a different bill of exchange status. You can take
required actions such as changing the bill of exchange status, defining bank data, setting posting and tax dates, and so on.
To access the Bill of Exchange Management window, choose Banking Bill of Exchange Bill of Exchange
Management . In the Bill of Exchange Management:— Selection Criteria window, specify your selection criteria and
choose the OK button.
Every change you make in one of your bills of exchange is recorded in the Bill of Exchange Transactions window. This
window is displayed automatically as you change a bill of exchange status.
To access the Bill of Exchange Transactions window, choose Banking Bill of Exchange Bill of Exchange Transactions
You can display and print your bills of exchange using the Bill of Exchange - Payables and Bill of Exchange - Receivables
windows. This function is required for sending a bill of exchange to be signed and approved by your customer, prior to you
depositing it in your bank.
To access the Bill of Exchange - Payables window, choose Banking Bill of Exchange Bill of Exchange — Payables
To access the Bill of Exchange - Receivables window, choose Banking Bill of Exchange Bill of Exchange —
Receivables
You can display data and history for each bill of exchange using the Bill of Exchange Register window.
To access the Bill of Exchange Register window, choose Banking Bill of Exchange Bill of Exchange Register .
Bill of Exchange Management: Selection Window
The following are the fields in the selection window of the Bill of Exchange Management function.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/12/26, 12:24 PM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Management: Selection Window
Doc. Type
Specify whether to display bills of exchange created from incoming or outgoing payments.
Status
Specify a specific status to display only bills of exchange to which the selected status has been assigned.
Bill of Exchange No. From...To...
Specify a bills of exchange range according to their number.
Due Date From...To...
Specify a bills of exchange range according to their due date.
Reference No. From...To...
Specify a bills of exchange range according to their reference number.
Payment No. From.. To...
Specify a bills of exchange range according to the number of the payment documents linked to them.
Payment Posting Date From...To...
Specify a bills of exchange range according to the posing date of their linked payments.
BP Bank Code From... To...
Define the range of bills of exchange according to the bank code of their linked business partners. This field is displayed only when
the status Generated is selected.
Deposit No. From...To
Specify a bills of exchange range according to the numbers of their linked deposit documents. Only available with the status
Deposited or Paid.
Deposit Bank Acct No. From...To...
Specify range of bank account numbers to display only bills of exchange deposited to these accounts.
Deposit Type
Select to display bills of exchange according to their deposit type. Only available with the status Deposited or Paid.
Reconciled Only
Select to display only bills of exchange that are reconciled. Only available with the status Deposited or Paid.
Add Tolerance Days
Takes into account both the tolerance days defined in the House Bank Accounts – Definitions window and the defined value date
range. Only available with the status Deposited or Paid.
Payment Methods
All payment methods whose payment means are defined as bill of exchange. Select the payment methods to include in the Bill of
Exchange Management window.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/12/26, 12:24 PM
More Information
Bill of Exchange Management
Bill of Exchange Management Window
The following are the fields in the Bill of Exchange Management window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management . Set the required parameters in the
selection window and choose OK.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Management Window
Sent, Generated, Deposited, Paid, Cancelled, Failed
Represents the statuses a bill of exchange can have:
When you select Incoming Payment as document type in the selection criteria, all the drawers appear.
When you select Outgoing Payment, only the following drawers appear:
Generated
Paid
Cancelled
Find Bill of Exchange No.
Specify a number to locate a bill of exchange by it.
Status
Groups the bills of exchange according to the statuses assigned to them. Only available if you selected the status All in the
selection criteria window.
Selection Column
Select the bills of exchange you want to process. Only available with one of the following statuses/drawers:
Sent
Generated
Deposited
Paid.
Due Date
Due date of the bill of exchange.
Posting Date
Posting date of the incoming/outgoing payment document.
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/12/26, 12:24 PM
Bill of Exchange Total (LC)
Total amount paid by the bill of exchange - in local currency.
Remarks
Remarks as specified in the bill of exchange.
Reference No.
Reference number assigned to the bill of exchange in the Payment Means window.
Expand, Collapse
Expands or collapses the entire display of the window. Only available if you selected the status All in the selection criteria window.
Move To
Only available with the statuses/drawers, Sent, Generated, Deposited, and Paid. Specify how to process the selected bills of
exchange. The options available depend on the selected drawer:
Drawer - Sent:
Generated transfers the bill of exchange to the Generated drawer.
Cancelled cancels the bill of exchange and transfers it to the Cancelled drawer.
Drawer - Generated:
Deposited creates deposit documents for bills of exchange created from incoming payments.
Paid indicates that the amounts in the bills of exchange created from outgoing payments were transferred from
your account to the vendor’s account.
Cancelled cancels the bill of exchange and transfers it to the Cancelled drawer.
Drawer - Deposited:
Paid transfers the bills of exchange to the Paid drawer. Shows that the bill of exchange amount was transferred to
your bank account.
Generated cancels the deposit and transfers bills of exchange back to the Generated drawer.
 Note
You can only transfer back bills of exchange that have not been reconciled.
Drawer - Paid:
Deposited transfers the bills of exchange to the Deposit drawer. Cancels the indication that the bill of exchange
amounts were received at your bank account. Available only for incoming payments.
Failed cancels the incoming payment and transfers the bills of exchange to the Failed drawer.
Generated reverses the payment transaction and transfers the bills of exchange created by outgoing payments
back to the Generated drawer.
Posting Date, Document Date
By default, the current date. Available only with the drawers Sent, Generated, Deposited or Paid.
House Bank Country/Region, House Bank, House Bank Account, House Bank Branch
Only available when the Generated drawer is selected for incoming payments.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/12/26, 12:24 PM
Choose to open the Choose Bank window, in which you select the bank account for the bill of exchange transaction. The details
of the selected bank account are then displayed in the respective house bank fields.
Collection
Indicates that the bank collects the bill of exchange on its due date. Available only when the Generated drawer is selected for
incoming payments.
Discounted
Creates the deposit before the due date of the bill of exchange. Available only when the Generated drawer is selected for incoming
payments.
Norm
Specify the deposit norm number, which will be displayed in the OPEX file. Available only when the Generated drawer is selected
for incoming payments.
More Information
Bill of Exchange Management
Deposited - Details
Use this window to view additional details of selected deposited bills of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management Bill of Exchange Management ,
select and double-click the table row labeled Deposited.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Bank
Code, Name, Account Number, Branch, Control Key, Country/Region
Displays details of bank account in which bill of exchange was deposited.
Deposit
Type
Displays the type of deposit:
Collection – when the bank collects the Bill of Exchange on its due date.
Discounted – when you make an advanced deposit, that is, if you make a deposit before the due date of the bill of exchange.
Number
Displays deposit number from the Deposit window, general area.
Bill of Exchange
Number
Displays bill of exchange number from the Bill of Exchange — Receivables window.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/12/26, 12:24 PM
Due Date
Displays bill of exchange due date from the Bill of Exchange — Receivables window.
Amount
Displays amount of the selected bill of exchange.
More Information
Bill of Exchange - Receivables
Bill of Exchange Transactions
This window appears each time you record transactions in the Bill of Exchange Management window. It displays the details
concerning the transactions you have just recorded.
To open the window, choose Banking Bill of Exchange Bill of Exchange Transactions .
More Information
Bill of Exchange Transactions Window
Bill of Exchange Transactions Window
Use this window to display information about transactions comprising the bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange Transactions .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Transactions Window
Transaction Number
Number of this transaction. Begins at 1 and runs sequentially.
Journal Entry No.
Number of the journal entry created by the transaction. A link to the journal entry is available for the following transactions:
Changing status from Generated to Deposited
Reconciliation
Changing status from Deposited to Paid
Changing status from Paid to Deposited
Status Changed From...To...
Previous and current status of the bill of exchange.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/12/26, 12:24 PM
User Name
User who recorded the transaction.
Action
Action performed on the bill of exchange: status change or reconciliation.
Reference No.
Reference for the bill of exchange.
Due Date
Due date of the bill of exchange.
Posting Date
Posting date of the payment document.
Document Date
Document date for tax purposes.
Bill of Exchange Total
Total amount of the bill of exchange.
BP Bank Country/Region, BP Bank Code, BP Bank Name, BP Bank Account, BP Bank Branch
Bank details of the business partner linked to the bill of exchange.
BP Bank Control Key
Control key defined for the business partner’s bank account.
Remarks
Remarks for the bill of exchange.
Payment Method Code, Payment Method Description
Code and description of the payment method linked to the bill of exchange.
More Information
Bill of Exchange Transactions
Bill of Exchange - Receivables
When you create an incoming payment with bill of exchange as the payment means, a bill of exchange record is created. Use the
Bill of Exchange - Receivables window to view these records.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables .
More Information
Bill of Exchange – Receivables Window
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/12/26, 12:24 PM
Bill of Exchange - Receivables Window
This window provides receivables information pertaining to a bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange – Receivables Window
Received from
Code and name of the customer who sent the bill of exchange.
Address
Pay to address specified in the Incoming Payment document.
Number
Number of the bill of exchange.
Reference
Reference for the bill of exchange and a link to the relevant incoming payment document.
Status
Current status of this bill of exchange.
Signature
User code of the person who recorded the bill of exchange.
Bill of Exchange - History
Opens the Bill of Exchange – History window with the historical statuses of the current bill of exchange and a link to each
transaction.
Remarks
Remarks in the A/R invoices paid by this bill of exchange (assuming the payment was based on an A/R invoice).
Total, Amount in Words
Total amount paid in this bill of exchange, the figure and in words.
Bank Account
Customer’s bank details linked to the bill of exchange.
Journal Remarks
Specify any comments regarding the journal entry posted by this bill of exchange.
More Information
Bill of Exchange - Receivables
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/12/26, 12:24 PM
Bill of Exchange - History
Use this window to view historical transactions of each bill of exchange receivables/payables.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables/Payables . Display the required bill
of exchange. Choose Bill of Exchange – History.
More Information
Bill of Exchange - History Window
Bill of Exchange - History Window
The following are the fields in the Bill of Exchange – History window.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables/Payables . Display the required bill
of exchange. Choose Bill of Exchange – History.
Bill of Exchange – History Window
Bill of Exchange No.
Number of the bill of exchange for which the transaction history is provided.
Reference No.
Reference assigned to the bill of exchange in the Payment Means window.
Transaction No.
Sequential number of the transaction. For a detailed view, choose .
Changed to Status
Status of the bill of exchange after the transaction was performed.
Date
Creation date of the transaction.
More Information
Bill of Exchange - History
Bill of Exchange - Payables
When you create an outgoing payment with bill of exchange as the payment means, a bill of exchange record is created. Use the
Bill of Exchange – Payables window to view these records.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Payables .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/12/26, 12:24 PM
Bill of Exchange – Payables Window
Bill of Exchange - Payables Window
This window provides payables information pertaining to a bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Payables .
Bill of Exchange – Payables Window
To Order of
Code and name of the vendor who received the bill of exchange.
Address
Address specified in the Pay to field in the Outgoing Payment.
Number
Number of the bill of exchange.
Reference
Reference for the bill of exchange and a link to the outgoing payment document.
Posting Date
Posting date of the bill of exchange.
Due Date
Due date of the bill of exchange.
Status
Current status of this bill of exchange.
Signature
User code of the person who recorded the bill of exchange.
Bill of Exchange - History
Opens the Bill of Exchange – History window, with all the historical statuses of the current bill of exchange and a link to each
transaction.
Remarks
Remarks entered in the incoming payment document.
 Example
Invoice number.
Total
Amount paid in this bill of exchange.
Amount in Words
Amount paid in this bill of exchange – in words.
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/12/26, 12:24 PM
Country/Region, Bank, Account, Branch, Control Key
Details of the house bank linked to the bill of exchange.
Journal Remarks
Specify any comments regarding the journal entry posted by this bill of exchange.
More Information
Bill of Exchange - Payables
Bill of Exchange Register
SAP Business One uses the bill of exchange register to store information about all bills of exchange received and issued by the
company. The register reflects the current status of every bill of exchange and provides information regarding status history.
To access the bill of exchange register, choose Banking Incoming Payments Bill of Exchange Bill of Exchange Register
.
More Information
Bill of Exchange Register - Selection Criteria
Bill of Exchange Register Window
Bill of Exchange Register - Selection Criteria
The following are the fields in the Bill of Exchange Register – Selection Criteria window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Register .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Doc. Type
Select the bill of exchange type to display.
Status From...To...
Specify a range of statuses for the bills of exchange. The statuses available depend on the type of document selected:
With incoming payments: Sent, Generated, Deposited, Paid, Cancelled and Failed
With outgoing payments: Generated, Paid, Cancelled
Bill of Exchange No. From...To...
Specify a bills of exchange range according to their sequential numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/12/26, 12:24 PM
Due Date From...To...
Specify a bills of exchange range according to their value dates.
Reference No. From...To...
Specify a bills of exchange range according to their reference numbers.
Payment No. From...To...
Specify a payment documents range for which you want to display the related bills of exchange.
Payment Posting Date From...To...
Specify a bills of exchange range according to the posting dates of the payment documents.
Deposit No. From...To...
Specify a bills of exchange range according to their deposit numbers.
Deposit Type
Specify to display bills of exchange according to their deposit type.
Reconciled Only
Displays only reconciled bills of exchange.
Payment Method
To display bills of exchange linked to specific payment methods, select the relevant payment methods.
More Information
Bill of Exchange Register
Bill of Exchange Register Window
Bill of Exchange Register Window
The following are the fields in the Bill of Exchange Register window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Register . Specify the required parameters in the
Bill of Exchange Register – Selection Criteria window and choose OK.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Register Window
Number
Enter the number of a bill of exchange to view the details about this bill of exchange.
Currency
To display bills of exchange created for a specific currency, specify the relevant currency.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/12/26, 12:24 PM
Status
To display only bills of exchange with a specific status, specify the relevant status.
Reference No.
Reference number of the bill of exchange.
Date
Due date of the bill of exchange.
Bank, Branch, Account No.
Bank details for the bill of exchange (house bank for outgoing payments, customer bank for incoming payments).
Status
Current status of the bill of exchange.
Amount
Amount of the bill of exchange.
Deposit
Details of the deposit, if the selected bill of exchange was deposited.
Deposit No. – number assigned to the deposit.
Deposit Date – deposit date.
G/L Account/BP Code – G/L account code or business partner code to which the bill of exchange was deposited.
Bank Country/Region, Bank, Branch, Account No. – information about the customer’s bank.
Payment
Details of the incoming/outgoing payment document linked to the selected bill of exchange:
Incoming/Outgoing Payment No. – number of the payment document.
Date – posting date of the document.
Customer/Vendor Code – code of the customer/vendor for which the payment was created.
Bill of Exchange Status
Displays the status history of the selected bill of exchange (one row for each status):
Bill of Exchange Trans. No. – number of the bill of exchange transaction and a link to it.
Bill of Exchange Status – status to which the bill of exchange was changed.
Date – date of the transaction.
More Information
Bill of Exchange Register
Bill of Exchange Register – Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/12/26, 12:24 PM
Canceling a Bill of Exchange
You can cancel a bill of exchange that was received as an incoming payment but has not yet been deposited, or has been deposited
as postdated. To view the status of a bill of exchange, select the bill of exchange in the Bill of Exchange Register window, and view
the Status field.
Process
In the Bill of Exchange Management window, select the checkbox in the table row of the bill of exchange that you want to cancel,
then in the Move To dropdown list, select Canceled.
Result
The bill of exchange is transferred to the Canceled drawer in the Bill of Exchange Management window.
The incoming payment is canceled.
The A/R Invoice can be paid by other payment means.
A reverse journal entry is recorded.
Deposit: Bill of Exchange Tab
The Bill of Exchange tab in the Deposit window is available for deposit documents created for bills of exchange using the Bill of
Exchange Management window.
To view details on deposited bills of exchange, choose Banking Deposits Deposit . Then, select a deposit created for a bill of
exchange.
Deposit: Bill of Exchange Fields
Norm
Norm number of the deposit as defined in the Generated drawer in the Bill of Exchange Management window.
Collection/Discounted
Selection made in the Generated drawer in the Bill of Exchange Management window.
Due Date, Bill of Exchange, Bank, Branch, Account No., Customer Code, Amount
Information about the deposited bills of exchange. The total amount of the deposited bills of exchange is displayed in the row
below the table.
Payment Means: Bill of Exchange Tab
To access the Bill of Exchange tab in the Payment Means window, choose Banking Incoming Payments Incoming
Payments . Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment,
choose . In the Payment Means window, choose the Bill of Exchange tab.
Payment Means: Bill of Exchange Tab Fields
Bill of Exchange Accounts Receivables
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/12/26, 12:24 PM
Account debited when the incoming payment is added. This account is defined in Administration Setup Financials G/L
Account Determination Sales General Accounts Receivable Control Accounts - Accounts Receivable .
Bill of Exchange Accounts Payable
Account credited when the outgoing payment is added. This account is defined in Administration Setup Financials G/L
Account Determination Purchase General Accounts Payable Control Accounts - Accounts Receivable .
Bill of Exchange No.
For incoming payment documents:
Unique number of the incoming payment, which can be changed if required. Two bills of exchange cannot be assigned to the same
number.
Bill of Exchange No. (op)
For outgoing payment documents:
Unique number of the outgoing payment, which can be changed if required. Two bills of exchange cannot be assigned to the same
number.
Bill of Exchange Due Date
For incoming payment documents:
Specify the date on which the bill of exchange is due.
If the payment is based on one or more A/R invoices with the same due date, the default due date is the due date of the
A/R invoice(s).
If the payment is based on several A/R invoices with different due dates, enter a due date manually.
 Note
After the bill of exchange is recorded, you can still change its due date. The updated due date will appear in the following places:
Due Date column in the table area of the corresponding journal entry
Due Date field in the general area of the payment
Due Date column for this bill of exchange in the Bill of Exchange Management window
Due Date column for this bill of exchange in the Cash Flow window
Bill of Exchange Due Date
For outgoing payment documents:
Specify the date on which the bill of exchange is due.
If the payment is based on one or more A/P invoices with the same due date, the default due date is the due date of the
A/P invoice(s).
If the payment is based on several A/P invoices with different due dates, enter a due date manually.
 Note
After the bill of exchange is recorded, you can still change its due date. The updated due date will appear in the following places:
Due Date column in the table area of the corresponding journal entry
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/12/26, 12:24 PM
Due Date field in the general area of the payment
Due Date column for this bill of exchange in the Bill of Exchange Management window
Due Date column for this bill of exchange in the Cash Flow window
Reference
For incoming payment documents:
If the customer created the bill of exchange, specify its number here.
Reference (op)
For outgoing payment documents:
If the vendor creates the bill of exchange, specify its number here.
Payment Method
Specify the required payment method for the bill of exchange.
Status
When you choose the payment method, the status changes to Generated. This means that a journal entry for the payment will be
recorded and the invoice will be considered as paid (closed).
Reference 2
If another reference number exists, specify it here.
Remarks
Enter any remarks here.
BP Bank Data
Business partner bank details for the selected method of payment, showing the bank account to be credited at the end of the
process. You can change this bank account.
Total
Total amount paid in this bill of exchange.
Tax Reports: Central MENA/AE/EG/LB/OM/QA/SA
Following is information about tax reports required in Central MENA /AE/EG/LB/OM/QA/SA and additional information related to
tax handling in SAP Business One:
Tax Report
Withholding Tax Report
Tax Reconciliation Report
Tax Declaration Box Report
Business Activity Statement Reporting
Tax Report
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/12/26, 12:24 PM
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
Round Amount
Rounds the total amounts calculated in the report.
Series
Generates the report for documents created according to specific numbering series. After selecting, choose the ... button to open
the Series – Filter window in which you can define the required numbering series.
Transact.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/12/26, 12:24 PM
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
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Only includes in the report documents with an externally calculated tax amount on at least one row.
 Note
If you select this checkbox, the Externally Calculated Tax field is displayed in the tax report window.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/12/26, 12:24 PM
Update/ OK
When you change the preferences in the Tax Report – Selection Criteria window, the OK option changes to the Update mode.
Choose Update to save the report under the name you entered in the Report Name field.
The preferences chosen for the report are saved.
Tax Report Window
This window displays the tax report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report Window: Europe
Tax Code
Displays the tax code.
Choose to display a list of transactions involving this tax code.
EU
Indicates whether the tax group is used for transactions with other European Union countries, as defined in the EU field of the
Define Tax Groups window. Relevant only for output tax groups.
Tax %
Displays the tax rate of the tax group as a percentage.
Posting Date
Displays the posting date of the documents included in the report. Appears in expanded display only.
Document Date
Displays the document date defined for the document or transaction.
Base Amount
Total amount of the document, excluding tax; serves as the base value for the tax calculation.
Tax Amount
Tax amount calculated for the tax group: Total Tax field minus Non-Deductible field.
Total Tax
Displays the total amount of tax.
Non-Deductible
The tax amount that cannot be deducted.
Vendor Ref. No.
Displays the vendor’s reference number as recorded in the A/P invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/12/26, 12:24 PM
Tax Report
Withholding Tax Report
This report displays the withholding tax amounts collected and paid during specific periods.
 Note
If a payment on account with withholding tax has been fully reconciled (that is, the reconciled amount equals the payment
amount), the withholding tax report does not include the payment information.
 Note
When you print the report, you can print the selection criteria on a separate page.
More Information
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner
Vendor Mode – Detailed Format Window
Withholding Tax Report by WTax Code
Withholding Tax Report - Selection Criteria
Use this window to specify selection criteria for the Withholding Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Withholding Tax Report. Alternatively,
open it from the Reports module.
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
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/12/26, 12:24 PM
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
Vendor Mode - Detailed Format Window
Withholding Tax Table
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
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/12/26, 12:24 PM
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
Withholding Tax Table
Withholding Tax Table
This window appears when you create a document related to withholding tax-liable business partners. The window displays the
default ITW and VATW codes.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
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
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/12/26, 12:24 PM
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
Tax Reconciliation Report
This report enables you to track the tax amounts that were posted in sales and purchasing documents and in manual transactions.
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
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/12/26, 12:24 PM
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
If the specified From date falls into the effective period range of a tax declaration box group, all the tax declaration boxes within
this group are automatically displayed in the Tax Declaration Boxes table. For more information about the effective period of a tax
declaration box group, see the Effective From field in Tax Declaration Boxes - Setup window.
Round Amount
Report rounds off its displayed amounts.
Tax Declaration Boxes
This table displays the tax declaration boxes according to the specified From date. It includes the following columns:
Code – displays the code of the box
Name – displays the name of the box
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
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/12/26, 12:24 PM
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
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/12/26, 12:24 PM
Prerequisites
Initializing the BAS Reporting Function
To initialize the BAS reporting function, you have done the following:
1. You have selected the Extended Tax Reporting checkbox in Administration System Initialization Company Details
Accounting Data .
2. You have defined the period type for BAS reporting at the same location.
More Information
Defining BAS Codes
Generating BAS Reports
Retrieving BAS Reports and Saving Report Data
Generating BAS Reports
Procedure
1. Choose Financials Financial Reports Accounting Tax BAS Report Generation .
The BAS Report Generation - Selection Criteria window appears.
2. Specify the tax declaration type:
Original: To save the report for the first time in a given period.
Replacement: To correct a report that has already been saved.
Adjusted: To show only documents that have not yet been included in any previous report for a given period.
3. Specify the tax declaration name by selecting the appropriate year and period. For a replacement declaration, also select
the desired adjustment number.
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
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/12/26, 12:24 PM
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
4. To export the values to Microsoft Excel, choose File Export MS-EXCEL . You can then open the file in Microsoft
Excel, fill in the electronic or paper form of the business activity statement and submit it to the tax authorities.
Related Information
Business Activity Statement Reporting
Generating BAS Reports
This is custom documentation. For more information, please visit SAP Help Portal. 70