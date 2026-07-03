6/8/26, 6:21 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:21:01 GMT+0000
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

6/8/26, 6:21 AM
FAQs
General
How can I restore icons to the toolbar?
When trying to connect a base document to a target document, the List of Base Documents window does not contain the
required base document, although it appears in the Open Items List report. What could be the reason?
How can I simultaneously close all the open SAP Business One windows?
How can I verify which version of SAP Business One I am using?
The Main Menu window disappeared. How can I restore it?
How can I use the F keys to create keyboard shortcuts for SAP Business One functions?
How do I find information about a specific field in SAP Business One?
Printing
When printing SAP Business One documents, the text Printed by SAP Business One appears in the document
footer. Is it possible to prevent it from being printed?
When I add an SAP Business One document, it is automatically printed, although the option Print Document is deselected
in Administration System Initialization Print Preferences Per Document When Adding Document section.
What is the reason?
In printed documents, the country/region name appears abbreviated, for example, GB instead of United Kingdom. How can
I have the full name printed?
Master Data
Is it possible to remove a customer master data record of a business partner?
Is it possible to remove an item master data record?
How do I cancel an item record if it is not possible to remove it?
Financials
Is it possible to replace the chart of accounts template defined for a company?
Why do journal entries that were created with the conversion differences function not include values in local currency?
The chart of accounts contains accounts colored in green. What is special about these accounts?
Is it possible to change the currency defined for G/L Account or Business Partner after journal entries have been posted?
Why is the Inventory tab in the G/L Account Determination window disabled?
How do I type the special symbols of the Euro and British Pound currencies?
Banking
How do I correct a wrong due date of a check after the incoming payment has been added?
General
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:21 AM
How can I restore icons to the toolbar?
1. Right-click an empty area in the toolbar to display a menu that lists the different groups of icons available.
2. Select the relevant group to place its icons on the toolbar.
When trying to connect a base document to a target document, the List of Base Documents window does not contain
the required base document, although it appears in the Open Items List report. What could be the reason?
The type (item/service) of the target document must be identical to the type of the base document. Change the type of the target
document, and open the list of base documents again.
How can I simultaneously close all the open SAP Business One windows?
In the Window menu of the menu bar, choose Close All.
How can I verify which version of SAP Business One I am using?
In the Help menu of the menu bar, choose About.
The Main Menu window disappeared. How can I restore it?
In the Window menu of the menu bar, choose the Main Menu option or press CTRL + 0 .
How can I use the F keys to create keyboard shortcuts for SAP Business One functions?
1. In the Tools menu of the menu bar, choose My shortcuts Customize .
2. In the Customize window, choose Keyboard.
3. In the Customize Keyboard window, you can allocate a specific function to each F key.
How do I find information about a specific field in SAP Business One?
Right-click the required field and choose the option What's This?.
Printing
When printing SAP Business One documents, the text Printed by SAP Business One appears in the document
footer. Is it possible to prevent it from being printed?
Yes. Choose Administration System Initialization Print Preferences General tab, and deselect Print Sap Business One
Generation Message.
When I add an SAP Business One document, it is automatically printed, although the option Print Document is
deselected in Administration System Initialization Print Preferences Per Document When Adding Document
section. What is the reason?
User defaults have been defined for that user, and the option Print Document is selected in Administration Setup General
Users Defaults field (Link to User Defaults) Print tab Add button will also....
In printed documents, the country/region name appears abbreviated, for example, GB instead of United Kingdom.
How can I have the full name printed?
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:21 AM
In Administration Setup Business Partners Address Formats , select the option Description for the Country/Region
component.
Master Data
Is it possible to remove a customer master data record of a business partner?
Yes, as long as no accounting or inventory transactions have been posted to this customer.
Is it possible to remove an item master data record?
Yes, if this item has no related inventory transactions.
How do I cancel an item record if it is not possible to remove it?
Display the required item master data, and choose Data Cancel . The item will not appear in the inventory reports and will not
be available for selection in marketing documents. To reactivate, display the item and choose Data Restore .
Financials
Is it possible to replace the chart of accounts template defined for a company?
You can specify a different chart of accounts template on condition that:
No transactions have been posted to the database
No new G/L accounts have been added
Why do journal entries that were created with the conversion differences function not include values in local
currency?
Journal entries resulting from conversion differences reflect the difference between the system currency rate on the posting date
of a journal entry and on the date the conversion differences are performed. The system currency balance of the G/L
account/business partner is updated accordingly.
Local currency values are not relevant for this comparison. Therefore, the journal entries created with the conversion differences
function do not include values in local currency.
The chart of accounts contains accounts colored in green. What is special about these accounts?
The green accounts are the default accounts to which the different accounting transactions performed in SAP Business One are
posted. These accounts are defined in Administration Setup Financials G/L Account Determination .
Is it possible to change the currency defined for G/L Account or Business Partner after journal entries have been
posted?
If the currency defined for this G/L account or business partner is either the local currency or a specific foreign currency, it is
possible to change it to All Currencies. If the originally specified currency is All Currencies, it is not possible to change it.
Why is the Inventory tab in the G/L Account Determination window disabled?
This tab is active only in companies that run a perpetual inventory accounting system (the option Default Valuation Method is
selected in Administration System Initialization Company Details Basic Initialization tab).
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:21 AM
How do I type the special symbols of the Euro and British Pound currencies?
| Currency         |     | Key Combination |               |     |
| ---------------- | --- | --------------- | ------------- | --- |
| Euro: €          |     | Alt  +  0  +    | 1  +  2  +  8 |     |
| British Pound: £ |     | Alt  +  0  +    | 1  +  6  +  3 |     |
Banking
How do I correct a wrong due date of a check after the incoming payment has been added?
Correction is possible only if the check has not yet been deposited, or was deposited as postdated.
| 1. Choose  | Banking  |  Incoming Payments  |  Check Register | .   |
| ---------- | -------- | ------------------- | --------------- | --- |
2. Display the required check.
3. Change its due date in the field Date.
This is custom documentation. For more information, please visit SAP Help Portal. 5