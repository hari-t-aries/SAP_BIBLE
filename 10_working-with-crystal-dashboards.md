6/8/26, 6:07 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:07:28 GMT+0000
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

6/8/26, 6:07 AM
Working with Crystal Dashboards
Dashboards are an element of the cockpit, which present easy-to-understand visualizations, such as bar or pie charts, of
transactional data from the SAP Business One database. Depending on the dashboard, data can be presented either as time-
specific static snapshots or as refreshable visualizations.
SAP Business One delivers predefined Crystal dashboards for financials, sales, and service modules. In addition, SAP Business
One partners and customers can create their own dashboards.
In the interactive graphics below, you can hover over each area for short description and choose the highlighted areas for more
information.
Key Users
Please note that image maps are not interactive in PDF outputs.
Individual Users
Please note that image maps are not interactive in PDF outputs.
As of the end of 2020, SAP no longer supports Adobe Flash-based dashboards, i.e., Crystal dashboards, embedded within SAP
Business One. For more information, see SAP Note 3014120 .
For information about installing the integration component, see Administrator’s Guide for SAP Business One at SAP Help Portal.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:07 AM
For more information about working with pervasive dashboards, see the How to Work with Pervasive Analytics guide at SAP Help
Portal.
More Information
Working with the Cockpit
Viewing Dashboards in SAP Business One
Prerequisites
Your system administrator or key user has done the following:
Installed the integration component for SAP Business One
Enabled the use of the cockpit and dashboards in SAP Business One
Assigned the correct user authorization for dashboards
Context
Depending on the dashboards that have been installed and the authorizations you have been granted, you can view SAP-defined
dashboards for financial, sales, and service areas. In addition, your company can deploy dashboards created specifically for your
company by SAP Business One partners or your internal IT staff.
Procedure
1. From the SAP Business One navigation panel on the left side of the window, under My Cockpit, select the cockpit you want
to use.
The cockpit appears
2. In the navigation panel, choose Widget Gallery General Widgets .
3. Click Dashboards and drag it into the open cockpit area.
A Dashboard window appears with a message about how to add a dashboard.
4. To add a dashboard to your cockpit, in the top right Dashboard widget window bar, choose .
5. From the dropdown list, select Settings.
A Select Dashboard window appears, listing in alphabetic order the active dashboards which you have permission to view.
For more information about activating a dashboard, see Activating or Deactivating a Dashboard. For more information
about assigning user authorizations for your dashboard, see Setting Up User Authorizations for a Dashboard.
 Note
If you do not have permission to view dashboards, if dashboards are not activated, or if no dashboards have been loaded
into your system, you get the following error message:
No dashboard available for you. Contact your system administrator.
6. To add one or more dashboards to the cockpit, select the appropriate checkbox.
7. If you select only one dashboard, that dashboard is the default dashboard. If you select two or more dashboards, to specify
the dashboard that you want to appear by default whenever you log on to the cockpit, highlight the dashboard line and
choose Set as Default. The default dashboard appears in bold font.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:07 AM
8. To confirm your choices, choose OK.
The default dashboard appears.
Related Information
Working with Crystal Dashboards
Monitoring Your Dashboards Using a Web Browser
Monitoring Your Dashboards Using a Web Browser
Prerequisites
Your system administrator or key user has done the following:
Installed the integration component for SAP Business One
For information about installing the integration component, see the Administrator’s Guide for SAP Business One.
Installed a Web browser and ensured the Web connection
Supported Web browsers include: Microsoft Internet Explorer (6–9), Google Chrome, and Mozilla Firefox.
Enabled the cockpit function in SAP Business One
For more information, see Enabling the Cockpit Function and the Dashboard Widget.
You are using the SAP Business One version for Microsoft SQL.
Context
You may want to monitor the business performance of your company without running the SAP Business One application. The SAP
Crystal Dashboard Web Portal lets you monitor your dashboards in a Web browser.
Procedure
1. For first-time use of the dashboard portal, from the SAP Business One Main Menu, choose Administration System
Initialization General Settings and select the Cockpit tab.
2. Select the Cockpit radio button, and choose the More... button.
The Cockpit Options window appears.
3. Select the Enable SAP Crystal Dashboards checkbox and click the SAP Crystal Dashboard Web Portal link.
The login page appears.
4. Specify the following fields:
Company: From the dropdown list, select one company database.
Language: From the dropdown list, select the language for the user interface. By default, the language is US English.
ID: Specify your user ID.
Password: Specify the password.
Remember Settings: Select this checkbox to let the browser remember all the above settings except your
password.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:07 AM
5. Choose the Login button.
6. Select a dashboard.
 Note
Make sure you have authorization to view the dashboard you select.
Related Information
Working with Crystal Dashboards
Importing a Dashboard Package
Procedure
SAP Business One partners and your own IT department can develop industry-specific and company-specific dashboards and
queries. To use these dashboard packages, you need to import them into SAP Business One.
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager
2. In the Dashboard Manager window, choose the Import button.
The Import Wizard window appears.
3. To import a package of dashboards and related queries, choose Next.
4. In Step 1 of the wizard, you select a dashboard package file in your file system. In the Open window, select the name of the
dashboard package file (with .zip extension) and choose Open.
The name of the file appears in the Dashboard Package field.
5. To continue, choose Next.
Information about the dashboard package appears. This information is stored in the info.xml file in the dashboard
package.
6. To continue to Step 2 of the import wizard, choose Next.
7. If the dashboard package contains queries, the Import queries in this package checkbox is selected by default. If the
dashboard package does not contain queries, you receive the message: There are no queries in this package.
If a query in this package is linked to more than one dashboard, you receive the message:
A query cannot be linked to more than one dashboard. Ensure that it is linked to one
dashboard only.
A table containing the query category, name, and status appears.
8. To import the dashboards and queries in the package, choose the Execute button.
Step 3 of the import wizard appears. You receive one of the following:
Confirmation that the dashboards and queries were imported successfully.
Notification that the import failed and the reason for the failure.
9. To end the wizard, choose the Close button. If the import was successful, you can now set up user authorizations for the
new dashboards in the package.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:07 AM
More Information
Working with Crystal Dashboards
Setting Up User Authorizations for a Dashboard
To assign user authorizations for a dashboard, proceed as follows:
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager
2. In the Dashboard Manager window, from the menu on the left side, open a dashboard package and select a dashboard.
You can view information about the dashboard you selected.
3. To set a user’s authorization for the selected dashboard, choose Define User Authorizations.
The Authorizations window in SAP Business One appears.
4. Select the user, locate the dashboard in the Dashboards folder in the permission tree, and assign an authorization for the
user: Full Authorization or No Authorization.
5. To save the change, choose the Update button.
Exporting a Dashboard Package
Procedure
To modify existing dashboards in SAP Business One or to use an existing dashboard to create a new dashboard, you can export a
dashboard package to your computer, modify one or more dashboards in the package or create new dashboards, and then import
the modified or new dashboard package to SAP Business One.
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager .
2. In the Dashboard Manager window, from the menu on the left side, select a dashboard package.
Information about the dashboard package you selected appears on the right side of the window.
3. To start the export of the dashboard package, choose the Export button.
The Export Package window appears.
4. Accept the default file location and file name or specify a different location and file name.
The file extension must be .zip.
5. To complete the export, choose the Save button.
SAP Business One confirms the export of the dashboard package to the specified location in your file system.
More Information
Working with Crystal Dashboards
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:07 AM
Deleting a Dashboard Package
Procedure
If a dashboard package is no longer relevant for your company, you can delete it. If a newly created or modified dashboard in a
dashboard package has errors that you need to correct, you must delete the dashboard package, correct the errors, and then
import the changed dashboard package.
 Note
You cannot delete an SAP-defined dashboard package.
You cannot delete a single dashboard; you must delete the dashboard package.
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager .
2. In the Dashboard Manager window, from the menu on the left side, select a dashboard package.
Information about the dashboard package you selected appears on the right side of the window.
3. To start the deletion of the dashboard package, choose the Delete button.
A message appears asking you to confirm that you want to delete the package.
4. Do one of the following:
To confirm the deletion, choose Yes.
You receive a confirmation that the deletion was successful.
To cancel the deletion and return to the Dashboard Manager window, choose No.
 Note
If you have chosen a dashboard from the deleted dashboard package as your default dashboard, you receive the following
message when trying to add the dashboard to the cockpit:
The default dashboard is not available. Contact your system administrator.This message also
appears if your permission for the dashboard package is revoked or if the dashboard is set as Inactive.
More Information
Working with Crystal Dashboards
Activating or Deactivating a Dashboard
Procedure
A dashboard package contains one or more dashboards and queries. If you want to let users view some, but not all, the dashboards
in a package, you can activate or deactivate individual dashboards as required, either those developed by SAP or ones developed
by a partner or your IT staff. You can achieve the same result by adding or removing each user’s authorization for each dashboard,
but activating or deactivating is faster and easier.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:07 AM
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager .
2. In the Dashboard Manager window, from the menu on the left side, select a dashboard package.
Information about the dashboard package you selected appears on the right side of the window.
3. To activate or deactivate the selected dashboard, from the Status dropdown list, select the appropriate status, either
Active or Inactive.
4. To save the change, choose the Update button.
More Information
Working with Crystal Dashboards
Scheduling a Daily Data Refresh for Dashboards
Procedure
Each time a user opens a dashboard, SAP Business One loads and displays the latest data in real time. For data-intensive
dashboards, such as Sales Analysis, this can impact system performance. As your database grows or the number of employees
who use dashboards increases, you may also notice a decrease in the performance of dashboards. During peak usage time, when
users navigate from one dashboard to another and thus cause the dashboard to reload real-time data, they may report delays of
several minutes or more. To minimize the impact on system performance during peak business hours, the system administrator
can choose to change the data reload from real time to a scheduled data reload. In addition to the automatic data refresh settings
you make here, a user can also refresh data in real time while viewing a dashboard by choosing the Refresh Data button in the
dashboard. However, this user-triggered data refresh is not available for the Service Call Status dashboard and the Cash Flow
dashboard.
 Note
After you enable the data cache and the scheduled daily data refresh, the settings here apply to all dashboards which support
scheduled refresh, including the SAP-defined dashboards and the imported ones.
For SAP-defined dashboards, the settings would impact only the Sales Analysis dashboard. The Service Call Status dashboard
and the Cash Flow dashboard, for which data is always refreshed every 60 minutes, would not be affected.
To enable and schedule a daily data refresh for a dashboard, proceed as follows:
1. From the SAP Business One navigation panel on the left side of the window, choose Modules Administration Setup
General Dashboard Manager .
2. In the Dashboard Manager window, from the menu on the left side, select a dashboard package.
Information about the dashboard package you selected appears on the right side of the window.
3. To enable the scheduled data refresh function for dashboards, choose the Data Refresh Settings button.
The Data Refresh Settings window appears. By default, the data cache and the data refresh settings are disabled.
4. To enable the server cache, choose the Enable Data Cache checkbox.
The data refresh settings are enabled for data entry.
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:07 AM
5. To set the time of day at which you want the data refresh to start, on the right of the Refresh Data At column, select one or
more checkboxes to schedule your daily data refresh. To select or deselect all the 24 checkboxes that correspond to the 24
hours of a day, click the column header area.
 Note
If you do not make any changes after you select the Enable Data Cache checkbox, the default setting is used: refresh
data at 00:00 every day.
6. To save the data refresh settings, choose the OK button.
You receive a message that the operation was successful, and the window is closed.
If you select the Enable Data Cache checkbox and you do not select any checkbox for daily refresh time settings before you
choose OK, you receive the following message:
To define the daily refresh times for the dashboard, select one or more checkboxes.
 Note
To enhance the performance of dashboards, only displayed data would be cached when you choose to enable the data
cache. This means that the data in unloaded sub-charts of a dashboard would not be cached. Therefore, when you load
dashboards before the first automatic data refresh takes place, you may note data inconsistencies between the sub-
chart data and the main chart data. To solve this issue, you can choose the Refresh Data button or wait until the next
automatic data refresh finishes.
More Information
Working with Crystal Dashboards
SAP Predefined Dashboards
Dashboards delivered in the integration component of SAP Business One are based on SAP Business One standard functionality
and the demo database set up for OEC, the demo company. You may need customization help depending on your implementation
of the SAP Business One application and data range requirements. For information about creating dashboards, see the how-to
guide How to Develop Your Own Dashboards for SAP Business One at SAP Help Portal.
SAP predefines the following dashboards:
Cash Flow Forecast Dashboard
Delivery Analysis Dashboard
Inventory Counting Recommendation Dashboard
Inventory Status Dashboard
Payment Collection Dashboard
Purchase Quotations Dashboard
Sales Analysis Dashboard
Sales Employee Performance Dashboard
Service Call Status Dashboard
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:07 AM
Cash Flow Forecast Dashboard
 Note
This function is not available if you are using SAP Business One version for MS SQL and have installed SAP Business One
analytics powered by SAP HANA.
The status of this dashboard is Inactive by default if you are using SAP Business One, version for SAP HANA.
For more information about activating dashboards, see Activating or Deactivating a Dashboard.
The Cash Flow Forecast dashboard lets a finance manager forecast a company’s future cash on hand based on transaction
documents, projected postings, journal vouchers, and recurring postings. This dashboard presents cash account details that let
you arrange payments in advance. It shows large incoming and outgoing transactions of a period according to your definition and
helps you to identify key payments and business partners.
The Cash Flow Forecast dashboard has the following two tabs:
Cash Flow Forecast Overview
Use this tab to monitor the general incoming/outgoing amount and the opening balance for the selected period.
Cash Flow Details
Use this tab to view large incoming and outgoing transactions as well as related business partners.
To view this tab, on the Cash Flow Forecast Overview tab, click the chart section of the specific time period you want to
view. The Cash Flow Details window appears, displaying detailed information of the selected time period. To return to the
Cash Flow Forecast Overview tab, on the Cash Flow Details tab, choose the Overview link.
Cash Flow Forecast Overview
The Cash Flow Forecast Overview tab presents a bar-line combination chart showing the same data as in the Cash Flow Report.
Working with this chart typically involves the following operations:
Observe cash flow trends:
Incoming amount: shown as the deep blue bars, representing the incoming payments amount received from a
customer or an account.
Outgoing amount: shown as the light blue bars, representing the outgoing payments amount issued to a vendor or
an account.
Opening balance: shown as a dotted line. Each dot represents the opening balance of the corresponding time point.
The opening balance of a day equals the closing balance of the previous day, as shown in the Cash Flow Report (the
Balance column).
Numbers: Below the chart, three numbers display the real-time data of incoming amount, outgoing amount, and
opening balance. The numbers are refreshed when you move your mouse over different time periods.
Traffic Light Indicators: There are indicators (different color dots) displayed before the time points on the horizontal
axis of the charts. The colors indicate the following situations:
Green: optimistic situation, when you have sufficient cash flow on hand.
Yellow: poor situation, when you do not have enough cash flow on hand and you need to be cautious in
balancing your accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:07 AM
Red: dangerous situation, when you have inadequate cash flow on hand and urgently need to balance your
accounts.
 Note
SAP predefined the indicator thresholds in the Dashboard Parameters window. To change the thresholds, see
Configuring Dashboard Parameters, below.
Add data sources:
To add additional data sources for the cash flow forecast, select or deselect the Journal Vouchers and the Recurring
Postings checkboxes above the chart, as necessary.
Switch time intervals:
In the View by dropdown list, choose to view by Day, Week, or Month.
 Note
The week and month do not refer to calendar weeks and months. The definitions for week and month are in accordance
with the logic of the Cash Flow Report.
SAP predefined the number of days/weeks/months displayed in the chart. To change the settings, see Configuring
Dashboard Parameters, below.
View today’s account details:
To do so, choose the Account Details link below the chart. All the Cash, Credit Card, and Checks accounts are displayed
with the balance data of the current system time.
Drill down to view period details:
To view detailed information for a certain time period, click the chart section of that time period. The Cash Flow Details tab
appears, displaying the account details for the specified period of time.
Cash Flow Details
The Cash Flow Details tab contains a table showing large transaction details and a pie chart presenting the major business
partner or employee involved in the transactions; this helps you identify key payments and partners.
Large Transactions Table:
The table displays all transactions with an amount that is larger than the defined threshold. By default, any transaction
larger than 5000 (in local currency) is displayed. You can change this definition in the Dashboard Parameters window. For
more information, see Configuring Dashboard Parameters, below.
Pie Chart:
You can view the pie chart either by Incoming Amount or Outgoing Amount. After you select the data source, you can
choose to view the chart either by business partner or by sales employee, so as to observe the involvement of key business
partners and sales employees.
By default, the chart displays 5 business partners/employees, and the data of all the other business partners or employees
are grouped and displayed as Others. You can change the settings in the Dashboard Parameters window. For more
information, see Configuring Dashboard Parameters, below.
Configuring Dashboard Parameters
The Cash Flow Forecast dashboard uses the dashboard parameters to enable user customization of the dashboard configuration.
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:07 AM
To change the default settings, proceed as follows:
1. To open the Dashboard Parameters window, from the SAP Business One Main Menu, choose Administration Setup
General Dashboard Parameters .
2. In the Dashboard Parameters - Setup window, press Ctrl + F to switch to Find mode.
3. In the Code field, enter CFC and choose Find. The Cash Flow Config parameter set appears.
4. In the Value column, change the parameter values if necessary.
The following table explains the parameters for this dashboard.
Parameter Name Function Definition
No. of Days/Weeks/Months Defines the number of time points Enter an integer from 3 to 14. If you
(days/weeks/months) displayed on the define a value larger than 14, the
horizontal axis of the Cash Flow Forecast dashboard displays only 14 time periods
Overview chart. and the following message appears:
Dashboard displays no more
than 14 days/weeks/months
from today on
.
If you enter a number with decimals, the
decimals are rounded off automatically in
counting the days/weeks/months.
No. of BPs/Employees Defines the number of BPs/employees Enter an integer value no larger than 5. If
displayed in the pie chart in the Cash you define a value larger than 5, the
Flow Details window. dashboard displays only 5
BPs/employees and the following
message appears:
Dashboard displays no more
than 5 BPs/employees
.
If you enter a number with decimals, the
decimals are rounded off automatically in
counting BPs/employees.
Red/Yellow Defines the threshold for the traffic light By default, the threshold for the red
indicators. The value here stands for the indicator is 1 and that for the yellow
ratio of opening balance to outgoing indicator is 1.2.
amount. In the Cash Flow Forecast
Change the ratio threshold if necessary.
Overview chart, if the ratio of a certain
time period is:
No greater than the value defined
for red, the traffic light indicator
is red.
Greater than the value defined
for red, but smaller than the
value defined for Yellow, the
traffic light indicator is yellow.
No smaller than the value defined
for yellow, the traffic light
indicator is green.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:07 AM
Parameter Name Function Definition
Large Transaction Amount Defines the large transaction threshold. Enter a positive number. If you enter a
number with decimals, the decimals is
All transactions no smaller than the
rounded off automatically in calculation.
threshold value are displayed in the large
transactions table of the Cash Flow
Details window.
More Information
Working with Crystal Dashboards
Customer Receivables Aging Dashboard
 Note
This function is available only if you are using the SAP Business One version for Microsoft SQL.
The Customer Receivables Aging dashboard lets a finance manager review accounts receivables and identify current or potential
problems. This dashboard provides an overall analysis of a company’s accounts receivables collection efforts and the status of key
accounts.
Customer Receivables Aging: Dashboard Structure and Behavior
This dashboard has two sections:
The upper part provides an aging overview and an analysis of either overdue receivables or future remittances.
The lower part displays an analysis of overdue receivables or future remittances for the top five customers or sales
employees.
All the amounts in the dashboard are given in the local currency, which is displayed under the title bar on the right side. In the
lower part of the dashboard, you can use the dropdown list to switch the analysis from Customers, which is the default, to Sales
Employees. By default, details for the top customer or sales employee are displayed on the right side of the lower part. To display
the details for another customer or sales employee, in the bar chart, click the bar for the customer or sales employee for which you
want to view detailed information. For more information about the data refresh options and settings, see Scheduling Daily Data
Refresh for Dashboards.
Customer Receivables Aging: Dashboard Behavior Details
The balance due for a customer, a sales employee, or a specific aging interval should be a positive value. A negative value is not
shown correctly in the dashboard. To enable values to be displayed correctly in the dashboard, before displaying the dashboard
you must first reconcile credit memos and any other documents that result in a negative value. When you select the Customer
Receivables Aging dashboard, it displays the default time interval, which is 90+ Days. If there is no data for this time interval, the
display does not default to another time interval. Instead, the dashboard appears as follows:
In the Overdue Analysis line chart, the Overdue Total line appears with data; the 90+ Days line displays a zero value.
In the Overdue Analysis by Customers or Overdue Analysis by Sales Employees, no Top 5 Customers or Top 5 Sales
Employees bar chart appears.
In the Aging Versus Revenue line chart, the 90+ Days line displays a zero value. There is no Overdue Total and Revenue.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:07 AM
The default selection of the top-ranked customer or the top-ranked sales employee is realized only at initialization of the
dashboard (“at initialization” refers to selecting a new dashboard or clicking a different aging interval for the first time after
opening the first dashboard). If you change the selected aging interval to a different interval and then return to the previously
selected aging interval, the default display of the top-ranked customer or top-ranked employee in the Aging Versus Revenue line
chart does not occur. This also happens when you change the default display of Overdue Analysis by from Customers to Sales
Employees. This may result in no data being displayed in the Aging Versus Revenue and Future Remit Versus Sales Opportunities
line charts.
 Example
The dashboard shows the Top 5 Customers (31-60 Days) bar chart and the Aging Versus Revenue line chart. For both charts,
data for the top-ranked customer is shown. To display the second-ranked customer, you click the bar chart for the second-
ranked customer. Both charts now display data for the second-ranked customer. Now you change the Overdue Analysis by
from Customers to Sales Employees. The bar chart displays up to five top sales employees, depending on the data available.
The Aging Versus Revenue line chart displays data for the second-ranked sales employee (the expectation is that data for the
top-ranked sales employee is displayed). However, if there is only one “top” sales employee (one bar in the Top 5 Sales
Employees (31-60 Days) bar chart), no data is displayed in the Aging Versus Revenue line chart because there is no data for
the second-ranked sales employee. In this example, the line chart retains the ranking value (second-ranked) from the
previously displayed line chart.
 Example
The dashboard shows the Top 5 Customers (31-60 Days) bar chart and the Aging Versus Revenue line chart. For both charts,
data for the top-ranked customer is shown. First you display the second-ranked customer by clicking the bar chart for the
second-ranked customer. The line chart displays data for the second-ranked customer. Now you select a different aging interval
by clicking the relevant time slice in the Aging Overview pie chart. For the new aging interval, the bar chart displays up to five
top customers, depending on the data available. The Aging Versus Revenue line chart displays data for the top-ranked
customer. Then you change the aging interval back to 31-60 Days. The dashboard shows the Top 5 Customers (31-60 Days)
bar chart. The Aging Versus Revenue line chart displays data for the second-ranked customer (the expectation is that data for
the top-ranked customer is displayed). See also the example above.
Customer Receivables Aging: Company Overview
In the Customer Receivables Aging dashboard, the Aging Overview chart provides the percentage of overdue customer
receivables for specific time intervals. It controls the time interval for the other charts in the dashboard and lets you switch
between the Overdue Analysis and Future Remit Analysis.
Type and Display Behavior KPI
Chart showing aging total and percentage 90+ Days is the default time interval for the The KPI is the percentage of the amount
distribution of customer receivables by other charts in the dashboard. (Overdue due for each time interval. Data comes from
time interval and future remittances Analysis, Top 5 Customers <time the Customer Receivables Aging report.
period>,Top 5 Sales Employees <time
period> and Aging Versus Revenue). To
change the time interval, click one of the
<n> Days segments in the chart.
Overdue Analysis: Company Overview
This chart provides a historical analysis of customer receivables for the time interval you selected in the Aging Overview chart.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:07 AM
Type and Display Behavior KPI
Two-line chart showing the trend of a Changing the time period in the X axis Amount for the current month is from the
company’s overdue accounts receivables refreshes the Overdue Total and <n> Days Customer Receivables Aging report with
total and overdue accounts for the time lines. To change the time period displayed in the Aging Date and Posting Date set to the
interval selected in the Aging Overview the X axis, from the View by dropdown list current date. Amount for previous months
chart. The Overdue Total line is always select one of the following options: is from the same report when the Aging
displayed. Date is set to the ending date of the
Last 6 Months: 6 months from
previous month.
current month (default)
Last 12 Months: 12 months from
current month The default time
interval is 90+ Days.
To change the time interval for the Overdue
Total and <n> Days lines, in the Aging
Overview chart click one of the <n> Days
segments. To view the future remittances
analysis, in the Aging Overview chart, click
the Future Remit segment.
Overdue Analysis: Customer and Employee Details
Overdue Analysis by Customers and Overdue Analysis by Sales Employees list the top five accounts and provide a historical
analysis of aging receivables versus revenue.
From the dropdown list, you select Customers or Sales Employees.
Chart Type and Display Behavior KPI
Top 5 Customers Bar chart with overdue To display the KPIs on the right The overdue amount for each
receivables for each of the top side of the chart for a different customer or sales employee is
Top 5 Sales Employees
five customers or sales customer or employee, click the from the Customer Receivables
employees for the selected time bar for the desired customer or Aging report.
interval in the Aging Overview employee. To change the time
chart interval, in the Aging Overview
chart click one of the <n> Days
segments. To view the future
remittances analysis, in the
Aging Overview chart, click the
Future Remit segment.
Aging Versus. Revenue Two-line chart (Overdue Total , For information about the Overdue Total is Balance Due
<n> Days) overlaying the behavior in this chart, see minus Future Remit in the
Revenue area Overdue Analysis: Company Customer Receivables Aging
Overview. report. The selection criteria
are:
Currency: Local
Aging Date: Current
Date
Age By: Due Date
Revenue is derived from the
selection criteria for the Sales
Analysis report. The document
should be Invoices. Posting
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
Date is from the beginning of
the selected horizon to the
current date.
Invoice-related documents and
localization A/R documents
that impact the revenue
account, such as credit memo,
A/R invoice exempt, A/R debit
memo, A/R bill, A/R exempt bill,
A/R export invoice, A/R
correction invoice, A/R
correction invoice reversal, and
A/R reserve invoice, are also
considered.
Future Remit Analysis: Company Overview
Type and Display Behavior KPI
Bar chart showing future remittances for a To change the time period displayed in the The future remittance amount for each time
selected time period X axis, from the View by dropdown list, period comes from the Customer
select one of the following options: Receivable Aging report, where Aging Date
is set to the end of each week or month.
Next 4 Weeks: 4 weeks from next
week (default)
Next 12 Weeks:12 weeks from next
week
Next 6 Months:6 months from next
month
The number of the week is taken from the
SAP Business One 8.81 calendar.
To view the overdue analysis, in the Aging
Overview chart, click one of the <n> Days
segments.
Future Remit Analysis: Customer and Employee Details
Chart Type and Display Behavior KPI
Top 5 Customers (Future Bar chart and future remittance To display the KPIs on the right The future remittance amount
Remit) amount for each of the top five side of the chart for a different for each time period comes
customers or sales employees customer or employee, click the from the Customer Receivables
Top 5 Sales Employees (Future
bar for the desired customer or Aging report; Aging Date is set
Remit)
employee. to the end of each week or
month.
Future Remit Versus Sales Clustered bar chart comparing For information about the The query for sales
Opportunities future remittances versus sales behavior in this chart, see opportunities is based on the
opportunities Future Remit Analysis: selection criteria for the
Company Overview. Opportunities Forecast Over
Time report.
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:07 AM
More Information
SAP Predefined Dashboards
Delivery Analysis Dashboard
 Note
This function is available only if:
You are using SAP Business One, version for SAP HANA.
Or, you are using SAP Business One version for MS SQL, and have installed SAP Business One analytics powered by SAP
HANA.
 Note
This dashboard considers only the sales orders that are fully copied to deliveries or A/R invoices, i.e., the sales orders are
closed.
The Delivery Analysis dashboard enables supervisors to identify whether the company delivers goods to customers on time. This
dashboard shows sales orders with on-time delivery and delayed delivery, in addition to the average number of delay days. This
dashboard also lists sales orders for which the delivery exceeds the user-defined delay days.
The Delivery Analysis dashboard contains the sections in the following table.
You can find the definitions used in the dashboard as follows:
Actual delivery date: Delivery Date of the delivery or Posting Date of the A/R invoice
Scheduled delivery date: the latest date taken from the following fields:
Delivery Date of the sales order
Del. Date in the item rows of the sales order
Delay days: number of days between the scheduled delivery date and the actual delivery date
Chart Type and Display Behavior KPI
Monthly Sales Orders Bar chart showing the number You can place your mouse Number of sales orders for
of monthly sales orders with on- cursor over a bar to view the which the delivery is on time or
time delivery and delayed exact number of sales orders. delayed.
delivery, respectively, in the
On Time Sales Orders:
past 6 months.
sales orders with actual
delivery date before or
equal to the scheduled
delivery date
Delayed Sales Orders:
sales orders with actual
delivery date after the
scheduled delivery date
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
Average Delay Days for Line chart showing the trend of You can place your mouse The average Delay Days for
Delayed Orders average delay days (for delayed cursor over a dot to view the each month is calculated as:
orders only) in the past 6 average number of delay days in
Sum of actual delay days / total
months. that month.
number of delayed sales orders
The month for which a sales
order is calculated is based on
its posting date.
Sales Orders Delayed More A table listing sales orders for You can change the number of
Sales Order: document
Than <user-defined number> which the delivery is delayed for days as follows:
number of the sales
Days more than <user-defined
1. From the SAP Business order
numbers> days. By default,
One, version for SAP
sales orders delayed by more BP Name: BP name of
HANA Main Menu,
than 2 days are shown. The the customer
choose
table is sorted by Delay Days in
descending order. Administration Setup Scheduled Delivery
General Dashboard Date: the latest date
Parameters .
taken from the following
fields:
2. In the Dashboard
Parameters – Setup
Delivery Date of
window, press CTRL + the sales order
F to switch to Find
mode. Del. Date in the
item rows of the
3. In the Code field, enter sales order
DPD and choose Find.
Actual Delay Days:
4. In the Value column, number of days
change the value of
between the scheduled
Allowed Delay Days.
delivery date and the
actual delivery date
To view details of a sales order,
click the sales order number in Amount: amount of the
the table. sales order, given in the
currency displayed
Use the page buttons in the
above the table
lower-right corner to navigate
through the pages.
Inventory Counting Recommendation Dashboard
 Note
This function is not available if you are using SAP Business One version for MS SQL and have installed SAP Business One
analytics powered by SAP HANA.
The Inventory Counting Recommendation dashboard enables managers to have a comprehensive view of the current status of
the company warehouses as regards inventory counting execution. It analyzes the values of warehouses, and recommends the
start of inventory counting process in certain warehouses according to user-defined rules.
The dashboard comprises the following two reports:
Warehouse Valuation Report
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:07 AM
Inventory Counting Risk Assessment Report
In addition, a section in the lower left part of the dashboard displays last count date, last counted warehouse, and the days since
last count.
 Note
The Last Count Date field displays the count date that appears in the latest inventory counting document or inventory posting
document that is not based on an inventory counting document. The same logic applies to the Last Counted Warehouse field
and the Days Since Last Count field.
Warehouse Valuation
This report appears in the upper part of the dashboard. It presents the warehouses’ value according to the items’ value, which is
calculated by the selected price source or according to the items’ quantities.
The bar chart displays only the top 10 warehouses with the highest total value or total quantity.
Field and Chart Series Description
Source Price List for Item Value Select a source price for the calculation of the items’ value from the
dropdown list.
This field is disabled when you choose to valuate warehouses by
quantity.
Warehouse Valuation by Choose to valuate warehouses by Item Value or Quantity.
Relative Count Date Specify a date.
The report takes into account only the items in inventory counting
documents (or inventory posting documents that are not based on
inventory counting documents) with the count date of the one you
specify and onwards.
By default, this field displays the beginning date of the fiscal year.
Note that you cannot enter a future date.
Currency Displays the local currency in the upper right corner of the
dashboard.
Counted Value/Quantity The total value or quantity of items in the warehouse which were
counted since the Relative Count Date.
Uncounted Value/Quantity The total value or quantity of items in the warehouse that were not
counted since the Relative Count Date.
Total Value/Quantity Total Value/Quantity = Counted Value/Quantity + Uncounted
Value/Quantity
Value = Quantity × Price ( from selected price source)
 Note
If an item in a specific warehouse was counted even if only in one bin of the warehouse, SAP Business One considers the item
as counted.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:07 AM
SAP Business One considers a negative quantity as zero quantity in this dashboard.
Inventory Counting Risk Assessment
This report appears in the lower right part of the dashboard, and displays the assessment of inventory counting risk by warehouse.
It comprises the following three parts:
Pie Chart
It shows the proportions of warehouses with high risk, medium risk, and low risk, respectively.
Warehouse Risk Rank
When you click different risks in the pie chart, you see the top 6 warehouses at the corresponding risk level. By default,
warehouses with high risk are displayed.
Detailed Risk Assessment Report
When you click the Details link in the Reference field under the pie chart, a detailed report appears to show you the risk
assessment per item per warehouse. This detailed report presents all warehouses at the corresponding risk level and all
items in these warehouses, except the items that are linked to these warehouses but have never been used in any
transactions involving these warehouses.
In this report, you can select item rows and press the Inventory Counting button to initiate an inventory counting process for
them.
The following chart illustrates how the report calculates the risk level of a certain warehouse based on the risk levels of the items in
it. The KPIs and related values given in the following chart are only default ones. You can change them to suit your own situation.
Each KPI has two values, value 1 and value 2 (value1 < value 2), and the system calculates the risk level of an item based on rules
involving these values.
Risk Level KPI Rule
Item Risk Level Days Since Last Inventory Count: Low Risk Item:
The more time that passes since last The values of all KPIs are below value 1.
inventory counting, the higher the risk is. If
Medium Risk Item:
the item is new and has never been counted
before, the creation date of the item is used The value of the first KPI (Days Since Last
as the last count date. Inventory Count) is between value 1 and
value 2, or the value of the first KPI is above
Transaction Volume:
value 2, but the values of the other two KPIs
The larger the transaction volume (since are below value 2.
last inventory count), the higher is the
High Risk Item:
priority for inventory counting, and
therefore, the higher the risk. The value of the first KPI (Days Since Last
Inventory Count) is above value 2, and the
The transaction volume is calculated
value of at least 1 more KPI (second or
according to the inventory turnover. One
third) is above value 2.
transaction with a large quantity is also
considered as a high-risk case.
Item Value:
The higher the cost of the item, the higher
is the priority for inventory counting, and
therefore, the higher the risk.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:07 AM
Risk Level KPI Rule
Warehouse Risk Level Percentage of Items at High Risk: Low Risk Warehouse:
The percentage of items that belong to the The percentage of items at high risk in this
“High Risk Item” category according to the warehouse is below 25% (value1).
KPIs and values that you define at the item
Medium Risk Warehouse:
level.
Includes all the cases which do not fit the
low risk warehouse and the high risk
warehouse categories.
High Risk Warehouse:
The percentage of items at high risk in this
warehouse is above 75% (value2).
Inventory Status Dashboard
 Note
This function is available only if:
You are using SAP Business One, version for SAP HANA.
Or, you are using SAP Business One version for MS SQL, and have installed SAP Business One analytics powered by SAP
HANA.
The Inventory Status dashboard helps department managers in operations, manufacturing, financials, or sales to manage
inventory in the following four categories, based on the trend of inventory value and turnover rate:
Potential Insufficient Inventory
Potential Excessive Inventory
Higher Inventory & Faster Moving
Lower Inventory & Slower Moving
The inventory depletion trends and values in this dashboard help managers to determine whether a promotion is needed to
decrease excessive inventory, or whether purchases are needed to avoid inventory shortage.
The Inventory Status dashboard consists of two sections:
Company Overview: A bar chart providing an overview of the company inventory status.
Category Details (Chart View & Table View): A scatter chart or a table displaying the detailed information for warehouse
items in the selected category.
All the amounts in the dashboard are given in the local currency, which is displayed in the upper-right corner of the window.
Inventory Status: Company Overview
The Company Overview section covers 2 KPIs:
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:07 AM
Inventory amount of each warehouse item
Turnover rate of each warehouse item
The turnover rate is calculated as follows:
Turnover rate = 360 / (last day - first day) / ((cumulative quantity of last day + cumulative quantity of first day) / 2 / (sum
of negative quantity of the period))
The dashboard compares items' inventory amount and turnover rate on the trend of the KPIs. A bar chart is presented showing the
inventory amount of warehouse items in four categories:
Potential Insufficient Inventory – Total value of items that are going to be in short supply due to decreased inventory value
and/or increased turnover rate.
 Note
The dashboard compares the inventory value and turnover rate between the current posting period and the last posing
period to determine whether they are increased or decreased.
Potential Excessive Inventory – Total value of items that are going to be overstocked due to increased inventory value
and/or decreased turnover rate.
Higher Inventory & Faster Moving – Total value of items whose inventory value and turnover rate were increased or
unchanged.
Lower Inventory & Slower Moving – Total value of items whose inventory value and turnover rate were decreased.
Working with this chart typically involves the following operations:
To switch the analysis from all item groups in all warehouses, which is the default, to a certain item group and/or in a
certain warehouse, select the desired item group and/or warehouse in the Analyzed by dropdown list below the chart title.
To view the total inventory amount for all items in a category, place your mouse cursor over the bar for the category,
without clicking it. The inventory amount for that category is shown in a small text box.
To display the details for items in a category, click the bar for the category. This switches the view to the Category Details
section.
Inventory Status: Category Details
The Category Details section covers the same KPIs as the Company Overview section. The chart view presents a scatter chart
showing the amount and turnover rate for individual warehouse items in the selected category. The table view lists more detailed
item information in a tabular format.
Working with this section typically involves the following operations:
To go to the Company Overview section, click Back to Overview in the upper-left corner.
To switch between the chart view and table view, click the Table View or Chart View icon to the right of the category title.
In the chart view, you can use the range sliders for the X and Y axes to filter the items displayed on the scatter chart.
In the chart view, you can place your mouse cursor over a dot to view the item name and its inventory amount and turnover
rate. More detailed information for the selected item is displayed on the right side of the window.
In the table view, you can export the current tables as an Excel file by choosing the Export to Excel button.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:07 AM
Payment Collection Analysis Dashboard
 Note
This function is available only if:
You are using SAP Business One, version for SAP HANA.
Or, you are using SAP Business One version for MS SQL, and have installed SAP Business One analytics powered by SAP
HANA.
The Payment Collection Analysis dashboard helps financial analysts or managers to monitor the payment collection of a
company’s sales orders. This dashboard shows paid and unpaid sales orders on a monthly basis, and the average number of days
passed from the sales order posting date to the payment date. This dashboard also lists sales orders that are paid more than a
user-defined number of days after the posting date.
The Payment Collection Analysis dashboard contains the sections in the following table.
Chart Type and Display Behavior KPI
Sales Orders Payment Status Bar chart showing the summed You can place your mouse Summed document total of
document total of monthly cursor over a bar to view the paid and unpaid sales orders.
sales orders that are paid and amount of paid or unpaid sales
Amount Paid: summed
unpaid, respectively, in the past orders.
document total of sales
6 months.
orders for which the
payment has been
collected
Amount Unpaid:
summed document
total of sales orders that
were not paid or not
fully paid
Average Order-to-Payment Line chart showing the trend of You can place your mouse The Average Order-to-Payment
Days average order-to-payment days cursor over a dot to view the Days for each month is
in the past 6 months. average number of order-to- calculated as:
payment days in that month.
Sum of order-to-payment days
/ total number of sales orders
Order-to-Payment
Days: number of days
passed from the sales
order posting date to
the closing date of all
invoices
The month to which a
sales order is calculated
is based on its posting
date.
Sales Orders Paid More Than A table listing sales orders for You can change the number of
Sales Order: document
<user-defined number> Days which the payments were days as follows:
number of the sales
After Posting Date collected more than <user-
order
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
defined number> days after the 1. From the SAP Business BP Name: BP name of
posting date. By default, sales One, version for SAP the customer
orders paid more than 0 days HANA Main Menu,
Sales Order Posting
after posting date are shown. choose
Date: posting date of
Administration Setup
The table is sorted by sales the sales order
General Dashboard
order document number in
Parameters . Order-to-Payment
ascending order by default.
Days: number of days
2. In the Dashboard
passed from the sales
Parameters – Setup
order posting date to
window, press CTRL +
the closing date of all
F to switch to Find
invoices
mode.
Amount: amount of the
3. In the Code field, enter
sales order, given in the
PCA and choose Find.
currency displayed
4. In the Value column, above the table
change the value of
Allowed Delay Days.
To view details of a sales order,
click the sales order number in
the table.
Use the page buttons in the
lower-right corner to navigate
through the pages.
Purchase Quotations Dashboard
You can use the Purchase Quotations dashboard to monitor open purchase quotations. Using the filter, you can view open
purchase quotations by selected vendor, item, buyer, and valid date. You can use this dashboard to view how vendors respond to
your quotations. For quotations with responses, you can compare quotations and close quotations.
The Purchase Quotations dashboard presents a pie chart displaying open purchase quotations for a certain time period. Working
with this chart typically involves the following operations.
View Quotation Status
Responded: If a quotation has a full response from the required vendor (with all items quoted with quantity and unit
price), then this quotation is defined as Responded.
Partial/No Response: If a quotation does not have a full response from the vendor (with one or more items not
quoted), then this quotation is defined as Partial/No Response.
Overdue: Quotations with a Valid Until date that is earlier than the current system date.
To view detailed information, click a segment of the pie chart. The Purchase Quotations Details window appears,
displaying a list of relevant purchase quotations and containing the following information: group number, document
number, supplier name, supplier telephone number, reference number, and valid date information.
You can also click a row in the table to open the corresponding SAP Business One, version for SAP HANA purchase
quotation document.
Filter Data by Valid Date
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:07 AM
This dashboard enables you to filter open purchase quotations by expiration date. To do so, in the “Valid Until” No Later
Than field, select a date. The chart presents all purchase quotations that expire before the specified date.
 Note
If you specify a date earlier than the current system date, all displayed purchase quotations are overdue quotations.
View Data of Selected Vendors/Items/Buyers
By default, this dashboard displays data for all open purchase quotations (including overdue purchase quotations). You can
use the filter to view data for selected vendors/vendor groups, items/item groups, and buyers. To do so, proceed as follows:
From the Choose Scope dropdown list, select to view data by Vendor, Item, or Buyer.
If you select Vendor or Item in the previous step, from the Choose Group dropdown list, select a group. The
dashboard displays open purchase quotations for the specified vendor/item group.
If you want to view data for a specific vendor/item/buyer, from the Choose or Choose Buyer dropdown list, select a
vendor/item/buyer.
The dashboard displays open purchase quotations for the selected vendor/item/buyer only.
More Information
Working with Crystal Dashboards
Sales Analysis Dashboard
 Note
The status of this dashboard is Inactive by default if either of the following is true:
You are using SAP Business One, version for SAP HANA.
You are using SAP Business One version for MS SQL and have installed SAP Business One analytics powered by SAP
HANA.
For more information about activating dashboards, see Activating or Deactivating a Dashboard.
The Sales Analysis dashboard enables sales managers to understand the sales performance and status of a company’s most
important customers and employees.
The dashboard KPIs are based on the standard functions of SAP Business One, version for SAP HANA. The application makes the
following assumptions for sales processes:
The sales quota is maintained in the budget of the sales revenue account by month.
The sales process starts with opportunity creation and ends with invoice creation. Only the invoiced amount is revenue
realized. Canceling an invoice or creating a credit memo impacts the revenue of the month in which the cancellation or
credit is posted.
If an opportunity is lost, the sales employee changes the opportunity status to Lost.
Sales Analysis: Dashboard Structure and Behavior
The Sales Analysis dashboard has the following sections:
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:07 AM
The upper part provides an overview of sales performance.
The lower part displays detailed information about the top five customers or sales employees.
All amounts in the dashboard are shown in the local currency, which is displayed under the title bar on the right side. In the lower
part of the dashboard, you can use the dropdown list to switch the analysis from Customers, which is the default, to Sales
Employees. By default, details about the top customer or top employee are displayed on the right side of the lower part. To display
the details for another customer or employee, click the bar for the customer or employee for which you want to view detailed
information.
Sales Analysis: Company Overview
The upper general sales performance part covers four KPIs: sales amount by month, last year’s sales amount by month, sales
quota, and sales opportunity win rate.
Chart Type and Display KPI
Fiscal Year Analysis Bar chart showing revenue for the current The sales amount calculation is based on
year and the previous year (Sales Amount invoice installment amount and grouped by
and Last Year’s Sales Amount); line for posting calendar month.
Quota. For the current year and last year,
Invoice-related documents and localization
the sales amount is shown for all months.
A/R documents that impact the revenue
account are also considered.
Quota uses the budget definition of revenue
account, which is the first budget scenario
defined for one fiscal year. Make sure the
revenue account has an account type of
Sales and is on the credit side.
Opportunity Win Rate Line chart showing the ratio of won The chart compares the current year’s win
opportunities to the total of closed rate to the previous year’s rate by month.
opportunities for the period.
For each displayed month, the win rate
Two lines are shown: one line for the equals the number of won opportunities in
previous year, one line for the current year this month divided by the total number of
to date. closed opportunities in this month. Closed
opportunities include opportunities with
status Won or Lost. Closing date refers to
opportunity Closing Date.
Sales Analysis: Customer and Employee Details
Chart Type and Display Behavior KPI
Top 5 Customers Top 5 Sales Clustered bar chart (one for To display the KPIs on the right Year-to-date sales amount and
Employees sales amount and one for gross side of the chart for a different gross profit of top 5 customers
profit) for each of the top 5 customer or employee, click the or top 5 employees are
customers or employees Sales Amount bar for the displayed as a clustered bar
desired customer or sales chart.
employee.
Item Ranking Customer Table with top 5 items (for To display the KPIs for a
For selected customer:
Ranking Customers selection) and top 5 different customer or employee,
customers (for Sales in the Top 5 Customers or Top 5 Top 5 items by each
Employees selection) sorted by Sales Employees chart, click
item’s sales amount for
sales amount. the sales amount bar for the
the current fiscal year.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
desired customer or sales Revenue: current fiscal
employee. year revenue of the item
You can click an item in the %: percentage this item
table to display the Item Master contributes to the
Data window. customer’s total sales
amount
Quantity: number or
quantity of the item sold
to the customer (by
inventory unit of
measure)
For selected sales
employee:
Top 5 customers by
customer’s sales
amount for the current
fiscal year.
Revenue: current fiscal
year revenue of the
customer
%: percentage this
customer contributes to
total sales for this sales
employee
Profit: current fiscal
year gross profit for
customer related to this
sales employee
Opportunities Status Pie chart None Depending on the selection in
the dropdown list (Customers
or Sales Employees), the
number of won and lost
opportunities for the fiscal year
to date and the number of open
opportunities, for the selected
customer or selected sales
employee.
More Information
SAP Predefined Dashboards
Sales Employee Performance Target Dashboard
 Note
This function is available only if:
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:07 AM
You are using SAP Business One, version for SAP HANA.
Or, you are using SAP Business One version for MS SQL, and have installed SAP Business One analytics powered by SAP
HANA.
The Sales Employee Performance Target dashboard helps sales managers to review the performance of each sales employee,
including his or her sales target, year-to-date sales amount, ongoing sales opportunities, and contribution to the overall sales
revenue.
The Sales Employee Performance Target dashboard contains the sections shown in the following table. All amounts in the
dashboard are shown in the local currency, which is displayed in the upper-right corner.
Chart Type and Display Behavior KPI
Sales Employees List displaying the names of all You can click a name to display
Names of sales
sales employees, sorted by each the KPIs on the right side of the
employees
employee’s year-to-date window for that employee.
contribution (%) in descending
YTD contribution % is
By default, All Sales Employees
order.
calculated by:
is selected.
When a sales employee is
(each employee’s year-
selected, his or her year-to-date to-date sales amount) /
contribution (%) is shown (all employees’ year-to-
beside the employee name. date sales amount) *
100%
The sales amount data
comes from the Sales
Analysis report.
Monthly Sales by <sales The upper bar chart shows the To display the potential sales
Target: sales target for
employee> monthly sales target, actual amount in the future, select
that month. The amount
sales amount (in the past) or Weighted Potential.
is set in the Dashboard
potential sales amount (in the
To display last year's data, Parameters – Setup
future) in the current or
select Last Year. window. See the Setting
previous year for selected
Monthly Sales Target
employee or all employees. To display the data for a
section for details.
different employee, click the
The lower bar chart shows the
employee name on the left side. Actual: actual sales
yearly sales target, the yearly
amount for that month.
actual or forecasted sales You can place your mouse
Data comes from the
amount in the current or cursor over a bar to view more
Sales Analysis report.
previous year for the selected
KPIs.
employee or all employees.
Weighted Potential:
weighted amount of
open opportunities in
that month. Data comes
from the Weighted
Open Amt field of the
Opportunity Statistics
report.
The lower bar chart has 2 KPIs:
Projected Year Sales is
calculated by:
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
(actual year-to-date
sales amount) +
(weighted amount of
open sales
opportunities)
Year Target: total sales
target amount of the
current or previous year.
You can set the monthly
sales target as
described in the Setting
Monthly Sales Target
section.
Setting Monthly Sales Target
To set a monthly sales target amount for each employee, do the following:
1. From the SAP Business One, version for SAP HANA Main Menu, choose Administration Setup General Dashboard
Parameters .
2. In the Dashboard Parameters – Setup window, press CTRL + F to switch to Find mode.
3. In the Code field, enter SEPT and choose Find.
4. In the table, enter the monthly sales target amount for each employee.
Service Call Dashboard
The Service Call dashboard enables service managers to identify current and potential problems with service call responsiveness.
This dashboard presents key performance indicators that provide different views of service calls being handled by your employees.
It shows the overall service call status by number of new service calls for the current date, backlog trends, and call status. For each
service queue, the dashboard shows the service call workload and status by employee.
Service Call: Dashboard Structure and Behavior
The Service Call dashboard has the following sections:
The upper part provides a company overview.
The lower part displays detailed information about a selected service queue.
By default, the data is refreshed every 60 minutes. When you select a different service queue name from the dropdown list in the
lower part of the dashboard, the application refreshes the data in the lower part for the selected service queue. The service queue
names displayed in the company overview section and in the dropdown list are taken from the description field of the queue setup.
Only active service queues are shown. The names in the Details of dropdown list are displayed in the same order as in the Queues -
Setup window.
Service Call: Company Overview
The company overview covers KPIs that inform the service manager about new service calls for the current day, any calls due
today or overdue calls, and the trend of service calls for a specific time period.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:07 AM
Chart Type and Display Behavior KPI
Incoming Calls Today Pie chart with total number of None Service call with Created On
today’s new service calls by date equal to current date
active service queue
Calls to Close: <n> Pie chart with in-process None
Overdue: service call
service calls of active service
with Resolution By date
queues, grouped by category of
before the current date
due date
Due by Today: service
call with Resolution By
date equal to the
current date
Others: service call with
Resolution By date
after the current date
and service call with no
Resolution By date
Backlog of <time period Line chart with a line for each The user selects a time period The backlog of calls is the
selection> service queue showing the from Backlog of dropdown list. number of in-process service
trend of the service call backlog Last 7 Days is the default. The calls at the end of each day. For
for the selected time period number of backlog calls for example, if a user selects Last 4
each active service queue is Weeks or Last 6 Months, the
refreshed, the lines are backlog is the in-process
repositioned, and the X axis service calls for the last day of
changes as follows: each time period.
Last 7 Days: dates of
last 7 days including
today
Last 4 Weeks: last 4
calendar weeks
including the current
week
Last 6 Months: last 6
calendar months
including the current
month
Service Call: Service Queue Details
The lower queue part covers the following queue-specific KPIs:
Employees workload
Service call turnover
To display a queue, select an option from the Details of dropdown list.
Chart Type and Display Behavior KPI
Employee Workload Bar chart displays the workload None Number of in-process calls
of employees. Each bar assigned to each member of the
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:07 AM
| Chart | Type and Display              | Behavior | KPI                          |
| ----- | ----------------------------- | -------- | ---------------------------- |
|       | represents a service employee |          | selected service queue. Each |
assigned to the service queue, call is classified as Overdue,
|     | and displays the total number   |     | Due byToday , and Others.    |
| --- | ------------------------------- | --- | ---------------------------- |
|     | of service calls assigned to an |     | Unassigned service calls are |
|     | employee. Color coding shows    |     | combined in the Not Assigned |
service calls that are overdue, bar. For information about the
|     | due by today, and due in the  |     | coding, see the Calls to Close: |
| --- | ----------------------------- | --- | ------------------------------- |
|     | future or those without a due |     | <n> row in the Service Call:    |
|     | date.                         |     | Company Overview section.       |
Service Call Turnover of <time Line chart with a line for new The user selects a time period New service calls and closed
period selection> service calls and a line for from the Service Call Turnover service calls jointly show service
|     | closed service calls for the     | of <time period selection> | call turnover. |
| --- | -------------------------------- | -------------------------- | -------------- |
|     | selected time period over a gray | dropdown list.             |                |
A new service call is created
area representing call backlog
|     |     | For information about the | during the displayed time |
| --- | --- | ------------------------- | ------------------------- |
as reference.
|     |     | behavior in this chart, see the | period, regardless of status. A    |
| --- | --- | ------------------------------- | ---------------------------------- |
|     |     | Backlog of<time period          | closed call is a service call that |
|     |     | selection> row in the Service   | is closed during the displayed     |
|     |     | Call: Company Overview          | time period, regardless of when    |
|     |     | section.                        | it was created.                    |
Create date refers to the
Created On date of a service
call. Close date refers to a
service call’s status of Closed
and a Closed On date within the
displayed time period.
More Information
SAP Predefined Dashboards
This is custom documentation. For more information, please visit SAP Help Portal. 31