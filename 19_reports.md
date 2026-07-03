6/8/26, 6:12 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:12:31 GMT+0000
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

6/8/26, 6:12 AM
Reports
SAP Business One contains an integrated and extensive Reports module that includes reports from the following modules. In the
interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Please note that image maps are not interactive in PDF outputs.
You can compile reports in almost any configuration to match the needs of your business.
SAP Business One contains many predefined reports that you can analyze in various ways by using the selection and sort
functions. Navigating in a report enables you to quickly access the underlying detailed information that it contains.
You can also export all reports to Microsoft Excel and some to a Microsoft Word document. This capability gives you access to data
from outside of SAP Business One.
More Information
For more information about working with the Crystal Reports software, version for the SAP Business One application, see the how-
to guide, which you can download from SAP Help Portal
Financial Reports
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:12 AM
This menu option includes all reports pertaining to the analysis of the financial and accounting activities of the company. The
reports comprise the following main categories:
Financial
Accounting
Comparison
Budget Setup
Related Information
Financial
Accounting
Comparison
Budgets
Generating Electronic Reports
Use Electronic Reports to generate reports with electronic formats.
Prerequisites
You have set up the electronic file formats using the electronic file manager.
Procedure
Based on the definition of Module in the Electronic File Manager: Format Definition add-on, the available electronic formats are
listed in Electronic Reports, under the reports menu entry of the specific SAP Business One module.
1. From the SAP Business One Main Menu, choose module module Reports Electronic Report the specific electronic
report . Alternatively, choose it from the Reports module.
The report wizard appears. The number of steps in the wizard depends on the parameters to be configured for the specific
report.
In each step, choose the appropriate button, as follows:
Next: proceed to the next step
Back: return to the previous step
Cancel: quit the process
Preview: preview the report based on the parameters that you have specified
2. In step 1 and up to the Save Option step, specify the parameters required by the Electronic Format Manager: Format
Definition for this report.
3. In the Save Option step, specify the destination file path for the generated electronic report.
4. In the Result Summary step, do the following:
To view the system log, choose the View Log button.
To open the generated electronic report, click the hyperlink.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:12 AM
To close the wizard, choose the Finish button.
More Information
For more information about defining electronic formats, see the online help for the Electronic File Manager: Format Definition
add-on after installing it.
Accounting
The Accounting Reports folder contains:
Reports that provide an overview of the objects and data in your accounts
Tax reports that you must submit to the tax authorities
To access these reports, choose Financials Financial Reports Accounting . Alternatively, access them from the Reports
module.
G/L Accounts and Business Partners
This report enables you to generate a list of G/L accounts and/or business partners. Use this window to specify selection criteria
for the report.
To access the report, choose Financials Financial Reports Accounting G/L Accounts and Business Partners .
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
BP
Displays business partners in the report.
 Note
When not selected, other options pertaining to business partner selection criteria are not available.
Display Leads
Report includes business partners defined as leads.
Customer Group, Vendor Group
Specify the group from which to display business partners.
 Example
To display only customers, choose None in the Vendor Group field.
Properties
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:12 AM
Opens the Properties window where you select the required properties. Your choices appear in the adjoining field.
G/L Accounts
Includes G/L accounts in the report.
 Note
When not selected, options related to G/L account selection criteria are not available.
Find
Opens the Find G/L Accounts window in which you select the G/L accounts to be included in the report. For more information, see
the online help topic Finding G/L Accounts to Include in Financial Reports/Period-End Closing.
[Level]
Select the level of the accounts to display in the table. Selecting Level 1 displays the account titles on the highest level.
 Note
A selected row includes all accounts appearing under the title.
X, Account
Indicates accounts selected to appear in the report.
Clear the X from a row to deselect the account.
Click the X in the column header to select or clear all accounts or selections, respectively, in the table.
Related Information
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
Properties
G/L Accounts and Business Partners Window
This window displays the G/L Accounts and Business Partners report according to your defined selection criteria.
G/L Accounts and Business Partners Window
G/L Accounts
Displays only the list of G/L accounts.
BP
Displays the list of business partners.
G/L Accounts/BP
Displays the name, number, and group for each account in a combined list of G/L accounts and business partners.
Display Currency
Specify whether to display the balance in the local currency, system currency, or respective account foreign currency.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:12 AM
General Ledger
This report enables you to generate a list of journal entries posted to the company database according to various criteria. Use this
window to specify selection criteria for the report.
To open the window, choose Financials Financial Reports Accounting General Ledger . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the General Ledger window (For more information, see the topic General Ledger
Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Selection Criteria Name
You can save a specific set of selection criteria and generate the report accordingly whenever required. To do so press CTRL +
A , enter a meaningful name, and set all the required selection criteria for the report. Choose Save. To generate a report based on
a saved selection criteria set, click the icon. The List of Reports - Selection Criteria window appears. Highlight the required
selection criteria set from the list, and choose the Choose button. The selected selection criteria set is populated. To generate the
report, choose OK.
Business Partner
Displays business partners in the report.
 Note
If not selected, other fields pertaining to business partner selection criteria are not displayed.
Customer Group, Vendor Group
Enables you to include business partners from a specific group, divided between customers and vendors.
 Note
To display only customers, choose None in the Vendor Group field.
Properties
Opens the Properties window, where you select the required properties. Your choices appear in the adjoining field.
G/L Accounts
Includes G/L accounts in the report.
 Note
If not selected, other fields related to G/L account selection criteria are not displayed.
Find
Opens the G/L Accounts window, where you specify G/L accounts for the report.
Level
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:12 AM
Select the level of the accounts displayed in the table.
Selecting Level 1 displays the account titles on the highest level.
 Note
A selected row includes all accounts appearing under the title.
Level
Indicates accounts selected to appear in the report.
To deselect an account, clear the X from its row.
To select/clear all accounts/selections in the table, click the X in the column header.
Posting Date From...To..., Due Date From...To..., Document Date From...To...
Specify the date type by which to define the transaction range for the report.
You can:
Use more than one date range
Specify a specific financial period
Expanded
Opens the Expanded Selection Criteria window, where you define additional parameters for the transactions to be included in the
general ledger report.
Print Each Account on Sep. Page
Prints the transactions related to each account on a separate page. Otherwise, the transactions are printed successively.
Print Directly to Printer
Prints the report without displaying it on the screen.
Order Acct By Chart of Accounts
Report displays accounts in the same order as in the Chart of Accounts window.
Ignore Adjustments
Report excludes transactions with Adj. Trans. (Period 13) selected.
Foreign Names
The report displays the foreign names defined for business partners and accounts.
Summarize Control Accounts
Select the checkbox to summarize the transactions posted to the control accounts in the report.
Hide Zero Value LC Rows
Select this checkbox to hide any transaction row which has a zero posting amount in the local currency.
Display Postings Summary
Includes a summary of the postings displayed in the bottom line of the report.
Opening Balance for Period
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:12 AM
Select this checkbox to display the opening balance of the selected BP and G/L accounts, as accumulated in the time range from
the following option date to the start date specified in the Selection options:
OB from Start of Company Activity – displays the opening balance accumulated after company activity started.
OB from Start of Fiscal Year – displays the opening balance accumulated after the start of the fiscal year specified in the
Selection options.
 Example
You have selected the OB from Start of Fiscal Year radio button.
The posting date range defined in the Selection option is 01/04/2005–31/03/2006, and the posting periods defined for the
company are four quarters per calendar year.
The date to be considered as "Start of Fiscal Year" is then 01/01/2005 .
The opening balance display is then the accumulated balance from 01/01/2005 to 01/04/2005.
 Caution
The calculation of the opening balance is influenced by the date range defined for the report. If you specify more than one date
range, SAP Business One calculates opening balance as follows:
If Posting Date is one of the selected options, all transactions with posting date earlier than the date defined in the Posting
Date From field are included.
If Posting Date is not one of the selected options, all transactions with document date earlier than the date defined in the
Document Date From field are included.
Display
Choose the transactions to display in the report:
All Postings – Displays all transactions posted to the selected BP and G/L accounts.
Not Fully Reconciled – Displays transactions posted to the selected BP and G/L accounts that are either partially
reconciled or not reconciled.
You can internally reconcile the BP or G/L accounts in the BP Internal Reconciliation - Selection Criteria or G/L Internal
Reconciliation - Selection Criteria window.
Fully Reconciled Only – Displays only the transactions posted to the selected BP and G/L accounts that are fully
reconciled.
Unreconciled Externally – Displays transactions posted to the selected BP and G/L accounts that are not reconciled with
any external account statement.
You can externally reconcile the BP or G/L accounts in the External Reconciliation - Selection Criteria window.
Reconciled Externally – Displays transactions posted to the selected BP and G/L accounts that are reconciled with
external account statements.
Consider Reconciliation Date
 Note
This field is available only if you select All Postings, Not Fully Reconciled, or Fully Reconciled Only in the Display field.
Enables you to do the following:
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:12 AM
If you select the checkbox, the report displays transactions with a correct historic balance due as at the specified posting
date To date as follows:
If the reconciliation date is later than the specified posting date To date, the transaction (or partial transaction if
partially reconciled) is shown as un-reconciled, and the un-reconciled Balance Due value is displayed.
If the reconciliation date is earlier than or same as the specified posting date To date, the transaction (or partial
transaction if partially reconciled) is shown as reconciled, and the reconciled Balance Due value is displayed.
If you do not select the checkbox, the report displays transactions with the latest balance due.
Hide Zero Balance Due
 Note
The field is available only if you select All Postings in the Display field and select Consider Reconciliation Date checkbox.
Select to hide the transactions which have a zero balance due as calculated when the Consider Reconciliation Date checkbox is
selected.
Hide Zero Balanced Acct
Excludes zero balanced accounts from the report.
 Note
Available only if Hide Acct with no Postings is not selected.
Hide Acct with no Postings
Report excludes accounts with no postings.
Sort and Summarize
Enables you to specify sorting criteria for displaying the report on the screen:
In the field below, specify what is to be sorted.
In the table, define up to three levels of sort.
In each row, specify:
Sort Field
Order
Summary
Revaluation
Opens the Revaluation Selection Criteria window where you can specify how to revaluate report results.
 Note
The revaluation is for display purposes only and does not affect the postings values.
Related Information
Expanded Selection Criteria
Revaluation - Selection Criteria
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:12 AM
Properties
Expanded Selection Criteria
This window enables you to set additional selection criteria for the general ledger report and fine tune the report results.
To open the window, choose Financials Financial Reports Accounting General Ledger ; then, in the General Ledger –
Selection Criteria window, choose Expanded.
Expanded Selection Criteria
Original Journal
Document and transaction types by which journal entries are created in SAP Business One. To display in the report only journal
entries created by specific documents or transaction types, select the respective ones.
Parameters
Select the parameters you want to apply to optimize the range of transactions to display in the general ledger report, and specify
the required range in the respective From...To... field.
Reference Fields
Enables filtering the report according to reference fields defined in Administration Setup General Reference Field Links .
Therefore, filtering the report data according to the level of granularity required for IFRS and for other purposes becomes possible.
User-Defined Fields
Enables filtering the report according to the user-defined fields defined in Administration Setup General Reference Field
Links . Therefore, filtering the report data according to the level of granularity required for IFRS and for other purposes becomes
possible.
Series
Opens the Series Selection window where you can choose to view only journal entries related to specific numbering series.
Clear Sel.
Clears all selections made in this window.
Series Selection
This window appears when you specify selection criteria for the General Ledger.
To access the window, choose Financials Financial Reports Accounting General Ledger . In the General Ledger –
Selection Criteria window, choose Expanded, and in the Expanded Selection Criteria window, choose Series.
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Series Selection
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:12 AM
Document
Specify the document.
Series
Numbering series defined in the Document Numbering window for documents available in the Expanded Selection Criteria
window.
Related Information
General Ledger
Revaluation - Selection Criteria
Use this window to specify selection criteria for the Revaluation report.
To open the window, choose Financials Financials Reports Accounting General Ledger. In the General Ledger –
Selection Criteria window choose Revaluation.
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
FC Tab
Currency
Choose the currency to which you want to revaluate.
Revaluation Method
Choose whether to calculate the revaluation according to the rate defined in the Posting Date or Due Date of the transaction, or
according to Fixed Rate. If you choose the last option, enter the required fixed rate.
Average Rate from Interval (in Days)
Specify the number of days for calculating an average rate in case an exchange rate was not defined for a specific date.
Refer to Rates in Journal Entry
Select this checkbox to use the rate defined in the journal entries, if it is different from the rate defined in the Exchange Rates and
Indexes window.
Revaluate All Currency G/L Account/BP
All currency accounts and business partners must have their values converted to one currency before they can be revaluated.
Select whether to revaluate All currency G/L accounts or business partners by local currency or by system currency.
Index Tab
To
Choose the required month and year of the index.
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:12 AM
Value
Displays the index defined for the chosen month and year. Change this value if required.
Revaluation Method
Choose whether to calculate the revaluation according to the index defined for the Posting Date or the Due Date of the
transaction.
Related Information
General Ledger
Selecting Control Accounts in the General Ledger Report (BP
View)
Context
In the General Ledger report (BP view), you can select the transactions per control account.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting General Ledger .
2. In the General Ledger – Selection Criteria window, select the BP checkbox and specify the selection criteria for the report.
For more information, see the topic General Ledger.
3. If required, select the desired control accounts.
4. To run the report, choose OK.
Related Information
General Ledger
Summarizing Control Accounts in the General Ledger Report
Context
In the General Ledger report (G/L view), you can summarize the transactions posted on the control accounts.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting General Ledger .
2. In the General Ledger – Selection Criteria window, select the Accounts checkbox and specify the selection criteria for the
report. For more information, see the topic General Ledger.
3. If you want to summarize the transactions per control account, select the Summarize Control Accounts option.
4. To run the report, choose OK.
5. To print the report, choose Print General Ledger .
Results
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:12 AM
SAP Business One creates a general ledger report that displays only the selected accounts and prints only the totals for the
control accounts.
Related Information
General Ledger
General Ledger Window
 Note
This topic contains an SAP Note that explains additional information.
This window displays the General Ledger report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Ledger Window
Posting Date, Due Date
Posting date and due date of the accounting document.
Series
Numbering series assigned to the displayed journal entry.
Doc. No.
Number of the document that created the transaction and its original journal entry (IN for A/R Invoice, RC for Incoming Payments,
and so on).
Trans. No.
Number of the journal entry.
Remarks
Text entered in the Remarks field in the journal entry.
Offset Acct
Offsetting account from the journal entry.
 Example
In a journal entry created by an incoming payment, the cash fund account is displayed.
Deb./Cred.(LC)
Posting amounts in local currency. Credit postings are in green and placed in brackets.
Balance (LC)
Account balance, recorded cumulatively with each posting, in the national currency.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:12 AM
Cumulative Balance Due (LC)
Total due from business partner or G/L account, recorded cumulatively with each posting, in the national currency, reflecting the
payment and account activity.
Blanket Agreement
Related blanket agreement number and a link to the blanket agreement.
Project, Project Name
Display the code and name of the project each transaction is allocated to.
 Note
By default, these two columns do not appear in the General Ledger window. You can select them in the Form Settings window.
To open the window, in the toolbar, choose .
 Note
Choosing to preview/print displays a window where you select the general ledger that you want to print: either the Book of
Account or the Subsidiary account. For more information about using system variables when designing a print template for the
General Ledger report, see SAP Note 867048
Related Information
General Ledger
Printing Totals by Control Account in the General Ledger Report
(BP View)
Context
In the General Ledger report (BP view), you can print the totals per control account for each business partner and a summary of
the control accounts at the end of the report.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting General Ledger .
2. In the General Ledger – Selection Criteria window, select BP and specify the selection criteria for the report. For more
information, see the topic General Ledger.
3. To run the report, choose OK.
4. To print the report, choose Expand Ledger General Ledger by Control Account .
5. Click Set as Default and Cancel.
6. Choose Print Expand Ledger .
Results
SAP Business One creates a report that displays the transactions with totals per control account for each business partner and a
summary by control account at the end of the report.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:12 AM
Related Information
General Ledger
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
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:12 AM
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
Months – Each column represents one month, moving back from the aging date month.
Periods – Each column represents one period as defined in Administration System Initialization Posting Periods ,
moving back from the aging date period.
[Top Total Row]
Displays the sum of amounts listed in one column
[Bottom Total Row]
Displays the percentage of open receivables for each time interval
Transaction Journal Report
Use this window to specify selection criteria for the Transaction Journal report, which displays a list of transactions according to a
selected transaction type.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:12 AM
To open the window, choose Financials Financial Reports Accounting Transaction Journal Report . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the Transaction Journal Report window.
Selection Criteria
Original Journal
Specify the type of transaction to display.
Transaction No. From...To...
Specify a range of transaction numbers to include only transactions whose numbers fall within the range.
Series
Opens the Series Selection window, where you can choose to display only transactions with numbers of specific numbering series.
Related Information
Series Selection
Transaction Journal Report Window
This window displays the Transaction Journal Report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Transaction Journal Report Window
Original Journal
Original journal defined for the report.
Currency
Currency to use for displaying transaction amounts.
Date
Posting date of each transaction.
Series
Numbering series assigned to each transaction.
Type
Type of transaction.
 Note
Each document has a different transaction type. For example, IN is for A/R invoice.
Trans.#
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:12 AM
Transaction number with a link to the transaction.
Creator
User who created the document or the transaction.
G/L Acct /BP Code
Code of the G/L account and/or business partner involved in the transaction.
G/L Acct/BP Name
Name of the G/L account and/or business partner involved in the transaction.
Debit, Credit
Debit or credit values in the transaction, per G/L account/business partner.
Total debit and credit amounts are displayed at the bottom of the columns.
Series
Opens the Series Selection window, where you can choose to display only transactions with numbers of specific numbering series.
The report is updated accordingly.
Related Information
Series Selection
Transaction Report by Projects
This report displays the transactions made in SAP Business One and groups them by their related projects.
 Note
Failure to consistently relate projects to transactions may result in an inaccurate report.
Use this window to specify selection criteria for the Transaction Report by Projects.
To open the window, choose Financials Financial Reports Accounting Transaction Report by Projects . Alternatively,
open it from the Reports module.
After defining the report, you can view it in the Transaction Report by Projects window.
Selection Criteria
Project From...To..., G/L Account From...To...
Specify the required project/range of projects, and the required G/L account/range of G/L accounts.
Due Date From...To..., Posting Date From...To..., Document Date From...To...
Specify the required date ranges for the report.
 Note
The default values for these fields are the date ranges defined for the current posting period.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:12 AM
Transaction Report by Projects Window
This window displays the Transaction Report by Projects according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Transaction Report by Projects Window
Trans. No.
Number and link to journal entry.
Project Code
Project code to which the transaction is linked.
Account Number
Code of the G/L account involved in the transaction that is linked to the project code.
Posting Date
Posting date of the transaction.
Debit, Credit
Credit and debit amounts of the rows in the transaction that are linked to the project code.
Total
Total amount per account, per project code. Credit amounts are marked with a negative sign.
Document Journal
This report displays in detail journal entries created manually or automatically by documents produced in SAP Business One. The
large variety of selection criteria can create the most accurate report as per company requirements.
Use this window to specify selection criteria for the Document Journal report.
To open the window, choose Financials Financial Reports Accounting Document Journal Report . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the output modes Detailed Transactions or Month Totals.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Selection Criteria Name
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:12 AM
You can save a specific set of selection criteria and generate the report accordingly whenever required. To do so press CTRL +
A , enter a meaningful name, and set all the required selection criteria for the report. Choose Save. To generate a report based on
a saved selection criteria set, click the icon. The List of Reports - Selection Criteria window appears. Highlight the required
selection criteria set from the list, and choose the Choose button. The selected selection criteria set is populated. To generate the
report, choose OK.
BP
Displays business partners in the report.
 Note
When not selected, all other fields pertaining to business partner selection criteria are unavailable.
Customer Group, Vendor Group
Specify whether to display business partners from specific groups, divided into customers and vendors.
 Note
To display only customers, choose None in the Vendor Group field.
Properties
Opens the Properties window where you can specify properties as selection criteria. Your choices appear in the adjoining field.
Accounts
Includes G/L accounts in the report.
 Note
When not selected, all other fields related to G/L accounts selection criteria are unavailable.
Find
Opens the Find G/L Accounts window, where you can specify G/L accounts to be included in the report.
[Level]
Select the level of the accounts to display in the table. Selecting Level 1 displays the account titles on the highest level.
 Note
A selected row includes all accounts appearing under the title.
X, Account
Indicates accounts selected to appear in the report:
Clear the X from a row to deselect the account.
Click the X in the column header to select/clear all accounts/selections in the table.
Posting Date From...To, Creation Date From...To, Document Date From...To
Define the transaction range by posting, creation and/or document date, and specify a date range.
Output Mode: Detailed
Specify the output mode of the report:
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:12 AM
No Total: Displays all journal entries
Month (Posting Date): Displays all journal entries per month based on the posting date
Month (Posting Date) and Original Journal: Displays all journal entries per month based on the posting date and original
journal
Period (Posting Date) and Original Journal: Displays all journal entries per period based on the posting date and original
journal
Output Mode: Totals
Specify the output mode of the report:
Month (Posting Date): Displays the totals per month based on the posting date
Month (Creation Date): Displays the totals per month based on the creation date
Month (Posting Date) and Original Journal: Displays the totals per month based on the posting date and original journal
Period (Posting Date) and Original Journal: Displays the totals per period based on the posting date and original journal
Creation Date
Groups the postings by month, based on the creation date.
 Note
Only available for Month Totals Mode.
Display Postings Summary
Displays the postings summary in a separate row at the end of the report.
 Note
Only relevant for Month Totals Mode.
Opening Balance for Period
Select this checkbox to display the opening balance of the selected BP and G/L accounts, as accumulated in the time range from
the following option date to the start date specified in the Selection options:
OB from Start of Company Activity – displays the opening balance accumulated after company activity started.
OB from Start of Fiscal Year – displays the opening balance accumulated after the start of the fiscal year specified in the
Selection options.
 Example
You have selected the OB from Start of Fiscal Year radio button.
The posting date range defined in the Selection option is 01/04/2005–31/03/2006, and the posting periods defined for the
company are four quarters per calendar year.
The date to be considered as "Start of Fiscal Year" is then 01/01/2005 .
The opening balance display is then the accumulated balance from 01/01/2005 to 01/04/2005.
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:12 AM
The calculation of the opening balance is influenced by the date range defined for the report. If you specify more than one date
range, SAP Business One calculates opening balance as follows:
If Posting Date is one of the selected options, all transactions with posting date earlier than the date defined in the Posting
Date From field are included.
If Posting Date is not one of the selected options, all transactions with document date earlier than the date defined in the
Document Date From field are included.
Ignore Adjustment
Report excludes adjustment transactions.
Display Installments in One Row
Group installments included in transactions in one row. The row representing the installments displays the cumulative amount of
all the installments in the transaction, while all the other details of that row refer to the last installment.
 Note
Only relevant for the Detailed Transactions output mode.
Numbering for Detailed Mode, First Sequential No., No. on First Printed Page
Specify the first sequential number and the first page number to be displayed in the detailed mode of the report.
 Note
Page numbering is only relevant for printed reports.
Sort
Report sorts using the criteria that you specify.
In the table, specify the required sorting fields and their preferred order.
Related Information
Expanded Selection Criteria
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
Properties
Document Journal: Detailed Transactions
This window displays the Document Journal in the Detailed Transactions output mode, according to your selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Document Journal: Detailed Transactions
Seq. No.
Successive numbers of transactions, according to the value entered in the First Sequential No. field in the selection criteria.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:12 AM
Trans. No.
Transaction number and a link to the journal entry.
Posting Date
Posting date of each row in the transaction.
 Note
If you selected Display Installments in One Row in the selection criteria, the posting date displayed in the installment rows is
the one assigned to the last installment.
Series
Numbering series linked to the transaction.
G/L Acct/BP Code, G/L Acct/BP Name
Code and name of the G/L account or business partner to which the row of the transaction is related.
Debit/Credit (LC)
Total amount of the credit or debit fields, in local currency.
Remarks
Additional details for the document or journal entry.
Blanket Agreement
Related blanket agreement number and a link to the blanket agreement.
Document Journal: Month Totals Mode
This window displays the Document Journal in the Month Totals Mode output mode, according to your selection criteria.
Document Journal: Month Totals Mode
Date
Month and year when the transactions summarized in this row were created.
Total Credit (LC), Total Debit (LC)
Sum of G/L account, customer and vendor credit or debit, in local currency.
Credit Account (LC), Debit Account (LC)
Cumulative credit and debit amounts related to G/L accounts, in local currency.
Credit Customers (LC), Debit Customers (LC)
Cumulative credit and debit amounts related to customers, in local currency.
Credit Vendors (LC), Debit Vendors (LC)
Cumulative credit and debit amounts related to vendors, in local currency.
Cash Flow Reference Report
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:12 AM
This window displays a list of cash flow relevant transactions that may or may not have been assigned a cash flow line item within a
certain period. With the exception of the report reference period, you cannot modify the fields in this report.
To open this window, choose Financials Financial Reports Accounting Cash Flow Reference Report . Alternatively, open it
from the Reports module.
Cash Flow Reference Report - Selection Criteria Window
Date From … To
Select the date range for displaying the cash flow relevant transactions. This field may be left blank.
Unassigned Transactions Relevant to Cash Flow
Generates a list of cash flow relevant transactions that have not been assigned a cash flow line item. This is the default setting.
All Transactions Relevant to Cash Flow
Generates the entire list of cash flow relevant transactions.
Cash Flow Reference Report Window
Currency
The selected currency in which the accounting documents are displayed.
From Date, To Date
Cash flow relevant transactions that occurred within the specified period.
Date
Posting date and value date of the accounting document.
Type
Type and number of the accounting document, for example, JE (journal entry).
Trans. #
Transaction number of the journal entry.
Creator
Person who created the corresponding transaction.
Debit/Credit
Posting amounts displayed in the national currency. Credit postings appear in green between brackets.
For transactions for which more than one cash flow line item is assigned, the debit/credit amounts are displayed separately
according to their corresponding cash flow line items.
Primary Form Item
Primary form line item assigned to the cash relevant transaction.
Glossary of Journal Types and Abbreviations
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:12 AM
| Abbreviation | Journal Type        |     |     |     |
| ------------ | ------------------- | --- | --- | --- |
| OB           | Opening Balance     |     |     |     |
| JE           | Journal Entry       |     |     |     |
| IN           | A/R Invoice         |     |     |     |
| CN           | A/R Credit Memo     |     |     |     |
| PU           | A/P Invoice         |     |     |     |
| PC           | A/P Credit Note     |     |     |     |
| RC           | Incoming Payment    |     |     |     |
| PS           | Payments to Vendors |     |     |     |
| DP           | Deposits            |     |     |     |
| CP           | Checks for Payment  |     |     |     |
| DN           | Delivery            |     |     |     |
| RE           | A/R Returns         |     |     |     |
| PD           | Goods Receipt PO    |     |     |     |
| SI           | Goods Receipt       |     |     |     |
| SO           | Goods Issue         |     |     |     |
| MI           | Inventory Posting   |     |     |     |
| WO           | Work Order          |     |     |     |
Tax
This menu option includes tax reports according to the company's localization. The same tax reports are available in multiple
localizations if the localizations fall under wider reporting regions, such as the European Union.
Information about tax reports that are specific to a country/region is available in the localization-specific online help file in:  Help
 Documentation   Localization-Specific Information  or by choosing  F1  while the relevant tax report is the active window in
SAP Business One.
To create tax reports, choose  Financials   Financial Reports   Accounting   Tax . Alternatively, create them from the Reports
module.
One-Stop Shop
The One-Stop Shop (OSS) scheme is available in multiple localizations across the European Union (EU). OSS allows companies to
register and report value-added tax (VAT) through only one EU country, regardless of how many EU countries the companies
supply.
One-Stop Shop Declaration is available as an Output Mode in Tax Report - Selection Criteria. From the SAP Business One Main
| Menu, choose  | Reports   Financials  |  Accounting  |  Tax   Tax Report | .   |
| ------------- | --------------------- | ------------ | ----------------- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:12 AM
Select the tax group codes that you want to report in the Output section of Tax Report - Selection Criteria, and other criteria for
One-Stop Shop Declaration, to produce a report.
The selection One-Stop Shop Declaration can be made whether or not Extended Tax Reporting is active. For each EU country that
is traded with, Tax Groups setup is required for OSS.
In the report, tax codes can be filtered to show transactions that are relevant for OSS. Filtering of document types and numbering
series is also available. Crystal Reports are available for OSS.
Financial
This menu option includes the financial reports required to present a company's business activity results.
To create financial reports, choose Financials Financial Reports Financial . Alternatively, create them from the Reports
module.
Balance Sheet
This report displays the accumulated assets and liabilities of a company up to a particular date, using the accounting formula:
Total Assets = Total Liabilities + Equity.
 Note
When printing the report, you can print the selection criteria on a separate page.
Balance Sheet - Selection Criteria
Use this window to specify selection criteria for the Balance Sheet report.
To open the window, choose Financials Financial Reports Financial Balance Sheet . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the Balance Sheet window.
Selection Criteria
Date From... To...
Specify:
Whether to create the balance sheet according to posting date or document date
The date up to which the report should be created.
Template
Select the template to be used for the report. The options available in this dropdown list are the financial report templates of type
Balance Sheet that defined in: Financials Financial Report Template . If you have not defined any financial report template,
the default option is Chart of Accounts.
Display in Report
Choose one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:12 AM
Accounts with Balance of Zero – report displays accounts with a balance of zero.
Foreign Name – report displays the foreign names defined for G/L accounts.
Nothing is displayed for accounts for which a foreign name was not defined.
External Code – report displays external codes defined for G/L accounts.
Add Journal Vouchers
Includes transactions that are recorded in Open journal vouchers, but not yet permanently saved in the database.
Add Closing Balances
The report includes period-end closing journal entries, for the chosen posting period only; as such, Profit Period shows a zero
balance for a closed posting period.
If you do not select this option, the Profit Period shows the balance prior to the period-end closing process.
The balance of previously closed periods is displayed in the Retained Earnings G/L account, whether this field is selected or not.
 Example
The company has two closed posting periods: 2003 and 2004.
Add Closing Balances is not selected, and you run the report to 2004.
The report displays the balance of the Profit Period from the beginning of 2004.
The balance of the previous periods (2003) is displayed in the Retained Earnings G/L account.
Add Closing Balances is selected, and you run the report to the last day of the posting period (December 31, 2004).
The report displays a zero balance for the Profit Period.
The balance of the previous posting periods (2003) is displayed in the Retained Earnings G/L account.
The balance of the profit and loss accounts of 2004 is displayed in the Period-End Closing G/L account.
Add Closing Balances is selected, and you run the report to the next posting period (2005). The balance of the previous
posting periods is displayed in the Retained Earnings G/L account.
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Choose Segments
Opens the Find G/L Accounts window, where you can choose the accounts to include in the balance sheet, according to segments.
 Note
Available only if the company maintains a chart of accounts based on segments.
Revaluation
Opens the Balance Sheet Revaluation window.
Balance Sheet Window
This window displays the Balance Sheet report according to the defined selection criteria.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:12 AM
Balance Sheet Window
Up to
Date specified in the To field in the selection criteria.
Display Subtotals
Displays a subtotal opposite each title.
Hide Titles
Selecting the checkbox changes the display and print mode of the report in the following ways:
Hides all the title accounts
Displays the active accounts in the current level and higher levels
Selecting the checkbox does not hide the special row Profit Period, which is taken from the profit and loss statement report and is
used for calculating the total in the balance sheet report.
 Note
Selecting the checkbox enables you to sort the accounts in the report.
Level
Specify the account level you want to display in the balance sheet.
The balance sheet is displayed at the latest level selected in the window.
Level 1 includes a summary of all G/L accounts under the titles Assets, Liabilities, and Equity.
The transition to a higher level of detail conforms to the levels defined in the chart of accounts. Level 2 usually breaks down:
The assets into current assets, long-term investments, and fixed assets
The liabilities into current and long-term liabilities
The equity sections include share capital and profit for the period.
 Note
You can distinguish among the various display levels by color: drawers in red, titles in blue, and active accounts in black.
Account Name
Displays the names of the drawers (Assets, Liabilities, Equity, and so on), titles, and accounts in the chart of accounts, according
to the selected display level.
If you select Foreign Names in the selection criteria, foreign names are displayed next to the account codes.
If you select External Code in the selection criteria, the external code is displayed instead of the original account code.
 Note
You can sort the accounts in the report as follows:
1. Select the Hide Titles checkbox.
2. To sort the accounts alphanumerically in ascending order, double-click the column header Account Name.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:12 AM
To sort the accounts alphanumerically in descending order, double-click the column header again.
Balance
Balance of the drawer, title, or G/L account, according to the display level.
Foreign Currency
Balance in foreign currency for foreign currency G/L accounts.
 Note
Displayed only when you select Foreign Currency as a selection criterion.
System Currency
Balance in the system currency.
 Note
Displayed only when you select System Currency as a selection criterion.
Relative Percentage
Relative percentage of each balance in the company’s assets, liabilities, and equity set. Each first-level title (drawer) equals 100 %,
and its related titles and active G/L accounts display their relative percentage.
 Note
Displayed only when you select Relative Percentage as a selection criterion.
Revaluation - Selection Criteria
Use this window to specify selection criteria for the Revaluation report.
To open the window, choose Financials Financials Reports Accounting General Ledger. In the General Ledger –
Selection Criteria window choose Revaluation.
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
FC Tab
Currency
Choose the currency to which you want to revaluate.
Revaluation Method
Choose whether to calculate the revaluation according to the rate defined in the Posting Date or Due Date of the transaction, or
according to Fixed Rate. If you choose the last option, enter the required fixed rate.
Average Rate from Interval (in Days)
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:12 AM
Specify the number of days for calculating an average rate in case an exchange rate was not defined for a specific date.
Refer to Rates in Journal Entry
Select this checkbox to use the rate defined in the journal entries, if it is different from the rate defined in the Exchange Rates and
Indexes window.
Revaluate All Currency G/L Account/BP
All currency accounts and business partners must have their values converted to one currency before they can be revaluated.
Select whether to revaluate All currency G/L accounts or business partners by local currency or by system currency.
Index Tab
To
Choose the required month and year of the index.
Value
Displays the index defined for the chosen month and year. Change this value if required.
Revaluation Method
Choose whether to calculate the revaluation according to the index defined for the Posting Date or the Due Date of the
transaction.
Trial Balance
This report displays a summary of all accounts and/or business partner balances for a specific date. The report can comprise all
accounts and business partner balances in SAP Business One, or only a particular cross section.
 Note
If the trial balance includes all the accounts, the debit and credit side totals must be equal.
 Note
When printing the report, you can print the selection criteria on a separate page.
Related Information
Trial Balance - Selection Criteria
Trial Balance Window
Trial Balance - Selection Criteria
Use this window to specify selection criteria for the Trial Balance report.
To open the window, choose Financials Financial Reports Financial Trial Balance . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Trial Balance window.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:12 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
BP
Includes business partners in the report.
Properties
Open the Properties window and use the business partner properties as selection criteria.
G/L Accounts
Report includes G/L accounts.
Find
To find a special account, choose this button and specify the account code. SAP Business One automatically displays an X next to
this account.
Level
Choose the level of the account displayed in the table.
If you choose Level 1 here, the table displays the highest level titles for the accounts.
If you select a row in the table, you actually select all the accounts that appear under this title.
Date, From...To...
Click and choose the date range type for displaying the report.
Then, define the actual range in the From ...To.. fields.
Click to define a range of posting periods.
Display in Report
You can select the following options to display in the report:
Hide Zero Balanced Acct – Select this checkbox to exclude zero balanced accounts from the report.
Hide Acct with No Postings – Select this checkbox to exclude accounts with no postings. This checkbox is only available if
Hide Zero Balanced Acct is deselected.
Foreign Names – Displays only the foreign names defined for G/L accounts in Financials Chart of Accounts Account
Details Foreign Names .
 Note
When this checkbox is selected, nothing is displayed for accounts for which the foreign name was not defined.
External Code – Displays external codes defined for G/L accounts in Financials Chart of Accounts External Code .
Opening Balance for Period – Select this option when you need to differentiate between the balance of the selected
posting period and that of the previous periods. When a date range of a current posting period is selected, you can select
this checkbox to display the bookkeeping balance prior to the selected date range in a separate column: OB.
As default, the checkbox is cleared. Selecting it displays the following options:
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:12 AM
OB from Start of Company Activity – Displays the opening balance accumulated since the company’s activity
started.
OB from Start of Fiscal Year – Displays the opening balance accumulated from the start of the current fiscal year.
Accumulative Balance – Displays Accumulative Debit Opening Balance/Closing Balance (OB/CB) and Accumulative Credit
Opening Balance/Closing Balance (OB/CB) in the results.
Foreign Currency – Displays amounts in local and foreign currency. When the option System Currency is also selected, the
amounts are displayed in system and foreign currency.
 Note
For All Currencies accounts and business partners, if all the journal entries were recorded using the same foreign
currency, the trial balance shows the actual foreign currency balance. Otherwise, **** is displayed instead of the
amounts.
System Currency – Displays amounts in system currency only.
Local and System Currency – Displays amounts in system and local currencies.
Template
Click and select a template for displaying the balance sheet.
Annual Report, Quarterly Report, Monthly Report
Select:
Annual Report to calculate the trial balance for the entire year
Quarterly Report to calculate the trial balance separately for each quarter
Monthly Report to calculate the trial balance separately for each month
Periodic Report
Displays the report according to the posting periods included in the defined date range.
Add Journal Vouchers
Includes in the report Open transactions that are recorded in journal vouchers, but are not yet saved in the database.
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Add Closing Balances
Selected: Report includes period-end closing journal entries and balances of the selected posting period only. All profit and
loss accounts that were closed by the period-end closing process show a zero balance.
CB of Life-to-Date: Reports includes the closing balance from the system go life date to the end of the selected
period.
CB before Selected Period Only: Reports includes the closing balance from the system go life date to the beginning
of the selected period.
Not selected (default): Report does not include period-end closing journal entries. All profit and loss accounts that were
closed by the period-end closing process show the G/L account balance prior to the closing process.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:12 AM
Period-end closing journal entries of posting periods prior to the selected period are included in the Opening Balance
column.
In certain countries/regions, you can transfer the balances of Balance Sheet accounts from one fiscal year or period to
another. In these localizations the period-end closing process is different than described above; therefore, the effect of
this box on the report is different. For additional information see the localization-specific online help file under Help
Documentation Localization-Specific Info .
Revaluation
Opens the Trial Balance Revaluation window. After the revaluation is made, the option next to this button is selected.
Expanded
Opens the Expanded Selection Criteria window, where you can use a transaction code, project, and distribution rule range, as well
as series, as selection criteria for this report.
Related Information
Revaluation - Selection Criteria
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
Properties
Expanded Selection Criteria
Use this window to apply additional selection criteria to the Trial Balance report.
Reference Fields
Enables filtering the report according to reference fields defined in Administration Setup General Reference Field Links .
Therefore, filtering the report data according to the level of granularity required for IFRS and for other purposes becomes possible.
Project From...To...
Select Project and specify a project range.
The report includes transactions pertaining to the projects within the defined range.
Distr. Rule From...To...
Select Distr. Rule and specify a distribution rule range. The report covers transactions related to the distribution rules within the
defined range.
User-Defined Fields
Enables filtering the report according to the user-defined fields defined in Administration Setup General Reference Field
Links . Therefore, filtering the report data according to the level of granularity required for IFRS and for other purposes becomes
possible.
Trial Balance Report Details by Control Account
Context
In the Trial Balance report, you can print the totals per control account for each business partner and a summary of the control
accounts at the end of the report.
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:12 AM
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Financial Trial Balance .
2. In the Trial Balance – Selection Criteria window, select the BP checkbox and specify the selection criteria for the report.
For more information, see the topic Trial Balance – Selection Criteria.
3. Select the Show Info per Ctrl Acct checkbox.
4. To run the report, choose OK.
Trial Balance Window
This window displays the Trial Balance report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Trial Balance Window
Hide Titles
Selecting the checkbox changes the display and print mode of the report as follows:
Hides all the title accounts
Displays the active accounts in the current level and higher levels
Displays the total
 Note
Selecting the checkbox enables you to sort the accounts in the report.
Name
Displays the names of the drawers (assets, liabilities, equity, and so on), titles, and accounts in the chart of accounts, according to
the selected display level.
A separate section for displaying business partner balances appears at the end of the trial balance.
 Note
You can sort the accounts in the report by G/L accounts and BP sections, as follows:
1. Select the Hide Titles checkbox.
2. To sort the accounts alphanumerically in ascending order, double-click the column header Account Name.
To sort the accounts alphanumerically in descending order, double-click the column header again.
OB
Displays the opening balance amounts.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:12 AM
This column is displayed only when the Disp.Opening Balance for Period checkbox is selected in the Selection Criteria
window.
Accumulative Debit OB
Displays a balance of all debit transactions on account until the report start date.
Accumulative Credit OB
Displays a balance of all credit transactions on account until the report start date.
Accumulative Debit CB
Displays a balance of all debit transactions on account until the report end date.
Accumulative Credit CB
Displays a balance of all credit transactions on account until the report end date.
Debit
Displays the total debit amount for each drawer, title, active account, and business partner according to the selected display level.
Credit
Displays the total credit amount for each drawer, title, active account, and business partner, according to the selected display level.
Balance
The balance of the drawer, title, active account, or business partner, according to the display level.
Calculation: debit amount – credit amount + O.B. amount
System Currency
Displays the balance in the system currency.
To display only the Balance column in the system currency, double-click the title System Currency.
When you print the trial balance, the debit and credit data, as well as the balance, are displayed in the Local, System and foreign
currencies.
 Note
The System Currency column is displayed only if the checkbox Display in SC is selected in the Selection Criteria window.
Foreign Currency
Displays the balance in foreign currency for foreign currency G/L accounts and business partners.
To display only the Balance column in a foreign currency, double-click the title Foreign Currency. When you print the trial balance,
the debit and credit data, as well as the balance, are displayed in the local, system and foreign currencies.
 Note
The Foreign Currency columns are displayed only if the checkbox Foreign Currency is selected in the Selection Criteria
window.
Level
Select the account level you want to display in the trial balance.
Level 1 includes a summary of all G/L accounts under each drawer.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:12 AM
The transition to a higher level of detail will conform to the levels you defined in the Chart of Accounts.
 Note
You can distinguish between the various display levels by color.
A title is also shifted slightly to the left of the active account or of a subtitle beneath it.
Profit and Loss Statement
This report lets you view the balance of all Profit and Loss G/L accounts. The total result of the statement is the profit or loss for
the company in the selected period.
 Note
When printing the report, you can print the selection criteria on a separate page.
Profit and Loss Statement - Selection Criteria
Use this window to specify selection criteria for Profit and Loss Statement reports.
To open this window choose Financials Financial Reports Financial Profit and Loss Statement . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the Profit and Loss Statement window.
Profit and Loss Statement – Selection Criteria
Date, From ... To...
Click and choose the date according to which to generate the profit and loss statement.
Next, define the required date range, or choose in the From... To... fields to select the required period range.
Display in Report
Select any of the following options to display in the report:
Accounts with Balance of Zero – Displays accounts with a balance of zero.
Foreign Name – Displays only the foreign names defined for G/L accounts in Financials Chart of Accounts Account
Details Foreign Name .
 Note
When this checkbox is selected, nothing is displayed for accounts lacking a foreign name.
External Code – Displays external codes defined for G/L accounts in Financials Chart of Accounts External Code .
Annual Report, Quarterly Report, Monthly Report
Select:
Annual Report to calculate the profit and loss statement for the entire year
Quarterly Report to calculate the profit and loss statement separately for each quarter
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:12 AM
Monthly Report to calculate the profit and loss statement separately for each month
Periodic Report
Select this option to display the report according to the posting periods included in the defined date range.
Template
Choose a template for displaying the profit and loss statement. By default, the template chart of accounts is selected.
Click to select a different template.
 Note
Different templates might show different results, due to the different G/L accounts assigned to them.
Display in First Column
Select whether to display figures in local currency or in system currency, in the first column of the report.
Display in Second Column
Select one of the following options to display in the report's second column:
System Currency – figures in system currency.
 Note
If you chose to display system currency in the first column, this option is disabled.
Foreign Currency – figures in foreign currency.
Balance for Comparison – once this option is selected, select one of the following radio buttons:
Life to Date – to display the balance from beginning of company activity up to the date defined in the To field.
Year to Date – to display the balance from day one of the selected posting period up to the date defined in the To
field.
 Note
The first day of the selected posting period is the one defined in Administration System Initialization
General Settings Posting Periods . The date appears in the From field of the first sub period.
Add Journal Vouchers
Includes in the report Open transactions that are recorded in journal vouchers, but are not yet saved in the database.
Ignore Adjustments
Report excludes adjustment journal entries from its profit and loss statement calculation.
Choose Segments
Opens the Find G/L Accounts window, in which you can choose the accounts to include in the profit and loss statement, according
to segments.
 Note
Appears only if the company maintains a chart of accounts based on segments.
Revaluation
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:12 AM
Select this option and choose the required parameters to generate a revaluated report.
Expanded
Opens the Expanded Selection Criteria window, where you can define additional parameters for the report.
Related Information
Expanded Selection Criteria
Profit and Loss Statement Window
This window displays the Profit and Loss Statement report according to the defined selection criteria.
Profit and Loss Statement Window
From Date, To
Selected date range for the report.
Hide Titles
Selecting the checkbox changes the display and print mode of the report as follows:
Hides all the title accounts
Displays the active accounts in the current level and higher levels
 Note
Selecting the checkbox enables you to sort the accounts in the report.
Display Subtotals
Displays subtotals next to each Title G/L account.
Account Name
Displays the names of the drawers, titles, and active accounts in the chart of accounts, according to the chosen display level.
 Note
You can sort the accounts in the report as follows:
1. Select the Hide Titles checkbox.
2. To sort the accounts alphanumerically in ascending order, double-click the column header Account Name.
To sort the accounts alphanumerically in descending order, double-click the column header again.
Balance
The balance of the drawer, title, or G/L account, according to the display level.
Multi-Year Cumulative
Displays the G/L account balance from the company start date.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:12 AM
If the selected date range is not from the beginning of work in the company, there will be a difference in the data displayed in the
Balance and Current Year columns.
System Currency
Displays the balance in the System currency.
This column appears only if the checkbox SC is selected in the Selection Criteria window.
FC
Displays the balance in foreign currency for foreign currency G/L accounts.
The FC column is displayed only if the checkbox FC Column is selected in the Selection Criteria window.
Display Subtotals
Displays subtotals next to each Title G/L account.
Level
Choose the account level you want to display in the profit and loss statement.
The report is always displayed at the last level established in the window.
The transition to a higher level of detail will conform to the levels you defined in the Chart of Accounts.
Cash Flow
This report lets you analyze your cash flow based on all revenues and expenses, for example, checks, credit cards, recurring
account transactions, customer liabilities, and so on. You define the level of detail for the individual results.
The report provides information about the liquidity of your business that is beyond the scope of a profit-and-loss statement.
The report:
Takes into account whether open payments have since been paid, and if not, the likelihood of these receivables being
collected.
Lets you forecast future revenues and expenses to facilitate business decisions.
Can raise your awareness of possible future liquidity problems, enabling you to act accordingly.
You can find more information in this blog .
Cash Flow - Selection Criteria
Use this window to specify selection criteria for the Cash Flow report.
To open the window, choose Financials Financial Reports Financial Cash Flow . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Cash Flow window.
Selection Criteria
Date From...To
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:12 AM
Specify a date range. The report includes documents and transactions with due dates within this range.
Time Interval
Specify a time interval as a preliminary report format. Each row in the report will represent a time interval: day, week, month, and
so on.
Add Recurring Postings
Adds to the cash flow recurring transactions, which appear in green in the report.
Add Journal Vouchers
Adds open journal vouchers to the report calculation, which is displayed in blue in the report.
Consider Delays in Payments
Specifies that the average number of delay days, if defined for the business partner, should be included in the cash flow.
 Example
If the due date of an A/R invoice is 03/10/05 and the average delay defined for the customer is five days, the due date
calculated for the cash flow (when this option is selected) is 03/15/05.
Display Fully Reconciled Postings
Includes transactions reconciled internally.
 Example
Outgoing invoices and the reconciled incoming payments are displayed together in the report.
 Note
In the Poland localization, if the Display Fully Reconciled Postings checkbox is selected, down payment invoices are displayed
in the Cash Flow window as forecast transactions with the Customer Liabilities or Payable to Vendors security level.
Add Blanket Agreement
Adds approved blanket agreements to the report calculation.
Add Marketing Documents
Adds selected marketing documents to the report calculation.
Add Document Drafts
Adds selected marketing document drafts to the report calculation.
Add Recurring Transactions
Adds selected recurring transactions to the report calculation.
Tax
Report includes tax transactions.
In the appurtenant field, specify whether to display transactions as they are reported monthly, or every two months, depending on
how your business pays tax.
 Note
This field is not available in localizations using the US tax system.
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:12 AM
Opening Balance/Calculate Opening Balance
Select Opening Balance to enter an opening balance manually for the selected accounts.
Select Calculate Opening Balance to display the opening balance according to the data recorded in SAP Business One.
Include Projected Postings Table
Specify future transactions that have not been recorded yet in SAP Business One, such as the purchase of a new car for the
business, designated to be executed next month.
Specify the following for the expected transactions:
Date – due date
Description – brief text insertion
Incoming Total, Outgoing Amount – incoming or outgoing sum
Security Level – security level at which the report should display them
The report displays the additional transactions in green.
Cash Tab
Displays G/L accounts defined as Cash Accounts in the Chart of Accounts.
Select the accounts to be included in the report. The amounts transferred through these accounts will appear in the report at
security level 1 – Cash Accounts.
Credit Card Tab
Credit funds used when incoming payments for credit card vouchers were created. Amounts transferred through these accounts
will appear in the report at security level 2 – checks and credit.
Checks Tab
Check funds.
Amounts transferred through these accounts appear in the report at security level 2 – checks and credit.
Business Partner
Specify a range, a group, or the properties of business partners to include in the report.
Amounts transferred through these business partners will appear in the report at level 3 – customer liabilities, and security level 4
– payable to vendors.
Cash Flow Window
This window displays the Cash Flow report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cash Flow Window
Cash Accounts, Credit, Checks, Customer Liabilities, Debts to Vendors
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:12 AM
Each option represents a security level. Select the respective options to display in the report according to the relevant security
levels.
Due Date
Each row represents a time interval. The postings are assigned to a time interval according to their due date. Expand the display
mode to see the security levels.
Origin
Transaction type of the postings in each security level and a link to the document by which the transaction was created. The origin
is displayed only when the display is expanded.
Reference
Reference number of the documents/transactions.
Control Account
Control account linked to the transaction.
G/L Account/BP Code
Business partner code or G/L account code involved in the transaction.
 Note
The display of accounts in the Cash Flow report is subject to user authorizations. SAP Business One does not display
confidential accounts if the user is not permitted to access confidential accounts.
Remarks
Details entered in the Remarks field in the transaction or document.
Debit, Credit
Debit or credit amounts for the postings.
Total
Total for a posting, security level, or time interval. Rows representing the security level and time interval are highlighted in blue.
Negative balances are indicated with a minus sign (-).
Balance
Total cumulative amounts.
In each row, the total of the balance of the previous row plus the total amount for the current row is calculated. This means that the
balance is always displayed for each detailed row. Negative balances are indicated by a minus sign (-).
 Note
In the Russia, Hungary, and Czech Republic localizations, down payment invoices and down payment credit memos are not
displayed in the report.
Cash Flow Report
The Cash Flow report is a standard financial statement. It details information relating to cash relevant income and expenses, and
cash equivalents within a defined period.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:12 AM
The report comprises two types of forms:
Primary – Relates to the cash flow of income and expenses during business, investment, and financial activities.
Supplementary – Relates to:
Investment and financial activities not related to cash income and expenses
The cash flow of business activities relating to net profit adjustments
The increase in net value of cash and cash equivalents
Related Information
Cash Flow Reference Report
Cash Flow Statement Selection Criteria
Use this window to specify selection criteria for the cash flow report.
To open this window, choose Financials Financial Reports Financial Cash Flow Report . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the Cash Flow Report window.
Cash Flow - Selection Criteria
Actual Period
Specify a date range for the report.
Previous Period
Specify a date range for the comparison period. Select the checkbox to display the comparison period in the report.
Date
Using the date bar, specify a time frame for the report.
For a report covering an entire year, select the year, click to clear, and click again to select all the months.
For a report that extends to the end of a particular month, select the month.
From … To
Specify a date range for the report.
Template
Specify a template for displaying the report.
Cash Flow Report Window
This window displays the Cash Flow Report according to your defined selection criteria. The report details information relating to
cash relevant income and expenses and cash equivalents within a defined period. In order to generate this report, you must assign
pre-defined cash flow line items to cash relevant transactions.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:12 AM
To access the Cash Flow Statement Selection Criteria window, choose one of the following:
Reports Financials Financial Cash Flow Report .
Financials Financial Reports Financial Cash Flow Report .
After finish defining cash flow report, choose OK to generate cash flow report.
Cash Flow Report
Company
Displays the name of the company database that the user is generating the report from.
From, To
Displays the period in which the report is being generated.
Line Items
The cash flow line items for the 'Primary form' and 'Supplementary form' are listed together with their corresponding line number
and accumulated value in the same window. They are identified by the line item of level 1 displayed in red.
Line No.
The line number represents the line item previously defined in the Define Cash Flow Line Items window.
Actual Period
Displays the value for particular lines according to the template you specified in the selection criteria. This column can be adjusted
by clicking on the Adjust button. Users require full authorization to manually adjust the amount of the cash flow line item.
 Note
You can only change an amount that is independent of a predefined formula.
Previous Period
Displays the value for particular lines according to the template you specified in the selection criteria.
Level
Defines the level of hierarchy for display and printing. The default value is level 10.
Adjust
By selecting this button you are able to manually adjust the amounts in the Amount column. This button is disabled when viewing
a previously saved report.
Related Information
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Creating a Cash Flow Report
Context
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:12 AM
The cash flow report for a particular period shows the accumulated amounts of cash flow line items assigned to cash relevant
transactions.
Procedure
1. From the SAP Business One Main Menu, choose Reports Financials Company Cash Flow Report – Selection
Criteria .
2. Using the date bar in the Cash Flow Statement Selection Criteria window, choose a time frame for the report.
For a report covering an entire year:
a. Select the year, for example, 2006.
b. Click to clear all the months.
c. Click again to select all the months.
For a report that extends to the end of a particular month, select the month.
For a report that extends to a specific date, for example, 10.16.2006, specify the date in the To field.
Business Assessment Report
Context
You can use the financial report templates to create the Business Assessment report. Therefore, you can easily adjust the report
structure according to your needs.
Procedure
1. In the SAP Business One Main Menu, choose Reports Financials Financial Business Assessment Report .
Alternatively, choose Financials Financial Reports Financial Business Assessment Report .
2. In the Business Assessment Report - Selection Criteria window, define the following:
Period: select the posting period in which you want to display the data.
Financial Template: select the template that you want to use. You can find the templates in the Financial Report
Templates window ( Main Menu Financials Financial Report Templates ).
Hide G/L Accounts: select this checkbox to display only the account titles.
Hide G/L Accounts with Zero Balance: select this checkbox to hide the G/L accounts that has a zero balance.
Report Mode: select the report mode you want to use to display the report.
3. Based on your selected report mode, the report displays the following:
Budget Comparison: this report mode displays the expenses, the budgets, and their deviations in the posting period
you selected and the current fiscal year YTD.
Monthly Comparison: this report mode displays the expenses in each month of the fiscal year that includes the
posting period you selected.
Yearly Comparison: this report mode displays the expenses in the posting period you selected, the corresponding
one of its previous fiscal year, the current fiscal year YTD, and the corresponding period of the previous fiscal year.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:12 AM
In the report, you can choose a line to display a list of related journal entries, and also choose link arrows to display
specific journal entries directly from the report.
Comparison
These reports let you review the results of business activities of two posting periods, or compare two companies.
Balance Sheet Comparison
This report compares the balance sheet reports of two companies, or of two periods of the same company, with the same chart of
accounts. Use this window to specify selection criteria for the Balance Sheet Comparison report.
To open the window, choose Financials Financial Reports Comparison Balance Sheet Comparison . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the Balance Sheet Comparison window.
Selection Criteria
Company Name
Name of the company to which you are currently logged on.
Database Name
Name of the database to which you are currently logged on.
Posting Date/Document Date
Specify whether to generate the report according to a posting or a document date range.
From...To
Specify the dates of the first and last day to be included in the report.
Company Name
Name of the company to which the figures of the current company should be compared. By default, the name of the current
company is displayed.
Database Name
Name of the database to which the figures of the current company should be compared. By default, the database of the current
company is displayed.
Change
Opens a window in which you can choose the company to which the figures of the current company should be compared.
 Note
You can only select companies that are located on the same database server as the current company.
Posting Date/Document Date
Specify whether to generate the report according to a posting or a document date range.
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:12 AM
From...To
Specify the dates of the first and last day in the comparison company to be included in the report.
Display in Report
Accounts with Balance of Zero – Report displays accounts with zero balance.
Differences in % – Adds a column displaying the differences between the compared companies or posting periods, as a
percentage.
Amount Differences – Adds a column displaying the differences between the compared companies or posting periods, as a
percentage.
Foreign Name – Displays only foreign names defined for G/L accounts.
 Note
Accounts for which a foreign name was not defined are not displayed in the report.
External Code - Displays external codes defined for G/L accounts in Financials Chart of Accounts External Code .
Local Currency – Displays the results in local currency.
System Currency – Displays the results in system currency.
Foreign Currency – Displays the results in foreign currency.
Template
Specify the template to be used for the report.
Add Journal Vouchers
Includes in the report transactions that are recorded in Open journal vouchers, but are not yet saved in the database.
Add Closing Balances
Includes period-end closing journal entries, for the chosen posting period only, in the report. As such, the Profit Period shows a
zero balance for a closed posting period.
Add Closing Balances is not selected: period-end closing journal entries are not included in the report, and the Profit Period
shows the balance prior to the period-end closing process.
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Choose Segments
Opens the Find G/L Accounts window where you can choose the accounts to include in the report, according to segments.
 Note
Only available if the company maintains a chart of accounts based on segments.
Revaluation
Opens the Balance Sheet Revaluation window where you can make additional selection criteria for revaluation.
Balance Sheet Comparison Window
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:12 AM
This window displays the Balance Sheet Comparison report according to your defined selection criteria.
Balance Sheet Comparison Window
Current Period
The date you entered in the To field for the period of the current database.
Comparison Period
The date you entered in the To field for the comparison period of the current database or a compared database.
Account Name
According to the display level, the names of the drawers (Assets, Liabilities, Equity, and so on), titles, and accounts in the chart of
accounts template.
If you selected Foreign Names in the selection criteria, the foreign names are displayed, as defined for each account in the chart of
accounts.
Current Period
Balance of the drawer, title, or account – according to the selected display level – to the requested date of the current period /
company in the current database, in the selected currency.
Comparison Period
Balance of the drawer, title or account – according to the display level – to the requested date of the compared period/company in
the current or compared database, displayed in the selected currency.
Display Subtotals
Displays a subtotal for each drawer or title, according to the display level.
Level
Select the account level you want to display in the balance sheet comparison.
The balance sheet is displayed at the latest level applied in the window. Level 1 displays a summary of all accounts under the titles
Assets, Liabilities, and Equity.
The transition to a higher level of detail conforms to the levels defined in the Chart of Accounts. Level 2 usually breaks down
assets into current assets, long-term investments, and fixed assets; and liabilities into current and long-term liabilities. The equity
sections include share capital and profit for the period.
Level 5 displays all the active accounts in SAP Business One.
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black.
Difference Amount
Difference between compared periods / Companies according to this accounting formula:
Difference Amount = Current Period / Company - Comparison Period/company
Percentage Difference
Difference between the current period/company and the compared period/company according to the accounting formula:
Percentage Difference = Difference Amount / Compared Period x 100
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:12 AM
Trial Balance Comparison
This report compares the trial balances of two different companies or two different posting periods. Use this window to define
selection criteria for the Trial Balance Comparison Report.
To open the window, choose Financials Financial Reports Comparison Trial Balance Comparison . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the Trial Balance Comparison window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Business Partner
Select to include business partners in the report.
Properties
Open the Properties window and use the business partner properties as selection criteria.
G/L Accounts
Report includes G/L accounts.
Find
To find a special account, choose this button and specify the account code. SAP Business One automatically displays an X next to
this account.
Level
Choose the level of the account display in the table. If you choose Level 1 here, the table displays the highest level titles for the
accounts. If you select a row in the table, you actually select all the accounts that appear under this title.
Company Name
Displays the company and database names of the current company and the comparison company.
Period
In this section, define the periods to be compared by the report:
Current, Comparison – Click and select whether to generate the report according to posting date, due date, or document
date.
From, To, – Define the current period and comparison period by entering the required date ranges. Click to define the
date ranges according to posting periods.
Display in Report
You can select the following options to display in the report:
Hide Zero Balanced Acct – Select this checkbox to exclude zero balanced accounts from the report.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:12 AM
Hide Acct with No Postings – Select this checkbox to exclude accounts with no postings. This checkbox is only available if
Hide Zero Balanced Acct is deselected.
Differences in % - select to display the differences between the compared companies / periods as percentages.
Amount Differences - select to display the differences between the compared companies/periods in amounts.
Foreign Name – to display the foreign names defined for G/L accounts in Financials Chart of Accounts Account
Details Foreign Name .
When this checkbox is selected, only foreign names are displayed. Nothing is displayed for accounts lacking a foreign
name.
External Code - to display external codes defined for G/L accounts in Financials Chart of Accounts External Code .
Opening Balance for Period - Select this checkbox when you need to differentiate between the balance of the selected
posting period and the balance of the previous periods.
As default, the checkbox is deselected. When a date range of a current posting period is selected, you can select this
checkbox to display the bookkeeping balance prior to the selected date range in a separate column, O. B. This opening
balance includes:
Bookkeeping balance prior to the selected date range.
Journal entries created in the selected posting period through Administration System Initialization Opening
Balances (Origin = O.B, Transaction Type = -2).
Period-end closing journal entries of posting periods prior to the selected period.
Local Currency – displays the report in the local currency.
System Currency – displays amounts in the system currency only.
Foreign Currency – displays the report in a foreign currency.
Template
Choose and select a template for displaying the balance sheet.
Add Journal Vouchers
Includes transactions in the report that are recorded as Open in journal vouchers, but have not yet been saved to the database.
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Add Closing Balance
Includes closing balances in the report.
Revaluation
Opens the Trial Balance Revaluation window. After the revaluation is made, the option next to this button is selected.
Expanded
Opens the Expanded Selection Criteria window, where you can use a project range and a distribution rule range as selection
criteria for this report.
Related Information
Revaluation - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:12 AM
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
Properties
Trial Balance Comparison Window
This window displays the Trial Balance Comparison report according to your defined selection criteria.
Trial Balance Comparison Window
Name
The names of the drawers, titles, and accounts according to the display level you selected.
The list of business partners appears in the lower part of the report, divided into customers and vendors.
Current Period
Displays the totals for the debit, credit, and balance of each business partner and/or G/L account in LC/SC/FC (according to the
selection made in the Trial Balance Comparison – Selection Criteria window) for the requested date range for the Current Period
in the current database.
Comparison Period
Displays the totals for debit, credit, and balance of each business partner and/or G/L account (according to the selection made in
the Trial Balance Comparison – Selection Criteria window) for the requested date range of the Comparison Period in the current
database or in the compared database.
Differences in Amounts
The difference between the compared periods according to the accounting formula:
Differences in Amounts = Current Period - Previous Period
Differences in Percentage
The difference between the current period and the comparison period according to the accounting formula:
Differences in Percentage = Differences in Amounts / Previous Period x 100
Level
The trial balance comparison is always displayed at the last level established in the window. Level 1 displays a summary of all
accounts under the titles (Assets, Liabilities, Equity, and so on), and a summary of Customers and Vendors.
If you are interested in more detail than is provided in Level 1, choose the appropriate level in the Trial Balance Comparison
window.
The transition to a higher level of detail conforms to the levels you defined in the Chart of Accounts. Display at Level 2 usually
breaks down assets into current assets and long-term investments; customers and vendors are divided into groups.
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black. A title is also
displayed slightly to the left of the active account or to the left of the subtitle below it.
The subtitle for a title is shown immediately after the displayed title.
Current Period From To
The dates you entered as the date range for the Current Period in the Trial Balance Comparison – Selection Criteria window.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:12 AM
Comparison Period From To
The dates you entered in the Trial Balance Comparison – Selection Criteria window as the date range for the Comparison Period
in the current database or in the compared database.
Profit and Loss Statement Comparison - Selection Criteria
This report lets you compare the profit and loss statements of two companies or periods. Use this window to specify selection
criteria for the profit and loss statement comparison report.
To open the window, choose Financials Financial Reports Comparison Profit and Loss Statement Comparison .
Alternatively, open it from the Reports module.
After defining the report, you can view it in the Profit and Loss Statement Comparison window.
Selection Criteria
Current Company
The following fields contain data from the current company:
Company Name, Database Name – System displays the current company and database names, as they appear in the
Choose/Create Company window.
Date, From...To ...– Click and specify whether to generate the report according to posting date, due date, or document date.
Then define the date range for transactions to include in the report.
Click to define a range based on posting periods.
Comparison Company/Posting Period
The following fields contain data from the company or posting period to which you are comparing the current company/period:
Company Name, Database Name, Change – The defaults displayed are the current company name and the current
database name, as they appear in the Choose/Create Company window. Choose Change to select a different company.
Date, From...To ...– Click and specify whether to generate the report according to posting date, due date, or document date.
Then define the date range for transactions that you are including in the report. Click to define a range based on posting
periods.
Display in Report
You can select the following options to display in the report:
Accounts with Balance of Zero – if this checkbox is not selected accounts with balance of zero will not be displayed in the
report.
Differences in % - select this option to add to the report a column which displays the differences between the compared
companies/posting periods in percentage rate.
Amount Differences - select this option to add to the report a column which displays the differences between the
compared companies/posting periods in percentage rate.
Foreign Name – to display the foreign names defined for G/L accounts in Financials Chart of Accounts Account
Details Foreign Name .
When this checkbox is selected, only foreign names will be displayed, therefore nothing will be displayed in case of
accounts for which the foreign name was not defined.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:12 AM
ExternalCode - to display external codes defined for G/L accounts in Financials Chart of Accounts External Code .
LocalCurrency – select to display the results in local currency.
SystemCurrency – select to display the results in system currency.
ForeignCurrency – select to display the results in foreign currency.
Template
Specify the template to use for the report.
Add Journal Vouchers
Includes transactions in the report that are recorded as Open in journal vouchers, but have not been saved yet in the database.
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Choose Segments
Opens the Find G/L Accounts window, in which you can select the accounts to include in the report, according to segments.
 Note
Appears only if the company maintains a chart of accounts based on segments.
Revaluation
Choose to open the Balance Sheet Revaluation window. After you make your selections and close this window, the option next to
the button is selected.
Expanded
Opens the Expanded Selection Criteria window, in which you can define additional parameters for the report.
Related Information
Expanded Selection Criteria
Profit and Loss Statement Comparison Window
This window displays the Profit and Loss Statement Comparison report according to your defined selection criteria.
Profit and Loss Statement Comparison Window
Account Name
Displays the names of the drawers (Revenues, Cost of Sales, Expenses, and so on), titles and accounts, according to the display
level you selected, and the selections made in the Profit and Loss Statement Comparison – Selection Criteria window.
Current Period
Displays the balance of the drawer, title, or account (according to the selected display level) to the requested date of the Current
Period in the current database.
Comparison Period
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:12 AM
Displays the balance of the drawer, title, or account (according to the selected display level) to the requested date of the
Comparison Period in the current database or in the compared database.
Difference Amount
Difference between compared periods according to the accounting formula:
Difference Amount = Current Period - Previous Period
Percentage Difference
The difference between the current period and the comparison period according to the accounting formula:
Percentage Difference = Difference Amount / Previous Period x 100
Display Subtotals
Displays subtotals for each title and drawer.
Level
The Profit and Loss comparison is always displayed at the last level established in the window. Level 1 displays a summary of all
accounts under the titles Revenues, Cost of Sales, Expenses, and so on.
For more detail than is provided in Level 1, select the appropriate level in the Profit and Loss Comparison window.
The transition to a higher level of detail will conform to the Levels you defined in the Chart of Accounts.
Level 2 displays greater detail – primary titles and primary accounts.
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black. A title is also
displayed slightly to the left of the active account or the subtitle below it.
The subtotal for a title is shown immediately after the displayed title.
Current Period From To
The dates you entered in the date range for the Current Period in the Profit and Loss Statement Comparison – Selection Criteria
window.
Comparison Period From To
The dates you entered in the Profit and Loss Statement Comparison – Selection Criteria window, as a date range for the
Comparison Period in the current database or in a compared database.
Budgets
If your company manages budgets, you can create a budget report to review business activities from a budget perspective.
Budget Report
This report analyzes the business activities that took place during a defined period, with reference to a selected budget scenario.
Use this window to specify its selection criteria.
To open the window, choose Financials Financial Reports Budget Setup Budget Report . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the Budget Report window.
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:12 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Annual Report, Quarterly Report, Monthly Report
Specify the time frame of the report.
Local Currency, Display in SC
Specify whether to display the report in local currency or in system currency.
Scenario
Specify the scenario according to which the report will be created.
Distr. Rule
Specify the distribution rule for which to create a report reflecting the budget used for the cost accounting activities.
 Note
If you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General Settings window under
Administration System Initialization General Settings , you can select distribution rules of specific dimensions from the
dropdown lists. Only active dimensions are editable.
Project
Specify a project for which to create a report reflecting the budget used for the project.
Future Balances
Includes open purchase orders, open purchase requests, and open purchase delivery notes in the Future column of the report.
Find
Opens the Find G/L Accounts window, where you can select specific G/L accounts for the report.
Account
Specify the G/L accounts you want to include in the report.
[Level]
Specify the detail level of the account display in the account table. Level 1 displays the drawers, Level 2 drills down to the main
titles, and so on.
Date From...To...
Date range of the report, as defined in the months table below.
Date
Specify the year for the report. Then, select the month or months for which the report should be created. The Date From...To...
fields are updated accordingly.
Related Information
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:12 AM
Budget Report Window
This window displays the Budget Report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Budget Report Window
Display Subtotals
Displays a subtotal for each title and drawer.
Budget
Budget amount for the account as specified in the Define Budget window.
Actual
Actual amount used of the budget amount.
Difference
Difference between the budget amount and the actual balance.
Chart Style
Specify the style of the graphic display.
[Level]
Specify the detail level of the account display in the account table. Level 1 displays the drawers, Level 2 drills down to the main
titles, and so on.
Balance Sheet Budget Report
This report displays a balance sheet based on a selected budget scenario. Use this window to specify selection criteria for the
Balance Sheet Budget report.
To open the window, choose Financials Financial Reports Budget Reports Balance Sheet Budget Report . Alternatively,
open it from the Reports module.
After defining the report, you can view it in the Balance Sheet Budget Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Date
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:12 AM
Specify the year, then click the month or months for which the report should be created. The date field below is updated
accordingly.
External Code
Displays external codes that you defined for G/L accounts in Financials Chart of Accounts External Code .
Ignore Adj. Trans. (Period 13)
Report excludes adjustment transactions.
Accounts with Balance of Zero
Report includes accounts with zero balance.
Budget-Relevant Accounts Only
Report includes only G/L accounts defined as relevant to the budget.
Foreign Names
Displays foreign names that you have defined for G/L accounts in Financials Chart of Accounts Account Details Foreign
Name .
Choose Segments
Opens the Find G/L Accounts window, where you can select the accounts to include in the report, according to segments.
 Note
Only available if the company maintains a chart of accounts based on segments.
Balance Sheet Budget Report Window
This window displays the Balance Sheet Budget report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Balance Sheet Budget Report Window
As of
Date specified in the To field in the selection criteria.
Display Subtotals
Displays subtotals opposite each title.
Level
The report is displayed at the latest level applied in the window. Level 1 displays a summary of all accounts under the Assets,
Liabilities, and Equity titles.
If you want more details, choose the appropriate level.
The transition to a higher level of detail conforms to the levels you defined in the Chart of Accounts. Level 2 usually breaks down
assets into current assets, long-term investments, and fixed assets; and liabilities into current and long-term liabilities. The equity
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:12 AM
sections include share capital and profit for the period.
Level 5 displays all the active accounts in SAP Business One.
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black.
Budget
Planned amount for the account as specified in the Define Budget window.
Actual
Actual balance of the account.
Difference
Difference between planned amount and the actual balance.
Trial Balance Budget Report
This trial balance report is based on a specific budget scenario. Use this window to specify selection criteria for the report.
To open the window, choose Financials Financial Reports Budget Reports Trial Balance Budget Report . Alternatively,
open it from the Reports module.
After defining the report, you can view it in the Trial Balance Budget Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
G/L Accounts
Report includes G/L accounts.
Find
To find a special account(s), choose this button and specify the account code or range of account codes. SAP Business One
automatically displays an X next to this account(s).
Level
Choose the level of the account display in the table.
If you choose Level 1 here, the table displays the highest level titles for the accounts. If you select a row in the table, you actually
select all the accounts that appear under this title.
Posting Date / Due Date / Document Date
Click the icon and choose to display the report according to posting date, due date or document date range.
Scenario
Preferred budget scenario (displayed according to the selected financial period).
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:12 AM
Display LC, Display in SC
Select whether to display the report in local currency or in system currency
External Code
Select this option to display external codes that you have defined for G/L accounts in their master records ( Financials Chart
of Accounts External Code ).
Ignore Adjustments
Report excludes adjustment journal entries from its balance calculation.
Hide Zero Balanced Acct
Select this checkbox to exclude zero balanced accounts from the report.
Hide Acct with No Postings
Select this checkbox to exclude accounts with no postings. This checkbox is only available if Hide Zero Balanced Acct is
deselected.
Budget Accounts Only
Select this option to include in the report only G/L accounts that were defined as relevant to the budget ( Financials Chart of
Accounts Account Details Relevant to Budget ).
Foreign Names
Select this option to display foreign names that you have defined for G/L accounts in their master records ( Financials Chart of
Accounts Account Details Foreign Name ).
Expanded
Opens the Expanded Selection Criteria window, where you can define the range of projects and/or profit centers as additional
parameters for the report.
Related Information
Finding G/L Accounts to Include in Financial Reports/Period-End Closing
Trial Balance Budget Report Window
This window displays the Trial Balance Budget report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Trial Balance Budget Report Window
From Date To
Displays the dates you entered in the range of dates in the Trial Balance Budget Report – Selection Criteria window.
Budget
The planned amount for each account as specified in the Define Budget window.
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:12 AM
Actual
Actual balance of this account.
Difference
Difference between planned amount and actual balance.
Difference in %
Calculates the difference in percentage.
Level
Level 1 displays a summary of all accounts under titles such as Assets, Liabilities, Equity, and so on.
If you are interested in more detail than is provided in Level 1, select the appropriate level in the Trial Balance Budget Report
window.
The transition to a higher level of detail will conform to the levels you defined in the chart of accounts.
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black. A title is also
displayed slightly to the left of the active account or the subtitle below it.
Profit and Loss Statement Budget Report
This report displays a profit and loss statement based on a selected budget scenario.
Profit and Loss Statement Budget Report - Selection Criteria
Use this window to specify selection criteria for the Profit and Loss Statement Budget Report.
To open the window, choose Financials Financial Reports Budget Profit and Loss Statement Budget Report .
Alternatively, open it from the Reports module.
After defining the report, you can view it in the Profit and Loss Statement Budget Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Date
In the ruler, select the required period.
Posting Date / Due Date / Document Date
Specify whether to create the report according to the posting date range, the due date range or the document date range.
Scenario
Select the budget scenario according to which the report should be generated.
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:12 AM
Local Currency
Displays the report figures in local currency.
System Currency
Displays the report figures in system currency.
External Code
Displays the external codes of the accounts in the report, as defined in Financials Chart of Accounts External Code field.
Ignore Adj. Trans. (Period 13)
Generates a report without adjustment transactions.
Accounts with Balance of Zero
Report includes zero-balance accounts.
Budget-Relevant Accounts Only
Report displays only accounts with a budget amount.
Foreign Names
Displays the foreign name of the accounts in the report, as defined in Financials Chart of Accounts Account Details
Foreign Name field.
Annual / Quarterly / Monthly Report
Specify the required display mode for the report.
Choose Segments
Opens the Find G/L Accounts window, where you can select the accounts to include in the report, according to segments.
 Note
Only available if the company maintains a chart of accounts based on segments.
Expanded
Opens the Expanded Selection Criteria window where you can define a range of projects and/or profit centers as additional
parameters for the report.
Profit and Loss Statement Budget Report Window
This window displays the Profit and Loss Statement Budget Report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Profit and Loss Statement Budget Report Window
Date From...To...
The dates you specified in the selection criteria.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:12 AM
Display Subtotals
Displays subtotals above each title for levels higher than Level 1.
Budget
Planned amount for the account as specified in the Define Budget window.
Actual
Actual balance of the account.
Difference
Difference between planned amount and actual balance.
Difference in %
Difference in percentage.
Level
The report is always displayed at the last level established in the window.
Level 1 displays a summary of all accounts under the titles Revenues, Cost of Sales, Expenses, and so on.
For more detail, select the appropriate level. The transition to a higher level of detail will conform to the levels you defined in the
Chart of Accounts.
Level 2 displays greater detail – primary titles and primary accounts.
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black. A title is also
displayed slightly to the left of the active account or the subtitle below it. The subtotal for a title is shown behind the displayed
title.
Support for IFRS in SAP Business One
SAP Business One includes a number of enhanced features that support companies in the preparation of financial statements
according to International Financial Reporting Standards (IFRS) in addition to their group reporting and also any other GAAP
reporting needs.
Accurate reporting in SAP Business One depends not only on functionality, but also on correct setup and handling. Additionally,
SAP Business One localizations vary according to different local GAAP requirements. Therefore we strongly recommend that you
consult with your SAP partner and your company accountant when identifying what your IFRS requirements are, how to
implement them, and which authorizations to define for them. You are responsible for carrying out all the appropriate operations
and providing the appropriate documentation to ensure the accuracy and completeness of your financial reports.
 Note
Both SAP Business One IFRS-related capabilities and the IFRS are subject to future change.
Preparing for Financial Reporting According to IFRS
Before you start adjusting your SAP Business One application for the purpose of preparing financial statements according to IFRS,
we strongly recommend that you follow the steps below:
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:12 AM
1. Analyze the differences between the local GAAP and IFRS. The most common differences are:
Valuation and depreciation of fixed assets
Foreign currency valuation
Provisions
Inventory valuation
Revenue and cost recognition
2. Identify which differences are relevant for your company.
3. Minimize the number and extent of the differences as much as possible (for example, by adjusting the internal accounting
policy).
4. Prepare the internal accounting policy to support the preparation of financial statements according to IFRS.
Basic Concepts of the IFRS Setup
You have the following options regarding how IFRS is implemented and used at your company:
Parallel postings to specifically created G/L accounts
Using reference fields and user-defined fields to mark journal entries and then setting filters accordingly in the reports’
selection criteria
A combination of these two methods
The following figure shows you the recommended accounts setup for the two different types of reporting:
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:12 AM
Recommended Accounts Setup
Parallel Accounting Systems
Business transactions can have different meanings and/or valuation for local GAAP and for IFRS purposes. You can create different
types of G/L accounts in the chart of accounts to support both local GAAP and IFRS-related postings. If your company needs to
report according to both the local GAAP and to IFRS, the chart of accounts can include three types of G/L accounts:
Local G/L accounts – for local GAAP purposes only
IFRS G/L accounts – for IFRS purposes only
Common G/L accounts – for both local GAAP and for IFRS purposes
 Recommendation
Use different G/L account codes and/or names to indicate the type of G/L account.
Example
41100 – Sales Revenue – Domestic
IFRS – 41110 – Sales Revenue – Domestic
Local – 41120 – Sales Revenue – Domestic
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:12 AM
You cannot change an account code once the account already has postings. However, you can change existing account names.
 Note
SAP Business One allows a maximum length of 15 characters for G/L account codes and of 100 characters for G/L account
names.
Possible Scenarios
SAP Business One allows you to cover the following scenarios in your accounting system:
A transaction has the same impact for the local GAAP and for the IFRS rules. The transaction is posted to the common G/L
accounts; for example, a purchasing invoice for services.
A transaction has different valuations for the local GAAP and for IFRS. It is posted in parallel to both local and IFRS G/L
accounts; for example, pension liabilities or depreciation of fixed assets.
A transaction is required only by local GAAP rules. It is posted to local G/L accounts only; for example, a specific provision.
A transaction is required only by IFRS rules. It is posted to IFRS G/L accounts only; for example, financial leasing.
A transaction is required only by local GAAP rules or only by IFRS rules. It is posted to the common accounts. When the
GAAP and IFRS reports are created, you filter the relevant postings based on selection criteria for reference fields and user-
defined fields. For example, 3 of 10 postings to a common account are not relevant for IFRS, so you exclude them from the
IFRS report based on selection criteria filters.
The following figure shows account postings for the first four of these scenarios:
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:12 AM
Examples of Postings to Common Accounts, Local GAAP Accounts, and IFRS Accounts
Manual Postings
You adopt one of the following approaches for manual parallel postings to local GAAP accounts and to IFRS accounts:
Posting only local transactions and marking them as local. At the end of the financial year, filtering the transactions and
manually creating relevant postings for IFRS purposes, transaction by transaction.
Posting only local transactions, and marking them as local. At the end of the year, filtering the transactions and manually
creating relevant postings for IFRS as aggregate transactions.
 Note
When you are setting up IFRS, make sure to discuss with your partner and your company accountant which IFRS postings will
be made manually and which IFRS postings, if any, can be made automatically. The standard case is that the majority of IFRS
postings are done manually.
As an alternative to the manual posting scenarios (see above), you can manually create documents twice, once for local GAAP
and once for IFRS. In this case, a second numbering series is required for each affected document type. Automatic parallel
posting to the accounts is done by specifying the account in the invoice.
Creating an IFRS Setup in SAP Business One
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:12 AM
Prerequisites
You have made the necessary preparations as described in Support for IFRS in SAP Business One.
Procedure
1. Create additional IFRS accounts and rename existing accounts, as required. For more information, see Chart of Accounts.
2. If required, adjust the settings that determine which G/L accounts are posted when transactions occur in SAP Business
One. For more information, see G/L Account Determination.
 Note
The standard case is that IFRS postings are done manually. Discuss with your partner and with your company
accountant whether there are any IFRS postings that you can post automatically.
3. Check and, if necessary, adjust the predefined values for the reference fields and any user-defined fields in journal entries.
For more information, see the topic Setting Up Reference Field Links and UDF Links for IFRS.
4. If you use automatic or semi-automatic internal reconciliation, decide whether to set any of the reference fields as
matching rules (automatic) or reference parameters (semi-automatic). Define these settings as necessary.
In business partner internal reconciliation, you can use Ref. 1 (BP Row), Ref. 2 (BP Row), and/or Ref. 3 (BP Row). In G/L
internal reconciliation, you can use Ref. 1 (Row), Ref. 2 (Row), and/or Ref. 3 (Row).
 Note
These settings affect the reconciliation process, not IFRS directly.
5. Define the financial report templates that you want to use for IFRS. The templates will include a mix of IFRS accounts and
common accounts.
a. For G/L accounts that you intend to include more than once in the same template, set the checkbox Allow Multiple
Linking to Financial Templates in the G/L Account Details window.
This is useful if you need to include the debit and the credit sides of an account rather than the overall balance, one
side in the assets section and the other side in the liabilities section of the balance sheet.
 Example
You want the VAT account to be part of an assets account group if the closing balance is positive (+) and part of a
liabilities account group if the closing balance is negative (-).
b. Create the financial report templates that you intend to use for IFRS.
In the Account Category - Details window, adjust the values in the Linked and Sign fields as required. For more
information, see the topic Account Category - Details Window.
For general information about how to create financial templates, see Creating Financial Report Templates and
Creating Financial Report Templates Based on Existing Templates.
c. Review which accounts are linked to which balance sheet templates by choosing Tools Queries System
Queries G/L Account Location in Balance Sheet Templates .
6. Decide which G/L accounts to use in which reports.
For information about how to find and select the relevant G/L accounts for a report, see the topic Finding G/L Accounts to
Include in Financial Reports/Period-End Closing.
7. If you have not already done so, check and adjust the user authorizations for your company as required for IFRS.
8. Manually create any parallel postings that are required for IFRS. For more information, see the sections Basic Concepts of
the IFRS Setup and Manual Postings in the topic Support for IFRS in SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:12 AM
9. Before creating the following reports, specify the selection criteria for reference fields and user-defined fields as your
company requires them for IFRS:
G/L report
Document journal
Trial balance
Balance sheet
Profit and loss statement
For more information, see the topic Setting Filters on Reports for IFRS.
10. Generate the financial reports as required by your company for IFRS.
11. Generate the following inventory reports as required by your company for IFRS:
Inventory valuation method report
Inventory valuation simulation report
Inventory audit report
Related Information
Inventory Valuation Method Report
Inventory Valuation Simulation Report
Inventory Audit Report
Setting Up Reference Field Links and UDF Links for IFRS
Context
SAP Business One gives you considerable flexibility to differentiate and analyze the effect of business transactions in your financial
reports, based on values in reference fields and in user-defined fields (UDFs).
To enable you to record specific source document information with the journal entries in the accounting system, SAP provides a
number of reference fields in the journal entry to which values can be copied from the source document. A source document in this
context can be any document in SAP Business One that gives rise to journal entries and therefore affects the financial accounts.
SAP Business One comes with predefined values for the reference fields – which differ depending on the source document – but
you can overwrite the predefined values, either when setting up your system (for example, for IFRS purposes) or when manually
creating a journal entry. For example, your company may need to store varying or additional information as part of journal entries,
either for its day-to-day work or for IFRS or in order to fulfill localization-specific, industry-specific, or legal requirements.
 Caution
You can change the reference field and UDF links at any time. However, we recommend that you set up these links in advance of
the financial year in which you produce IFRS reports and only change the links at the end of the financial year and prior to the
start of the next financial year.
Make sure you discuss and validate these changes with your company account and partners in relation to how these changes
will impact automatic or semiautomatic reconciliation, bank statement processing, and other financial processes as well as any
partner add-ons or other enhanced functionality such as formatted search.
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:12 AM
Target Fields
The following reference fields are available:
Ref. 1 (header)
Ref. 2 (header)
Ref. 3 (header)
Ref. 1 (BP row)
Ref. 1 (row)
Ref. 2 (BP row)
Ref. 2 (row)
Ref. 3 (BP row)
Ref. 3 (row)
“Header” refers to the header of the journal entry. “BP row” refers to the journal entry row with the business partner control
account. “Row” refers to the journal entry row with the standard G/L account.
You can also copy to any user-defined field in the journal entry, apart from to the following combinations of type and structure:
Type Structure
General Link
General Image
Alphanumeric Text
Source Fields
With regard to the source fields, you can copy from selected fields in business documents that create accounting entries. Fields
that are automatically copied to other fields in journal entries – such as the due date, posting date, or document date – are not
available for copying to reference fields as well. However, with that exception, you may copy from the same source field to multiple
target fields.
Fields that are available for copying from a business document are available as a dropdown list for each reference field.
 Note
You can copy from standard fields or from user-defined fields on header level only, not on line level.
Special Considerations
There are some special considerations that you need to be aware of for the documents of payments, landed costs, and inventory
transfers as well as for form settings and user-defined field verification. For more information, see Reference Field Definition:
Special Considerations.
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup General Reference Field Links .
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:12 AM
2. In the Reference Field Links – Setup window, double-click the initial column next to the business document whose
reference links you want to review.
3. In the Reference Field Links – Definition window, review the predefined values for each reference field and also for any
user-defined fields.
In the left column (entitled Field Name), you see the name of the reference field or user-defined field in the journal entry. In
the middle column (entitled Field Value), you see in a dropdown list the names of the available fields from the respective
document. In the right column (entitled Default Value), you see the predefined SAP value for that field.
Make adjustments as required.
4. To save your settings, choose Update and choose OK in first the Reference Field Links – Definition window and then the
Reference Field Links – Setup window.
Results
From now on, whenever a journal entry is created, the reference fields and any user-defined fields in the journal entry are filled
according to the values you have defined for the respective document.
Any changes to the reference field links and/or user-defined field links of a document are indicated by the status Customized in
the Reference Field Links – Setup window, while documents with all default source fields are shown with the status Original.
Reference Field Definition: Special Considerations
Before you define reference field links and user-defined field links for journal entries, we recommend that you consider the features
and special cases described below.
For general information about this task, see Setting Up Reference Field Links and UDF Links for IFRS.
Form Settings
In the Form Settings window for journal entries, all of the reference fields for the header are on the General subtab of the
Document tab and the reference fields for the grid are on the Table Format tab.
Incoming and Outgoing Payments
Ref. 2
The Ref. 2 field in the journal entry is not copied directly from the Reference field in the payment document. Instead, it is copied
from a field that is not visible on the user interface, the Ref. 2 field in the payments table on the database.
The standard behavior is that SAP Business One copies the field value from the payment document to the field in the database,
and then from the field in the database to the field in the journal entry. However, if you use a partner add-on that modifies the value
of the Ref. 2 field in the payments table, this logic does not apply.
Ref. 3
The value that is copied to the Ref. 3 field for rows depends on the payment means. However, if you select a value other than
Default in the Reference Links – Definition – Incoming/Outgoing Payments window for Reference 3 – BP Row or Reference 3 –
Row, this is the value that is then copied to these rows for all payment means.
If you leave the value for rows as predefined by SAP – that is, as Default –, the value that is copied depends on the payment
means, as shown in the following table:
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:12 AM
Source Value Copied
BP row Payment number (document number)
Check Check number
Contra payment row Payment number (document number)
VAT correction and discount Payment number (document number)
Rate difference row Payment number (document number)
Credit card payment row Voucher number
Split credit voucher Voucher number/index
Any other row Empty
Remarks
The Remarks field in journal entry rows is not copied from the Doc. Remarks field from payments for G/L accounts. To configure
this, select Details for Remarks – Row in the definition page for incoming payments, and Description for Remarks – Row in the
definition page for outgoing payments.
Landed Costs
The source field Reference 1 in the Reference Links – Definition – Landed Costs window corresponds to the Reference field in the
landed costs document.
The source field Reference 2 that is shown in the Reference Links – Definition – Landed Costs window is not otherwise visible on
the user interface. The only way to edit the value in this field is through the SAP Business One Software Development Kit (SDK).
Inventory Transfers
The source field Reference 2 that is shown in the Reference Links – Definition – Inventory Transfers window is not otherwise
visible on the user interface. The only way to edit the value in this field is through the SAP Business One Software Development Kit
(SDK).
Verification of User-Defined Fields
When defining reference links to user-defined fields, you need to ensure the following:
That the source and target field types match
That the source and target field lengths match
That the source and target field values match
That any truncation due to the target field being shorter than the source field is acceptable, or else change the definition of
the target field
That the target field is none of the following combinations:
Type Structure
General Link
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:12 AM
Type Structure
General Image
Alphanumeric Text
If the application detects any of these situations, you receive an appropriate system message.
Setting Filters on Reports for IFRS
Context
SAP Business One allows you to filter your financial reports and accounting reports according to the level of granularity your
company requires for IFRS. You do this by specifying selection criteria for the reference fields and user-defined fields that were
defined in Administration Setup General Reference Field Links .
Procedure
1. Open the selection criteria window of one of the following reports:
General ledger
Document journal
Balance sheet
Trial balance
Profit and loss statement
2. Choose the Expanded button.
The Expanded Selection Criteria window opens.
3. To the right of the Reference Fields checkbox, click the button or click the Reference Fields checkbox.
4. In the Reference Fields window, specify the following data for one or more reference fields:
Field Description
Field Displays the reference field name and position in the following order:
Ref. 1 (header)
Ref. 2 (header)
Ref. 3 (header)
Ref. 1 (BP row)
Ref. 1 (row)
Ref. 1 (all rows)
This setting applies to both Ref. 1 (BP row) and Ref. 1 (row).
Ref. 2 (BP row)
Ref. 2 (row)
Ref. 2 (all rows)
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:12 AM
Field Description
This setting applies to both Ref. 2 (BP row) and Ref. 2 (row).
Ref. 3 (BP row)
Ref. 3 (row)
Ref. 3 (all rows)
This setting applies to both Ref. 3 (BP row) and Ref. 3 (row).
Rule To determine how to filter the values for a particular field, select one of the following from the
dropdown list:
Equal
Not Equal
In Range
Out of Range
Greater than
Greater or Equal
Smaller than
Smaller or Equal
Contains
Does Not Contain
Start with
End with
Is Empty
Is Not Empty
If you do not want to filter this reference field, do not specify a rule.
Value Specify the required value for each field that you filter.
To Value If the rule that you selected is either In Range, or Out of Range, specify a value. For all other rules,
this field is disabled.
5. Optionally, do one or more of the following:
To cancel the operation, choose the Cancel button.
To clear all values in the window, choose the Clear button.
6. To save your settings and to return to the Expanded Selection Criteria window, choose the OK button.
The Reference Fields checkbox now appears as selected.
7. To set one or more filters based on user-defined fields, click the button to the right of the User-Defined Fields
checkbox or click the User-Defined Fields checkbox, and proceed as described in steps 3–5 above.
Once you have set filters on user-defined fields, the User-Defined Fields checkbox appears as selected.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:12 AM
User-defined fields of the following definition types and structures are not available:
Type Structure
General Link
General Image
Alphanumeric Text
8. To return to the selection criteria window, choose the OK button.
Results
The respective financial reports and accounting reports are generated according to the rules and values that you have defined in
this procedure.
Reports based on these filters have the following features:
The logical operator between the filters – that is, between the rows in the definition table – is AND not OR.
Any filter settings that were made against the All Rows option affect both accounting entries in the report (BP row and
row).
In the balance sheet, trial balance, and profit and loss statement, the printed/printable report's selection criteria shows the
filters on reference fields and/or user-defined values that were used to generate the report.
In the general ledger and document journal, the reference fields and user-defined values are displayed in the detailed views
of the report results. You can activate/deactivate the display of these fields in the Form Settings window in exactly the
same way as you can for standard fields.
Related Information
General Ledger
Document Journal
Balance Sheet
Trial Balance
Profit and Loss Statement
Finding G/L Accounts to Include in Financial Reports/Period-End
Closing
Context
You can specify through detailed selection criteria which accounts should be included in your company's financial reports and
which accounts should be included in period-end closing.
In the case of financial reports, these selection criteria help you prepare the reports according to the following groups:
Common accounts and local G/L accounts = for local GAAP reports
Common accounts and IFRS G/L accounts = for IFRS reports
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:12 AM
To find and select the required accounts, follow the procedure below.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting .
2. Open the selection criteria window of one of the following reports, or of the period-end closing transaction:
Financials — Financial Reports — Accounting
G/L Accounts and Business Partners
General Ledger
Document Journal
Financials — Financial Reports — Financial
Trial Balance
Financials — Financial Reports — Comparison
Trial Balance Comparison
Financials — Financial Reports — Budget
Budget Report
Trial Balance Budget Report
Administration — Utilities
Period-End Closing
Alternatively, you can open any of the above reports from the Reports module.
3. To clear previous G/L account selections, click the “x” sign at the top of the accounts grid.
 Note
If you do not clear previous account selections, these are added to the newly made account selections and the results
are displayed cumulatively.
4. Choose the Find button.
5. In the Find G/L Accounts window, select whether you want to identify the relevant G/L accounts for the report by segment
or by G/L account.
If your company does not use account segmentation, skip this step.
6. Depending on what you specified in the previous step, do one of the following:
Specify by G/L account codes or by G/L account names, or a mixture of both, which accounts are to be included or
excluded in the respective report, together with the appropriate filtering rules.
 Note
If the rule that you have selected is either In Range or Out of Range, you must specify a value in the To Value
column. For all other rules this field is disabled.
Perform one or more of the following actions, as required:
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:12 AM
To perform this task... Do this...
Create a new row Right-click an existing row and choose Duplicate Row.
Alternatively, from the menu bar, choose Data
Duplicate Row .
Delete a row Right-click the row and choose Delete Row. Alternatively,
from the menu bar, choose Data Delete .
 Note
If the window contains only one account code row and
you delete this row, you can only create further account
code rows by choosing Restore. The same applies if you
delete a single account name row.
Cut/copy, and paste a value from one row to another Click the source cell and choose Cut or Copy. Then click
the target cell and choose Paste.
Delete a value from a row without deleting the entire row Click the cell and choose Delete.
Restore the window to its original state, with one empty row Right-click a row and choose Restore.
for account code and another empty row for account name
Cancel the current operation Choose the Cancel button.
Remove all rules and values, while retaining the same Choose the Clear button.
number of rows as well as the Field column
Transfer the specified accounts to the selection criteria Choose the OK button.
 Note
The relationship between the selection criteria is such that if you specify more than one row, the OR condition
applies.
Specify according to segments or segment ranges which G/L accounts are to be included in the report.
This radio button is available only if your company uses account segmentation, that is, if you have selected the Use
Segmentation Accounts checkbox on the Basic Initialization tab in Administration System Initialization
Company Details .
7. Specify the other selection criteria and verify that the accounts marked with an “x” in the accounts grid are the ones you
require.
8. To apply the specified filters to the report, choose the OK button.
Results
G/L accounts are displayed in the financial reports according to the rules and values, or the segments, that you defined in the Find
G/L Accounts window.
 Note
The settings you make in the Find G/L Accounts window are retained in the application until you change them. However, it is
not possible to save them as part of an entire set of selection criteria for the report.
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:12 AM
Account Category - Details Window
When you create financial report templates, the account hierarchy display is limited to 4 levels only, while in the chart of accounts
there may be up to 8 levels depending on your localization.
To display the child accounts located under a specific account, double-click this account in the Financial Report Templates
window. The Account Category – Details window appears.
Account Category – Details
G/L Account, Account Name
The code and name of the accounts located under the selected account in chart of accounts.
Linked/Sign
The fields define whether the overall balance, the debit side of the account, or the credit side of the account is included in this
account category of the balance sheet, and how the value being positive or negative influences the result.
 Example
You want the VAT account to be part of an assets account group if the closing balance is positive and part of a liabilities account
group if the closing balance is negative. You therefore link the account as a debit with a + sign under assets and also as a credit
with a - sign under liabilities.
The default is Balance in the Linked field with the Sign field empty. If you overwrite the default value in the Linked field and the
checkbox Allow Multiple Linking to Financial Templates has not been selected in the G/L Account Details window, the application
issues a warning message but you are not prevented from saving the change.
After an upgrade from a previous release version of SAP Business One, the results for accounts linked using the checkbox Transfer
Accounts with Negative Sign are as follows:
The Linked field value is Balance.
If the account balance is a positive value, the Sign field value is +.
If the account balance is a negative value, the Sign field value is –.
 Note
Values are included differently in the asset accounts and the liabilities accounts, according to the following logic:
Asset Accounts
Linked Sign Included in this account group if the
following applies:
Balance + Debit > Credit
(Balance = Debit – Credit)
Balance - Debit < Credit
(Balance = Debit – Credit)
Balance Included regardless of whether the value is
positive or the value is negative
(Balance = Debit – Credit)
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:12 AM
| Linked | Sign |     | Included in this account group if the |
| ------ | ---- | --- | ------------------------------------- |
following applies:
If the checkbox Accounts with Balance of
Zero is selected in the Balance Sheet –
Selection Criteria window, G/L accounts
with a balance of 0 (zero) are also
included.
| Debit | +   |     | Debit > 0                                   |
| ----- | --- | --- | ------------------------------------------- |
| Debit | -   |     | Debit < 0                                   |
| Debit |     |     | Included regardless of whether the value is |
positive or the value is negative
  Note
If the checkbox Accounts with Balance of
Zero is selected in the Balance Sheet –
Selection Criteria window, G/L accounts
with a balance of 0 (zero) are also
included.
| Credit | +   |     | 0 > Credit                                  |
| ------ | --- | --- | ------------------------------------------- |
| Credit | -   |     | 0 < Credit                                  |
| Credit |     |     | Included regardless of whether the value is |
positive or the value is negative

 Note
If the checkbox Accounts with Balance of
Zero is selected in the Balance Sheet –
Selection Criteria window, G/L accounts
with a balance of 0 (zero) are also
included.
Liability Accounts
Linked Sign Included in this account group if the following applies:
| Balance | +   | Debit < Credit |     |
| ------- | --- | -------------- | --- |
(Balance = Credit – Debit)
| Balance | -   | Debit > Credit |     |
| ------- | --- | -------------- | --- |
(Balance = Credit – Debit)
Balance Included regardless of whether the value is positive or the
value is negative
(Balance = Credit – Debit)

 Note
If the checkbox Accounts with Balance of Zero is selected
in the Balance Sheet – Selection Criteria window, G/L
accounts with a balance of 0 (zero) are also included.
| Debit | +   | Debit < 0 |     |
| ----- | --- | --------- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:12 AM
Linked Sign Included in this account group if the following applies:
Debit - Debit > 0
Balance Included regardless of whether the value is positive or the
value is negative
(Balance = Credit – Debit)
 Note
If the checkbox Accounts with Balance of Zero is selected
in the Balance Sheet – Selection Criteria window, G/L
accounts with a balance of 0 (zero) are also included.
Credit + 0 < Credit
Credit - 0 > Credit
Credit Included regardless of whether the value is positive or the
value is negative
 Note
If the checkbox Accounts with Balance of Zero is selected
in the Balance Sheet – Selection Criteria window, G/L
accounts with a balance of 0 (zero) are also included.
Delete Rows
Deletes accounts that are currently located under the selected account in the financial report template. Your action in this window
applies only to the financial report template. It does not influence the chart of accounts, even if the financial report template is
based on the chart of accounts.
More Information
Creating Financial Report Templates
Opportunity Reports
Consistently generated and correctly analyzed reports can provide valuable insight into the reasons for both failures and
successes with the company's sales and purchasing opportunities.
SAP Business One provides windows for creating reports and others for viewing them.
You can base a report on all parameters, or filter it to determine the scope and the focus of the report.
Once you enter a value for an option, SAP Business One selects the checkbox beside the appropriate field. If the checkbox is
deselected, the data is not taken into account during the next selection process, although the fields remain selected with the
chosen criteria.
Certain reports can be displayed in graph or table formats. You can choose in each of the reports to display or hide selected
columns.
All opportunity reports can be generated from Opportunities Opportunities Reports , or from the Reports module, including
the following:
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:12 AM
Opportunities Forecast
Opportunities Forecast Over Time
Opportunity Statistics
Opportunities Report
Stage Analysis
Information Source Distribution Over Time
Won Opportunities
Lost Opportunities
My Open Opportunities
My Closed Opportunities
Opportunities Pipeline
Related Information
Dynamic Opportunity Analysis
Opportunities Forecast
This report generates a projection of future opportunities, based on the predicted dates. The information presented is useful for
planning and prioritizing.
Opportunities Forecast - Selection Criteria
Use this window to specify selection criteria for the Opportunities Forecast report.
To open the window, choose Opportunities Opportunities Reports Opportunities Forecast Report , or open it from the
Reports module.
After defining the report, you can view it in the Opportunities Forecast Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Forecast Report
Territories
Required territories from those defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Required sales employee or buyer; usually the one that opened an opportunity.
Last Sales Emp. /Buyer
Last sales employee or buyer that handled the opportunity.
Stages
Stages to be included in the report.
Dates
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:12 AM
Any combination of the required start, closing, and predicted closing date.
Industry
Required industries.
Documents
Required document types related to your opportunities.
Sources
Required information sources.
Partners
Required partners.
Competitors
Required competitors.
Group By:
Required option to define a group display of specific parameters.
Group By (2):
Required option to define a secondary group display under the primary one defined in Group By.
This affects each defined primary group.
Related Information
Opportunity Reports
Opportunities Report
Opportunities Forecast Report Window
This window displays the Opportunities Forecast report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Forecast Report
Oppr. No.
System-generated opportunity number.
To display the opportunity, click .
Oppr. Name
Oopportunity name, if defined.
Contact Person
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:12 AM
Contact person of the business partner, as defined in the general area of the Opportunity window.
BP Channel Code
Business partner through which your company can provide services in certain transactions.
BP Channel Name
Name of business partner defined in BP Channel Code.
Closing %
Last value entered in the % field on the Stages tab of the Opportunity window.
Closing Date
Either the expected or actual closing date recorded for closing the opportunity.
Days in Pipeline
Number of days this opportunity has been active.
Gross Profit (LC)
Gross profit, in local currency, expected from the final sale.
You can import this figure from a document related to a stage.
Gross Profit (SC)
Gross profit, in system currency, expected from the final sale.
You can import this figure from a document related to a stage.
Industry
Industry group of the customer/lead or buyer.
Last Sale Emp./Buyer
The sales employee or buyer who involved in the last stage achieved in an opportunity.
Last Stage
Last stage reached in an opportunity.
Level of Interest
Description of how interested the business partner is in the opportunity.
Main Sales Emp./Buyer
Owner of an opportunity.
Potential amount (LC)
Potential amount, in local currency, for the opportunity.
Potential amount (SC)
Potential amount, in system currency, for the opportunity.
Predicted Closing Date
Date by which the current stage of the opportunity should be completed.
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:12 AM
Reason
Remarks recorded as an explanation for the success or failure of the opportunity.
Information Source
Original catalyst of interest in the opportunity, such as a conference or personal contact.
Status
Outcome of the last stage: won, lost or open.
Territory
Territory defined for business partner.
Weighted Amount (LC)
Sum of Potential amount (LC) multiplied by Closing % of the last stage.
Weighted Amount (SC)
Sum of Potential amount (SC) multiplied by the Closing % of the last stage.
Related Information
Opportunity Reports
Opportunities Report
Opportunities Forecast Over Time
This report presents a prognosis of open and closed opportunities, grouped by selected time periods. It displays the total number
of won, lost, and closed opportunities. The total opportunity amounts appear in the selected currency.
Opportunities Forecast Over Time - Selection Criteria
Use this window to specify selection criteria for the Opportunities Forecast Over Time report.
To open the window, choose Opportunities Opportunities Reports Opportunities Forecast Over Time Report .
Alternatively, open it from the Reports module.
After defining the report, you can view it in the Opportunities Forecast Over Time window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Forecast Over Time - Selection Criteria Fields
Territories
Required territories from those defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Required sales employee or buyer; usually the one that opened an opportunity.
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:12 AM
Last Sales Emp./Buyer
Last employee or buyer who handles an opportunity.
Stages
Stages to be included in the report.
Dates
Any combination of the required start, closing, and predicted closing date.
Industry
Required industries.
Documents
Required document types related to your opportunities.
Percentage Rate
Required range of closing percentage (%).
Sources
Required information sources.
Partners
Required partners.
Competitors
Required competitors.
Status
Required statuses.
Group By:
Required option to define a group display of specific parameters.
Display in System Currency
Open amount, displayed in system currency.
Opportunities Forecast Over Time Window
This window displays the Opportunities Forecast Over Time report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Forecast Over Time Report Fields
Month/Quarter/Year
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:12 AM
The period according to which the opportunities are grouped in the report. This value is determined by the selection you made in
the field Group By in the Opportunities Forecast Over Time Report — Selection Criteria Window.
Open Amount
Total open amount of all the opportunities per time period.
Total Open
Total number of open opportunities per time period.
Total Won
Total number of won opportunities per time period.
Total Lost
Total number of lost opportunities per time period.
Total Closed
Total number of closed opportunities, won and lost, per time period.
Opportunity Statistics
This report displays the number of open and completed opportunities. You can sort the data by various combinations of options
and groupings.
The columns on the right display the permanent options. The optional columns reflect the choices made in the selection criteria
window.
Clicking in the fields Total, Total Open, Total Won, Total Lost, and Total Completed opens an Opportunity List. In each instance,
the list presents particulars of each component of the total, according to the opportunity number.
Opportunities Statistics Reports - Selection Criteria
Use this window to specify selection criteria for the Opportunities Statistics report.
To open this window, choose Opportunities Opportunities Reports Opportunities Statistics Report . Alternatively, open it
from the Reports module.
After defining the report, you can view it in the Opportunity Statistics window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunies Statistics Report - Selection Criteria
Territories
Required territories, as defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Required sales employee or buyer; usually the one that opened the opportunity.
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:12 AM
Last Sales Emp./Buyer
Last employee or buyer that handled the opportunity.
Stages
Required stages.
Dates
Any combination of the required start, closing, and predicted closing date.
Industry
Required industries.
Documents
Required document types related to the opportunity.
Percentage Rate
Required range of closing percentage (%).
Sources
Required information sources.
Partners
Required partners.
Competitors
Required competitors.
Group By:
Required option to define a group display of specific parameters.
Group By (2):
Required option to define a secondary group display under the primary one defined in Group By.
This affects each defined primary group.
Opportunity Statistics Window
This window displays the Opportunity Statistics report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunity Statistics Report Fields
Total
Total number of open and closed opportunities.
Total Open
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:12 AM
Total number of open opportunities.
Total Won
Total number of won opportunities.
Total Lost
Total number of lost opportunities.
Total Closed
Total number of won and lost opportunities.
Success %
Success percentage, calculated according to the total won / (total won + total lost).
Pot.Open Amount
Total of expected amounts of all open opportunities.
Weighted Open Amt
Total of weighted amounts of all open opportunities.
Won Amount
Total amounts of won opportunities.
Lost Amount
Total amounts of lost opportunities.
Related Information
Opportunity Reports
Opportunities Report
This report summarizes, in table format, all sales and purchasing opportunities.
Opportunities Report - Selection Criteria
Use this window to specify selection criteria for the Opportunities report.
To open this window, choose Opportunities Opportunities Reports Opportunities Report . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the Opportunities Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Report Fields
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:12 AM
Territories
Required territories, as defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Required sales employee or buyer; usually the one that opened the opportunity.
Last Sales Emp./Buyer
Last sales employee or buyer that handled the opportunity.
Stages
Required stages.
Dates
Any combination of the required start, closing, and predicted closing date.
Industry
Required industries.
Documents
Required document types.
Percentage Rate
Required range of closing percentage (%).
Sources
Required sources.
Partners
Required partners.
Competitors
Required competitors.
Status
Required statuses.
Related Information
Opportunity Reports
Opportunities Window
This window displays the Opportunities report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:12 AM
Opportunities Report Fields
Oppr. Num
System-generated opportunity number.
To display the opportunity, click .
Oppr. Name
Opportunity name.
Last Sales Emp./Buyer
Person who worked on the opportunity in the last stage.
Last Stage
Displays the most recent stage achieved in the opportunity.
Status
Status chosen in the Summary tab of the Opportunity window.
Closing %
Last value entered in the Closing % field on the Stages tab of the Opportunity window.
Potential Amount (LC)
Potential Amount, in local currency, for the last stage achieved.
Stage Analysis
This report provides an overview of the success rate of sales and purchasing activities. It contains data such as how many sales
opportunities were concluded in a specific stage, or for how long sales opportunities remained in each stage of the sales process.
Note that only closed opportunities are displayed as either won or lost.
Stage Analysis - Selection Criteria
Use this window to specify selection criteria for the Stage Analysis report. All closed opportunities can be displayed, or the report
can be filtered according to certain parameters.
To open this window, choose Opportunities Opportunities Reports Stage Analysis . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Stage Analysis window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Stage Analysis - Selection Criteria Fields
Start Date From...To ...
Range of start dates to view a limited time period.
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:12 AM
Predicted Closing Date From...To...
Range of closing dates to view a limited time period.
Opportunity Stage
Required stages.
Add Opportunities with Expired Closing Date
Displays also opportunities of which the closing date has passed.
Stage Analysis Window
This window displays the Stage Analysis report according to the defined selection criteria.
Access the details of a specific stage by double-clicking a stage row.
To filter the display to a specific stage or sales employee or buyer, click , choose the required options, and Refresh.
The lower part of the screen displays the value for each stage, subdivided per sales employee or buyer in a printable graph form.
To display opportunities with an expired closing date, select the corresponding checkbox, and Refresh.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Stage Analysis Fields
Stage
All stages, or only the specific stages chosen in the Selection Criteria window.
Defined %
Probability of success defined for each stage.
Actual %
Number of opportunities concluded profitably as a percentage of all concluded opportunities.
For example: If one out of four sales opportunities has been closed as Won, then the Actual % column displays 25%.
If one sales opportunity out of one has the status Closed and Won, then the Actual % column displays 100%.
These totals are also displayed per sales employee or buyer, in addition to the totals.
Leads in Stage
Number of times each stage appears in all the closed opportunities. This figure is also displayed per sales employee or buyer, in
addition to the total.
Information Source Distribution Over Time
This report presents sales and purchasing opportunities according to their sources. The data can be grouped to display in specific
time periods, either days, weeks, or months.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:12 AM
Related Information
Opportunity Reports
Information Source Distribution Over Time - Selection Criteria
Use this window to specify selection criteria for the Information Source Distribution Over Time report.
To open this window, choose Opportunities Opportunities Reports Information Source Distribution Over Time Report .
Alternatively, open it from the Reports module.
After defining the report, you can view it in the Information Source Distribution Over Time window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Source Distribution Over Time Report Fields
Territories
Required territories, as defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Required sales employee or buyer; usually the one that opened the opportunity.
Last Sales Emp./Buyer
Last sales employee or buyer who handles the opportunity.
Stages
Required stages.
Dates
Any combination of the required start, closing, and predicted closing date.
Industry
Required industries.
Documents
Required document types related to your opportunities.
Percentage Rate
Required range of closing percentage (%).
Sources
Required sources.
Partners
Required partners.
Competitors
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:12 AM
Required competitors.
Status
Required statuses.
Group By:
Required option to define a group display of specific parameters.
Related Information
Opportunity Reports
Information Source Distribution Over Time Window
This window displays the Information Source Distribution Over Time report according to the defined selection criteria.
Choosing Show Graph displays the report in a graphical format.
Choosing Settings enables additional options, such as:
Various graph formats, such as a pie or bar graph
Limited number of information sources
Different time range than the one specified
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Information Source Distribution Over Time Report Fields
Days, Weeks, Months
Opportunities grouped by days, weeks or months, according to the Predicted Closing Date.
Type of Information Source column
Number of opportunities in each column according to the type of the source.
Total
Total number of opportunities for each time period.
Won Opportunities
This report details information about successful opportunities. It displays:
Days remaining until closing
Number of won opportunities
Total receivables
Total income and number of opportunities within a specific time range (graph form).
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:12 AM
You can filter the report to include specific dates, sales employees or buyers, and business partners.
Won Opportunities - Selection Criteria
Use this window to specify selection criteria for the Won Opportunities report.
To open the window, choose Opportunities Opportunities Reports Won Opportunities Report . Alternatively, open it from
the Reports module.
After defining the report, you can view it in the Won Opportunities window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Start Date From
Opening date of time period encompassed by report.
Closing Date From
End date of time period encompassed by report.
Sales Employee/Buyer
Employees authorized to view reports.
BP Code
Business partners authorized to view reports.
Range in Days
Number of days displayed in each section of the table or graph.
Related Information
Opportunity Reports
Won Opportunities Window
This window displays the Won Opportunities report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Won Opportunities Report Fields
Days Until Closing
Number of days required to win an opportunity.
This value comes from the Predicted Closing In field of the Opportunity window.
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:12 AM
No. of Opportunities
Number of successful opportunities, per time period.
Total Amount
Total of all potential amounts per time period.
Lost Opportunities
Use this report to analyze unsuccessful sales and purchasing opportunities. Filter the report according to various relevant criteria
such as business partner and territory.
Lost Opportunities - Selection Criteria
Use this window to specify selection criteria for the Lost Opportunities report.
To open this window, choose Opportunities Opportunities Reports Lost Opportunities Report . Alternatively, open it from
the Reports module.
After defining the report, you can view it in the Lost Opportunities window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Lost Opportunities - Selection Criteria Fields
Territories
Required territories, as defined in the Business Partner Master Data.
Main Sales Emp./Buyer
Usually the employee that opened the opportunity.
Last Sales Emp./Buyer
Last employee that handled the opportunity.
Stages
Required stages.
Industry
Required industries.
Documents
Required document types related to the opportunity.
Percentage Rate
Required range of closing percentage (%).
Sources
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:12 AM
Required sources.
Partners
Required partners.
Competitors
Required competitors.
Group By:
Required option to define a group display of specific parameters.
Group By (2):
Required option to define a secondary group display under the primary one defined in Group By.
This affects each defined primary group.
Related Information
Opportunity Reports
Lost Opportunities Window
This window displays the Lost Opportunities report according to the defined selection criteria.
Lost Opportunities Report
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Oppr. No.
System-generated opportunity number.
To display the opportunity, click .
Oppr. Name
Opportunity name, if defined.
Territory
Territories to which business partner is assigned.
Industry
Industries related to a business partner.
Closing %
Percentage entered in the Closing % field in the Opportunity window.
Potential Amount (LC)
Local currency value of Potential Amount for the last stage achieved.
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:12 AM
Weighted Amount (LC)
Local currency value of Weighted Amount entered in the last stage.
Related Information
Opportunity Reports
My Open Opportunities
This report displays all open sales and purchasing opportunities, per sales employee or buyer, and requires no selection criteria.
The report is restricted to the sales employee or buyer concerned, and users who are linked to this sales employee or buyer. The
link is created either in the Employee Master Data window, or in the User Defaults window.
To generate this report choose Opportunities Opportunities Reports My Open Opportunities . Alternatively, generate it
from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
My Open Opportunities Fields
Oppr. Num
System-generated opportunity number.
To display the opportunity, click .
Oppr. Name
Opportunity name, if defined.
Last Sales Employee
Person who worked on the opportunity in the last stage.
Last Stage
Most recent stage achieved in the opportunity.
Status
Status chosen in the Summary tab of the Opportunity window.
Closing %
Percentage entered in the Closing % field in the last stage.
Potential Amount
Potential amount, in local or system currency, for the last stage achieved.
Related Information
My Closed Opportunities
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:12 AM
My Closed Opportunities
This report displays all closed sales and purchasing opportunities, per sales employee or buyer, and requires no selection criteria.
The report is restricted to the selected sales employee or buyer, and users who are linked to this sales employee or buyer. The link
is created either in the Employee Master Data window, or in the User Defaults window.
To generate this report, choose Opportunities Opportunities Reports My Closed Opportunities . Alternatively, generate it
from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
My Closed Opportunities Fields
Oppr. Num
System-generated opportunity number.
To display the opportunity, click .
Oppr. Name
Opportunity name, if defined.
Last Sale Employee/Buyer
Person who worked on the opportunity in the last stage.
Last Stage
Most recent stage achieved in the opportunity.
Status
Status chosen in the Summary tab of the Opportunity window.
Closing %
Percentage entered in the Closing % field in the Opportunity window.
Potential Amount
Potential amount, in local or system currency, for the last stage achieved.
Related Information
Opportunity Window
Opportunities Pipeline
This report lets you analyze open opportunities in the sales and purchasing pipelines and to identify the most potentially
successful ones.
Opportunities Pipeline - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:12 AM
Use this section of the Opportunities Pipeline window to specify selection criteria for the Opportunities Pipeline report.
To open this window, choose Opportunities Opportunities Reports Opportunities Pipeline . Alternatively, open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Pipeline Report - Selection Criteria Fields
Sales Employee/Buyer
Last employee who handles an opportunity.
Stage
Required stage.
Date
Any combination of the required start, closing, and predicted closing dates to filter the report to a specific time period.
Documents
Required document types related to your opportunities.
Percentage Rate
Required range of closing percentage (%).
Opportunities Pipeline Window
This window lets you select the criteria for the Opportunities Pipeline report and generate it.
Display an opportunity in a row of the table or as a segment in the graphic.
Double-click either a row or a segment to open an additional window displaying the list of open opportunities for each stage.
To display a summary of the data for each stage, click a segment in the graphic once and keep the mouse button depressed.
Choose Clear Conditions and Refresh to display the table and graph with different selection criteria.
To print the graphic shown in the window, choose Print Graph.
To view the open opportunities in dynamic mode, see the topic Dynamic Opportunity Analysis.
To open this window, choose Opportunities Opportunities Reports Opportunities Pipeline . Alternatively, open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Opportunities Pipeline Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:12 AM
BP Code
Required business partner code.
Optionally, include the customer group, and other defined properties, in the report.
Sales Employee/Buyer
Last employee who handles the opportunity.
Stage
Required stage.
Date
Any combination of the required start, closing, and predicted closing dates to filter the report to a specific time period.
Documents
Required document types related to your opportunities.
Percentage Rate
Required range of closing percentage (%).
Opportunities Pipeline Fields
Description
A sales or purchasing stage.
No.
Number of open opportunities for each stage.
Expected Total
Estimated total amount to be received should the opportunity succeed.
Weighted Amount
Sum of Potential Amount multiplied by the percentage of the last stage.
%
Closing percentage of the last stage reached in opportunities.
Related Information
Opportunity Reports
Dynamic Opportunity Analysis
Dynamic Opportunity Analysis
This window is part of the Opportunities Pipeline report.
Each sales or purchasing opportunity is represented by a balloon, whose size corresponds to the size of the planned opportunity.
Each vertical division represents a stage in the sales or purchasing process.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:12 AM
The balloons progress along the longitudinal axis according to their changing status.
A balloon floats upwards/downwards to indicate a won/lost opportunity.
The display options can be modified by choosing the Form Settings icon on the menu bar.
To display this report, see the topic Displaying the Dynamic Opportunity Analysis Report.
Related Information
Displaying the Dynamic Opportunity Analysis Report
Dynamic Opportunity Analysis: Form Settings
Customize the display of the Dynamic Opportunity Analysis report further, by choosing various options in the Form Settings –
Opportunities window.
Opportunities
Set the maximal number (1-30) of balloons (opportunities) to be displayed in the report.
Sort by
Choose a parameter, such as Start Date or Sales Employee/Buyer, and sort order (Ascending or Descending) for sorting the
balloons.
Color
Choose the parameter for displaying the balloon colors:
Random: every opportunity is in a different color.
By Employee: All opportunities, per employee, are the same color.
By BP: All opportunities, per business partner, are the same color.
By BP Groups: All opportunities, per business partner group, are the same color.
Step Size (Days)
Display the progress of each step in the report according to the number of days.
Step Delay (Seconds)
Display the delay between steps in increments of seconds.
Displaying the Dynamic Opportunity Analysis Report
Procedure
1. From Opportunities Reports, display the Opportunities Pipeline window.
2. In the menu bar, choose Go To Dynamic Opportunity Analysis . The Dynamic Opportunity Analysis window appears,
with each opportunity represented by a balloon.
3. To start, accelerate, interrupt, forward or reverse the dynamic display, click the control arrows at the bottom left of the
screen. The slider moves accordingly.
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:12 AM
4. To choose a specific date, move the slider. The date is displayed at the bottom of the screen in the center.
Related Information
Opportunity Reports
Sales and Purchasing Reports
Use the reports listed under this entry to:
Analyze purchasing and sales transactions
View open documents
Generate backorder report
View and process documents saved as drafts
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
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:12 AM
Open Items List Fields
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
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:12 AM
Original Amount
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
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:12 AM
Number of items on consignation. The value in this field is a result of the quantity in open deliveries minus the quantity in open
returns
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
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:12 AM
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
2. If approval isn’t required, you use the Save as Draft function to save the target document. If approval is required, the
system automatically creates a draft after you add the document, pending approval.
3. You (or another user) use the Copy To or Copy From function to copy the same base documents to another target
document again.
4. You (or another user) try to add the target document, save the target document as a draft again, or add the target
document for approval again.
Before making your decision, you can open this window to view details of the existing drafts using the provided draft numbers.
Backorder Report
This report displays a list of overdue sales orders or A/R reserve invoices that cannot be shipped due to inventory shortages. It lets
you define priorities and accelerate purchase orders or production orders.
To access this window, choose Sales - A/R Sales Reports Backorder .
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:12 AM
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
Backorder Report - Selection Criteria
Use this window to specify selection criteria for the Backorder report, which displays a list of overdue sales orders or A/R reserve
invoices that cannot be shipped due to stock shortages. The report lets you define priorities and accelerate purchase orders or
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:12 AM
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
Analyze the sales volume for each customer or for customer groups. See Sales Analysis Report: Customers Tab.
Items
Analyze the sales volume either per item or per item group. See Sales Analysis Report: Items Tab.
Sales Employee
Analyze the sales volume per sales employee. See Sales Analysis Report: Sales Employee Tab.
Each tab displays different selection parameters and generates reports that provide different aspects of the sales volume in your
company.
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:12 AM
To open the window, choose Sales – A/R Sales Reports Sales Analysis . Alternatively, open it from the Reports module.
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
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:12 AM
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
Sales Analysis Report: Customers Tab
Use this tab to specify selection criteria for the Sales Analysis by Customer report. When you run the report, SAP Business One
creates a corresponding sales volume analysis for each customer.
To access the tab, choose Sales – A/R Sales Reports Sales Analysis Customers . Alternatively, access it from the
Reports module.
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
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:12 AM
Returns are displayed as part of delivery notes and they decrease the sales amount.
Individual Display
Displays the report for individual customers.
Group Display
Displays the report for customer groups, with each customer group appearing in a separate row. To display the sales for each
customer in a customer group, double-click the row number of the respective customer group.
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
Sales Analysis Report: Sales Employee Tab
Use this tab to specify selection criteria for the Sales Analysis by Sales Employee report, which analyzes the sales volume per sales
employee. SAP Business One creates a corresponding sales volume analysis for each sales employee.
To access the tab, choose Sales – A/R Sales Reports Sales Analysis Sales Employee.
Alternatively, access it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Employee Fields
Annual Report, Monthly Report, Quarterly Report
Select whether you want the report to reflect results for the entire year, per month, or per quarter.
If you select the Monthly Report or the Quarterly Report radio button, the total for the year is also displayed. In addition, if you
select one of these options, you can hide empty periods by selecting the Hide Empty Months/Quarters checkbox.
Invoices, Orders, Delivery Notes
Select the document type on which you want to base the sales analysis.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:12 AM
If you base an A/R credit memo on an A/R down payment invoice, that A/R credit memo does not appear in the report.
Cancelled sales orders do not appear in the report.
Returns are displayed as part of delivery notes and they decrease the sales amount.
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
Sales employee code or name
To view the detailed information related to each row in the report, double-click the number of the row. A detailed window appears.
To display the report results as a graph, choose . A new window with the graph display of the report appears. Choose the
Settings pushbutton to define the display parameters.
More Information
Sales Analysis Report
Sales Analysis Report: Detailed View
This window displays the details for a specific row of the Sales Analysis report. One section displays a table listing all sales
documents and their details; another contains a diagram of the sales information.
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:12 AM
You can select different types of diagrams. To print the diagram when you print the report, select Print Diagram.
More Information
Sales Analysis Report
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
Purchase Analysis: Items Tab
Use this tab to specify selection criteria for the Purchase Analysis by Items report. This report lets you analyze purchases either
per item or per item group. SAP Business One creates a purchase volume analysis for each item.
 Note
Service invoices are not included when you run the Purchase Analysis by Items report.
Use this tab to create a purchase analysis per item or item group.
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:12 AM
 Note
If you base an A/P credit memo on an A/P down payment invoice, that A/P credit memo does not appear in the report.
Cancelled purchase orders do not appear in the report.
Goods returns are displayed as part of the Goods Receipt PO, and they decrease the purchased amount.
Display Amounts in System Currency
Displays amounts in the system currency.
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
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:12 AM
Group Display
Select whether you want to display the report for an individual vendor or for a group of vendors.
If you select the group display option, each vendor group appears in a separate row in the report. To display the purchase analysis
for each vendor in a vendor group, double-click the row number of the respective vendor group.
Total by Vendor
Choose how to group the report data.
Total by Blanket Agreement
Choose how to group the report data.
Display Amounts in System Currency
Displays amounts in the system currency.
Related Information
Transaction Codes
Journal Entry Window
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
The criteria you select determine the details displayed in this window. Changing the selection criteria changes the columns in the
report.
To view a detailed breakdown of the data of a row in the report, double-click its row number in the first "#" column. A detailed
report appears.
To display the results of a report as a graph, click . The graph for the report appears in a new window.
Choose Settings to define the parameters for displaying the graph.
Purchase Analysis Report: Detailed View
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:12 AM
This window displays the details for a specific row of the purchase analysis report. It comprises two sections:
A detailed table view
A graphical view of the purchase analysis
Specify the required type of chart display by clicking Chart Style.
To print the chart when you print the report, select Print Graphs.
Regardless of the selection you have made, decide whether to display the vendor code, item number, sales employee code, or
name in the report. To do this, choose Go To in the menu bar.
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
Aging
My Activities
This report lets you view all activities assigned to you, by yourself or by other users.
To create the report, choose Business Partners Business Partner Reports My Activities .
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:12 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
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
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:12 AM
Address details entered for a Meeting type of activity.
Content
Text specified on the Content tab of the activity.
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
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:12 AM
Activities Overview - Selection Criteria
Use this window to specify selection criteria for the Activities Overview Report.
To open the window, choose Reports Business Partners Activities Overview .
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
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:12 AM
 Note
By default, only some columns are displayed. To display additional columns, choose .
 Note
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
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:12 AM
Telephone
Phone number entered in the Activity window.
Room, Street, City, Country/Region, State
Address details entered for a Meeting type of activity.
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
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:12 AM
Inactive Customers - Selection Criteria
The Inactive Customers report indicates whether a customer is inactive by checking whether or not specific sales documents were
created to the customer within a defined period.
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
This is custom documentation. For more information, please visit SAP Help Portal. 130

6/8/26, 6:12 AM
Properties
Opens the Properties window, where you can set properties as selection criteria.
Due Date From...To...
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
This is custom documentation. For more information, please visit SAP Help Portal. 131

6/8/26, 6:12 AM
Due date as defined in the document.
Last Dunning Date
Last dunning date, in case the document was dunned previously.
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
Tracking Dunning Levels
You use the customer receivables aging report to view customer due debts and interest rates, and to manage dunning levels. You
can also decide to send a letter to remiss customers, which progresses them to a more severe level.
 Note
If you send a dunning letter via e-mail or facsimile from SAP Business One, the dunning level does not increase, as these are not
legal documents.
Procedure
1. From the SAP Business One Main Menu, choose Reports Sales and Purchasing Aging Customer Receivables
Aging .
The Customer Receivables Aging - Selection Criteria window appears.
2. Select filtering options to display the customers you want.
3. Set the report options to Age by Due Date and double-click the customer row to display all the documents composing the
debt.
4. Select the Letter column to schedule this invoice for a dunning letter.
You can manually change the dunning level by choosing the Level column.
 Note
You cannot check rows that are based on manual journal entries and credit memos.
This is custom documentation. For more information, please visit SAP Help Portal. 132

6/8/26, 6:12 AM
5. Choose the Print Preview icon and view the dunning letter.
6. Choose the Print icon to print this letter.
The dunning level for this invoice is updated in the report and in the invoice document.
If you select more than one invoice, a message appears letting you summarize invoices of the same level into one letter.
 Note
You can block dunning letters for specific customers and invoices.
To block a customer, select Block Dunning Letters on the Accounting tab of the business partner master data.
To block an invoice, select Block Dunning Letters on the Logistics tab of the invoice document.
Customers Receivables by Customer Cross-Section Report
You can use this window to generate the customer receivables by customer cross-section report. To do it.
To open the window, choose one of the following from the SAP Business One Main Menu:
Business Partners Business Partner Reports Customers Receivables by Customer Cross-Section
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
This is custom documentation. For more information, please visit SAP Help Portal. 133

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 134

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 135

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 136

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 137

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 138

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 139

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 140

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 141

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 142

6/8/26, 6:12 AM
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
Months – Each column represents one month, moving back from the aging date month.
Periods – Each column represents one period as defined in Administration System Initialization Posting Periods ,
moving back from the aging date period.
[Top Total Row]
Displays the sum of amounts listed in one column
[Bottom Total Row]
Displays the percentage of open receivables for each time interval
Inventory Reports
The inventory reports enable you to display information about items and their inventories, as well as the valuation of the
inventories.
To access these reports, choose Inventory Inventory Reports .
All the images here in this topic are interactive. You can choose each tile to dive into a specific topic.
Generate a list of all the items defined in the system (active and inactive), as well as information about the items such as
their prices and serial/batch numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 143

6/8/26, 6:12 AM
Please note that image maps are not interactive in PDF outputs.
Create a list of inventory postings and counting.
Please note that image maps are not interactive in PDF outputs.
Analyze the inventory situation for items or display the inventories of items in each warehouse, to get an overview of your
inventory.
Please note that image maps are not interactive in PDF outputs.
This is custom documentation. For more information, please visit SAP Help Portal. 144

6/8/26, 6:12 AM
Start a valuation and audit for warehouse inventory.
Please note that image maps are not interactive in PDF outputs.
Items List - Selection Criteria
Use the item list report to create lists of items defined in the system together with their prices. To select the items to be included in
the report, use the Items List – Selection Criteria window.
To access the Items List Selection Criteria, choose Inventory Inventory Reports Items List .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Items List, Selection Criteria Fields
Item Properties button
Opens the Properties window.
Specify the item properties to be used as selection criteria.
Hide Items with No Quantity in Stock
Excludes items with zero quantity from the list.
Items List
This report generates a list of items, as defined in the Items List - Selection Criteria window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Item List Fields
In Stock
Total quantity of item in stock.
Bar Code
International item number (EAN) or bar code, if specified in the item master data.
This is custom documentation. For more information, please visit SAP Help Portal. 145

6/8/26, 6:12 AM
Inventory UoM
The item's inventory UoM, if specified in the Item Master Data.
Last Revaluation Price
If inventory revaluation has been carried out, the last revaluation price is displayed.
Last Purchase Price
The last purchase price for the item, as defined in the Last Purchase Price list.
Price List 01,. Price List 02 etc.
Item prices in the price lists as defined in the system, with one column for each price list. Scroll horizontally in the window to
display the columns for additional price lists.
 Note
You can print the prices from one price list only.
To choose the price list to print, click its column header and then click the print icon in the toolbar. If you do not select a price
list, the system prints by default the prices from the Cost/Price column.
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
This is custom documentation. For more information, please visit SAP Help Portal. 146

6/8/26, 6:12 AM
In addition to last prices, displays the Special Prices defined for the selected item.
This selection is optional.
Date
Enter a date to display Special Prices for that specific date.
Quantity
Enter a quantity to display Special Prices for that specific quantity.
To generate the report, enter the necessary information and choose Refresh.
Inactive Items - Selection Criteria
Use this report to find out which items have not been used for a defined transaction since a specified date.
To access the Inactive Items – Selection Criteria window, choose Inventory Inventory Reports Inactive Items .
Inactive Items Report
The list shows all items that do not appear in any of the selected sales documents since a specified date.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inactive Items Report Fields
Sales Quotations, Deliveries, A/R Down Payments, Orders, A/R Invoices
If you want to exclude a document type, deselect the corresponding checkbox and then choose the Refresh button. Items that
have been inactive only with the selected document type will not be displayed.
The A/R Down Payments option applies to both A/R down payment requests and A/R down payment invoices.
In Stock
Displays the available inventory of the inactive items.
Preferred Vendor
Displays the code of the default preferred vendor of this item, as defined in the Item Master Data window.
Generating the Inventory Posting List
Context
The inventory posting list provides an overview of all postings in the system, based on various selection criteria and sort options.
You can generate a report for specified warehouses based on one of the following selection criteria:
Item
This is custom documentation. For more information, please visit SAP Help Portal. 147

6/8/26, 6:12 AM
Business partner
Other: Enables you to specify a selection criterion such as warehouse or sales employee.
Procedure
1. Choose Inventory Inventory Reports Inventory Posting List .
The Inventory Posting List – Selection Criteria window appears.
2. To base the report on items, business partners or other criteria, choose one of the following tabs and make the required
selections:
Item
BP
Other
For more information, see Inventory Posting List – Selection Criteria: Items, BP, Other.
3. Make the required selections in the Trans. Selection Criteria area.
For more information, see Inventory Posting List – Selection Criteria: Transaction.
4. To select by location or warehouse, select one of the following tabs and specify the required criteria:
By Location
By Warehouse
5. To generate the Inventory Posting List Report, choose OK.
Results
The Inventory Posting List Report is generated. It contains the data defined by the selection criteria.
Example
In this example, an inventory posting list is created, based on two sales employees. The example assumes that the system has
been set up with the required data.
You open the Inventory Posting List – Selection Criteria window. The three tabs – Item, BP and Other – are displayed. You choose
the Other tab. You click the By field and select Sales Employees from the list. Then you choose Selection and select two
employees from the list. To restrict the report to specific warehouses, you choose the Whse tab and enter the required range of
warehouses. You choose OK and the report is generated in a new window. The report shows the documents that were selected by
the selected sales employees. To view more information, you click in any of the rows.
Inventory Posting List - Selection Criteria: Items, BP, Other
The inventory posting list can be displayed in various grouping options:
Item
Business partner
Other criteria, such as warehouse
The grouping option is determined by your selection of tabs (Item, BP or Other).
This is custom documentation. For more information, please visit SAP Help Portal. 148

6/8/26, 6:12 AM
To open this window, choose Inventory Inventory Reports Inventory Posting List by Item .
Select the Item tab to include items from transactions with vendors and customers or other inventory transactions.
Select the BP tab to include all upward and downward inventory adjustments for the specified items for each business partner.
Select the Other tab to include one of a range of selection criteria, for example:
Sales employee
Project code
Serial number
Receipt quantity
Issue quantity
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Items Tab
Hide Items with Zero Quantities
Excludes items with a zero quantity.
Other Tab
By
Criterion according to which the inventory posting report is displayed.
Selection
Opens a list of additional values for the selection criterion specified in the By field.
Choose the required values from the list.
Inventory Posting List - Selection Criteria (“Other” Tab)
This window enables you to make selections when you have chosen the Other tab in Inventory Posting List - Selection Criteria.
The contents of the window are defined according to the option you select on the Other tab.
To open the window, choose the Selection button on the Other tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Display
Displays the data from this criterion.
Criterion Value
This is custom documentation. For more information, please visit SAP Help Portal. 149

6/8/26, 6:12 AM
This column presents values for selection, according to the criterion chosen in the By field in the Inventory Posting List –
Selection Criteria, Other tab. Before selecting the Display field, you can see the description of the line in this column. These values
can be of warehouse, sales employees, etc.
Inventory Posting List - Selection Criteria: Transaction
The Inventory Posting List – Selection Criteria window includes the following areas:
Trans. (Transaction) Selection Criteria
By Location tab
By Whse (Warehouse) tab
For more information, see Inventory Posting List – Selection Criteria: Items, BP, Other.
To open this window, choose Inventory Inventory Reports Inventory Posting List by Item .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Transaction (Trans.) Selection Criteria Fields
Sort
Select Sort to open the sort table.
You can specify up to three parameters by which you want to sort the report results.
If Sort is not selected, the system sorts the documents for each item or business partner by the posting date in ascending order.
Use the field on the right to determine whether you want to display all the postings with totals, only the postings, or only the totals
in the report results. Click and select the relevant entry from the list.
You can sort the report results by any field in the table, for example, by warehouse number or serial number. In addition to the main
criterion, you can specify two additional sort criteria. For example, if you select the warehouse number as the main sort criterion
and the display by serial number as the second criterion, the system sorts all postings by warehouse and serial number. Click
and select the sort criterion or criteria from the list.
Select whether you want the list to be sorted in ascending or descending order.
Select Yes in the Total column if you want the system to display subtotals for a sort criterion. If you enable the display of subtotals,
the report list displays different subtotals for each change of the sort criterion.
 Note
If you choose the warehouse number as a sort criterion, for example, the system displays subtotals for each warehouse with
inventory postings for an item. Therefore, you should consider which totals information is the most important and limit the
number of subtotals to avoid cluttering up the display.
Print BP/Item on Separate Page
Prints each item or business partner on a separate page.
If this option is not selected, the list is printed continuously when you print the report results. This means that a single page may
contain documents for several items or business partners, depending on your selection. This minimizes the amount of paper used.
This is custom documentation. For more information, please visit SAP Help Portal. 150

6/8/26, 6:12 AM
Print Directly
Prints the report results without displaying them on the screen first.
Choose All
Generates the list of all inventory postings in the system.
You can also specify information regarding the printing of the report results.
Hide Trans. Without Qty Change
Excludes inventory transactions without changes in quantity.
Split Display by Bin Locations
 Note
The checkbox is available only if you have enabled bin locations for at least one warehouse.
Select the checkbox to split each transaction row in the report by bin locations.
If you do not select the checkbox, the report displays only the first bin location used in each transaction.
Once you select the checkbox, the report displays all the bin locations used in each transaction.
Split Display by Batch/Serial Numbers
Select the checkbox to split each transaction row in the report by batch and serial numbers.
If you do not select the checkbox, the report displays only the first serial and batch number of the items in each transaction.
Once you select the checkbox, the report displays all the serial and batch numbers of the items in each transaction.
By Whse (Warehouse) Tab
Select the By Whse tab to make the selection by warehouse.
You can define a range of included or excluded warehouses. For example, if you include warehouses 01 to 10 and exclude
warehouses 06 to 08, only warehouses 01 through 05 and warehouses 09 and 10 are considered in the report.
By Location Tab
Select the By Location tab to make the selection by location.
Select or deselect the locations to be included in or excluded from the report.
Inventory Posting List Report
You can view the list of inventory-related postings for each item or business partner or other criteria, depending on your selection.
To open the report, choose Inventory Inventory Reports Inventory Posting List In the Inventory Posting List – Selection
Criteria window, select the relevant data and choose the OK button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 151

6/8/26, 6:12 AM
Inventory Posting List By Items or Business Partners
Posting Date
Date on which the document that changed the inventory was created.
Document
The type and number of the document (the type is displayed as an abbreviation, such as IN for invoice).
G/L Acc. / BP Code
Code of the business partner for whom the document was entered, or the G/L account in which the inventory transaction was
posted (relevant for list by item only).
G/L Acc. / BP Name
Name of the business partner for whom the document was entered, or the G/L account in which the inventory transaction was
posted (relevant for list by item only).
Qty
Quantity of the item in the document. For inventory transactions only.
Price
Price of the item in the transaction.
Balance
The cumulative balance for each inventory posting of the item (relevant for list by item only).
Details
Remarks are displayed as they appear in the documents.
First Bin Location
 Note
The field is available only if you have enabled bin locations for at least one warehouse and have not selected the Split Display
by Bin Locations checkbox.
By default, the field is hidden. To make it visible, use Form Settings.
Displays the bin location code as follows:
If the item is allocated from or to more than one bin location in the transaction, the field displays the bin location code that
is first in the alphanumeric sequence.
If the item is allocated from or to only one bin location in the transaction, the field displays the code of the bin location.
To view the item's detailed bin location allocation information in the transaction, click before the bin location code to open the
bin location contents list.
Bin Location
 Note
The field is available only if you have enabled bin locations for at least one warehouse and have selected the Split Display by
Bin Locations checkbox.
By default, the field is hidden. To make it visible, use Form Settings.
This is custom documentation. For more information, please visit SAP Help Portal. 152

6/8/26, 6:12 AM
Displays all bin locations from/to which the item is allocated in the transaction.
To view the detailed information about the bin location, click to open the bin location master data.
 Note
The following two fields are available only if you have not selected the Split Display by Batch/Serial Numbers checkbox.
By default, the fields are hidden. To make them visible, use Form Settings.
First Serial Number
If the item is managed by serial numbers, the field displays the alphabetically first serial number that is relevant to the transaction.
First Batch Number
If the item is managed by batch numbers, the field displays the alphabetically first batch number that is relevant to the
transaction.
 Note
The following two fields are available only if you have selected the Split Display by Batch/Serial Numbers checkbox.
By default, the fields are hidden. To make them visible, use Form Settings.
Serial Number
If the item is managed by serial numbers, the field displays all serial numbers that are relevant to the transaction.
Batch
If the item is managed by batch numbers, the field displays all batch numbers that are relevant to the transaction.
Inventory Posting List By Other Criteria
Posting Date
Posting date of the inventory transaction.
Document
Document type of the inventory transaction.
WH
Warehouse number of the inventory transaction.
BP Code
Code of the business partner who participated in the inventory transaction.
Item No.
Code of the item in this inventory transaction.
Qty
Quantity of the item in the specific warehouse.
Price
Price of the item in the transaction.
This is custom documentation. For more information, please visit SAP Help Portal. 153

6/8/26, 6:12 AM
Details
The remarks are displayed as they appear in the documents.
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
This is custom documentation. For more information, please visit SAP Help Portal. 154

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 155

6/8/26, 6:12 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 156

6/8/26, 6:12 AM
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
Inventory in Warehouse Report - Selection Criteria
Whenever an item is purchased, sold, produced, or used in production, you specify the issuing or receiving warehouse in the
corresponding document. The system proposes the default warehouse automatically. You can change this if necessary. You can
also define inventory transfers between warehouses in the system.
To ensure accurate inventory management by warehouse, it is essential to record the correct warehouse in every single document.
If no warehouse is specified, SAP Business One proposes the defined default warehouse.
This report lists the current inventories by warehouse based on the information in these documents. You can then implement
measures such as inventory transfers, for example, to supplement the inventory of a warehouse.
The information you specify here is displayed automatically the next time you call the report.
To open the window, choose Inventory Inventory Reports Inventory in Warehouse Report .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory in Warehouse Report – Selection Criteria Fields
Vendor From... To...
This is custom documentation. For more information, please visit SAP Help Portal. 157

6/8/26, 6:12 AM
You can restrict the selection by the main vendor of an item. The main vendor is specified in the item master record. You can
valuate all the items from one or more main vendors.
Hide Items with No Quantity in Stock
Select to exclude items with zero quantity from the list.
Warehouses Selection: By Location, By Warehouse (Including From ... To, Excluding From ... To)
Determine which storage locations will be included in the report. Make the selection by location, or by warehouse. If you select
warehouse, define the range of included or excluded warehouses.
You must select at least one warehouse for the report.
Display: Normal, Detailed Report
Select one of the following:
Normal: The report is displayed in normal layout
Detailed Report: The report is displayed in extended layout.
If Detailed Report is selected, the Price Source field appears. Click the dropdown list and choose the required price or price
list from the list.
Only Display Items With
 Note
The checkbox is available only if you have enabled bin locations for at least one warehouse.
To exclude items without default bin locations from the report, select this checkbox.
To further filter the report, select the radio button for any of the following:
Enforced Default Bin Locations – The report displays only the items that have default bin locations and where the use of
the default bin locations is enforced.
Unenforced Default Bin Locations – The report displays only the items that have default bin locations and where the use of
the default bin locations is not enforced.
Both – The report displays only the items that have default bin locations.
Related Information
Inventory in Warehouse Report (Normal)
Inventory in Warehouse Report (Detailed)
Inventory in Warehouse Report (Normal)
You can use this report to analyze the inventories of one or more selected items in one or more warehouses.
Enter an item number or the first characters of an item number in the Find field to position the cursor on that item in the list. The
system then places the first matching entry at the top of the list in the window.
If the inventory for an item is negative, the value is displayed in red.
To open the window, select Normal in the Inventory in Warehouse Report - Selection Criteria window.
This is custom documentation. For more information, please visit SAP Help Portal. 158

6/8/26, 6:12 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory in Warehouse Report Tabs
In Stock tab
Displays a list of the selected items along with the corresponding total inventory in all warehouses. The inventories are displayed
by warehouse for the selected warehouses in the columns to the right.
Committed tab
Displays a list of the selected items along with the corresponding total inventory for the item, as indicated in the sales orders and
production instructions. If production instructions are involved, the quantity of the item to use for production is displayed.
You can enter a warehouse for the delivery or issue for production in each of the documents. The total of the respective quantities
for the warehouses appears in the columns to the right.
Ordered tab
Displays a list of the selected items along with the corresponding total inventory for the item, as indicated in the purchase orders
and production instructions. If production instructions are involved, the quantity of the item to be produced is shown.
You can enter a warehouse for the delivery or confirmation from for production in each of the documents. The total of the
respective quantities for the warehouses appears in the columns to the right.
Inventory in Warehouse Report (Detailed)
Use this report to analyze the detailed inventories of one or more selected items in one or more warehouses.
To open the window, select Detailed in the Inventory in Warehouse Report - Selection Criteria window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory in Warehouse Report (Detailed)
First Bin Location
Displays the bin location code as follows:
If the item is stored in more than one bin location, the field displays the bin location code that is first in the alphanumeric
sequence.
If the item is stored in only one bin location, the field displays the code of the bin location.
To view the item's detailed inventory information in the bin locations, click before the bin location code to open the bin location
content list.
 Note
If the items in all bin locations have negative inventory, the field still displays the bin location code that is first in the
alphanumeric sequence.
This is custom documentation. For more information, please visit SAP Help Portal. 159

6/8/26, 6:12 AM
In Stock
Displays the quantity of the item physically located in the warehouse.
Committed
The quantity of an item reserved from the inventory for the following document types:
Sales orders
Production orders (the quantity used for producing a parent item)
A/R reserve invoices
 Note
In various localizations there might be differences in this functionality. For complete information refer to the localized online
help file provided with SAP Business One by choosing: Help Document Localization Specific Info
Ordered
The quantity of an item already purchased or produced, but not yet received. The following document types contribute to the
quantity displayed in this field:
Purchase orders
Production orders (the quantity planned to receive from production)
A/P reserve invoices
 Note
In various localizations there might be differences in this functionality. For complete information refer to the localized online
help file provided with SAP Business One by choosing: Help Document Localization Specific Info
Available
The available quantity of an item is displayed.
The quantity is calculated as:
In Stock + Ordered – Committed
If the available inventory for an item is negative, the value is displayed in red.
Default Bin Location
Displays the item’s default bin location.
Enforced Default Bin Loc.
Indicates whether the use of the default bin location is enforced or not.
Item Price
Displays item price, according to the price source selected in the Inventory in Warehouse Report – Selection Criteria window.
Total
The system valuates the warehouse inventory using the price of the item from the price list you specified above. These values are
subtotaled for each warehouse and a grand total calculated for all warehouses.
This is custom documentation. For more information, please visit SAP Help Portal. 160

6/8/26, 6:12 AM
To add more fields to the report, in the toolbar, click the icon.
Inventory Audit Report - Selection Criteria
This report provides an audit trail for the posted inventory transactions in the chart of accounts.
You use this report to make comparisons between the accounting view (inventory balance accounts) and the logistics view
(inventory value displayed by the audit report). The report explains the value changes in inventory accounts.
 Note
When you print the report, you can also print the selection criteria on a separate page.
This report does not recalculate the cost but displays the information from the database.
The report is available only for companies using the perpetual inventory system.
To access the window, choose Inventory Inventory Reports Inventory Audit Report .
 Note
To create what-if scenarios, use the Inventory Valuation Simulation Report - Selection Criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Audit Report – Selection Criteria Fields
Date Type List
Select one of the following options:
Posting Date
System Date
The report displays the relevant data accordingly.
Date From....To....
Enter the posting dates or system dates that you want to include in the report.
 Note
If you have included the posting dates of a purchasing document whose posting date differs from the system date, keep in mind
that SAP Business One relates to the system date for the document when generating this report. Even if you select Posting
Date in the date dropdown list, if the system date is not included in the range of dates you select, the corresponding line in the
report appears in blue.
Properties
Choose and then select the required properties from the Properties window.
Display
This is custom documentation. For more information, please visit SAP Help Portal. 161

6/8/26, 6:12 AM
Select one of the following:
By Items - view and audit the results by items
Summarize by Accounts - view the information summarized by accounts
Group by Warehouse
Select to group the items by warehouse.
 Note
This option is activated only if both the following are true:
In the Display area, you have selected the By Items radio button.
In the Company Details window, on the Basic Initialization tab, you have selected the Manage Item Cost per
Warehouse checkbox.
Display OB for Items/Accounts with no Transactions
Select this checkbox to display the opening balances for items or accounts that have no transactions posted in SAP Business One.
If an item has no transactions within the selected date range but has open transactions from previous periods, the total of these
transactions is presented as an open balance for this item. As a result, the report total displays the item valuation from the end
date of the defined date range - that is, it contains both the opening balance figures and the transactions that are within the
defined date range.
Enable Quick Display
Select this checkbox to display the report in pages and with navigation buttons.
Selecting this checkbox limits you to a maximum of 300 accounts or warehouses at one time.
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
Inventory Audit Report
This report displays the total inventory value for the items according to the selection criteria configured in the Inventory Audit
Report - Selection Criteria window. The fields that appear in the report depend on whether By Items or Summarize by Accounts
was selected.
 Note
The inventory audit report updates the last calculated price list.
 Note
If the report is based on posting dates, and includes inventory items whose purchasing system dates deviate from the selected
date range, these rows appear in blue in the inventory audit report.
The report is expandable and contains up to three levels. Each level displays summary information for the level below.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 162

6/8/26, 6:12 AM
If you select the Enable Quick Display checkbox in the Inventory Audit Report — Selection Criteria window, the report is not
expandable, and you can select the Detailed or Summary view for the report.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Audit Report Fields
Date From .... To....
Displays start and end dates for the report calculations, as defined in the selection criteria.
Currency
Displays the company’s local currency.
Items
Displays a range of items included in the report, as defined in the Inventory Audit Report – Selection Criteria window.
If you have not defined any items in the Code fields, the Items field displays All. If you have selected two or more criteria types,
the field displays Multiple.
 Note
This field appears only if you select the By Items radio button in the Inventory Audit Report – Selection Criteria window.
Warehouses
Displays the warehouses included in the report as defined in the selection criteria. If you have selected all warehouses, the field
displays All.
 Note
This field appears only if you select the By Items radio button in the Inventory Audit Report - Selection Criteria window.
Accounts
Displays the range of accounts to be included in the report, as defined in the selection criteria.
 Note
This field appears only if you select the By Items radio button in the Inventory Audit Report - Selection Criteria window.
Document
Displays the abbreviated name of the document.
Quantity
Displays the change in inventory resulting from the transaction. If the field is empty, this indicates that there was a change only in
the cost in the specific transaction.
Cost
Displays the cost of the item in the transaction. The summarized cost is calculated as Cumulative Value/Cumulative Cost. The
item cost cannot be used for the report because it would need to be up to the current date.
This is custom documentation. For more information, please visit SAP Help Portal. 163

6/8/26, 6:12 AM
Trans. Value
Displays the value that was posted to the inventory account.
Cumulative Qty
Displays the total quantity in stock after the transaction. At the summary levels, it summarizes the quantities from the lower levels,
up to the report end date.
Transactions that cause the cumulative quantity to fall below zero are highlighted in red when you display the expanded view of the
report.
Cumulative Value
Displays the total value of inventory after the transaction.
Transactions that cause the cumulative value to fall below zero are highlighted in red when you display the expanded view of the
report.
G/L Account
Displays the account number.
Balance from G/L
Displays the G/L account balance in the chart of accounts for the report's end date. Use this information to compare information
of the report and the G/L. This is relevant only when you run the report up to the current date.
 Note
This field appears only if you select the Summarize by Accounts radio button in the Inventory Audit Report - Selection
Criteria window.
Go to Row
Enter a row number and press Tab to display the data starting from this row.
 Note
The input number must be a number between 1 and the maximum row number.
 Note
This field is available when you select the Enable Quick Display checkbox in the Inventory Audit Report – Selection Criteria
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
This is custom documentation. For more information, please visit SAP Help Portal. 164

6/8/26, 6:12 AM
Last <Number> Rows – Choose this button to display the data in the last page of the table. This button is disabled if the
current display is the last page.
 Note
This dropdown list is available when you select the Enable Quick Display checkbox in the Inventory Audit Report – Selection
Criteria window.
Total Value
Display the cumulative value of all the data that meets the selection criteria.
 Note
This field is available when you select the Enable Quick Display checkbox in the Inventory Audit Report – Selection Criteria
window.
Production Std Cost
Displays the production standard cost of the item as defined in the Item Master Data window.
Total Production Std Cost
Displays the total production standard cost as calculated on the BOM.
View
Select the appropriate view to display the data:
Summary – Select the Summary option to display each item data consolidated in one row in the table including the basic
information. Note that this option is selected by default.
Detailed – Select the Detailed option to display detailed transactional data for each item.
 Note
This dropdown listis available when you select the Enable Quick Display checkbox in the Inventory Audit Report – Selection
Criteria window.
Inventory Valuation Simulation Report
 Note
If your company manages nonperpetual inventory, the name of this report is Inventory Valuation Report. There are some minor
differences between the Inventory Valuation Report and Inventory Valuation Simulation Report.
If you work with perpetual inventory, you can use this report to valuate the entire warehouse inventory of all items on a reporting
date. You would normally valuate the warehouse inventory on the balance sheet reporting date.
 Note
This report is intended to be a managerial report to check what-if scenarios. For instance, you can see what happens if you
value an item based on a different calculation method. This report is not intended to be used as a report for auditing. For
auditing purposes, use the Inventory Audit Report.
This is custom documentation. For more information, please visit SAP Help Portal. 165

6/8/26, 6:12 AM
If necessary, you can choose a different valuation method for warehouse inventory valuation, and you can also transfer the results
to accounting. If you use the moving average price method, you calculate the same values as in the Financials module. Once you
have selected a valuation method, we recommend that you continue to use the same method.
In addition to the standard report (classic inventory valuation simulation report), you can also run an enhanced version of the
standard inventory valuation simulation report (enhanced inventory valuation simulation report). The main differences in this
enhanced version are as follows:
It lets you valuate each item on the basis of the valuation method in the item master data; that is, different items may be
valuated using different valuation methods. Therefore, if you specify the common selection criteria for this report and for
the inventory audit report identically, then the results of both reports are also the same. Alternatively, you can select any of
the calculation methods offered in the classic report, for example, if you want to simulate one or more “what-if” scenarios.
You have the option to filter out inflation-based revaluations from the report. It is a requirement of IFRS not to include
inflation-based revaluations in inventory valuation. Alternatively, if required by local GAAP, you can take inflation-based
revaluations into account.
 Recommendation
For local reporting, use the inventory audit report, not the inventory valuation simulation report.
The results of the inventory audit report are based on the existing records in the database, while the inventory valuation
simulation report simulates the inventory value based on “what-if” scenarios.
 Note
When you print the report, you can also print the selection criteria on a separate page.
Procedures
To determine which report you are going to display, proceed as follows:
1. Go to Administration System Initialization General Settings
2. Under the Inventory tab, choose Reporting
3. You can then choose one of the following radio buttons under Inventory Valuation Simulation Report:
Classic Valuation Report, Excluding Item Master Valuation
Enhanced Valuation Report, Including All Valuation Methods
Related Information
Inventory Valuation Simulation Report - Selection Criteria
Enhanced Inventory Valuation Simulation Report - Selection Criteria
Inventory Valuation Simulation Report - Selection Criteria
This topic is used for the standard (classic) inventory valuation simulation report. For general information about this report, see
Inventory Valuation Simulation Report. For more information about the selection criteria of the enhanced inventory valuation
simulation report, see Enhanced Inventory Valuation Simulation Report - Selection Criteria.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 166

6/8/26, 6:12 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Valuation Simulation Report – Selection Criteria Fields
Vendor From... To...
You can restrict the selection by the main vendor of an item. The main vendor is specified in the item master record. You can
valuate all the items from one or more main vendors.
Warehouses Selection By Location, By Whse (Including From … To, Excluding From … To)
Determine which storage locations will be considered in the report. Make the selection by location, or by warehouse, in which case
you define range of included or excluded warehouses.
Do Not Display Inventory Transfers
Indicate whether or not you want inventory transfers for items to be displayed in the valuation. Depending on which warehouse you
select, both inventory placements and withdrawals are displayed in the list.
 Example
If you select only one warehouse, only the incoming and outgoing inventory transfers for this warehouse are displayed. The
offsetting movements with the other warehouses involved in the transfer are not shown.
 Note
Inventory transfers usually have no effect on the total warehouse inventory of an item, and therefore have no influence on the
valuation of the warehouse inventory.
Posting Date To
Enter the final date for the calculation.
Project From...To...
You can valuate the warehouse inventories for one or more projects. Enter the project(s) if relevant.
Calc. Method
Choose one of the calculation methods below.
 Note
You cannot select the same calculation method as that defined for the item, because this report is intended for examining
what-if scenarios.
Moving Average
SAP Business One valuates your inventories with the moving average price on an ongoing basis. This means a valuation takes
place based on the corresponding quantities and prices for each goods receipt and issue, and the moving average price is updated
accordingly. The valuation price is calculated as the quantity multiplied by the average price. Assuming prices will increase over
time, the items in stock will be overvalued. This gain is not as high as under the FIFO method.
FIFO
Under this valuation method, SAP Business One assumes that the items that entered the warehouse first will also exit first. This
means goods issues are valuated with the prices that are valid for the first goods receipts. For example, if you purchase an item at
three different prices on three different occasions, SAP Business One assumes that the first items you sell are from the first
delivery. This means the prices from the first purchase order are used for the sale and calculation of the corresponding gross
This is custom documentation. For more information, please visit SAP Help Portal. 167

6/8/26, 6:12 AM
profit, until the quantity from the first purchase document is gone. At this point, SAP Business One uses the price for the items
from the second purchase order. Assuming prices will increase over time, the items in stock will be valuated using the higher prices
from the later purchase documents.
By Price List
You can use one of the price lists defined in SAP Business One to valuate the warehouse inventories. When you choose this
method, the Price Source field appears. In the dropdown list, select a price list. SAP Business One then uses the prices defined for
the items in the price list you have selected.
Last Evaluated Price
You can also perform the valuation based on the last evaluated prices. In this case, SAP Business One uses the last calculated
costs for each item. If you run a valuation under the FIFO method, for example, and then run a valuation for the last calculated
costs, SAP Business One valuates the items using the last value that was determined for an item under the FIFO method.
Weighted Average
 Note
This option isn't supported in the Israel localization.
With this method, at the end of the reporting period, an average value is calculated as a base for the valuation of the goods issues
and inventory stock balance. The value is the total amount of inventory open balance plus all goods receipts, which are based on all
A/P documents. Goods issues are not considered. For more information, see Calculation of Weighted Average.
If this option is selected, the following checkboxes are displayed:
Include All Revaluations, enabling all revaluations for the selected period to be considered. Once chosen, the checkbox
Update Previous Closing Balance with Cross Period Revaluations isn't available.
OB from Start of Posting Period, allowing you to consider the opening stock balance from the beginning of the posting
period, in case it's generated at the end of the previous period.
Update Previous Closing Balance with Cross Period Revaluations, updating the closing balance of a previous period with
revaluations, that are posted in the current period but relevant for a receipt in the earlier period.
After running the valuation report by weighted average, a button Update is available in the footer of the result form. You can press
the button to save the calculated quantity and the weighted average price in a new table, which is used as the opening balance of
the next reporting period.
Price Source
If you selected the By Price List option, choose the price list for the report calculation.
Display Method
Choose one of the following display formats for the report:
Row per Item - Displays one row per item
Detailed Receipts/Releases - Displays all goods issues and receipts
FC Exchange Rate
If you valuate transactions in a foreign currency, select one of the following:
Exchange Rate on Report Date
The cumulative values are converted according to the exchange rate on the report date.
This is custom documentation. For more information, please visit SAP Help Portal. 168

6/8/26, 6:12 AM
Transaction Rate
If the calculation method is Moving Average or FIFO and you have selected Additional FC for Total and specified a
foreign currency, the exchange rate is used for display purposes only. The item costs are always based on the
transaction value in local currency. The foreign currency values are displayed according to the exchange rates that
exist for the dates on which the respective documents were added ( Administration Exchange Rates and
Indexes ).
If the calculation method is By Price List or Last Evaluated Price and the price is maintained in the respective price
list in a foreign currency, the exchange rates that exist for the dates on which the respective documents were added
( Administration Exchange Rates and Indexes ) are used to calculate the item costs in local currency.
The following example illustrates how the value of a transaction may be simulated differently according to the calculation
method:
 Example
Calculation Good Unit FC Goods Price Exchange Report: Report: Report:
Method Receipts Price in Translation Receipts in Rate in Cost in Transaction Transaction
Qty Goods Rate in Total Price Exchange LC Value in LC Value in FC
Receipt Goods List Rates and
Receipt Indexes
Window on
Transaction
Date
Moving 10 USD 10 0.75 CLP 75 N/A 1* CLP 8 CLP 75 USD 75
Average
FIFO 10 USD 10 0.75 CLP 75 N/A 1* CLP 8 CLP 75 USD 75
By Price 10 N/A N/A N/A USD 1** CLP 10 CLP 100 USD 100
List 10
Last 10 N/A N/A N/A CLP 5 1* CLP 5 CLP 50 USD 50
Evaluated
Price
* = Used to display transaction value in foreign currency
** = Used to display cost and transaction value in local currency
In Release Receipt Rate
 Note
This checkbox is available for non-perpetual inventory systems if the FIFO calculation method is used.
It determines which exchange rate is used for releases of goods from stock. If the checkbox is selected, the calculation is
based on the exchange rate of the day the inventory entered the stock (for example, when the item was bought). If the
checkbox is deselected, the calculation is based on the exchange rate of the day the item was released from stock (for
example, when the item was sold).
Allow Negative Inventory
Select the checkbox to allow negative inventory during valuation. Items may have negative inventories. From the accounting
perspective, no procedure is available for valuating negative inventories.
This is custom documentation. For more information, please visit SAP Help Portal. 169

6/8/26, 6:12 AM
 Note
For more information negative inventory settings, see Document Settings: General Tab.
If you allow negative inventories, the following situations are possible:
If an item has negative inventory during the reporting period and you have selected this option, the item is valuated based
on the selected valuation method. If SAP Business One finds such an item while running the report, the row for that item
appears in green in the report results.
If an item has negative inventory on the reporting date, the valuation result will depend on the selected valuation method. If
valuation by moving average price is selected, a negative value is calculated for the item. If the FIFO valuation method is
selected, no valuation is possible. The row for the item appears in red in the report results. If no valuation can be performed,
the row for the item contains the remark N/A (not applicable) to indicate that no valuation has been performed.
To avoid negative inventories on the reporting date, post a goods receipt for an A/P invoice on or just before the reporting date.
Additional FC for Total
Displays the valuation in a foreign currency.
By default the field is deselected and the results are displayed in local currency.
If you select Additional FC for Total, an additional field is displayed in which you must select the required currency. You can then
switch between the local currency and the selected foreign currency on the top left of the report results window.
If you specify an additional currency, it is displayed the next time you open the report.
Inventory Valuation Simulation Report - Detailed
 Note
If your company manages nonperpetual inventory, the name of this report is Inventory Valuation Report.
If you want to view the result of the next item, in the toolbar, click the icon. You can use the and icons to navigate
through the list of valuated items.
If you selected the Detailed Receipts/Releases option in the Inventory Valuation Simulation Report - Selection Criteria window,
the Inventory Valuation Simulation Report window displays all the document details for each item you have selected.
The upper section of the window indicates the:
Valuation method chosen for the report
Currency in which the report was prepared
Specified reporting date for valuation
The display also contains the number and a description of the selected item.
If you set the flag for an additional foreign currency in the selection window, you can switch to the display in this foreign currency
here.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 170

6/8/26, 6:12 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Valuation Simulation Report Fields
Posting Date, Reference
Contain the date and the type/number of the posting that was used to move the item.
Warehouse, Quantity
Contain the issuing/receiving warehouse of the goods movement, along with the quantity of the item recorded in the document.
Price
The unit price of the item in the document (for inventory receipts) or the calculated price (for issue from stock).
Total
Total document value. The value is calculated as Qty X Price.
Cumulative Qty
The cumulative quantity of an item inventory after the goods are moved.
Cumulative Value
The cumulative value (in local or in foreign currency) after the goods are moved.
 Note
The total balances for the quantities and values appear near the bottom of the list.
If you only need to compare the warehouse inventory value with the balance sheet value, you do not have to run the detailed
format of the report. The totals display with one row per item will suffice for this purpose.
 Recommendation
The preparation of the warehouse inventory valuation with the detailed option for displaying all the documents for an item can
take a long time. Therefore, we recommend that you start this report at the end of the workday.
Inventory Valuation Simulation Report - Row per Item
 Note
If your company manages nonperpetual inventory, the name of this report is Inventory Valuation Report.
If you selected the Row per Item option in the Inventory Valuation Simulation Report - Selection Criteria window, the Inventory
Valuation Simulation Report window displays a summary of each item you have selected on a separate row.
The upper section of the window indicates the valuation method chosen for the report, the currency in which the report was
prepared, and the specified reporting date for valuation.
If you select an additional foreign currency in the selection window, you can switch to the display in this foreign currency here.
Choose the entry you need from the dropdown list.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 171

6/8/26, 6:12 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Valuation Simulation Report – Row per Item Fields
Last Evaluated Price
Displays the valuation price for a unit of the item based on the selected valuation method.
Quantity
Displays the available quantity of the item in the warehouse.
Enhanced Inventory Valuation Simulation Report - Detail
The following information is provided to help you interpret the report results:
Each item's last evaluated price is updated with the item cost from the simulation. This applies not only to the items
displayed but to all simulated items. If the calculation method for an item was moving average price, the last evaluated
price = cumulative value/cumulative quantity. If the calculation method for an item was FIFO, the last evaluated price = the
next open layer's item cost.
Items with no transactions within the specified date range are displayed with an opening balance.
You can export the report results to Microsoft Excel. For more information, see Toolbar.
A simulation based on the same selection criteria as a previous simulation but run at a later time yields consistent results
even if changes have since been made to bills of materials or to the item master data fields Items per Sales Unit or Items
per Purchase Unit. The application reads from the database the historical bill of material or item master data that was valid
at the respective transaction dates.
If one of the following combinations of methods applies for an item, the simulation run ignores any inventory revaluations
done for that item:
Valuation Method on Inventory Tab of Item Master Data Calculation Method in Inventory Valuation Simulation Report
MAP FIFO
FIFO MAP
STD FIFO
Child items are simulated according to the same logic as parent items.
Examples of Parent Item and Child Item Valuation Methods
Valuation Method on Inventory Tab of Report Selection Criteria Valuation Method Used for the
Item Master Data Calculation
Parent item = MAP Parent item selected Parent item = FIFO
Child 1 = FIFO Calculation method = FIFO Child 1 = FIFO
Child 2 = Standard Child 2 = FIFO
Parent item = MAP Parent item selected Parent item = MAP
Child 1 = FIFO Child 1 = FIFO
This is custom documentation. For more information, please visit SAP Help Portal. 172

6/8/26, 6:12 AM
Valuation Method on Inventory Tab of Report Selection Criteria Valuation Method Used for the
Item Master Data Calculation
Child 2 = Standard Calculation method = Based on Item Child 2 = Standard
Definition
If the simulation run ends with errors or warnings, you can view them in a message log.
The report results are stored in the following tables: SITM, SITW, SIVL, SIVL1, SIVQ, SIVE, SIVK, OISL.
More Information
Support for IFRS in SAP Business One
Related Information
Enhanced Inventory Valuation Simulation Report - Selection Criteria
Inventory Valuation Simulation Report
Enhanced Inventory Valuation Simulation Report - Detail
The following information is provided to help you interpret the report results:
Each item's last evaluated price is updated with the item cost from the simulation. This applies not only to the items
displayed but to all simulated items. If the calculation method for an item was moving average price, the last evaluated
price = cumulative value/cumulative quantity. If the calculation method for an item was FIFO, the last evaluated price = the
next open layer's item cost.
Items with no transactions within the specified date range are displayed with an opening balance.
You can export the report results to Microsoft Excel. For more information, see Toolbar.
A simulation based on the same selection criteria as a previous simulation but run at a later time yields consistent results
even if changes have since been made to bills of materials or to the item master data fields Items per Sales Unit or Items
per Purchase Unit. The application reads from the database the historical bill of material or item master data that was valid
at the respective transaction dates.
If one of the following combinations of methods applies for an item, the simulation run ignores any inventory revaluations
done for that item:
Valuation Method on Inventory Tab of Item Master Data Calculation Method in Inventory Valuation Simulation Report
MAP FIFO
FIFO MAP
STD FIFO
Child items are simulated according to the same logic as parent items.
Examples of Parent Item and Child Item Valuation Methods
Valuation Method on Inventory Tab of Report Selection Criteria Valuation Method Used for the
Item Master Data Calculation
This is custom documentation. For more information, please visit SAP Help Portal. 173

6/8/26, 6:12 AM
Valuation Method on Inventory Tab of Report Selection Criteria Valuation Method Used for the
Item Master Data Calculation
Parent item = MAP Parent item selected Parent item = FIFO
Child 1 = FIFO Calculation method = FIFO Child 1 = FIFO
Child 2 = Standard Child 2 = FIFO
Parent item = MAP Parent item selected Parent item = MAP
Child 1 = FIFO Calculation method = Based on Item Child 1 = FIFO
Definition
Child 2 = Standard Child 2 = Standard
If the simulation run ends with errors or warnings, you can view them in a message log.
The report results are stored in the following tables: SITM, SITW, SIVL, SIVL1, SIVQ, SIVE, SIVK, OISL.
More Information
Support for IFRS in SAP Business One
Related Information
Enhanced Inventory Valuation Simulation Report - Selection Criteria
Inventory Valuation Simulation Report
Inventory Valuation Method Report
This report contains information that may be required for IFRS reporting disclosure. IFRS reporting requires an overview of the
method used to value your company's inventory, for example in the Notes to Financial Statements. In SAP Business One, it is
possible to specify the inventory valuation method at the item level, and to group the inventory items that are of a similar nature in
item groups. Inventory items with a similar nature should be valued using the same method, and this report can be used to validate
your inventory valuation methods prior to IFRS reporting. You may need to provide the result of this report as part of your IFRS
disclosure requirement.
This report can be found under Inventory Inventory Reports Inventory Valuation Method Report .
 Note
This report is relevant for perpetual inventory systems only. The valuation method for each item is read from the item master
data. If your company is running a nonperpetual inventory system, the Valuation Method field is not available in the item
master data.
Selection Criteria
By default, all items, item groups, locations, and warehouses are preselected. Therefore, to run the report for all items, item groups,
locations, and warehouses, all you need to do is choose the OK button.
If you need to define specific selection criteria, you have the following options:
Items
This is custom documentation. For more information, please visit SAP Help Portal. 174

6/8/26, 6:12 AM
You can specify the items you want to include in the report in several ways. You can specify:
Single item numbers
A range of item numbers
Whole item groups
Warehouse
You can also include items in the report based on their storage location. Every warehouse, each warehouse in a particular
location, or individual warehouses can be included in the report as required.
Report Result
The report displays the list of item groups chosen in the selection criteria and the items that fit those criteria, grouped by item
group. The name of each item group is displayed, along with the valuation methods used for the item group, and the number of
items valued using each method. You can drill down to the specific item or list of items summarized under a specific item group or
valuation method to see the item code, item name, and its valuation method. This can help you to analyze the valuation method
assigned to specific items and to decide whether there is a need to disclose the information in your financial statements.
Generating the Serial Number Transactions Report
The serial number transactions report displays all transactions made for each serial number-managed item currently in the
system and those that have been released in the past.
Procedure
1. Choose Inventory Inventory Reports Serial Number Transactions Report . The Serial Number Transactions Report
- Selection Criteria window appears.
 Note
After generating inventory receipt documents and inventory issue documents, you can also display the serial number
transactions report linked to the document by opening the required document and choosing Serial Numbers
Transactions Report from the Go To menu. Alternatively, right-click the window and select Serial Numbers
Transactions Report. The report displays all the serial numbers linked to the document.
2. Specify the following data to determine which transactions to display in the report:
Field Activity / Description
Item Number from ... To Specify a range of item codes.
Group Select item groups.
Properties Select item properties in the Properties dialog.
On the Dates tab, set the range of dates based on posting dates, release dates, expiration dates, creation dates, or
the start and end dates of the warranty for the report.
On the Numberings tab, specify the appropriate number ranges.
On the Warehouse tab, specify selection criteria by the warehouse location of the serial number.
This is custom documentation. For more information, please visit SAP Help Portal. 175

6/8/26, 6:12 AM
On the BP tab, specify the selection criteria by the business partners against whom the serial number transactions
are performed.
On the Documents tab and subtabs, define for which documents the serial number transactions are to be displayed,
and whether transactions from closed documents are to be displayed.
3. To generate the report, choose the OK button. The Serial Number Transactions Report window appears.
Serial Number Transactions Report - Selection Criteria Window
Use this window to specify selection criteria to display all transactions made for serial number-managed items and generate the
Serial Number Transactions report.
To access this window, choose Inventory Inventory Reports Serial Number Transactions Report .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
Item Number from...to
Specify a range of item codes.
Group
Select an item group.
 Note
The Default Settings button resets all the defined selection criteria.
Dates tab
You can use the Dates tab to set a range of dates based on posting dates, receipt dates, expiration dates, manufacturing dates, or
the start and end dates of the manufacturing warranty.
Posting Date from... to
Enter the necessary posting dates for the report.
Release Date from... to
Specify the necessary release dates for the report.
Expiration Date from ... to
Specify the necessary expiry dates for the report.
Creation Date from ... to
Specify the necessary creation dates of the serial numbers for the report.
Warranty Start from ... to
Specify the necessary warranty dates for the report.
This is custom documentation. For more information, please visit SAP Help Portal. 176

6/8/26, 6:12 AM
Warranty End from ... to
Specify the necessary warranty end dates for the report.
Numberings tab
You can use the Numberings tab to set selection criteria by System Number, Lot Numbers, Mfr. Serial No., or Serial Number. You
can also choose to display Available and/or Unavailable serial numbers.
System No. From ...To
Specify a range of system numbers.
Lot Number From ...To
Specify a range of lot numbers.
Mfr. Serial No. From ... To
Specify a range of manufacturer serial numbers.
Serial Number From ... To
Specify a range of internal serial numbers.
Status From ... To
Specify a range of statuses of the serial numbers.
Warehouse tab
You can use the Warehouse tab to set selection criteria by warehouse or location.
Warehouse From ... To
Specify the range of warehouses.
Location From
Specify the warehouse from which the items are delivered.
Location To
Specify the warehouse to which the items are delivered.
BP tab
You can use the BP tab to set the linked business partner range. Linked cards are those appearing in documents with serial
numbers.
Code From
Specify the range of Business Partner codes.
Customer Group
Specify the customer groups to which the Business Partners are associated.
Vendor Group
Specify the vendor groups to be included in the report.
Properties
This is custom documentation. For more information, please visit SAP Help Portal. 177

6/8/26, 6:12 AM
In the Properties window, specify Business Partner properties to use as selection criteria.
Documents tab
You can use the Documents tab to define from which documents to display the serial number transactions, and whether to display
transactions from closed documents.
Purchasing - A/P tab
You can use the Purchasing - A/P tab to specify the purchasing document types from which to display transactions.
Goods Receipt PO
Displays transactions created in Goods Receipt documents.
Goods Return
Displays transactions created in Goods Returns documents.
A/P Invoices
Displays transactions created in AP Invoice documents.
A/P Credit Memos
Displays transactions created in A/P Credit Memo documents.
Sales - A/R tab
You can use the Sales - A/R tab to specify the sales document types for which to display transactions.
Deliveries
Displays transactions created in Delivery documents.
Returns
Displays transactions created in Return documents.
A/R Invoices
Displays transactions created in A/R Invoice documents.
A/R Credit Memos
Displays transactions created in A/R Credit Memo documents.
Inventory Posting tab
You can use the Inventory Posting tab to specify inventory-related documents from which to display transactions.
Goods Issue
Displays transactions created in Goods Issue documents.
Goods Receipt
Displays transactions created in Goods Receipt documents.
Inventory Transfers
Displays transactions created in Inventory Transfer documents.
This is custom documentation. For more information, please visit SAP Help Portal. 178

6/8/26, 6:12 AM
Stock Updates
Displays transactions created in Stock Updates documents.
Doc. Settings tab
You can use the Doc. Settings tab to specify a range of documents to be included in this report.
Display Closed Documents
Select this option to display documents that have already been closed.
Related Information
Serial Number Transactions Report Window
Serial Number Transactions Report Window
The Serial Number Transactions report displays the inventory receipts and issues for each serial number for the selected criteria.
If you select a row in the Serial Numbers table in the window; the relevant transaction details appear in the Transactions for Serial
Number table.
The contents of the report varies, depending on how you open the report:
Choose Inventory Inventory Reports Serial Numbers Transactions Report . Then choose OK Enter the required
criteria in the Serial Number Transactions Report - Selection Criteria Window and choose the OK button.
The Serial Numbers table displays all series.
 Note
To view all the transactions associated with a selected serial number, select the Display All Transacs for Selected No.
checkbox at the bottom of the window.
In the Serial Number Details Window, right-click on the window, or choose the Go To menu, and choose the Serial Number
Transactions Report option.
The report opens with only the selected serial numbers in the Serial Numbers table. All serial number transactions of the
selected item are listed in the Transactions for Serial Number table.
To open from marketing documents, inventory transactions, or production inventory transactions, right-click on the
window, or choose the Go To menu, and choose the Serial Number Transactions Report option. (This option is enabled
only after the document has been added, and only for documents that have created the inventory transaction for the item.)
The Serial Numbers table displays all serial numbers that are associated with the document. To display all the receipt and
issue transactions for a serial number, highlight the row in the Serial Numbers table, and the transactions are displayed in
the Transactions for Serial Number table.
In the Item Master Data window, right-click on the window, or choose the Go To menu, and choose the Serial Numbers
Transactions Report option.
The Serial Numbers table displays all serial numbers associated with the item.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 179

6/8/26, 6:12 AM
Click to the left of Mfr. Serial No, Serial Number, or Lot Number to open the Serial Number Details window, where you can
update data for the selected serial number.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Serial Numbers Table
Expiration Date
Displays the expiration date of the item you selected in the previous window.
Mfr. Date
Displays the manufacture date of the item you selected in the previous window.
Mfr. Serial. No.
Displays the manufacturer serial number of the item you selected in the previous window.
Mfr. Warranty End
Displays the warranty end date of the item you selected in the previous window.
Mfr. Warranty Start
Displays the warranty start date of the item you selected in the previous window.
Serial Number
Displays the internal serial number of the item you selected in the previous window.
Lot Number
Displays the lot number of the item you selected in the previous window.
Admission Date
Displays the creation date of the serial numbers.
System No.
Displays the system number of the item you selected in the previous window.
Status
Displays the status of the serial numbers for an item namely, available or unavailable.
Transactions for Serial Number Table
Document
Displays the shortened title of the document and the document number.
Date
Displays the document date of the item.
G/L Acct./BP Code, G/L Acct./BP Name
Displays the name and code of the general ledger account or business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 180

6/8/26, 6:12 AM
Allocated
Displays the allocation status of the serial number item in each document as follows:
The positive number 1 shows that the item with this serial number is allocated in the document.
The negative number -1 shows that the item with this serial number is de-allocated in the document. The de-allocation
applies in the following scenarios:
You deselect the serial numbers that were previously allocated in the document.
You deliver the serial number items that were previously allocated in a document. SAP Business One automatically
de-allocates the serial number.
Direction
Describes the transaction – In, Out, Allocated, or Return Candidate.
Return Candidate only applies to a serial-numbered item that is added to a return request and is waiting to be returned.
The direction for a serial-numbered item in a return or an A/R credit memo is In.
Return Candidate
Displays the return status of a serial-numbered item as follows:
The positive number 1 shows that the item is added to a return request.
The negative number -1 shows that the item is selected in a return or A/R credit memo, which is copied from a return
request that includes the same item.
This column is hidden by default. You can display it via Form Settings.
Display All Transacs for Selected No.
Select to include all transactions, including those from non-selected serial numbers.
More Information
Serial Number Transactions Report - Selection Criteria Window
Serial Number Details Window
Generating the Batch Number Transactions Report
Context
This report displays different batch number transactions for the selected item number.
Procedure
1. Choose Inventory Inventory Reports Batch Number Transactions Report .
The Batch Number Transactions Report - Selection Criteria window appears.
2. Specify the selection criteria to determine which transactions to display in the report.
3. Choose the OK button to open the Batch Number Transactions Report window.
This is custom documentation. For more information, please visit SAP Help Portal. 181

6/8/26, 6:12 AM
Each row in the top table displays a single batch in a warehouse. The table shows various details from the batch master
data and displays the current quantity of the batch in the warehouse. If a batch exists in multiple warehouses, the table
shows the same batch in multiple rows with the quantities for each warehouse.
 Note
You can also open the report as follows:
In inventory receipt or issue documents:
Right-click and choose the Batch Number Transactions Report option
Choose the Batch Number Transactions Report option from the Go To menu
This option is enabled only after the document has been added, and only for documents that created the
inventory transaction for the batch.
In the Item Master Data window:
Right-click in the window and choose the Batch Number Transactions Report option
Choose the Batch Number Transactions Report option from the Go To menu
4. Highlight any row to display all its receipt and issue transactions based on your selection in the previous window.
The transactions are displayed in the Transactions for Batch table. Here, you can view details regarding the transaction
such as its origin, date, document number, and so on.
5. To display a full history of the selected batch, choose Display all Transactions for Selected Batches.
This displays transactions that do not match the settings made previously in the preferences window.
You can display the transactions according to relevant warehouses. Use the Whse From and To fields to set the desired
range.
6. To display batches with no available quantity, select the Display Batches With Zero Qty checkbox.
Batch Number Transactions Report - Selection Criteria Window
Use this window to specify selection criteria to display all transactions made for batch number-managed items and generate the
batch number transactions report.
To access this window, choose Inventory Inventory Reports Batch Number Transactions Report .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
Item Number From ... To
Select a range of items numbers to specify which items to display in the report.
Group
Specify the items' group.
Properties button
This is custom documentation. For more information, please visit SAP Help Portal. 182

6/8/26, 6:12 AM
Opens the Properties window where you can filter the report by item properties.
 Note
The Default Settings button resets all the defined selection criteria.
Dates Tab
Set the report date range by reference, manufacture, expiration dates, and more.
Posting Date From ...To
Specify the necessary posting dates for the report.
Release Date From ... To
Specify the necessary release dates for the report.
Expiration Date From ... To
Specify a range of item expiration dates.
Creation Date From ... To
Specify the necessary creation dates for the report.
Numberings Tab
Set the numbering ranges according to the parameters defined in the Batch Number Selection window.
Batch From ... To
Specify a range of batch numbers.
Batch Attribute 1 From ... To
Specify a range of batch attributes.
Batch Attribute 2 From ... To
Specify a range of batch attributes.
Status From ... To
Specify a range of batch number statuses.
Warehouse Tab
Specify the warehouse range to be selected.
Warehouse From ... To
Specify the warehouses to be shown in the report.
Location From ... To
Specify the shipping and receiving locations of the batch items.
BP Tab
Specify the range of business partners involved in the batch transactions (documents).
This is custom documentation. For more information, please visit SAP Help Portal. 183

6/8/26, 6:12 AM
Code From ... To
Specify the business partner codes.
Customer Group
Specify the customer group to determine which transactions are displayed in the report.
Vendor Group
Specify the vendor group pertaining to the selected business partners.
Properties button
Opens the Properties window where you can filter the report by business partner properties.
Select the documents in which batch numbers were created/selected.
Documents Tab
You can use the Documents tab to define from which documents to display the batch number transactions.
Purchasing - A/P Tab
Goods Receipt PO
Displays transactions created in goods receipt PO documents.
Goods Return
Displays transactions created in goods returns documents.
A/P Invoices
Displays transactions created in AP invoice documents.
A/P Credit Memos
Displays transactions created in credit memo documents.
Sales - A/R Tab
Deliveries
Displays transactions created in delivery documents.
Returns
Displays transactions created in returns documents.
A/R Invoices
Displays transactions created in invoice documents.
A/R Credit Memos
Displays transactions created in credit memo documents.
Sales Orders
Displays transactions created in sales order documents.
Inventory Posting Tab
This is custom documentation. For more information, please visit SAP Help Portal. 184

6/8/26, 6:12 AM
Goods Issue
Displays transactions created in goods issue documents.
Goods Receipt
Displays transactions created in goods receipt documents.
Inventory Transfers
Displays transactions created in inventory transfer documents.
Stock Updates
Displays transactions created in inventory documents.
Doc. Settings Tab
Display Closed Documents
Displays transactions created in documents that had already closed.
Display Canceled Documents
Displays transactions created in documents that may have been canceled.
Batch Number Transactions Report Window
The batch number transactions report displays the inventory receipts and issues for each batch number in the system for the
selected criteria.
To access this window, choose Inventory Inventory Reports Batch Number Transactions Report .
Define the selection criteria and choose the OK button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Batches Table
Batch
Batch number of the item you selected in the previous window.
Batch Attribute 1
Enter an additional number or attribute for the batch.
Batch Attribute 2
Enter an additional number or attribute for the batch.
Whse Code
Warehouse code of the item you selected in the previous window.
Quantity
Number of items included in the batch you selected in the previous window.
This is custom documentation. For more information, please visit SAP Help Portal. 185

6/8/26, 6:12 AM
Manufacturing Date
Manufacturing date of the item you selected in the previous window.
Status
Status of the item's batch you selected in the previous window.
Expiration Date
Expiration date of the item's batch you selected in the previous window.
Transactions for Batch Table
Document
Displays the shortened title of the document and the document number.
Date
Displays the document date of the item.
G/L Acct/BP Name
Displays the name of the general ledger account or business partner.
Qty
Displays the inventory change of the batch items triggered by each document as follows:
The positive number shows how many items of this batch are received in the inventory.
The negative number shows how many items of this batch are issued from the inventory.
Allocated
Displays the allocation details of the batch items in each document as follows:
The positive number shows how many items of this batch are allocated in the document.
The negative number shows how many items of this batch are de-allocated in the document. The de-allocation applies in
the following scenarios:
You deselect some or all of the batch items that were previously allocated in the document.
You deliver the batch items that were previously allocated in a document. SAP Business One automatically de-
allocates the batch items.
Direction
Describes the transaction – In, Out, Allocated, or Return Candidate.
Return Candidate only applies to part or all of the items in a batch that are added to a return request and are waiting to be
returned.
The direction for batch items in a return or an A/R credit memo is In.
Return Candidate
Displays the return status of part or all of the items in a batch as follows:
A positive number shows the number of items that are added to a return request.
This is custom documentation. For more information, please visit SAP Help Portal. 186

6/8/26, 6:12 AM
A negative number shows the number of items that are selected in a return or A/R credit memo, which is copied from a
return request that includes the same items.
This column is hidden by default. You can display it via Form Settings.
Display All Transactions for Selected Batches
Displays all historical transactions for the selected batch, regardless of the selection made in the previous window.
Display Batches with Zero Qty.
Displays all batches of the selected item with a zero quantity, regardless of the selection made in the previous window.
Whse From ... To
Specify the warehouses to be shown in the report.
Price Report
You can use this report to view the different prices defined for a specific item and for a specific business partner, according to the
defined selection criteria. (For more information, see Price Report - Selection Criteria Window.) The report lists the defined prices
of the selected price resources, which can be one or all of the following options:
Price List
Special Prices for Business Partner
Period and Volume Discount
The price report can be generated from the Inventory main menu or from the Reports main menu, and also by right-clicking the
row of a marketing document.
When you generate this report from a marketing document, the report displays all the price sources of the document's row and, if
required, enables choosing other prices to be updated in the document's row. For more details, see Tracking Prices and Discounts
from Marketing Documents.
Related Information
Price Report Window
Price Report - Selection Criteria Window
To open the Price Report - Selection Criteria window, from the SAP Business One Main Menu, choose Inventory Inventory
Reports Price Report . In the Price Report - Selection Criteria window, specify your selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Price Report – Selection Criteria Fields
Source of Price
From the dropdown list, select the price resource:
This is custom documentation. For more information, please visit SAP Help Portal. 187

6/8/26, 6:12 AM
All (default)
Price list
Special Prices for BP
Period and Volume Discount
 Note
When the Price List option is selected, another field is displayed, where you select a specific price list or all price lists (default).
Inactive price lists are available in this dropdown list according to the setting made in Administration System Initialization
General Settings Inventory Pricing Display Inactive Price Lists Reports .
Business Partners
Specify a range of business partners by BP code, group or properties, or leave the field empty to display all business partners in
the report.
 Note
The Business Partners fields are available only when All or Special Prices for BP is selected in the Source of Price field.
Expanded Selection Criteria
Displays additional selection fields according to the selection in the Source of Price field:
UoM Group
UoM
Quantity - Only items with the same quantity, selected in this field, are displayed in the report. The quantity is compared
with the defined quantity in the Special Prices - Volume Discounts window and in the Volume Discounts for Price List
window.
This field is not available when Price List is selected in the Source of Price field.
Date - Only items with the same date range, selected in this field, are displayed in the report. The date is compared with the
defined date range in the Period Discounts window.
Price lists with the same date range also are displayed in the report.
Base Price List – All price lists. Inactive price lists are available in this dropdown list according to the setting made in
Administration System Initialization General Settings Inventory Pricing Display Inactive Price Lists Reports .
Factor - This field is available only when All or Price List is selected in the Source of Price field.
User Defined Fields – Those are defined in the header of the Price List window and are available when the Price List or All
source of price is selected. Those are defined in any of the special prices windows (Special Prices for Business Partners,
Period and Volume Discounts, Periods Discounts, and Volume Discounts) and are available when the Special Prices for
BP or Period and Volume Discount or All source of price is selected.
Display Inactive Price Lists in Reports
Defines whether prices from inactive price lists are displayed in the report.
Hide Unpriced Items
Defines whether items with no price are displayed in the report.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 188

6/8/26, 6:12 AM
If this checkbox is not selected, items with no price are displayed in the report, regardless of the definition in the
Remove Unpriced Items from Price List in Database checkbox in General Settings. For more information, see General
Settings: Inventory Tab.
This checkbox is not relevant for prices in the Last Purchase Price and the Last Evaluated Price price lists.
Price Report Window
The Price Report window displays all prices, their sources and details, based on the defined selection criteria.
To open this window, from the SAP Business One Main Menu, choose Inventory Inventory Reports Price Report . In the
Price Report - Selection Criteria window, specify the selection criteria, and choose OK.
To generate the price report directly from a marketing document, right-click the document's row and choose Price Report. The
report is generated using all price sources and other data from the document as the selection criteria of the report.
 Note
All prices from Price Lists, Special Prices for Business Partner, and Period and Volume Discounts windows (including their
sub windows), are displayed in the report based on the selected criteria and regardless of the definition in the Remove
Unpriced Items from Price List in Database checkbox in the General Settings window. For more information, see General
Settings: Pricing Tab.
 Note
When All is selected in the Source of Price field, in the Price Report - Selection Criteria window, there might be defined
selection criteria that are not relevant for specific price sources. In those cases, the irrelevant selection criteria are ignored for
the specific price source.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Price Report Fields
Source of Price
The source of the price, which is one of the following:
Special Prices for BP
The price is taken from the Special Prices for Business Partners window, and in case prices are defined in its sub
windows (periods discount and volume discount), they are displayed in separate rows in the report.
A link arrow opens the Special Prices for Business Partners window, even when the price is taken from its sub
window.
Period and Volume Discount
The price is taken from the Period and Volume Discounts window, and in case prices are defined in its sub windows
(periods discount and volume discount), it is also displayed in separate rows in the report.
A link arrow opens the Period and Volume Discounts window, even when the price is taken from its sub windows.
This is custom documentation. For more information, please visit SAP Help Portal. 189

6/8/26, 6:12 AM
Price list name
The price is taken from the Price List window (for pricing unit UoM), and in case prices are defined for any UoM
other than the pricing unit UoM, then it is also displayed in separate rows in the report.
A link arrow opens either the Price List window or the Price List UoM Prices window, depending upon where the
price is defined.
Item No.
The number of the item, as displayed in the relevant source of price.
Item Description
The description of the item, as displayed in the relevant source of price.
BP Code
The business partner code as displayed in the Special Prices for Business Partners window.
 Note
This column is relevant only for the Special Prices for BP source of price.
Base Price List
The base price list as defined in the relevant source of price.
 Note
When the source of price is Price List, the base price is taken from the specific item row.
Factor
The factor as defined in the item row in the relevant price list window.
 Note
This column is relevant only for the Price List source of price.
Primary Currency - Price
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab
If the Price Mode defined on the General tab is Net, the net primary currency price as defined in the relevant source
of price is displayed.
If the Price Mode defined on the General tab is Gross, the gross primary currency price as defined in the relevant
source of price is displayed.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
If you have not selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab
The primary currency - price as defined in the relevant source of price is displayed.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 190

6/8/26, 6:12 AM
For the Special Prices for BP and Period and Volume Discount sources of price, the price is displayed in this column or
in the following columns, according to the source price selected in those sources.
For the Last Purchase Price and Last Evaluated Price sources of price, the price is always displayed only in primary
currency.
Additional Currency 1 - Unit Price
The Additional Currency 1- Unit Price as defined in the relevant source of price.
Additional Currency 2 - Unit Price
The Additional Currency 2 - Unit Price as defined in the relevant source of price.
Discount %
The discount percentage as defined in the item row in the relevant source of price.
 Note
This column is relevant only for the Special Prices for BP and Period and Volume Discount sources of price.
UoM
The item's unit of measurement for which the price is defined.
Quantity
The quantity as defined in the volume discount window in the relevant source of price.
 Note
This column is relevant only for the Special Prices for BP and Period and Volume Discount sources of price.
Active
Displays whether the price list is active as defined in the Price Lists window
 Note
This column is relevant only for the Price List source of price.
Valid From
The date on which the price validity starts, as defined in one of the following:
For the Price List source of price, as defined in the Price Lists window
For the Special Prices for BP and Period and Volume Discount sources of price, as defined in the Period Discounts window
Valid To
The date on which the price validity ends, as defined in one of the following:
For the Price List source of price, as defined in the Price Lists window
For the Special Prices for BP and Period and Volume Discount sources of price, as defined in the Period Discounts window
Remarks
When the base price list is inactive and the Apply Activity of Base Price List on: checkbox on the Pricing tab in Administration
System Initialization General Settings Inventory is selected, prices are taken into the document as zero and a relevant
This is custom documentation. For more information, please visit SAP Help Portal. 191

6/8/26, 6:12 AM
remark is displayed in this column.
Tracking Prices and Discounts from Marketing Documents
You can use the price report or the discount group report, generated from the document's row, to view the different prices defined
for a specific item and, if required, to replace the current price/discount in the document's row with other prices/discounts
displayed in the report.
Procedure
To generate the price report or the discount group report from a marketing document:
1. Open the document from which you want to generate the report.
2. Right-click the relevant document's row and choose Price Report or Discount Group Report.
3. Some data from the document, such as the business partner and the item, are selected automatically as the selection
criteria and the report is generated.
 Note
This option is available in all sales and purchase documents and drafts, except in a purchase request and in duplicated
documents, before choosing the BP. The report is available even when the document status is closed.
Result
The reports display all sources of the price/discount of the document's row.
 Note
When the UoM Group value in the document's row is other than Manual, then the following apply:
If the UoM Code value is the inventory UoM, only inventory UoM prices are displayed in the price report.
If the UoM Code value is a specific UoM other than Manual, both the prices of the specific UoM and the prices of the
inventory UoM are displayed in the price report.
When there is a match between the price/discount in the document's row and one of the sources of the price/discount, the
matched row is highlighted in blue in the report.
When there is no match between the price/discount in the document's row and one of the sources of the price/discount, a
message is displayed and the report is generated with no highlighted row.
 Note
When a discount percentage is a combination of more than one discount (for example, average, total) all relevant rows
are highlighted in blue in the discount group report.
When the source price of the document's row is Manual, a relevant message is displayed during report generation and
no row is highlighted in the report results.
This is custom documentation. For more information, please visit SAP Help Portal. 192

6/8/26, 6:12 AM
You can choose to replace the current price/discount of the particular document's row by double-clicking any row of the report
results. Then, in the document's row, the price/discount is replaced with the chosen price/discount and the price source is
changed to Manual.
 Note
You cannot replace the price/discount with any of the report's rows in the following cases:
For closed rows, for example, a closed row in a sales order
In added documents that are not editable, for example, an added invoice
When the document's row is linked to a blanket agreement
Price/Discount Change Rules
When choosing a different row in the price report, both price and discount are replaced in the document's row.
When choosing a different row in the discount group report, only the discount is replaced in the document's row.
When choosing a different row in any of the reports, the calculation of all relevant rows is updated (tax, gross price, price
after tax, total line, and so on).
When the UoM Code value in the document's row is a specific UoM, rather than an inventory UoM, and in the price report
you choose another price that is related to the inventory UoM, the price adjustment is done automatically according to the
specific UoM.
It is not possible to choose any row from the report if the UoM Code value of the document's row is empty. First you must
specify a UoM code.
When there are no authorizations for price lists or special prices, the prices are masked in the report and you cannot
choose those kinds of rows.
More Information
Price Report
Price Report Window
Discount Group Report
Discount Group Report Window
Inventory Counting Transactions Report
The inventory counting transaction report enables you to view and analyze the existing inventory counting and inventory posting
documents in one place.
Inventory Counting Transactions Report - Selection Criteria
Window
To open this window, from the SAP Business One Main Menu, choose one of the following paths:
This is custom documentation. For more information, please visit SAP Help Portal. 193

6/8/26, 6:12 AM
Inventory Inventory Reports Inventory Counting Transactions Report
Reports Inventory Inventory Counting Transactions Report
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Items Fields
Preferred Vendor
The default preferred vendor of an item. Even if an item has only one preferred vendor, but the preferred vendor is not set as
default, this criterion does not apply to the item.
Warehouses Fields
Warehouses Selection By Location, By Warehouse (Including From … To, Excluding From … To)
Determine which storage locations will be considered in the report. Make the selection by location, or by warehouse, in which case
you define the range of included or excluded warehouses.
Bin Locations
Choose this button to open the Inventory Counting Transactions Report – Bin Location Selection Criteria window, and specify
the criteria for selecting bin locations for the items you want to add to the report.
This button appears only when the selected warehouses are enabled with bin locations.
Inventory Counting Transactions Parameters Fields
Count Date, Posting Date, End of Fiscal Year
Specify the date ranges. The report thus includes documents with count date, posting date, or end of fiscal year within the defined
ranges.
User
Select the checkbox and click the ellipsis button to select users from the user list.
Employee
Select the checkbox and click the ellipsis button to select employees from the employee list. The employee list contains the active
employees who are not users.
User-Defined Fields
Select the checkbox and click the ellipsis button to select user-defined fields that are defined in the Inventory Posting, Inventory
Posting - Row, Inventory Counting, and Inventory Counting - Row categories in the User-Defined Fields - Management window.
Group by Fields
Items
If you select this option, all inventory counting and posting documents that are related to a certain item are grouped together, and
the report lists the documents item by item.
Documents
If you select this option, the report displays the inventory counting and posting documents in sequence of document number.
Display Fields
This is custom documentation. For more information, please visit SAP Help Portal. 194

6/8/26, 6:12 AM
 Recommendation
Do not select to display inventory posting and closed inventory counting at the same time because the same counting results
will be displayed twice. You may get a wrong impression about variances in inventory quantities and values.
Inventory Posting
Select to display inventory posting documents in the report.
Inventory Counting
Select to display only open or only closed inventory counting documents, or both, in the report.
Only Items Not Counted Since
Select to display only the items that have not been counted since a certain date with the selected range specified in the Items field
and Warehouses field. “Not counted” in this case means “not added in inventory counting documents” regardless of whether the
Counted checkbox is selected or not for an item in an inventory counting document.
Once you choose this option, all the selection criteria fields that are related to document selection are disabled. The report only
displays a list of items with general item details.
Only Items with Posted Variance % Greater Than
Select to display all the items that are posted with a variance percentage larger than a certain value.
The calculation of variance % is as follows:
Counted Qty > In-Whse Qty on Count Date: (Counted Qty − In-Whse Qty on Count Date) ÷ In Whse Qty on Count Date × 100
In-Whse Qty on Count Date > Counted Qty: (In-Whse Qty on Count Date − Counted Qty) ÷ In Whse Qty on Count Date × 100
Inventory Counting Transactions Report Window
To open this window, from the SAP Business One Main Menu, choose one of the following paths:
Inventory Inventory Reports Inventory Counting Transactions Report
Reports Inventory Inventory Counting Transactions Report
In the Inventory Counting Transactions Report – Selection Criteria window, select the relevant data and choose the OK button.
At the end of the report, an additional line displays the sums of various counted quantities, variances, and total values. Note that
negative quantities or variances are converted into positive values and then added up while negative inventory values are deducted
from the sum. In addition, the system does not differentiate between values from base documents and target documents; in other
words, if you chose to display both inventory posting documents and closed inventory counting documents, some values may be
counted twice.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Counting Transaction Report Fields
Doc. Row
Indicates the row number of an item in the corresponding document.
This is custom documentation. For more information, please visit SAP Help Portal. 195

6/8/26, 6:12 AM
Single Counter's/Team Qty, Counter X's QTy
The Single Counter's/Team Qty field displays one of the following values:
Inventory counting documents:
The counted quantity for the single-counter counting type.
The team counted quantity for the multiple-counter counting type.
Inventory posting documents: The counted quantity that is recorded in the system as the result of inventory counting.
The Counter X's Qty displays the counted quantity of an individual counter for the multiple-counter counting type. "X" represents
numbers from 1 to 5.
Max Variance, Max Variance %
Biggest variance between the counted quantities and the in-warehouse quantity recorded in the system.
In-Whse Qty on Count Date
Displays the quantities of the item in warehouses recorded by the system on the selected count date and time.
Price
Displays the price per unit of the item.
Total
Total = Price × Variance
Inventory Turnover Analysis - Selection Criteria
Use the Inventory Turnover Analysis report to specify how often average inventory has been consumed. Inventory turnover is
calculated as the ratio of cumulative usage to average inventory level.
An inventory turnover analysis allows you to identify whether there are any "slow-moving items". The Inventory Turnover Analysis
report results are displayed per warehouse, grouped by item group.
To open the Inventory Turnover Analysis - Selection Criteria window, from the SAP Business One Main Menu, choose one of the
following paths:
Inventory Inventory Reports Inventory Turnover Analysis
Reports Inventory Inventory Turnover Analysis
In the Inventory Turnover Analysis - Selection Criteria window, specify your selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Turnover Analysis Report – Selection Criteria Fields
Enter Date Range From...To...
Enter the date range that you want to include in the report.
Select Items
This is custom documentation. For more information, please visit SAP Help Portal. 196

6/8/26, 6:12 AM
Choose the ellipsis button to select the relevant items for the report.
Hide Items with No Quantity in Stock
Select to exclude items with zero quantity from the list.
Select Warehouses
Choose the ellipsis button to select which warehouses will be included in the report. Make the selection by location, or by
warehouse.
Related Information
Inventory Turnover Analysis
Inventory Turnover Analysis
The Inventory Turnover Analysis report shows the calculated inventory turnover as the ratio of cumulative usage to average
inventory level for each item per warehouse.
To open this window, from the SAP Business One Main Menu, choose one of the following paths:
Inventory Inventory Reports Inventory Turnover Analysis
Reports Inventory Inventory Turnover Analysis
In the Inventory Turnover Analysis - Selection Criteria window, select the relevant data and choose OK.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Turnover Analysis Report Fields
Item Group
Item group of the item.
Item
The description of the item.
UoM
Unit of measure of the item as defined in the Item Master Data Purchasing Data Packaging UoM Name .
Opening Inventory
Opening balance before the From date.
Closing Inventory
This value is calculated by using the following formula:
Sum of (Received Qty - Issued Qty) in the selected period range.
Period Goods Issue Qty
Issued quantity within the selected period range.
Days of Inventory Taking
This value is calculated by using the following formula:
This is custom documentation. For more information, please visit SAP Help Portal. 197

6/8/26, 6:12 AM
[(Opening Inventory + Closing Inventory) / 2 / Issued Qty] * [(1 + Days in the Period)]
**Days in the Period is the number of days between the From and To dates.
Inventory Turnover
This value is calculated by using the following formula:
Period Goods Issue Qty / ([Opening Inventory + Closing Inventory]/2).
Min.
The minimum Inventory Level defined in the Item Master Data Inventory Data tab.
 Note
An asterisk * sign is displayed to the left of the Min. value if the minimum inventory level is set on company level and not per
warehouse in the Item Master Data.
Lead Time
The Lead Time defined in the Item Master Data Planning Data tab.
Next Reorder Point
Calculates in how many days the item may need to be reordered.
This value is calculated by using the following formula:
[(OnHand Qty - Min Inventory) / Issued Qty] * [(1 + Days in the Period) - Lead Time].
 Note
An asterisk * sign is displayed to the left of this value if the minimum inventory level is set on company level and not per
warehouse in the Item Master Data Inventory Data tab.
Last Receipt Date
Last date of purchase order or production order of the item.
Production Reports
Use the reports listed under this menu entry to:
Generate the list of the bills of material
View open production orders
Related Information
Bill of Materials Report
Open Items List
Bill of Materials Report
This report provides the detailed list of all the bills of material that you have created.
Use this window to specify selection criteria for creating and displaying the list of bills of material.
This is custom documentation. For more information, please visit SAP Help Portal. 198

6/8/26, 6:12 AM
To open the window, choose Production Production Reports Bill of Materials Report .
After defining the report, you can view it in the Bill of Materials Report window (see Bill of Materials Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Properties
Opens the Properties window. Specify the item properties as selection criteria.
BOM Type
Choose the Bill of Materials type as a selection criterion.
To specify all types, choose All.
Bill of Materials Report Window
This window displays the bill of materials report according to the defined selection criteria (`see Bill of Materials Report).
Bill of Materials Report
UoM
The unit of measure of the BoM item and its components, as defined in Inventory Item Master Data Inventory Data tab.
Quantity
Displays the quantity of parent items and their components.
Whse
Displays the warehouse from which the components are issued to produce or to sell the finished product. To display Warehouses
(Default) – Setup, click .
Price
Displays the purchase price of the components or the standard or moving average price when working in perpetual inventory
system.
Depth
Displays the level in the bill of materials. The finished product of the bill of materials is at level 1.
BOM Type
Displays the type of the bill of materials.
Route Sequence
Displays the route sequence copied from the Bill of Materials (BOM) screen. The field is only visible when routing is applied to the
BOM.
Route Stage
This is custom documentation. For more information, please visit SAP Help Portal. 199

6/8/26, 6:12 AM
Displays the route stage copied from the Bill of Materials (BOM) screen. The field is only visible when routing is applied to the
BOM.
This is custom documentation. For more information, please visit SAP Help Portal. 200

6/8/26, 6:12 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:12:57 GMT+0000
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

6/8/26, 6:12 AM
Electronic Document Monitor
 Note
This report is available only if you have enabled the electronic documents feature. For more information, see Working with
Electronic Documents.
Use the Electronic Document Monitor to view the status of electronic documents that are created automatically. You can also
generate, send, import and export electronic documents through the Electronic Document Monitor.
More Information
Electronic Document Monitor Window
Electronic Document Monitor Window
Use this window to view or change the status of the electronic documents created.
To access this window, from the Main Menu, choose Reports Electronic Document Monitor .
Electronic Document Monitor Fields, General Area
View Type
Select one of the following options:
All - Displays all relevant documents.
Documents - Displays all marketing documents.
Documents - A/R - Displays A/R documents only.
Documents in Process - Displays documents that do not have the Sent status.
Failed Documents - Displays documents with error during processing.
Passed Documents - Displays documents that have the Sent status.
Date From... To
Specify the date range. The electronic documents monitor displays the documents that were created within the specified dates.
Generate
Generates the electronic document and sends it to the recipient through the SAP Business One Integration solution.
Highlight the document for which you want to generate and send the electronic file, and choose this button.
Export
If you want to save an XML file of a document on your computer, highlight the document, choose this button and save it to the
desired location.
Import
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:12 AM
Choose this button to select and then import an electronic document. Electonic documents must be in the correct format for
imports to work properly. Access the imported documents through the Electronic Document Monitor table, you can then make
amendments to the documents before adding them to the system.
Electronic Document Monitor Fields, Table
Type
Displays the type of the document.
Status
Displays the status of the document:
New - The document has just been created and has not yet been processed by the SAP Business One Integration solution.
Pending - The document has been created with the generation type Generate Later. To generate and send the electronic
file, choose the Generate button.
Sent - The document has been sent to the recipient through the SAP Business One Integration solution.
Doc. Number
Displays the number of the document. Click to access the document.
Date, Time
These fields display the date and time when the electronic document was added into the SAP Business One Integration solution.
Message
Displays the message related to the document, for example, an error message.
Banking Reports
Use the reports under this menu entry to analyze and generate overviews of:
Checks for payment issued to vendors and other entities
Drafts created for banking related documents
External reconciliations related data (only if the checkbox Install Bank Statement Processing on the Basic Initialization
tab of the Company Details window is selected).
Check Register Report
This report gives an overview of the checks for payment created in SAP Business One. According to the selection criteria you
define, the report lists checks for payment, grouped by the originating accounts, and provides information such as whether a
check was printed, its amount, the confirmation status, and more.
Check Register Report - Selection Criteria
Use this window to specify selection criteria for the Check Register Report.
To open the window, choose Banking Banking Reports Check Register Report .
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:12 AM
After defining the report, you can view it in the Check Register Report Window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Due Date From...To...
Specify a date range to display only checks with dates within the range.
Check No. From...To...
Specify a check number range to display only checks with numbers within the range.
 Note
Only relevant for printed checks.
Vendor Code From...To...
Specify a range of vendors to display only checks issued for these vendors.
Payment No. From...To...
Specify a range of Outgoing Payment numbers to display checks generated through these documents.
Checking Acct From...To...
Specify a range of house bank accounts to display in the report only checks issued by these accounts.
Display
Specify one of the following:
Voided checks only
Exclude voided checks
Printed checks only
Unprinted checks only
All checks
Display Results as List
When selected, a list of checks is displayed. When deselected, the checks are displayed grouped by credited bank account (the
account number appearing on the printed check).
Check Register Report Window
This window displays the Check Register Report according to the defined selection criteria.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:12 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Check Register Report Window
Account
Displays the house bank account issued the checks. Click the icon to display all the checks issued by that account.
Check No.
Displays the check number for printed checks. If the check is not printed yet this field displays 0 (=zero).
G/L Acct/BP Code, G/L Acct/BP Name
Displays the code and name of the vendor or account for which the check was created.
Internal ID
Displays the internal alphanumeric key of the Checks for Payment document linked to the check.
Pmt No.
Displays the number of the Outgoing Payment document through which the check was created, and provides a link to it. If the
check was not created by an Outgoing Payment document this field displays 0 (=zero)
Payment Amt.
Displays the amount paid by the check.
Trans. No
Displays the number of the journal entry that reflects the check and provides a link to the journal entry window.
Status
Displays the current status of the check. The possible statuses are:
Confirmed – the check has been printed and confirmed.
Unconfirmed – the check has been printed but the number is not yet confirmed.
Void – the check has been voided in the Void Checks for Payment window.
Reissued – the check has been voided and then reissued.
Not Printed – the check has not been printed.
Overflow – the check information has overflowed the preprinted check paper in the printer, and has been printed on the
next check.
Printed
Indicates whether the check was printed or not.
Printed By
Displays the name of the user who printed the check.
Remarks
Displays remarks related to the check.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:12 AM
Payment Drafts Report
Use this function to display and process drafts of incoming and outgoing payment documents.
To create the report, choose Banking Banking Reports Payment Drafts Report .
Deleting Drafts
Context
Follow this procedure to delete incoming and outgoing payments that were saved as drafts.
Procedure
1. Choose Banking Incoming Payments or Outgoing Payments Payment Drafts Report .
2. Specify the required parameters to display the drafts you want to delete.
3. Right-click the draft to be deleted and choose Remove.
 Note
You can only delete one draft at a time in the SAP Business One client.
To remove multiple drafts at the same time, please use SAP Business One, Web client. For more information, see the
topic Managing Drafts in the User Guide for the Web client.
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
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:12 AM
2. Double-click the required draft.
The document window appears in the Add mode.
3. Make any necessary changes and choose Add.
 Note
Since the number assigned to the regular document created from a draft is the one that currently appears in a new
document, it might be different than the one originally assigned to the draft.
Results
The status of the draft is Closed.
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
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:12 AM
Payment Drafts Report Window
This window displays the Payment Drafts Report.
To open the window, choose Banking Banking Reports Payment Drafts Report .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Payment Drafts Report Window
User
To display drafts created by a particular user, specify this user. Super users can view drafts created by all users, while regular users
can view only those drafts that they have created.
 Note
Regular users, if given the following two authorizations, can view incoming or outgoing payment drafts created by other users
respectively. To define the authorizations View Incoming Payment Drafts Created by Other Users and View Outgoing
Payment Drafts Created by Other Users, go to Administration System Initialization Authorizations General
Authorizations Banking Outgoing Payments Payment Drafts Report .
Open Only
Displays only the drafts that were not added as regular payment documents.
Incoming Payments
Displays drafts created for incoming payments.
Outgoing Payments
Displays drafts created for outgoing payments.
Document
Type of document: incoming or outgoing payment.
Posting Date
Posting date of the payment document.
Document Total
Total payment amount.
Document Remarks
Remarks specified in the Remarks fields of the payment document.
Closed
Indicates whether or not the status of the draft is closed. After the draft is added and becomes a regular document, its status
changes to closed.
Service Reports
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:12 AM
You can use service reports to do the following:
Extract important information about the efficiency and performance of your service department.
Obtain details about customer service contracts and equipment.
View your own service calls in order to assess your progress and take any necessary actions.
Service Calls Report
This report provides information on open and closed service calls and enables you to analyze all the information regarding the
management of service calls in your company.
Use this window to specify selection criteria for the Service Calls report.
To open the window, choose Service Service Reports Service Calls . Alternatively, open it from the Reports module.
After defining the report, you can view it in the Service Calls Report window (see Service Calls Report Window). You can view
summaries of the information about service calls for each employee.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Service Calls Report Window
This window displays the Service Calls report according to the defined selection criteria (see Service Calls Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Calls Report Fields
X Axis
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:12 AM
Select the time unit for displaying the service calls in the graph. The time frame of the x axis depends on the selection criteria.
Y Axis
Total number of service calls within the given selection
Print Graph
Includes the graph when you print the report
To display or remove additional report fields, choose in the toolbar.
Service Calls by Queue Report
This report provides you with information about service calls in each service queue and enables you to check all the service calls
waiting in a queue.
Use this window to specify selection criteria for the Service Calls by Queue report.
 Recommendation
If you use service queues, we recommend that your employees use this report when handling the messages that are displayed
in their queue.
To open the window, choose Service Service Reports Service Calls by Queue . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Service Calls by Queue Report window (see Service Calls by Queue Report
Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Service Calls by Queue Report Window
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:12 AM
This window displays the Service Calls by Queue report according to the defined selection criteria (see Service Calls by Queue
Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Calls by Queue Report Fields
Assign Date
Date on which the service call was assigned to a particular queue
Assign Time
Time at which the service call was assigned to a particular queue
Show Graph
Opens the Service Calls by Queue – Selection Criteria window and displays the data for the selected queue in a graph.
To open the Graph Settings window and change the settings for the graph, choose Settings in the Service Calls by Queue –
Selection Criteria window.
To display or remove additional report fields, choose in the toolbar.
Response Time by Assigned to Report
This report lets you analyze the response time of employees that are assigned to specific service calls. If a service call is in a
queue, you get information about the amount of time the service call was in the queue before an assignee responded to it.
Use this window to specify selection criteria for the Response Time by Assigned to Report.
 Recommendation
If you assign employees to service calls, we recommend that your employees use this report when handling the messages that
are displayed under their name.
To open the window, choose Service Service Reports Response Time by Assigned to Report . Alternatively, open it from
the Reports module.
After defining the report, you can view it in the Response Time by Assigned to Report Window (For more information, see
Response Time by Assigned to Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:12 AM
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Response Time by Assigned to Report Window
This window displays the Response Time by Assigned to report according to the defined selection criteria (see Response Time by
Assigned to Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Response Time by Assigned to Report Fields
Response Time
Amount of time it took to respond to the service call
Time in queue
Amount of time the service call waited in the queue
To display or remove additional report fields, choose in the toolbar.
Average Closure Time Report
This report provides details about the average amount of time required to close service calls. Use this report to check the
efficiency of the service department.
You can display service calls with the same closure date. You can also select service calls completed by a specific employee.
To access the window, choose Service Service Reports Average Closure Time . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Average Closure Time Report window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:12 AM
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Average Closure Time Report Window
This window displays the Average Closure Time report according to the defined selection criteria (see Average Closure Time
Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Average Closure Time Report Fields
Closure Time
Time at which the service call was closed
Time for Closure
Amount of time required to close the service call
X Axis
Select the time unit for displaying the service calls in the graph. The time frame of the x axis depends on the selection criteria.
Y Axis
Total number of service calls closed within the given selection
Print Graph
Includes the graph when you print the report
To display or remove additional report fields, choose on the toolbar.
Service Contracts Report
This report provides concise information about the service contracts of your company’s customers.
You can:
Create the report for different contract types and statuses.
View service contracts of specific customers.
To access the report, choose Service Service Reports Service Contracts . Alternatively, open it from the Reports module.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:12 AM
After defining the report, you can view it in the Service Contracts Report window (see Service Contracts Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
End Date From ... To...
Specify the range of dates on which the service contracts expire.
Termination Date From... To...
Specify the range of dates on which the service for certain or all items expires.
Contract Renewals Only
Displays only service contracts that can be renewed.
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Service Contracts Report Window
This window displays the Service Contracts report according to the defined selection criteria (see Service Contracts Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Contracts Report Fields
Renewal
Displays whether the contract can be renewed.
Reminder
Displays how many days or hours prior to the renewal of the service contract you get the reminder.
To display or remove additional report fields, choose in the toolbar.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:12 AM
Equipment Card Report
This report provides information about the specific items purchased by or assigned to each business partner.
Use this window to specify selection criteria for the Equipment Card report.
To open the window, choose Service Service Reports Equipment Card Report . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Equipment Card Report window.
Equipment Card Report Window
This window displays the Equipment Card report according to the defined selection criteria (see Equipment Card Report).
You can view information such as serial number, business partner, status of the equipment card, and contact person according to
the defined selection criteria.
My Service Calls
Use this report to view and analyze the service calls assigned to you. The report displays open, closed, and overdue service calls.
You can evaluate the priority of service calls and take any necessary action. You can also analyze your efficiency and performance.
To open the report window, choose Service Service Reports My Service Calls . Alternatively, open it from the Reports
module.
To display or remove additional fields in the report, choose in the toolbar.
My Open Service Calls
Use this report to view and analyze the open service calls for which you are responsible. You can check each service call, view its
progress, and take any necessary action.
To open the window, choose Service Service Reports My Open Service Calls . Alternatively, open it from the Reports
module.
To display or remove additional report fields, choose in the toolbar.
My Overdue Service Calls
Use this report to view and analyze service calls that have passed their due date. You can check single service calls, evaluate their
progress, and take the necessary action to solve the problem as quickly as possible. You can also analyze your efficiency and
performance.
To open the window, choose Service Service Reports My Overdue Service Calls . Alternatively, open it from the Reports
module.
To display or remove additional report fields, choose in the toolbar.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:12 AM
Human Resources Reports
Use these reports to retrieve data according to your specified selection criteria. You can:
View employee absences for the entire organization or a particular department.
Display contact details for every company employee.
Print phone books, or employee lists in various combinations.
To create a report, choose Human Resources Human Resources Reports .
Activities
Generating Reports
Employee List - Selection Criteria
Use this window to specify selection criteria for the Employee List Report.
To open the window, choose Human Resources Human Resources Reports Employee List .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Role
Specify the employees roles to include in the report.
More Information
Employee Master Data
Employee List Report
This window displays general information about employees from the different branches and departments in the company,
according to your selection criteria.
Absence Report - Selection Criteria
Use this window to specify selection criteria for the Employee Absence Report.
To open the window, choose Human Resources Human Resources Reports Absence Report .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:12 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Start Date, End Date
Specify the date range for employee absences to include in the report.
More Information
Absence Information Window
Employees Absence Report
This report displays information (sick days, vacation days, and so on) about an employee's absences, according to your selection
criteria.
Phone Book - Selection Criteria
Use this window to specify selection criteria for the company Phone Book.
To open the window, choose Human Resources Human Resources Reports Phone Book .
Phone Book
This window displays contact information for company employees, according to your selection criteria.
Audit Trail Report
This report provides a central place for you to view the changes made to master data and transactions. You can maintain the
settings for the history / log on the Services tab of the General Settings window. To view the changes made for a certain object or
document, use the Change Log window.
Use this window to specify selection criteria for the report. When you are printing or previewing the Audit Trail report, the detailed
selection criteria can also be printed or previewed.
To open the window, choose Reports Audit Trail Report .
After defining the report, you can view it in the Audit Trail Report window.
Selection Criteria
Dates: Creation Date, Update Date
Specify the date ranges of the audit trail that you want to view.
Updated By - User Selection
Specify the users who have changed the objects or documents.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:12 AM
Branch Selection
This field is only available when you have enabled the multiple branch functionality. Specify the branches of the audit trail that you
want to view.
Objects
Specify the tax-related objects for which you want to view the audit trail.
Documents
On the following tabs, select the documents for which you want to view the audit trail.
Marketing Documents
Banking Documents
Inventory Documents
Financials Documents
Fixed Asset Transactions
 Note
The transactions only appear when you enable the fixed assets function.
Settings and Definitions
Master Data
Others
Related Information
General Settings: Services Tab
Change Log Window
Differences Window
Audit Trail Report Window
This window displays the Audit Trail report according to the defined selection criteria. The changes related to the header
information of the master data and transactions are displayed in black, whereas the ones related to the tab information are
displayed in other colors, in the form of one color per tab.
After importing your own Crystal Reports layouts in the Report and Layout Manager window and setting a default one in the
Layout and Sequence window, you can print the report using the default layout. In the Report and Layout Manager window, there
is no corresponding entry on the List tab.
 Note
To import your own Crystal Reports layouts, in the Report and Layout Manager window, choose Import. In the report and
layout import wizard, select Layout as the content type, and Audit Trail Report as the document type.
Audit Trail Report Fields
Group By
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:12 AM
You can group the report by Updated On/At, Updated By - User Code, or Object Type.
Updated On/At
The date and specific time when an object or document was changed.
Updated By - User Code, User Name
The code and name of the user who changed the object or document.
Object Type, Object Code
The type and unique code of the object or document that was changed.
Instance
The sequential number of the change made. 1 is assigned to the first change, 2 is assigned to the second change, and so on.
Created On/At
The date and specific time when an object or document was created.
Created By - User Code, User Name
The code and name of the user who created the object or document.
Updated Field
The field that was changed.
Previous Value
Value of the field before the change.
New Value
Value of the field after the change.
Working with the Crystal Reports Software
Using SAP Crystal Reports, version for the SAP Business One application, you can create reports and layouts that are fully aligned
with the interface elements of SAP Business One and SAP Business One add-ons.
 Note
Only SAP channel partners, SAP Business One superusers, and SAP Business One authorized regular users can access the
Crystal Reports software.
More Information
For more information about working with the Crystal Reports software, see the following:
The how-to guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal
The SAP Crystal Reports online help, which you can access from the SAP Crystal Reports software
Report and Layout Manager
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:12 AM
The report and layout manager serves as a central workplace for administrators to manage reports, layouts, and printing
sequences of related marketing documents and production orders. You can perform the following tasks with this tool:
Edit reports and layouts
Change the details of user-defined reports and layouts
Set default layouts for document types and printing sequences
Delete user-defined reports and layouts
Create and maintain printing sequences of related marketing documents
Run reports
Import Crystal reports and Crystal Reports layouts
Export Crystal reports to a local disk or a Crystal Server
For more information, see the guide How to Integrate SAP Crystal Server with SAP Business One at SAP Help Portal.
Export Crystal Reports layouts to a local disk
Manage data sources for user-defined Crystal reports and Crystal Reports layouts
Set user authorizations for user-defined Crystal reports
More Information
Running a Report Created with the Crystal Reports Software
Previewing a Document in a Crystal Reports Layout
SAP Crystal Reports Viewer
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Report and Layout Manager Window
Use this window to manage all your reports and layouts. To access the window, from the SAP Business One Main Menu, choose
Administration Setup General Report and Layout Manager .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
List Tab
Lists the reports and document types in all SAP Business One modules. By clicking any document type, you display all its layouts
in the right pane of window. The layouts may include both PLD layouts and Crystal Reports layouts.
In addition to all the modules in the SAP Business One Main Menu, the following two folders are listed:
Lost Reports: Stores user-defined Crystal reports that have not been assigned to any specific folder. You cannot find these
reports in the SAP Business One Main Menu until you assign them to a module.
Add-On Layouts: Stores Crystal Reports layouts that are created for add-ons.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:12 AM
You can also find the add-on layouts in the corresponding module. For example, the Crystal Reports layouts of the fixed
assets history sheet are located in the following folders:
Add-On Layouts Fixed Assets
Financials Fixed Assets Fixed Asset Reports Asset History Sheet
Search Tab
You can search for reports and layouts by keyword.
To search for a report, select the Report radio button and search by the report name.
To search for a layout, select the Document Type radio button and search by one of the following:
Document type code
Document type name
Layout ID
Layout name
Asterisk Indicates
Select the Report checkbox to display an asterisk (*) beside each folder that contains Crystal reports.
Select the Layout checkbox to display an asterisk (*) beside each folder or document type that contains layouts. The layouts can
be either PLD layouts or Crystal Reports layouts.
Export
Choose this pushbutton to access the report and layout export wizard. You can conduct the following exports:
Export user-defined Crystal reports and Crystal Reports layouts to a local disk
Export system and user-defined Crystal reports to a Crystal Server that is integrated with SAP Business One
For more information, see the topic Report and Layout Export Wizard.
Import
Choose this pushbutton to access the report and layout import wizard. You can import the following files:
An rpt file
A b1p package file that contains either Crystal reports or Crystal Reports layouts
 Note
As of SAP Business One release 8.82, reports and layouts are exported into b1px packages instead of a b1p package.
A b1px package file that may contain both Crystal reports and Crystal Reports layouts
For more information, see the topic Report and Layout Import Wizard.
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Report and Layout Manager: Layouts Tab
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:12 AM
This tab is available when you click a document type in the left pane of the report and layout manager. It displays all layouts
assigned to the document type. Clicking a layout lets you view its details. For user-defined layouts, you can also edit the following
fields:
Name
Author
Status
Description
Printer
 Note
When SAP Business One cannot find the printer defined for a layout, and you are trying to print documents with this
layout, instead of printing the documents using the system default printer directly, the Printer Mapping Configuration
window appears for you to map the defined printer to any printer in the operating system. You can use the mapped
printer to print documents throughout your current login. For more information, see SAP Note 3235582 .
1st Page Printer
No. of Copies
Language
(PLD) Use Foreign Currency
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Layout Details
Layout Type
Indicates the type of the layout. The layout type is determined by the tool that is used to design the layout. The tools include the
following:
PLD (Print Layout Designer)
Crystal Reports
Status
For user-defined layouts, this field is editable.
For system layouts, this field is editable for superusers only.
 Note
If a layout is set as default for a user or business partner, the status of the layout cannot be changed to Inactive.
If the status of a layout is inactive, it is not displayed in the Layout and Sequence window. In addition, an inactive layout
is not available for selection when you preview or print a document or report. For more information, see Layout
Designer.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:12 AM
Language
Indicates the language of the UI elements of the layout.
This field is only informational. You can change the value of this field for a user-defined layout, but it does not change the display
language of the layout.
Functional Buttons
Set as Default
Choose this button to set the selected layout as default for the document type.
Advanced
Available for user-defined Crystal Reports layouts.
Choose this pushbutton to define the data source connections of the layout. For more information, see the topic Report and
Layout Manager: Advanced Settings.
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Related Information
Report and Layout Manager: Advanced Settings
Report and Layout Manager: Printing Seqs Tab
This tab is available when you click a marketing document type in the left pane of the report and layout manager. On this tab, you
can define a succession of related documents to print when you print the particular document type. For example, when you print a
service A/R invoice, you can also print its base quotation, base order, and two copies of its base delivery. You can also define a
layout for printing sequences as the default printing option.
More Information
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Report and Layout Manager: Report Details
The details of a Crystal report are displayed when you click the report in the left panel of the report and layout manager.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Status
Editable for user-defined Crystal reports.
If the status of a report is inactive, you cannot find it in the SAP Business One Main Menu.
Menu Location
Editable for user-defined Crystal reports.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:12 AM
Indicates the location of the report in the SAP Business One Main Menu. The asterisk (*) signifies that the folder contains Crystal
reports. For more information, see the topic Report and Layout Manager Window.
URL Reporting
Available if you have exported a report to a Crystal Server. You can run the report by clicking the hyperlink Show Report in Web
Browser.
Visible For Mobile
Select this checkbox to make the Crystal report visible within the mobile application for SAP Business One.
Set Authorization
Available for user-defined Crystal reports.
Choose this pushbutton to define authorizations for SAP Business One regular users in the Authorizations window.
You Can Also Buttons
Delete
Available for user-defined Crystal reports.
Define Advanced Settings
Available for user-defined Crystal reports.
Choose this pushbutton to define the data source connections of the report. For more information, see the topic Report and
Layout Manager: Advanced Settings.
Export to Crystal Server
Available if you have integrated at least one Crystal Server with SAP Business One. Choose this pushbutton to export the report to
the default Crystal Server with one click.
For more information, see the guide How to Integrate SAP Crystal Server with SAP Business One at SAP Help Portal.
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Related Information
Report and Layout Manager Window
Report and Layout Manager: Advanced Settings
Report and Layout Manager: Advanced Settings
Use this window to define data source connections for user-defined Crystal reports and Crystal Reports layouts. Note that you can
neither remove nor add a connection; the available data sources and the number of connections are established when designing
the report.
Data Source Tab Fields
Report
Indicates the main report and the names of subreports.
Reference Server, Reference Database
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:12 AM
Indicates the server and database that is used when designing the report or layout.
Server
The servers available for selection are those registered in your SLD (System Landscape Directory) service. For more information,
see the Administrator's Guide provided with SAP Business One.
The default server is the reference server.
Database
Available databases depend on the server that you have selected; you can select the database only after you have specified the
server.
The default database is the reference database.
More Information
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Report and Layout Export Wizard
The report and layout export wizard enables you to export Crystal reports and Crystal Reports layouts. The exportable files vary
depending on your export target location.
Target Location Exportable Files Comments
Local disk Reports and layouts can be exported
User-defined Crystal reports
together into a package.
User-defined Crystal Reports
layouts
Crystal Server In the course of export, you can define
System Crystal reports
which Crystal Server users have
authorization to the exported reports.
User-defined Crystal reports
If you want to export Crystal reports to a Crystal Server, you first need to integrate your Crystal Server with SAP Business One. For
more information, see the guide How to Integrate SAP Crystal Server with SAP Business One on SAP Help Portal.
More Information
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One on SAP Help Portal.
Report and Layout Import Wizard
The report and layout import wizard enables you to import user-defined Crystal reports and Crystal Reports layouts into SAP
Business One. In the course of import, you can perform the following:
Change the data sources of multi-database reports and layouts
Apply master layouts to appropriate document types
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:12 AM
Define authorizations for reports
If you have translated a Crystal report, all its language versions are imported along with the report.
More Information
For more information, see the guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
SAP Crystal Reports Viewer
 Note
You do not need to install the SAP Crystal Reports viewer in a separate procedure. It is an integral part of the SAP Business One
core product.
In the SAP Crystal Reports viewer in SAP Business One, you can view the following:
Crystal reports
Crystal Reports document layouts
The SAP Crystal Reports viewer provides the following functions for both reports and layouts:
Exporting documents and reports
Navigating to different pages
Searching for text
Changing the zooming factor
You can perform the following functions on reports only:
Filtering data by changing the parameters
Navigating to different groups of data
 Note
If the SAP Crystal Reports viewer does not support the chosen SAP Business One display language, the English language is
displayed. The SAP Crystal Reports viewer supports the following languages:
Portuguese (Brazil)
Chinese (Simplified)
Chinese (Traditional)
German
Dutch
English
French
Italian
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:12 AM
Japanese
Korean
Spanish
Swedish
Filtering Report Data by Changing Parameters
 Note
The Parameter panel is available only for reports that require users to enter parameters.
In the parameter panel of the SAP Crystal Reports viewer, you can change the report parameters to filter the data to be displayed
in the report. You change different types of parameters in different fields, for example, dropdown boxes, date or time pickers, and
advanced dialog boxes.
If a parameter is not mandatory, you can delete it from the parameter panel by selecting it and then clicking the Delete icon at the
top of the panel.
 Example
Changing Parameters in an Advanced Dialog Box
1. To display the parameter panel, in the toolbar of the parameter panel, click the icon.
2. In the parameter panel, click in the field of a parameter.
An icon appears beside the field.
3. Click the icon mentioned in Step 2.
4. In the Enter Parameter Values dialog box that appears, specify a parameter or parameter range.
5. Choose the OK pushbutton.
6. Click the Apply icon at the top of the parameter panel.
Exporting Documents and Reports
You can export a document or report via the SAP Crystal Reports viewer to your computer in one of the following file formats:
Crystal Reports (*.rpt)
PDF (*.pdf)
Character Separated Values (CSV) (*.csv)
Microsoft Excel (97-2003) (.xls)
Microsoft Excel [97-2003] Data-Only (.xls)
Microsoft Excel Workbook data-Only (*.xlsx)
Microsoft Word (97-2003) (.doc)
Microsoft Word (97-2003) - Editable (.rtf)
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:12 AM
Rich Text Format (RTF) (*.rtf)
XML (*.xml)
To export a document or report, proceed as follows:
1. In the toolbar of the SAP Crystal Reports viewer, click the icon.
2. In the Export Report window, navigate to the folder on your computer where you want to save the file.
3. In the File name field, enter a name for the file you are exporting.
4. From the Save as type dropdown list, select a file type.
5. Choose the Save button.
Navigating to Different Groups
Data in a report may be grouped according to the design. The SAP Crystal Reports viewer provides a group tree for you to find your
data more easily in a report.
To navigate to different groups, proceed as follows:
1. In the toolbar, click the icon.
2. In the group tree panel on the left, select a group.
A red box appears in the report to highlight the relevant data in the report.
Navigating to Different Pages
Depending on your data volume or parameters defined, a report or document may have more than one page. To navigate to
different pages, do either of the following:
In the toolbar of the SAP Crystal Reports viewer, click any of the following icons:
In the toolbar, in the page number field, enter a page number and press Enter .
Searching for Text
To search for text in the document or report:
1. In the toolbar, click .
2. In the Find Text dialog box, in the Find What field, enter the text you want to find.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:12 AM
3. Choose the Find Next button. To find multiple instances of the text, choose the Find Next button as many times as you
require.
Changing the Zooming Factor
To change the zooming factor in a document or report, in the toolbar, click and select an option from the displayed list.
To define a zooming factor that does not appear in the list, proceed as follows:
1. From the Zoom list, select Customize. The Zooming dialog box appears.
2. In the field, enter a value from 25 to 400.
3. Choose the OK pushbutton.
More Information
For more information, see the how-to guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Running a Crystal Report
Procedure
To run a Crystal report in SAP Business One, do one of the following:
Run the report from the SAP Business One Main Menu:
1. From the SAP Business One Main Menu, locate the report that you want to run and select it.
2. If the report contains multiple data source connections that are not all covered in the license server or the license
file, the Log On to Data Source window opens. Specify the user code and password for each data source and
choose the OK button.
3. In the Report Selection Criteria window, enter required information.
4. Choose the OK push button.
Run the report from the Report and Layout Manager window:
 Note
Only superusers and authorized regular users can perform the procedure below.
1. From the SAP Business One Main Menu, choose Administration Setup General Report and Layout Manager
.
2. In the Report and Layout Manager window, in the navigation pane on the left, navigate to the report you want to run
and select it.
 Note
If a report has not been assigned to a specific folder, it is in the Lost Reports folder and is not displayed in the
SAP Business One Main Menu.
3. In the work area on the right, choose the Run Report button.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:12 AM
4. If the report contains multiple data source connections that are not all covered in the license server or the license
file, the Log On to Data Source window opens. Specify the user code and password for each data source and
choose the OK button.
5. In the Report Selection Criteria window, enter the required information.
6. Choose the OK pushbutton.
The report appears in the SAP Crystal Reports viewer. For more information, see SAP Crystal Reports Viewer.
More Information
Previewing a Document in a Crystal Reports Layout
For more information, see the how-to guide How to Work with SAP Crystal Reports in SAP Business One at SAP Help Portal.
Previewing a Document in a Crystal Reports Layout
Procedure
1. Open a document that you want to view with a Crystal Reports layout.
 Note
You can only preview a document that is already added to the database. In other words, you cannot preview a document
without data.
2. Choose one of the following menu paths:
File Preview
Choose this option if the Crystal Reports layout you want to view is already defined as the default layout of the
document type.
File Preview Layouts
Select a layout in the Choose Layout window and choose the OK pushbutton.
The document is displayed in the SAP Crystal Reports viewer. For more information, see SAP Crystal Reports Viewer.
More Information
Running a Crystal Report
This is custom documentation. For more information, please visit SAP Help Portal. 30