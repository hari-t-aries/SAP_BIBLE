6/8/26, 6:10 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:10:54 GMT+0000
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

6/8/26, 6:10 AM
MRP
The Material Requirements Planning (MRP) module enables you to plan material requirements for a manufacturing or
procurement process based on the re-evaluation of existing inventories, demands, and supplies on changing planning parameters
(such as lead time determination, make or buy decisions, and holiday planning).
MRP calculates gross requirements for the highest bill of materials (BoM) level, based on existing inventory, sales orders, purchase
orders, production orders, forecasts, and so on. It calculates gross requirements at the lowest BOM levels by carrying down net
parent demands through the BOM structure. Dependent levels might have their own requirements, based on sales orders and
forecasts.
The results of the MRP run are report and recommendations that fulfill gross requirements by taking into consideration the
existing inventory levels and existing purchase orders and production orders. The MRP run also takes into account predefined
planning rules such as Order Multiple, Order Interval, Minimum Order Quantity, Inventory Level, and so on.
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
For further information on MRP with additional examples, see the guide How to Configure and Use MRP in SAP Business One.
Please note that image maps are not interactive in PDF outputs.
Managing Forecasts
In many cases, production companies receive sales orders on short notice. However, the production process might take a great
deal of time. As a result, it is common for these companies to plan their purchasing and production in advance, even before they
receive actual sales orders. This is the goal of a forecast, which is designed to serve as an additional requirement. Therefore, the
goods are produced based on the forecast, and when the actual sales orders are received, the company is able to supply the order
quickly.
SAP Business One lets you generate forecasts based on historical sales records or manually entered forecast quantities. You can
then use the forecasts as an additional data source for the MRP calculation.
 Note
Although there is no restriction on the number of forecasts you can define, you can select only one forecast for a single MRP
scenario. For more information, see Running MRP - General Process, Prerequisites, and Procedure.
To add, duplicate, update, or delete an MRP forecast, from the SAP Business One Main Menu, choose MRP Forecasts and
follow the appropriate procedure listed below.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:10 AM
Once you have saved a forecast, you cannot change its view.
You can select multiple lines in the forecast to perform the following actions:
adjust the quantities for the lines by choosing the button or the button
delete the lines by choosing the Delete Row option from the context menu
In MRP calculations, you can consume a forecast using sales orders and blanket agreements. To do so, proceed as follows:
 Note
To enable the consume forecast function, make sure you have selected the Consume Forecast checkbox on the General
Settings: Inventory Tab.
1. To consume a forecast using sales orders, on the Contents tab of the Sales Order window, select Yes for the Consume
Forecast column.
For more information, see Sales Document: Contents Tab.
2. To consume a forecast using blanket agreements, in the Blanket Agreement Details window, select the Consume Forecast
checkbox. For more information, see Blanket Agreement Details.
 Note
Only blanket agreements of type Specific can be set to consume a forecast.
Procedure
Creating Forecasts
1. Switch to Add mode. For more information, see Working in Add Mode.
2. Enter the forecast code and name.
3. Enter the start and end dates for the forecast horizon.
The date you specify may change in accordance with the value selected in the View field. For examples, see Start Date, End
Date in the Forecasts Window.
4. In the View dropdown list, select a time period to manage the forecast.
 Note
You cannot update the view after adding the forecast.
For more information about view options, see View in the Forecasts Window.
5. Specify one or more items to include in the forecast.
To specify forecast items and quantities, do one of the following:
Manually Define a Forecast
a. Specify one or more items to include in the forecast.
b. Enter forecast quantities for each period in the items’ sales units. You can define Sales UoM for items under
Inventory Item Master Data Sales Data Sales UoM .
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:10 AM
 Note
You are not required to enter a value for every period. For example, if you create a weekly forecast for six
months, you are not required to enter a quantity for every week.
Automatically Generate a Forecast
 Note
If you are using SAP Business One, version for SAP HANA, there are two types of forecasts:
Basic forecast: you can find the description below.
Intelligent forecast: for more information, see Generating an Intelligent Forecast.
a. In the Forecast window, choose the Generate Forecast button.
 Note
If you are using SAP Business One, version for SAP HANA, to view the Generate Forecasts - Set Up
window, in the Forecast window, choose the Generate Forecast button, and choose Basic Forecast.
The Generate Forecasts - Set Up window appears.
Use the selection criteria to filter items to be included in the forecast. You may filter items by Item, Preferred
Vendor, or Default Warehouse.
b. Click to expand Advanced Settings.
c. Under Advanced Settings, define the sales records of a period as the calculation basis for the forecast
quantity.
To do so, select the Base on Sales History checkbox and specify the calculation method. Available
calculation methods vary in accordance with the definition of the View field. For more information about the
calculation algorithm for each option, see Base on Sales History in Generate Forecasts — Set Up Window.
d. Specify the sales documents to include in the calculation. You may select Sales Orders and Deliveries and
A/R Invoice.
 Note
A/R invoices based on a delivery and A/R reserve invoices are not considered.
Canceled documents and reserved invoices are not considered.
Only sales documents with posting dates within the range of history start and end dates are
considered.
e. Specify the History Start Date field and the application automatically calculates the history end date.
 Note
Make sure you specify a date no later than the forecast Start Date.
SAP Business One may adjust your History Start Date entry according to your definition for the
forecast View.
f. To save data and return to the Forecasts window, choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:10 AM
SAP Business One populates this window with items you select and displays the automatically generated
forecast quantities for each item in each period.
6. In some cases, you may want to adjust the forecast quantities by a certain percentage. For example, you generate a forecast
based on the sales history of the last three months. But you realize that the forecast period would be the peak period of the
year, so you decide to multiply the forecast quantities by 200%. To do so, in the top right corner of the Forecasts window,
use and to adjust forecast quantities.
For more information, see Forecast Quantity Adjustment in the Forecasts Window.
7. To save the forecast changes, choose the Add button.
Duplicating Forecasts
1. Switch to Find mode. For more information, see Working with Find Mode.
2. Enter an asterisk (*) and from the list, select the forecast to duplicate.
3. From the Data menu, choose the Duplicate button.
Updating Forecasts
1. Switch to Find mode. For more information, see Working with Find Mode.
2. Enter an asterisk (*) and from the list, select the forecast to update.
The details of the forecast are displayed.
3. Do one or more of the following, as required:
Change the forecast description.
Overwrite the dates to change the forecast horizon.
The period values are deleted and replaced by the new ones.
 Caution
If you change the range of dates in the Start and End Date fields, the data that does not fall within the range of
dates is deleted.
Update the item record.
To display the item master data for the item, in the Item No. field, click .
To overwrite the value in the Item No. field, enter a new item number, or remove the existing value, press
TAB , and select a value from the list.
Update quantities for each item in each period.
4. To save the changes, choose the Update button.
5. To close the window, choose the OK button.
Deleting Forecasts
1. Switch to Find mode. For more information, see Working with Find Mode.
2. Enter an asterisk (*) and from the list, select the forecast to delete.
3. From the Data menu, choose the Remove button.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:10 AM
 Caution
You cannot remove a forecast that has been used in an MRP run.
More Information
Forecasts Window
Generating an Intelligent Forecast
Intelligent Forecast Window
Forecasts Window
Use this window to create and maintain forecasts for items. For more information about how to create and maintain forecasts, see
Managing Forecasts.
To open the window, choose MRP Forecasts .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Forecasts Window Fields
Forecast Code, Forecast Name
Specify code and meaningful name for the forecast.
Start Date, End Date
Specify the period to which the forecasts is related. The date range is automatically adjusted according to the specified View.
 Example
The value in the View field is Daily, you specify a date range of 10 days, then, you change the View to Weekly. The date range is
automatically updated to cover two whole weeks.
 Example
You enter March 4, 2011 as the start date and March 15 as the end date with the field View elected as Monthly. SAP Business
One changes the two dates automatically to the beginning of the month, March 1, 2011 and the end of the month, March 31,
2011.
View
Select the view in which you want to manage the forecast. Each view defines a time-bucket resolution by which the forecast is
managed. The values are:
Daily
Select this option to divide the forecast into days. When you select this option, SAP Business One displays a column for
each day in the selected date range.
Weekly
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:10 AM
Select this option to divide the forecast into weeks. If you select this option, SAP Business One displays the week number
as the column's name (52 weeks in a year). MRP considers the weekly requirement as falling on the first day of each week.
 Note
The weekly numbering definition and weekend definition may affect the week numbers and the first day of the week. To
maintain the definitions, choose Administration System Initialization Company Details Accounting Data
Holidays Holiday Dates . For more information, see the Holiday Dates Window.
Monthly
Select this option to divide the forecast into months. When you select this option, SAP Business One displays the name of
the month as the column's name. MRP considers the monthly requirement as falling on the first day of the month.
Warehouse
Displays the warehouse in which the item is stored.
Quantity Per Period
Enter the quantity of the forecast item in each period for which demand has been forecast.
Forecast Quantity Adjustment
Adjusts forecast quantities by a defined percentage.
To do so, proceed as follows:
1. Select one or more rows in the table for which you are going to adjust the quantities.
2. To adjust the percentage, you can:
Use button and to increase or decrease target quantities by multiples of 5.
Enter a number and copy to the field.
 Note
Negative figures are not supported. If the decrement falls below 0, then 0 is displayed.
Sales UoM
Displays the sales UoM of this item as defined in the item master data. By default, this column is not displayed. To display this
column, click in the toolbar.
To view the definitions of Sales UoM and Items per Sales Unit, choose Inventory Item Master Data Sales Data .
To convert the forecast screen data to inventory quantities, multiply the forecast data by the value in the Items per Sales Unit
field.
 Example
You set the Items per Sales Unit to 5 for item A001, and the quantity entered into the item forecast for a specific day is 10. If
this forecast is included in the MRP calculation, it will add a demand of 5 x 10 = 50 items to the total demand for that specific
day.
 Note
Sales orders may have different Items per Sales Unit definitions. Therefore, when consuming a forecast using sales orders in
an MRP run, the application converts sales order quantities based on the same definition of Items per Sales Unit as the
forecast before actually consuming the forecast.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:10 AM
To select additional fields, such as Item Group and Sales UoM, click in the toolbar. You can also choose to display the column
headers for the MRP results in an abbreviated or long format.
More Information
Managing Forecasts
Generate Forecasts - Setup Window
Use this window to generate forecasts based on the sales history.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Forecasts Generation Fields
Select Items By
Filters to be included in the forecast.
You may filter items by Item, preferred Vendor, and Default Warehouse.
Generate Forecast for Warehouses
Select the browse button to open the Warehouse Selection window, in which you can select the warehouses that store the items
you want to include in the forecast.
When the checkbox is selected, it indicates that at least one warehouse is selected; when the checkbox is unselected, it indicates
that no warehouse is selected, and the default warehouse will be displayed in the forecast.
Base on Sales History
Determines the sales documents to be included into calculation and the calculation method.
Available calculation methods vary in accordance to the definition of the View field.
Simple Average
1. Total quantities for the selected item, from the selected sales document, within the history start and end date are
summed up.
2. Summed quantities are then averaged by the number of days, weeks or months according to the forecast start and
end date
Daily History
1. Total quantities for the selected item, from the selected sales document, for each day within the history start and
end date are extracted.
2. Extracted quantities per day are populated into each day within the forecast start and end date.
Weekly History
1. Total quantities for the selected item, from the selected sales document, for each week are summed up.
2. Summed quantities per week are populated into each week within the forecast start and end date.
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:10 AM
Monthly History
1. Total quantities for the selected item, from the selected sales document, for each month are summed up
2. Summed quantities per month are populated into each month within the forecast start and end date
History Start Date
Enter the sales history start date. SAP Business One automatically generates an end date according to your definition of the
forecast horizon.
 Note
SAP Business One may adjust your input of History Start Date according to your definition for the forecast View.
The application uses the dates below to filter the corresponding documents with the history range you defined:
Sales orders: Del. Date in item lines.
Deliveries: Actual Delivery Date in item lines
A/R invoices: Actual Delivery Date in item lines
More Information
Managing Forecasts
Generating an Intelligent Forecast
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
Prerequisites
You have installed the Application Function Library (AFL), which includes the SAP HANA Predictive Analysis Library (PAL).
For more information about the database role PAL_ROLE, look for the SAP Business One Administrator's Guide, version
for SAP HANA on SAP Partner Edge .
In the SAP HANA Studio, you have activated the script server in your SAP HANA instance. See SAP Note 1650957 for
further information.
Procedure
1. In the Forecasts window, choose the Generate Forecast button, and choose Intelligent Forecast.
The Intelligent Forecast window appears.
 Note
For more information about other actions that need to be performed in the Forecasts window, see Managing Forecasts.
2. In the Configuration area, perform the following. For more information, see Intelligent Forecast Window.
In the Select Items By dropdown list, use the selection criteria to filter items to be included in the forecast. You may
filter items by Item, Preferred Vendor, or Default Warehouse.
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:10 AM
Select the Warehouse checkbox to generate forecasts for filtered items in specific warehouses. If the checkbox is
deselected, only the item's default warehouse is considered in the forecast. If the item does not have a default
warehouse, then the company's default warehouse is considered in the forecast.
In the Sales History section, define the historic sales records as the calculation basis for the forecast.
In the Calc. Method dropdown list, select the algorithm to be used in the forecast.
 Recommendation
Use the automatic selection of calculation methods, which will apply the most suitable method and its
parameters based on the historic data.
3. To generate the forecast, choose the Forecast button.
4. In the Forecast Values area, you can find the generated forecast quantities for each item in specific warehouses in each
time bucket. For more information, see Intelligent Forecast Window.
5. Select one row in the Forecast Values area to display its graphic statistics below. By default, the first row is selected.
In the graphic area, the forecast is displayed in the orange area, and the forecast data is indicated by an orange line.
6. [Optional] In the graphic area, you can perform the following. For more information, see Intelligent Forecast Window.
To generate the forecast based on sales records of a different history period, modify the maximum history time
bucket number and choose the Forecast button.
To generate the forecast based on a different calculation method, choose Change and define parameters in the
Customized Forecast window.
After you change the parameters, the row in the Forecast Values area is tagged with an orange triangle, indicating
that the calculation method has been customized.
To customize past data, drag the amount to an adjusted value.
The forecast is updated and the customized data is indicated by a dotted line.
To test the accuracy of the calculation method, drag the arrow next to the orange forecast area.
A blue area appears, displaying both the actual data and forecast data based on past data to the left of the blue
area.
7. [Optional] In the lower right corner, to save the settings in the Configuration area, and the parameters you changed in the
Customized Forecast window, choose Save As A Template.
8. To save data and return to the Forecasts window, in the lower left corner, choose Save and Close.
SAP Business One, version for SAP HANA populates this window with the forecast values.
More Information
Managing Forecasts
Intelligent Forecast Window
Intelligent Forecast Window
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:10 AM
This function is available only if you are using SAP Business One, version for SAP HANA.
Configuration Area Fields
 Note
You may choose the collapse/expand button to display or hide the configuration area.
Select Items By
Filters to be included in the forecast.
You may filter items by Item, preferred Vendor, and Default Warehouse.
Warehouses
Select the checkbox to choose specific warehouses to be included in the forecast. If the checkbox is unselected, only the item's
default warehouse is considered in the forecast. If the item does not have a default warehouse, then the company's default
warehouse is considered in the forecast.
Sales History
Select the historic data source as the calculation basis for the forecast: Sales Order, Delivery, or A/R Invoice.
 Note
Canceled documents and reserved invoices are not considered.
Only sales documents with posting dates within the range of maximum history time buckets are considered.
For deliveries, returns and negative deliveries are also considered.
For A/R invoices, credit memos and negative A/R invoices are also considered.
Calc. Method
In the dropdown list, select the algorithm to be used in the forecast. This method will be used for all the filtered items. To change
the calculation method for specific items in specific warehouses, follow the procedure below:
1. In the Forecast Values area, select the row for the specific item in the specific warehouse.
2. In the graphic area, choose Change and define parameters in the Customized Forecast window.
 Recommendation
Use the automatic selection of calculation methods, which will apply the most suitable method and its parameters based on
the historic data.
For more information about the calculation methods, see the SAP HANA Predictive Analysis Library (PAL) Reference guide at
https://help.sap.com/viewer/p/SAP_HANA_PLATFORM.
Forecast Values Area Fields
Forecast Time Buckets
Displays the number of time buckets you selected in the View dropdown list of the Forecasts window.
Forecast Period
Displays the start date and end date you specified in the Forecasts window.
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:10 AM
Graphic Area Elements
 Note
You may choose the collapse/expand button to display or hide the graphic area.
Maximum History Time Buckets
Displays the maximum number of historic time buckets that are used as the calculation basis for the forecast.
To generate the forecast based on sales records of a different history period, modify the number and choose the Forecast button.
Current Calc. Method
Displays the calculation method used for the row you selected in the Forecast Values area.
To generate the forecast based on a different calculation method, choose Change and define parameters in the Customized
Forecast window. After you change the parameters, the row in the Forecast Values area is tagged with an orange triangle,
indicating that the calculation method has been customized.
The parameters for the calculation methods are as follows:
Triple Exponential Smoothing (TESM):
Automatic Optimization: select Yes to set the optimal parameters.
Alpha, Beta, Gamma: three factors used in the forecast calculation.
Base Cycle: the cycle used for calculation. You can change the cycle according to your own situation. For example, if
your production cycle is six months, you define the base cycle as 6 months, and the forecast will be calculated on a
six-month cycle basis.
Linear Regression with Damped Trend and Seasonal Adjust (LRDTSA):
Trend: damped trend factor. Value range is (0, 1].
For more information about the calculation methods, see the SAP HANA Predictive Analysis Library (PAL) Reference guide at
https://help.sap.com/viewer/p/SAP_HANA_PLATFORM.
Save As A Template
Choose this button to save the settings in the Configuration area, and the parameters you changed in the Customized Forecast
window.
You are authorized to save only the templates that were created by you.
 Note
You cannot use the following characters in a template name:
\ ' - , ; @ # % $ * : < > ? / { | }
Load Template
To load a template, choose this button, select a template, and choose the Forecast button.
To delete templates, choose this button, and delete the templates in the Load Template window.
More Information
Generating an Intelligent Forecast
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:10 AM
Running MRP - Prerequisites, Processes, and Wizard
Prerequisites
You have defined the following settings on the Item Master Data: Planning Data tab. For more information, see Item Master
Data: Planning Data Tab.
Planning Method
Only items with the Planning Method of MRP are available for selection when you are running the MRP wizard.
Procurement Method
The procurement method affects the order type MRP recommends for items with demands.
Order Interval
In MRP calculations, the application automatically groups the recommended orders into interval periods according
to your definition, and arranges orders within the same period into the first working day of that period. For more
information, see Example: Lead Time, Holidays, and Order Interval in MRP.
Order Multiple
Your definition of order multiple may affect the order quantities MRP recommends.
Minimum Order Qty
Your definition of minimum order quantity may affect the order quantities MRP recommends.
Lead time
The lead time definition affects the order recommendation calculation.
For more information, see Example: Lead Time, Holidays, and Order Interval in MRP and Examples: Cumulative Lead
Time.
 Note
You can either run MRP with the planning parameters you defined for each item in the Item Master Data window, or you
can define a set of parameters when running the MRP wizard and apply them to all the selected items in the MRP run.
For more information, see Update Selected Items in MRP Wizard, Step 3: Item Selection.
If necessary, define forecasts and consume forecast settings. For more information, see Managing Forecasts.
Context
The Material Requirements Planning (MRP) function lets you plan material requirements for complex manufacturing and
procurement processes. To create and run MRP scenarios, you use the MRP wizard. The wizard generates recommendations
(production orders, purchase orders, and inventory transfer requests) required to produce or procure the final product on time and
in the required quantity. In the Order Recommendation report, you create production and purchase orders based on these
recommendations.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:10 AM
The MRP Process in SAP Business One
Choose a wizard step, or the examples, from the list below to learn more.
Please note that image maps are not interactive in PDF outputs.
Results
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:10 AM
After completing the MRP wizard run, you need to create purchase and production orders, and possibly inventory transfer
requests, in accordance with the MRP recommendations. For more information, see Generating Orders from Saved
Recommendations.
MRP Wizard, Step 1: Scenario Selection
The MRP Scenario is a set of parameters defined by the user that are applied during the MRP run. You can define several MRP
scenarios for each company, but only one scenario can be used for each MRP run (MRP calculation of recommendations).
You select an existing MRP scenario or add a new scenario.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Select Scenario
Create New Scenario
Creates a new MRP scenario. Specify the scenario name and scenario description.
Scenario Name, Description
Specify a name (no more than 30 characters) and enter a detailed description (no more than 100 characters) for the new scenario.
Select Existing Scenario
Runs a scenario from the table that contains all the existing scenarios. The last-used scenario is selected by default.
 Note
You cannot change the name of the existing scenario, but you can change its description in the MRP Wizard: Scenario Details
window. You can reuse the name if you delete the MRP scenario.
To delete an existing scenario, select the scenario and choose Data Remove .
Start Date, End Date
Time period for the existing MRP scenarios.
Run
Runs the selected MRP scenario and goes directly to the MRP Wizard: MRP Results window. Enabled only when you select an
existing MRP scenario.
MRP Wizard, Step 2: Scenario Details
Specifies necessary parameters for the MRP run planning horizon and displays preferences.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:10 AM
MRP Wizard, Scenario Details
Description
Enter a description for the MRP scenario.
Start Date, End Date
Specify the start date (the first day of the first period) and end date (the last day of the last period) of the MRP planning horizon.
MRP considers all the demands and supplies that have a due date falling within the planning horizon you define.
The date range is automatically adjusted according to the period you define.
 Example
You enter March 4, 2011 as the start date and March 15 as the end date of the planning horizon. Then in the View Data in
Periods Of field, you specify 1 month. SAP Business One changes the two dates automatically to the beginning of the month,
March 1, 2011 and the end of the month, March 31, 2011.
View Data in Periods of
Define the length of each period, displayed in the MRP Results window, in days, weeks, or months, depending on the selected
option. All MRP calculations are displayed in the defined time buckets.
 Note
If you choose to group MRP results into period lengths other than one day, SAP Business One performs the MRP calculation on
the first day of each period. MRP groups all the existing data for that period (supplies and demands) in the first day.
The weekly numbering definition and weekend definition may affect the week numbers and the first day of the week. To
maintain the definitions, choose Administration System Initialization Company Details Accounting Data Holidays
Holiday Dates . For more information, see the Holiday Dates Window.
 Example
You make the following definitions:
View data in periods of:1 week
Weekly numbering: First week starts on January 1
Weekend from Saturday to Sunday.
So the working week starts on Monday and ends on Friday.
Working Week 2 of 2011 starts on 3 January and ends on 7 January. The MRP performs the calculation for the entire week as if
all of the business activity for the week happened on 3 January.
Planning Horizon Length
Displays the number of days/weeks/months of the planning horizon you define. Calculated automatically after you specify the
start date, end date, and period definition.
If you manually change the value of the field, MRP recalculates the value in the End Date field.
Consider Holidays For
Select the checkboxes to let MRP consider the holidays and weekends defined in Holiday Dates Window. SAP Business One
automatically adjusts demands and supplies that fall into defined holidays or weekends. For items that require a certain period of
lead time, considering holidays and weekends increases the lead time interval for MRP calculations. For more information about
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:10 AM
how holidays, lead time, and order interval jointly affect the MRO calculations, see Example: Holidays, Lead Time, and Order
Interval in MRP.
Consider holidays for Production Items: The holidays table is taken into account for items with a Procurement Method of
Make.
Consider holidays for Purchase Items: The holidays table is taken into account for items with a Procurement Method of
Buy.
For more information about the procurement method, see Item Master Data: Planning Data Tab.
SAP Business One adjusts demands and supplies that fall into defined holidays or weekends following the rules stated below:
Supplies
The application moves supplies forward to the first working day after the holiday or weekend.
In an inventory transfer request, the received quantity in a receiving warehouse is regarded as supply.
Demands
The application moves demands backward to the first working day before the holiday or weekend.
In an inventory transfer request, the issued quantity from the issuing warehouse is regarded as demand.
 Example
You have defined Saturday and Sunday as weekend and let SAP Business One consider holidays and weekends in MRP
calculation.
You have a purchase order (supply) on April 2, 2011 (Saturday). The application moves the purchase order to the first
working day after the weekend, April 4, 2011 (Monday).
You have a sales order (demand) on April 2, 2011 (Saturday). The application moves the sales order to the first working
day before the weekend, April 1, 2011 (Friday).
Sort by
Select the sort criteria for the MRP report:
Assembly Sequence: Sorts the report from the highest level to the lowest level of the production Bill of Materials.
For more information, see Example: Sort by Assembly Sequence.
Item Number: Sorts the report by the item number.
Item Description: Sorts the report by the item description.
Item Group: Sorts the report by the item group.
Display Items With No Requirements
Displays the items without actual requirements after the MRP run.
Items without requirements are items that, during the entire MRP horizon, have a sufficient quantity and do not require purchase
orders, production orders, or warehouse transfer requests.
If you do not select this checkbox, MRP items, without requirements or with incoming orders balancing the requirements, are not
displayed.
Simulation
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:10 AM
Defines this scenario as a simulation scenario.
You cannot save recommendations or create production or purchase orders from simulation scenarios.
Save Scenario
Saves the MRP scenario at the current stage.
Available only when you add a new scenario or update an existing one.
 Note
You cannot save an MRP scenario if it is a simulation.
Run
Runs the selected MRP scenario and goes directly to the MRP Wizard: MRP Results window.
Example: Sort by Assembly Sequence
In this example, three product trees are included. The low-level code 0 represents the finished goods, and the low-level codes 1, 2
and 3 represent subassemblies, or raw materials.
Sort by Assembly Sequence Example
Low Level Code BOM 1 BOM 2 BOM 3
0 A F X
1 B E
2 C
3 D
When you select Assembly Sequence in the Sort by field, the sort is carried out according to the low level-code, with the result as
follows: A, F, X, B, E, C, and D.
More Information
MRP Wizard, Step 2: Scenario Details
MRP Wizard, Step 3: Item Selection
Use this window to select items for the MRP run.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Item Selection
All Items
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:10 AM
Includes all items with the Planning Method of MRP in the MRP run. When you select this radio button, the application does not
display selected items in the table below.
 Note
For a parent item of a bill of materials (BOM), all the child items in the BOM chain are included in the MRP run, regardless of
their Planning Method attributes. The only exception is disassembly BOMs, for which the MRP does not calculate child items.
Selected Items
Includes selected items in the MRP run.
To do so, proceed as follows:
1. To select items, choose the Add Items button.
Selected items are then displayed in the table below.
 Note
You can select only those items with a Planning Method of MRP for the MRP run.
If you select a parent item of a bill of materials (BOM), all the child items in the BOM chain are included in the MRP run,
regardless of their Planning Method attributes. The only exception is for disassembly production orders, for which the
MRP does not calculate the child items in the BOM structure.
2. To sort selected items, double-click the grid column headers.
3. To remove an item from the table, right-click the item entry and choose Delete Row.
4. To remove all the items displayed in the table, choose the Remove Items button.
5. By default, the application selects the checkbox for all items you added to the list. You can deselect or select the
checkboxes using the Select/Deselect All button or by manual selection.
 Note
If you have added an item and then deselected it in an MRP run, the next time you run this scenario, you can still see the item
displayed in the table, deselected. This way you can include this item in the MRP run by selecting it.
If you removed this item from an MRP run, the next time you run this scenario, you are not able to view it in the selected items
table. If you want to include it in the MRP run, you have to add it again.
Add Items
Select items to be included in the MRP run.
Choose the button to open the Items List — Selection Criteria window. You can filter items by item number, item group, and item
properties.
If required, select the Expanded Selection criteria checkbox, you can then further filter items by the Preferred Vendor and UDFs
defined in the Item Master Data window.
Remove Items
Removes all the items selected and displayed in the table.
Select/Deselect All
Select or deselect all the items displayed in the table.
Update Selected Items
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:10 AM
Select to open the Items List – Update Selected Items window. In this window, select one of the methods to update the
parameters of the items selected for the MRP run.
Update with Specific Values
Update the item parameters by selecting the checkboxes and specifying new values for the parameters.
Update with Values from Item Master Data
Update the item parameters with the default values defined in the item master data. To update the values, choose the
checkbox to the left of each parameter you want to update.
The following parameters of the items can be updated according to the method you choose:
MRP Procurement method
MRP Component Warehouse
MRP Order Interval
MRP Order Multiple
MRP Minimum order quantity
MRP Lead time
MRP Tolerance Days
The updated value applies to all the items involved in the current scenario and MRP run. Your change here does not affect the item-
specific definition on the Item Master Data: Planning Data Tab.
Save Scenario
Saves the MRP scenario at the current stage.
Available only when you add a new scenario or update an existing one.
 Note
You cannot save an MRP scenario if it is a simulation.
MRP Wizard, Step 4: Inventory Data Source
You define the inventory data source for the MRP run, including storage locations, warehouses, and sources of demand and supply.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Data Source Fields
Run by Company or Warehouse
Choose one of the following:
Run by Company: Consolidate existing inventory, demand, and supply into default warehouse only.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:10 AM
To run the MRP calculations on the company level, select this option. SAP Business One calculates demands and supplies
jointly for all the selected warehouses. To do so, the application sums up all the initial inventory quantities, demands, and
supplies of the selected warehouses, and then consolidates all the quantities into the default warehouse for requirements
calculation.
Run by Warehouse: Include existing inventory, demand, and supply separately for each warehouse.
To run the MRP calculations on the warehouse level, select this option. SAP Business One calculates requirements
separately for each warehouse.
By default, the application selects the three checkboxes (Include Existing Inventory, Include Demand, and Include Supply) in the
grid for all warehouses except non nettable warehouses. You may manually select the non nettable warehouses if necessary.
Your definition here may affect MRP calculations for inventory level and demands raised by inventory level requirements. For more
information, see Inventory Level in MRP Wizard, Step 5: Documents Data Source.
Include Existing Inventory
To consider the existing inventory quantities of this warehouse in MRP calculation, select this checkbox.
Include Demand
To consider all sources of demand from this warehouse, including requirements from the inventory level in the MRP calculation,
select the checkbox.
 Note
Supplies with negative quantities are regarded as demands. For example, a purchase order is typically a source of
supply. However, if the purchase order has a line with a negative quantity, then this line is included as a demand.
If you deselect the checkbox, the MRP does not consider inventory level requirements for this warehouse, regardless of
your inventory level definition in MRP Wizard, Step 5: Documents Data Source.
If you deselect the checkbox, and there are items in this warehouse that happen to be child items in a bill of materials
(BOM), the planning for the parent item of the BOM may encounter problems because the demands for child items
(from parent items in the BOM) are not included in the MRP run.
In such a case, you receive a message stating that recommendations are not generated for this parent item due to
components defined in the BOM structure whose demand is not included in this MRP run. You can change your settings
for inventory date source and run the MRP again.
Include Supply
To consider all sources of supply in the MRP calculation, select the checkbox.
 Note
Demands with negative quantities are regarded as supplies. For example, a sales order is typically a source of demand.
However, if the sales order has a line with a negative quantity, then this line is included as supply.
Location
Shows the location of the warehouse.
Expand
Switches to the expanded view to display warehouses under each location. By default the warehouse list is expanded.
Collapse
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:10 AM
Switches to the compact view to display only warehouse locations.
Save Scenario
Saves the MRP scenario at the current stage.
Available only when you add a new scenario or update an existing one.
 Note
You cannot save an MRP scenario if it is a simulation.
MRP Wizard, Step 5: Documents Data Source
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Documents Data Source Fields
Time Range
Defines a time range for data to be included in the MRP calculation.
Within Planning Horizon
Only documents within the Start Date and End Date range (as defined in MRP Wizard, Step 2: Scenario Details) are
considered in MRP calculations and displayed with recommendations.
The application displays supplies and demands before the Start Date but does not include them in the calculation;
therefore, there are no recommendations for the demands before the Start Date.
Past due data is summed together with recommendations for the system date column.
Include Historical Data
All demands and supplies before the Start Date are considered in MRP calculations. Recommendations are summed
together and displayed in the system date column.
The Historic Data field in the MRP report is visible only after you have selected the Include Historical Data option in this
step.
Sources of Demand and Supply to Be Included in MRP Calculation
To include document sources in the MRP calculation, select corresponding checkboxes for the document type.
Purchase Requests
When you select the checkbox, in the MRP report, SAP Business One displays open purchase requests as supplies.
To include only selected purchase requests, select the Restrict Purchase Requests checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
Purchase Quotations
When you select the checkbox, in the MRP report, SAP Business One displays open purchase quotations as supplies.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:10 AM
To include only selected purchase quotations, select the Restrict Purchase Quotations checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
Purchase Orders
When you select the checkbox, in the MRP report, SAP Business One displays open purchase orders as supplies.
To include only selected purchase orders, select the Restrict Purchase Orders checkbox. For more information, see the
Documents Restrictions section at the end of the field help for Sources of Demand and Supply to Be Included in MRP
Calculation.
Blanket Purchase Agreements
When you select the checkbox, in the MRP report, SAP Business One displays blanket purchase agreements with the status
of Approved as supplies. The blanket agreements with a vendor code are considered as a blanket purchase agreement.
To include only selected purchase agreements, select the Restrict Purchase Agreements checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
 Note
MRP considers only the blanket agreements of type Specific.
Sales Quotations
When you select the checkbox, in the MRP report, SAP Business One displays open sales quotations as demands.
To include only selected sales quotations, select the Restrict Sales Quotations checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
Sales Orders
When you select the checkbox, in the MRP report, SAP Business One displays open sales orders as demands.
To include only selected sales orders, select the Restrict Sales Orders checkbox. For more information, see the Documents
Restrictions section at the end of the field help for Sources of Demand and Supply to Be Included in MRP Calculation.
Blanket Sales Agreements
When you select the checkbox, in the MRP report, SAP Business One displays blanket sales agreements with the status of
Approved as demands. The blanket agreements with a customer code are considered as a blanket sales agreement.
To include only selected sales agreements, select the Restrict Sales Agreements checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
 Note
MRP considers only the blanket agreements of type Specific.
Production Orders
To include only selected production orders, select the Restrict Production Orders checkbox. For more information, see the
Documents Restrictions section at the end of the field help for Sources of Demand and Supply to Be Included in MRP
Calculation.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:10 AM
MRP calculation considers only production orders with the Status Planned or Released. Completed production orders
are not relevant for calculation, because they have already impacted the inventory.
For Standard production orders, in the MRP report, the application displays the parent items as demands and the
child items as supplies.
For Disassembly production orders, in the MRP report, the application displays the parent items as supplies and the
child items as demands.
Inventory Transfer Requests
For the issuing warehouse, SAP Business One displays the requested quantities as demands.
For the receiving warehouse, SAP Business One displays the requested quantities as supplies.
To include only selected transfer requests, select the Restrict Transfer Requests checkbox to define the required
documents. For more information, see the Documents Restrictions section at the end of the field help for Sources of
Demand and Supply to Be Included in MRP Calculation.
 Note
The MRP cannot recommend inventory transfer requests for scenarios where you choose to run by company. The MRP
considers all the demands and supplies jointly for the whole company as one warehouse, and it does not make sense to
transfer inventory within one warehouse. For more information, see MRP Wizard, Step 4: Inventory Data Source.
Recurring Order Transactions
When you select this checkbox, SAP Business One considers recurring transactions that have been scheduled for sales and
purchase order documents.
 Note
The MRP includes a recurring order transaction only when it contains the following data:
A quantity per item line
A warehouse per item line
A Next Execution Date
For more information, see Managing Recurring Transactions.
Reserve Invoices
When you select this checkbox, SAP Business One considers open reserve invoices and open correction invoices for
reserve invoices in the MRP calculation.
For A/R reserve invoices and correction invoices, the application displays them as demands.
For A/P reserve invoices and correction invoices, the application displays them as supplies.
To include only selected reserve invoices, select the Restrict Reserve Invoices checkbox. For more information, see the
Documents Restrictions section at the end of the field help for Sources of Demand and Supply to Be Included in MRP
Calculation.
Documents Restrictions
Select the Restrict <Document Names> checkboxes to include only selected documents in the MRP calculation. To do so,
proceed as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:10 AM
1. For a specific document type, select the document restriction checkbox. For example, for sales orders, select the
Restrict Sales Orders checkbox.
2. In the Selected Documents window, to filter documents, choose the Add Documents button.
3. In the Add Documents window, use the selection criteria to specify documents to be added.
For purchase orders and sales orders, to include only orders with the Status of Approved, select Approved Orders
Only.
For production orders, to include only orders with the Status of Released, select Released Orders Only.
4. Choose OK to close the window and return to the Selected Documents window. The window displays all the
documents you added.
5. To exclude one or more records from the MRP calculation, deselect the Selected checkbox and choose OK.
The record remains in the window, but is not included in the MRP calculation.
6. To delete a record from the window, right-click the relevant row and select Delete Row.
7. To delete all the records from the window, choose the Clear All Documents button.
Inventory Level
Uses the specified inventory level as a demand in MRP calculation, to ensure that the required inventory level is available for
unexpected orders. Not to consider inventory level requirements in the calculation, leave this field blank.
Required - Replenish items up to the required inventory level.
Minimum - Replenish items up to the minimum inventory level.
Maximum - Replenish items up to the maximum inventory level.
Minimum - Maximum - Replenish items up to the maximum inventory level only when it falls below the minimum inventory
level.
 Note
To maintain an item's inventory level values (both company level and warehouse level), see Item Master Data: Inventory Data
Tab.
When you are running MRP by company (see MRP Wizard, Step 4: Inventory Data Source), the application consolidates the
inventory level requirements as one demand for the default warehouse.
On the Inventory Data tab of the Item Master Data window, if you have selected the Manage Inventory by
Warehouse checkbox for an item, the application sums up the inventory level values of all warehouses (Min.
Inventory, Max. Inventory, Req. Inventory, and Min. - Max. Inventory) for which Include Demand is selected in step
4.
On the Inventory Data tab of the Item Master Data window, if you have deselected the Manage Inventory by
Warehouse checkbox for an item, the application takes the defined company inventory level values (Required,
Minimum, Maximum, and Min. - Max.) as a demand for all warehouses together.
When you are running MRP by warehouse (see MRP Wizard, Step 4: Inventory Data Source), the application considers
inventory level requirements separately for each relevant warehouse.
On the Inventory Data tab of the Item Master Data window, if you have selected the Manage Inventory by
Warehouse checkbox for an item, and in the MRP wizard step 4 you have selected the Include Demand checkbox for
one or more warehouses, the application takes the defined warehouse inventory level values (Min. Inventory, Max.
Inventory, Req. Inventory, and Min. - Max. Inventory) separately as relevant for the warehouses.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:10 AM
On the Inventory Data tab of the Item Master Data window, if you have deselected the Manage Inventory by
Warehouse checkbox for an item, the application takes the company inventory level values (Required, Minimum,
and Maximum, and Min.- Max.) you defined respectively for each warehouse for which you have selected the
Include Demand checkbox.
Forecast
Use this field to decide whether to consider forecast data in MRP calculations.
If you do not want to consider forecast data in MRP calculations, leave the field blank.
If you want to consider forecast data in MRP calculations:
To consider data of only one forecast in the MRP calculation, in the dropdown list, choose one forecast, or choose
Define New to define a new forecast.
To consider data of multiple forecasts in the MRP calculation, in the dropdown list, choose Multiple Forecasts. When
the Selected Documents - Forecast window appears, select the forecasts you want to consider in this window.
If you have defined sales orders and blanket sales agreements to consume forecast, in the MRP calculation, the forecasted
amount, minus the amount consumed by sales orders and blanket sales agreements, is regarded as demands.
To configure the forecast consumption settings for open sales orders, choose Administration System Initialization
General Settings Inventory Planning tab. For more information, see General Settings: Inventory Tab.
To configure the forecast consumption settings for blanket sales agreements, in the Blanket Agreement Item Details
window, use the Consume Forecast checkbox to determine whether to use this item to consume a forecast when it is
involved in a blanket agreement.
When you choose to consider a forecast in the MRP calculation, the application assigns a warehouse to the demands from the
forecast according to the following rules:
If you select only one warehouse in step 4, the application links the demands from the forecast to this warehouse.
If you select more than one warehouse in step 4, and the default warehouse is one of them, the application links the
forecast to the default warehouse.
If you select more than one warehouse in step 4, and the default warehouse is not one of them, the application links the
forecast to the first warehouse code in ascending order.
 Note
The consumption of forecasted amount by sales orders and blanket sales agreements is irrespective of the warehouse of the
sales orders or the blanket sales agreements.
Recommendations
Defines the document types recommended after the MRP wizard calculates the results. Purchase orders and production orders
are mandatory recommended document types. You can define whether to recommend inventory transfer requests when you are
running the MRP by warehouse.
Purchase Orders
 Note
This checkbox is read-only and by default selected.
Items with the Procurement Method of Buy are recommended with purchase orders.
In step 4, if you have selected Run by Warehouse, you have the following warehouse options:
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:10 AM
To generate purchase orders to the default warehouse of the item, select Generate to Default Warehouse.
For more information about the default warehouse, see Item Master Data: Inventory Data Tab.
 Note
When you have not included the default warehouse to the MRP run in step 4, the recommendation still goes to
the default warehouse if you select this checkbox.
When there is no default warehouse defined for the item, the recommendation goes to the first warehouse
(sorted according to warehouse code) in the selection grid in step 4 for which the Include Demand checkbox has
been selected.
To generate purchase orders to the warehouse that demands inventory supplies, select Generate to Warehouse
with the Demand.
Production Orders
 Note
This checkbox is read-only and by default selected.
Items with the Procurement Method of Make are recommended with production orders. The application recommends the
production orders to the warehouse as defined in the production BOM.
Inventory Transfer Request
 Note
You can include inventory transfer request as one of the recommendation types only when you are running the MRP by
warehouse.
When you select this checkbox, the application recommends inventory transfer requests before recommending purchase
orders and production orders. Warehouses in the same Location have higher priorities. The application automatically
chooses the warehouse with the highest available inventory level as the sending warehouse.
If you have chosen to consider the Minimum and Required Inventory Level for warehouses, the application makes sure that
after the inventory transfer recommendation, the inventory level of the sending warehouse does not fall below the inventory
level you set. For the inventory level calculation algorithm, see the field explanation above for the Inventory Level.
Save Scenario
Saves the MRP scenario at the current stage.
Available only when you add a new scenario or update an existing one.
 Note
You cannot save an MRP scenario if it is a simulation.
MRP Wizard, Step 6: MRP Results
The MRP Results window appears after you run the MRP wizard and displays the results of the MRP run. You can view the schedule
for the MRP demands on the Report tab, and view the outcome – the recommendations that assemble the demands – on the
Recommendations tab.
The outcome of the wizard is a list of the recommendations for production orders, purchase orders, and inventory transfer
requests (if you have defined inventory transfer request as a source for recommendations). To issue actual orders, from the saved
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:10 AM
recommendations for a given scenario, you must use the order recommendation function (see Creating Order
Recommendations).
General Area
Planning Horizon
Displays the Start Date and End Date of the current MRP scenario. For more information, see the Planning Horizon explanation in
MRP Wizard, Step 2: Scenario Details.
Calculated At
Displays the date and time at which you ran the MRP report.
Find Item No.
Enter the code of the item you want to locate in the MRP report. The application then scrolls the report to the row where this item
code appears.
The field is case-sensitive.
Finish
Exits the wizard.
If the recommendation is not saved, MRP displays a warning message.
Report Tab
Use the Report tab to view the plan the MRP wizard scheduled to satisfy your inventory demands during the defined period.
The table displays MRP data in columns representing data periods according to your View Data in Periods of settings in MRP
Wizard, Step 2: Scenario Details.
The item row displays recommended quantities. You can view detailed information about initial inventory, supply, demand, and
final inventory in the expanded view. To view detailed information of the recommendations, click a cell displaying an amount, and
the Pegging Information Window appears.
If you defined more than one day/week/month in the View Data in Periods of field, the title of each column displays the first
day/week/month of the period in the chosen format, and the data of each column represents the sum data of the specified period
of time.
Preview MRP Run Results
Select the checkbox to display data after the MRP run, including the effect of implementing the newly recommended quantities. If
you deselect the checkbox, the results show the pre-MRP run situation, without calculating the newly planned quantities.
Filter Possible Problem Items
Select the checkbox to display only "problem items" – recommendations in red. Problem items are those for which demand
cannot be met, potentially because:
The final inventory of the item in the chosen MRP period is negative, including the Historic Data, Past Due Data, regular
period or Future Data fields.
The required quantity cannot be ordered in time because of lead times.
Historic Data
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:10 AM
Displays a consolidated value summing all the data before the Start Date of the planning horizon you defined in MRP Wizard, Step
2: Scenario Details.
This column is visible only when you have selected the Include Historic Data radio button in MRP Wizard, Step 5: Documents Data
Source.
Past Due Data
Displays a consolidated value summing up all the data that falls into the past due period.
The past due period starts from the Start Date of the planning horizon and ends with the current system date (not including the
current date). Therefore, when the Start Date is later than the current system date, there is no past due period and this column is
invisible from this window.
Future Data
Displays a consolidated value summing up all the data that falls into the future period.
The future period is the lead time period that starts right after the End Date of the planning horizon. The future period of each item
may vary because of different definitions for lead time.
 Example
You define a 10-day lead time for item A; therefore, the future data column presents the data of this item for the 10 days after
the planning horizon ends.
For more information about how the MRP handles the demands from future data, see Examples: BOMs and Future Data in MRP
Planning.
Expand/Collapse
Switches between the expanded view and the collapsed view.
By default, the report displays the collapsed view. You can observe the recommended quantities displayed in periods after
the Item No. and Item Description columns.
When you switch to the expanded view, you are able to view the detailed information of the item, including Initial Inventory,
Supply, Demand, and Final Inventory.
Save Recommendations
Saves the MRP recommendations in the Order Recommendation report. Recommendations are saved for each scenario.
 Note
You can view the following fields only when you switch to the expanded view using the Expand/Collapse button.
Initial Inventory
Initial quantity of the item in inventory, for each period. This quantity is based on the existing inventory of the current date. For
other periods, initial inventory derives from the final inventory of the previous period.
Supply
Displays the expected positive item inventory entries: purchase orders, production orders (parent item), A/P reserve invoices,
blanket purchase agreements, and recurring purchase transactions
To see a detailed list of data sources in the Pegging Information Window, click a cell containing a value in the Supply row.
For more information, see Pegging Information Window.
Demand
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:10 AM
Expected inventory releases of the following items for the defined period: sales orders, forecasts, production orders (child items),
A/R reserve invoices, blanket sales agreements, recurring sales transactions, and MRP-dependent requirements.
To see a detailed list of data sources in the Pegging Information Window, click a cell containing a value in the Demand row.
For more information, see Pegging Information Window.
Final Inventory
When you select the Preview MRP Run Results checkbox, this row displays the quantity remaining in inventory after MRP
recommendations were issued.
When you deselect the Preview MRP Run Results checkbox, this row displays final quantity calculated according to Initial
Inventory, Supply, and Demand only.
Recommendations Tab
This tab displays a list of the recommended documents you should issue according to the MRP calculation. The values in the
window are informative only.
To make changes to the recommended documents, or to issue actual orders and inventory transfer requests, in the Order
Recommendations window, locate the saved recommendations list and perform the necessary operations. For more information,
see Order Recommendation.
Order Type
Displays the type of this recommendation document. It can be Purchase Order, Production Order, or Inventory Transfer Request.
UoM Code, UoM Name
Unit of measurement (UoM) for purchase order recommendations and production order recommendations:
Purchase items: Purchasing UoM defined in the Item Master Data window, Purchasing Data tab
You can manually change this default UoM to any purchasing UoM before generating the recommendation.
Production items: Inventory UoM defined in the Item Master Data window, Inventory Data tab
Transferred items: Inventory UoM defined in the Item Master Data window, Inventory Data tab
Release Date
Date on which each recommended document should be released to meet its due date, depending on the lead time of the item;
cannot be earlier than today.
Due Date
Suggested delivery date for the recommended quantities. If the recommended order or inventory transfer request cannot be
fulfilled to satisfy the demand, the due date appears in red.
 Example
Today is July 15, 2008.
The child item's procurement method is Buy and it has a lead time of 3 days.
The purchase order’s due date is July 16, 2008. This date is in the future, but the due date is still red, since there is not enough
time to receive the order. The child item's lead time is July 13, 2008, 3 days prior to the due date, that is, in the past.
Vendor Code
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:10 AM
Displays the preferred vendor code of the item defined in the Preferred Vendor field in Item Master Data, Purchasing Data tab. It
is recommended only for purchase orders.
Price Mode
Appears only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Display the price mode of the preferred vendor. If there is no defined preferred vendor, SAP Business One automatically displays
Net in this field.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Price
Displays the price from the price list linked to the preferred vendor. If special prices are defined for the linked preferred vendor,
these are displayed instead (according to the standard behavior of prices in SAP Business One).
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab, the unit price displayed here agrees with the mode you have defined in the Price
Mode field.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
Discount
Displays the discount defined for the item's price list.
Price After Discount
Displays the price from the price list for the MRP recommendation.
 Note
This field is relevant only for purchase order recommendations.
From Whse
Displays the warehouse that issues the inventory in an inventory transfer.
 Note
This field is relevant only for inventory transfer requests.
To Whse
Displays the warehouse that receives the procured quantity.
For production order recommendations, the application displays the warehouse defined in Bill of Materials for this parent
item.
For purchase order recommendations, the application displays the warehouse according to your warehouse definition in
MRP Wizard, Step 5: Documents Data Source.
If you select Generate to Default Warehouse for Item, the application displays the item's default warehouse as
defined in the item master data.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:10 AM
If you select Generate to Warehouse with the Demand, the application displays the warehouse that has the
demand to procure this item.
For inventory transfer request recommendations, the application displays the receiving warehouse in the inventory transfer.
Total
Total amount for each item. The amount equals the item's Quantity * Price After Discount.
Exception
Displays the Past Due message for items with a due date in the past.
Save Recommendations
Saves the MRP recommendations in the Order Recommendation report. Recommendations are saved for each scenario.
Cell Color in MRP Results Window
The table below explains the colors (background and font colors) and their indications on the MRP Report and Recommendation
tabs:
Background Color
Color Description Example
White Indicates that there are more supplies
than demands. Therefore, the final
inventory is greater than zero and the
item's quantity is sufficient and there is
no need to issue recommendations.
 Note
The white color is only for the
item line. If you are in the
expanded view, the detail lines
for the item are not displayed
in white.
Historic data and Past Due
Data columns are always
displayed in dark gray.
Light Grey Indicates one of the following:
Today is July 1, 2011.
No data for this item in the given
A production order for a certain
period.
parent item is due on July 20,
The item has a supply or 2011.
recommendation that can be
The lead time of the item is 5
received in time to satisfy the
days.
demand. In this case, the
quantity appears in black. The order for the child items should be
issued on July 15, 2011. This is a future
date, so there is sufficient time to
complete the production.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:10 AM
| Color     | Description                               | Example |
| --------- | ----------------------------------------- | ------- |
| Dark Grey | Indicates that a sufficient supply cannot |         |
Today is July 14, 2011.
be received to satisfy the demand in
|     | time. | A production order is |
| --- | ----- | --------------------- |
recommended for a certain
In this case, the recommendation and
|     | supply quantity appear in red, indicating | parent item with the due date of |
| --- | ----------------------------------------- | -------------------------------- |
July 16, 2011.
that though the recommendation for this
item is issued anyway, the
The lead time of this production
|     | recommendation cannot be completed | BOM is 3 days. |
| --- | ---------------------------------- | -------------- |
to provide sufficient inventory before the
To complete the order by the due date,
due date. The application also marks the
|     | Due Date field for this kind of   | the child items should have been issued  |
| --- | --------------------------------- | ---------------------------------------- |
|     | recommendation in red (for the    | on July 13. However, this date is in the |
|     | Recommendations tab of MRP wizard | past. Therefore, the process cannot be   |
completed on time and the cell is dark
step 6, the Order Recommendations
|     | window, and the Pegging Information | grey. |
| --- | ----------------------------------- | ----- |
window).
Font Color
| Color | Description | Example |
| ----- | ----------- | ------- |
| Black |             |         |
In the item line, values in black
indicate the recommended
quantity for this item can be
received in time to satisfy the
demand.
In the expanded detail lines, all
positive values are displayed in
black.
| Red |     |     |
| --- | --- | --- |
In the item line, values in red
indicate the recommended
quantity for this item cannot be
received before the due date to
satisfy the demand in time.
In the expanded detail lines, all
negative values are displayed in
red.
When you are viewing the MRP
data in periods of 1 day, which
means you are viewing the MRP
schedule per day, the header
area displays a date in red to
indicate that this day is a holiday
you defined in the holiday table.
For more information, see
Holiday Dates Window.
On the Recommendation tab, if
the recommendation cannot be
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:10 AM
Color Description Example
received before the Due Date, the
Due Date appears in red.
Pegging Information Window
Use the Pegging Information window to view the detailed data sources of recommendations, supplies, and demands.
To open this window, on the Report tab of the MRP Results window, click a cell displaying the value of recommendations, supplies,
or demands.
 Note
For demands of an item that is an assembly BOM, sales BOM, or a phantom item, the MRP issues no actual recommendations
for the parent item.
Source
No. of the document. To open the document, choose .
Type
Displays one of the following document types:
For recommendations:
Purchase Order
Production Order
Inventory Transfer Request
For supplies:
Production Order (for parent items)
Purchase Order
A/P Reserve Invoice
Blanket Purchase Agreement
Recurring Purchase Transaction
Inventory Transfer Request
MRP Recommendation
For demands:
Sales Order
Forecast
Production Order (for child items)
A/R Reserve Invoice
Blanket Sales Agreement
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:10 AM
Recurring Sales Transaction
Inventory Transfer Request
MRP–dependent Requirement (for child items)
Due Date
Displays the due date of the corresponding document.
The due date is the demand date for the current period. If the document source is from an MRP-dependent requirement (demands
for child items in a BOM to produce a certain parent item), the calculated due date of the parent item is displayed.
 Note
For recommendations initially scheduled on holiday days and then moved to work days, the pegging information for the
recommendation shows the original recommendation date which is a holiday date and marks the due date in red.
Quantity
For recommendations: displays the recommended quantity for the item.
For supplies: displays the open quantity of the item from the production order or the purchase order
For demands: displays the open quantity of the item from sales orders and planned quantity from production orders.
For a forecast, the field displays the quantity that was not consumed by sales orders or blanket agreements.
More Information
MRP Wizard, Step 6: MRP Results
Examples of Working with MRP
Choose from the various examples of working with MRP to learn more.
Please note that image maps are not interactive in PDF outputs.
Example: Cumulative Lead Time Calculations
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:10 AM
The following example explains how to calculate cumulative lead time for a parent item in a bill of materials (BOM) structure.
Parent items can consist of components, other BOMs, and phantom items, which in turn can consist of further components.
Standard/Special Production Order for a Production BOM
The following list presents a production BOM structure.
Parent item PBOM1 (Production BOM; Lead Time: 1 Day) consists of the following:
C1 (Component; Lead Time: 1 Day)
ABOM2 (Assembly BOM; Lead Time: 2 Days)
C4 (Component; Lead Time: 4 Days)
P1 (Phantom Item, Lead Time: 1 Day)
C5 (Component; Lead Time: 5 Days)
PBOM3 (Production BOM, Lead Time: 3 Days)
C6 (Component; Lead Time: 6 Days)
SBOM4 (Sales BOM, Lead Time: 4 Days)
C7 (Component; Lead Time: 7 Days)
The MRP does not consider the lead time for actual assembly BOMs, sales BOMs, and phantom items. Therefore, in this example,
the lead time for ABOM2, SBOM4, and P1 are not included in the calculations. However, the components of assembly BOMs, sales
BOMs, and phantom items can have lead times.
The table below demonstrates how the lead time is calculated based on the BOM structure. "OR" stands for "Order
Recommendation," which refers to a planned suggestion to initiate a production or purchase order. Such recommendations are
scheduled based on each item's lead time.
  July 1 July 2 July 3 July 4 July 5 July 6 July 7 July 8 July 9 July 10 July 11
| PBOM1   |     |     |     |     | OR Requirement |
| ------- | --- | --- | --- | --- | -------------- |
from sales
order
| C1      |      |      |      |   OR |     |
| ------- | ---- | ---- | ---- | ---- | --- |
| ABOM2   |      |      |      |      |     |
| C4      |      |      | OR   |      |     |
| P1      |      |      |      |      |     |
| C5      |      |   OR |      |      |     |
| PBOM3   |      |      |   OR |      |     |
| C6 OR   |      |      |      |      |     |
| SBOM4   |      |      |      |      |     |
| C7      |   OR |      |      |      |     |
The cumulative lead time for PBOM1 is 10 days in total. In the schedule above, the lead time is from July 1 to July 10.
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:10 AM
Example: Holidays, Lead Time, and Order Interval in MRP
Calculations
This example presents how MRP calculates supplies and demands considering holidays, lead time, and order intervals. You can use
the example to understand how the three factors jointly affect the MRP calculation.
The following table shows an item's inventory demands. The planning settings are as follows:
Planning horizon: July 29 to August 5.
Lead time: three days.
Order Interval: start on each Monday. In this example, August 3 is Monday.
Holidays:
August 1 and 2 are the weekend, and August 3 is a public holiday.
You select the Consider Holiday checkbox in the MRP wizard.
You deselect the Set Weekends as Work Days checkbox in the Holiday Dates window.
In the table below, holiday dates are marked in boldface.
1. Identify the inventory demands as shown in the table below.
| Date    | 7.29 7.30 | 7.31 | 8.1 8.2 | 8.3 8.4 | 8.5 8.6  | 8.7      | 8.8      |
| ------- | --------- | ---- | ------- | ------- | -------- | -------- | -------- |
|         |           |      |         |         | (Future) | (Future) | (Future) |
| Demands |           |      | D1 D2   | D3 D4   | D5 D6    | D7       | D8       |
2. Adjust backwards those demands that fall on holiday dates. For more information about how MRP adjusts supplies and
demands for holidays, see MRP Wizard, Step 2: Scenario Details.
| Date    | 7.29 7.30 | 7.31     | 8.1 8.2 | 8.3 8.4 | 8.5 8.6  | 8.7      | 8.8      |
| ------- | --------- | -------- | ------- | ------- | -------- | -------- | -------- |
|         |           |          |         |         | (Future) | (Future) | (Future) |
| Demands |           | D1+D2+D3 |         |   D4    | D5 D6    | D7       | D8       |
3. Create initial order recommendations for demands based on the lead time definition.

 Note
When considering holidays in MRP calculations, lead time and order interval settings are both considered in work days.
In this case, the MRP recommends orders two work days prior to the due date.
For demands D1, D2, and D3, the MRP cannot fulfill the three-day lead time requirement, for the MRP cannot make any
recommendation before the start of the planning horizon. For demands D4, D5, and D6, the MRP moves them three work
days prior to the due date, skipping defined holidays, August 1 to 3. Therefore, the MRP schedules the recommendation for
these demands to the earliest possible date within the planning horizon, and that is July 29.
| Date | 7.29 | 7.30 | 7.31 8.1 | 8.2 8.3 8.4 | 8.5 8.6  | 8.7      | 8.8      |
| ---- | ---- | ---- | -------- | ----------- | -------- | -------- | -------- |
|      |      |      |          |             | (Future) | (Future) | (Future) |
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:10 AM
Initial IR1 IR2 IR3 IR4 IR5
Recommendations (D1+D2+D3+D4) (D5) (D6) (D7) (D8)
(IR)
4. Group demands to the first work day of each order interval period.
According to the order interval setting, each Monday is the beginning day of the weekly order interval. This planning horizon
covers two order intervals:
First interval date: July 27, Monday (Not included in the planning horizon)
Second interval date: August 3, Monday (Public holiday)
 Note
For weekly intervals and monthly intervals, if the first interval date is not covered in the planning horizon, the application
does NOT group the recommended quantities for the first interval. From the second interval on, the application groups
the recommended quantities to the interval date, and if it runs into holidays, moves the recommendations later to the
closest work date.
In this example, as shown in the table below, the application does NOT group the recommended quantities for the first
interval. The second interval starts on Monday, but August 3 happens to be a holiday; therefore, the application moves the
grouped recommended quantities later to the closest work day, and that is August 4.
In this example, the MRP finally creates four order recommendations:
July 29: Order recommendation OR1
 Note
Since the MRP cannot satisfy demands D1, D2, and D3 on time due to insufficient lead times, on the MRP Results
tab, the order recommendation R1 appears in red.
July 30: Order recommendation OR2
July 31: Order recommendation OR3
August 4: Order recommendation OR4
The table below shows how MRP groups the recommended quantities according to the order interval:
Date 7.29 7.30 7.31 8.1 8.2 8.3 8.4 8.5 8.6 8.7 8.8
(Future) (Future) (Future)
Order OR1 OR2 OR3 OR4
Recommendations (IR1) (IR2) (IR3) (IR4+IR5)
(OR)
5. If you select to group orders by Every X Days, the interval starts on the very first day when recommendations are needed. If
you select to group orders by every two days, the calculation goes as follows:
The planning horizon contains three order intervals:
July 29: the first day when recommendations are needed and thus the first order interval date
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:10 AM
If you choose to group order recommendations Every X Days, the first order interval date is the first day within
the planning horizon when there are recommendations required. Therefore, if there is no recommendation
needed on July 29 in this example, the first interval starts on the next work day with recommendations.
July 31: the second order interval, two work days after the first interval
August 5: the third order interval, two work days after the second interval
The table below shows how the MRP creates order recommendations if you use two-day order intervals.
Date 7.29 7.30 7.31 8.1 8.2 8.3 8.4 8.5 8.6 8.7 8.8
(Future) (Future) (Future)
Order OR1 OR2 OR3
Recommendations (IR1+IR2) (IR3+IR4) (IR5)
(OR)
Example: BOMs and Future Data in MRP Planning
Example 1
When inspecting parent item demands in a future period that is beyond the planning horizon, the MRP takes these demands into
consideration to calculate order recommendations for the child items involved. However, in the final result, the MRP generates only
order recommendations within the planning horizon. The example below demonstrates this scenario.
A parent item, PBOM1, is made from three child items: C1, PBOM2, and C3. PBOM2 is made from an assembly BOM, ABOM1, which
is assembled from child item C2 – as per the bullet structure below:
PBOM1 (Production BOM; Lead Time: 1 Day)
C1 (Lead time: 1 Day)
PBOM2 (Production BOM; Lead Time: 2 Days)
ABOM1 (Assembly BOM; Lead Time: Not Relevant)
C2 (Lead Time: 2 Days)
C3 (Lead Time: 3 Days)
The planning horizon for this MRP run is from October 22 to October 26, and there is a sales order requirement for PBOM1 due on
October 30. The following table shows the demands schedule after calculating the lead time in MRP.
 Note
In the tables below, OR is short for order recommendation.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:10 AM
|       | 10.22 | 10.23 | 10.24 | 10.25 | 10.26 | 10.27    | 10.28    | 10.29    | 10.30       |
| ----- | ----- | ----- | ----- | ----- | ----- | -------- | -------- | -------- | ----------- |
|       |       |       |       |       |       | (Future) | (Future) | (Future) | (Future)    |
| PBOM1 |       |       |       |       |       |          |          | OR       | Requirement |
from sales
order
| C1    |     |     |     |     |     |     | OR  |     |     |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| C3    |     |     |     |     | OR  |     |     |     |     |
| PBOM2 |     |     |     |     |     | OR  |     |     |     |
ABOM1
| C2  |     |     |     | OR  |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
The MRP generates only order recommendations that fall within the planning horizon. Therefore, in this case, the MRP generates
order recommendations for C2 on October 25 and C3 on October 26, and ignores recommendations for other items in the BOM
chain.
Example 2
When the MRP cannot create order recommendations in time to satisfy the demands due to the lead time required, the MRP
adjusts the order recommendation to the earliest and possible date within the planning horizon. The following example
demonstrates this scenario.
A parent item, PBOM1, is made of three child items: C1, PBOM2, and C3. PBOM2 is made from an assembly BOM, ABOM1, which is
assembled from child item C2 – as per the bullet structure below:
PBOM1 (Production BOM; Lead Time: 5 Days)
C1 (Lead time: 1 Days)
PBOM2 (Production BOM; Lead Time: 2 Days)
ABOM1 (Assembly BOM; Lead Time: Not Relevant,)
C2 (Lead Time: 2 Days)
C3 (Lead Time: 3 Days)
The planning horizon for this MRP run is from October 22 to October 26, and there is a sales order requirement for PBOM1 due on
October 30. The following table shows the demands schedule after calculating the lead time in MRP.
  10.21 10.22 10.23 10.24 10.25 10.26 10.27 10.28 10.29 10.30
|     | (Past) | Current |     |     |     | (Future) | (Future) | (Future) | (Future) |
| --- | ------ | ------- | --- | --- | --- | -------- | -------- | -------- | -------- |
System
Date
| PBOM1 |     |     |     | OR  |     |     |     |     | Requirement |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- | ----------- |
from sales
order
| C1  |     |     |   OR |     |     |     |     |     |     |
| --- | --- | --- | ---- | --- | --- | --- | --- | --- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:10 AM
10.21 10.22 10.23 10.24 10.25 10.26 10.27 10.28 10.29 10.30
(Past) Current (Future) (Future) (Future) (Future)
System
Date
C3 OR
PBOM2 OR
ABOM1
C2 OR
We can observe that the recommendation for C2 is on October 21, a day before the current system date. The MRP cannot generate
order recommendations in the past; therefore, the MRP moves the schedule to the earliest possible future time, and that is
October 22.
After the MRP delays the recommendation for C2, the entire planning schedule has to be moved to one day later to satisfy the lead
time requirements. In this case, PBOM1, the item on the top level of this BOM chain, is finally recommended on October 26. Since
PBOM1 requires a lead time of 5 days, the supply of this item is on October 31, which is one day late for the due date of the sales
order.
Example: Order Recommendations
The following example demonstrates how the MRP handles receipts from recommendations and demands from the future period
in order recommendation planning.
This scenario describes the calculation process for an item in a single warehouse. The following planning parameters are used:
Planning horizon: July 1 to July 5
Lead time: 2 days
Future period: July 6 and July 7
 Note
The future period is the lead time period right after the end of the planning horizon. To include future data in
order recommendation planning, the MRP lets you include future demands that can only be satisfied by
recommendations released within the current planning horizon.
In the MRP wizard, all future data is consolidated into one column. However, to present the calculation algorithm,
the future period is displayed in days.
The table below shows an item’s inventory status before implementing the MRP order recommendations.
 Note
The receipts and receipts from recommendations are actually consolidated into one row in the MRP wizard as Supplies. To
better present the calculation algorithm, the table displays the two types of receipts separately.
In the MRP wizard, if you want to view the origin of receipts, you can click the cells with supply values, and the Pegging
Information window appears, displaying in the Remaks column whether the supply is a receipt from existing purchase or
production documents, or a receipt from the orders recommended by the MRP.
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:10 AM
July 1 July 2 July 3 July 4 July 5 July 6 July 7
(Future) (Future)
Initial 75 5 -5 15 -15 -35 -125
Inventory
Receipts 30 50 60 70 40 10 20
Demands 100 60 40 100 60 100 120
Final 5 -5 15 -15 -35 -125 -225
Inventory
(Before MRP)
The MRP calculates order recommendations following the steps below:
 Note
Actual demands refer to the quantity needed to keep the inventory level from falling into negative.
1. July 1
Final inventory before MRP: 5
Actual demands: No demands
Receipts from recommendations: 0
Final inventory after MRP: 5
2. July 2
Final inventory before MRP: –5
Actual demands: 5
Receipts from recommendations: 0
There is a demand for 5 items on July 2. However, July 2 is within the lead time period, and due to the 2-day lead
time, demands fall into the lead time period cannot be satisfied by order recommendations. In this situation the
quickest supply can only arrive at the first day right after the lead time period, and that is on July 3 in this example.
In the MRP run, the application calculates based on the following steps:
a. Inspect the first day after the lead time period to see whether there would be any receipt from the existing
documents.
b. If the final inventory before MRP is positive (enough receipts happen to satisfy the inventory demands for
that day and the day before), the MRP does not make any recommendation.
c. If the final inventory before MRP is negative (receipts cannot fully satisfy the demands) , the MRP
recommends quantities to fulfill the demands.
In this case, there are receipts coming on July 3, and the final inventory is 15, therefore the MRP does not
make any recommendation for demands of July 2, and there is no receipt from MRP recommendation on
July 2.
Final inventory after MRP: –5
3. July 3
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:10 AM
Final inventory before MRP: 15
Actual demands: No demands
Receipts from recommendations: 0
Final inventory after MRP: 15
4. July 4
Final inventory before MRP: –15
Actual demands: 15
Receipts from recommendations: 15
The final inventory before MRP falls negative, therefore the MRP recommends an order with a due date on July 4.
Considering the 2-day lead time, the order is recommended on July 2 and there will be a receipt from MRP
recommendation on July 4. With this recommendation, the final inventory after MRP for July 4 is 0.
Final inventory after MRP: 0
5. July 5
Final inventory before MRP: –20 (Initial Inventory: 0; Receipts: 40; Demands: 60)
Actual demands: 20
Receipts from recommendations: 20
The MRP recommends an order on July 3 so that the final inventory after MRP is 0.
Final inventory after MRP: 0
6. July 6
Final inventory before MRP: –90 (Initial Inventory: 0; Receipts: 10; Demands: 100)
Actual demands: 90
Receipts from recommendations: 90
The MRP recommends an order on July 4 so that the final inventory after MRP is 0.
Final inventory after MRP: 0
7. July 7
Final inventory before MRP: –100 (Initial Inventory: 0; Receipts: 20; Demands: 120)
Actual demands: 100
Receipts from recommendations: 100
The MRP recommends an order on July 5 so that the final inventory after MRP is 0.
Final inventory after MRP: 0
The following table shows the inventory status after implementing the MRP recommendations.
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:10 AM
|                   | July 1 | July 2 | July 3 | July 4 | July 5 | July 6   | July 7   |
| ----------------- | ------ | ------ | ------ | ------ | ------ | -------- | -------- |
|                   |        |        |        |        |        | (Future) | (Future) |
| Recommendation    |        | 15     | 20     | 90     | 100    |          |          |
| Initial Inventory | 75     | 5      | -5     | 15     | 0      | 0        | 0        |
| Receipts          | 30     | 50     | 60     | 70     | 40     | 10       | 20       |
| Receipts from     | 0      | 0      | 0      | 15     | 20     | 90       | 100      |
Recommendations
| Demands         | 100 | 60  | 40  | 100 | 60  | 100 | 120 |
| --------------- | --- | --- | --- | --- | --- | --- | --- |
| Final Inventory | 5   | -5  | 15  | 0   | 0   | 0   | 0   |
(Before MRP)
Example: Inventory Transfer Request - Warehouse Selection and
Recommendation Algorithm
Prerequisites
The MRP only recommends inventory transfer request when:
You have selected to run the MRP by warehouse in MRP Wizard, Step 4: Inventory Data Source.
You have selected the Inventory Transfer Request checkbox as a recommendation type in MRP Wizard, Step 5: Documents
Data Source.
Warehouse Selection Rules
The MRP recommends inventory transfer requests per the following steps:
1. Inspect the demands from each warehouse and serves the warehouse with the largest demand first.
  Note
The MRP gives priority to inventory transfer request, which is to say, the MRP always recommends inventory transfer
request before it recommends purchase orders and production orders.
2. Select an issuing warehouse.

 Note
The application only considers warehouses for which you have selected the Include Initial Inventory checkbox in MRP
Wizard, Step 4: Inventory Data Source .
a. Filter all warehouses in the same location as the issuing warehouses.
b. Select the warehouse with the largest available inventory as the issuing warehouse.
c. If there are more than one warehouse that have the highest available quantity, sort the warehouses first by location,
then by warehouse code.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:10 AM
d. After MRP selects an issuing warehouse, it calculates to see whether this issuing warehouse can fully satisfy the
demands from the receiving warehouse.
If yes, the MRP moves to other warehouse with demands and repeat the calculation from the very beginning.
If no, the MRP moves back to step 2 and repeat the process to find another issuing warehouse.
If the MRP cannot find enough inventory to transfer to the receiving warehouse, it recommends purchase orders or
production orders.
Example 1: Inventory Transfer Requests Recommendations
This example uses the following planning parameters:
Lead time: 2 days
Planning horizon: July 1 to July 4
Warehouses: W1 and W2
The table below shows the inventory status after implementing MRP inventory transfer requests and order recommendations:
  Note
The receipts and receipts from recommendations are actually consolidated into one row in the MRP wizard as Supplies. To
better present the calculation algorithm, the table displays the two types of receipts separately.
In the MRP wizard, if you want to view the origin of receipts, you can click the cells with supply values, and the Pegging
Information window appears, displaying in the Remaks column whether the supply is a receipt from existing purchase or
production documents, or a receipt from the orders recommended by the MRP.
|       | July 1 | July 2 | July 3 | July 4 | July 5 | July 6 |
| ----- | ------ | ------ | ------ | ------ | ------ | ------ |
|       |        |        |        |        | Future | Future |
|       | W1 W2  | W1 W2  | W1 W2  | W1 W2  | W1 W2  | W1 W2  |
| Order | 6      |        | 2      | 3      |        |        |
Recommendations
| Initial Inventory  | 10 1 | -4 0 | -1 0 | 0 0    | 0 1  | 0 0 |
| ------------------ | ---- | ---- | ---- | ------ | ---- | --- |
| Demands            | 15   |      | 5    | 15     | 3    | 3   |
| Receipts           |      | 3    |      | 16     |      |     |
| Inventory Transfer | 1 -1 | 3 -3 |      | 15 -15 | 1 -1 |     |
| Receipts from      |      |      | 6    |        | 2    | 3   |
Recommendations
| Final Inventory | -4 0 | -1 0 | 0 0 | 0 1 | 0 0 | 0 0 |
| --------------- | ---- | ---- | --- | --- | --- | --- |
July 1
Warehouse W1 needs 5 items to stay balanced. The MRP first considers inventory transfer from W2 to W1, because
inventory transfers are not confined to lead time requirements. Now W2 only has 1 items to be transferred, therefore, the
final inventory on July 1 is -4 for W1 and 0 for W2.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:10 AM
July 2
Warehouse W2 receives 3 items on July 2. The MRP recommends to transfer these 3 items to W1 so that the final inventory
on July 2 is -1 for W1 and 0 for W2.
July 3
No extra items from W2 can be transferred, yet there is a demand for 6 items from W1. Since July 3 is out of the lead time
period, the MRP recommends orders for 6 items on July 1, the first day of the planning horizon, so that W1 has a receipt
from recommendation to keep inventory balance.
July 4
Warehouse W1 has a demand of 15. Since W2 has 16 items received this day, the MRP recommends to transfer 15 of them to
W1, so that both warehouses are balanced with the final inventory of 0 and 1.
July 5
Warehouse W1 has a demand of 3, but W2 only have 1 item to offer. Therefore the MRP first transfers this 1 item to W1, then
schedules an order recommendation on July 3, 2 days prior to July 5, to fulfill the demand for another 2 items.
July 6
Warehouse W1 has a demand of 3 items and W2 has no inventory left. The MRP can only recommend orders for W1 on July
4 to fulfill the demand on July 6.
Example 2: Inventory Transfer Requests Recommendations (Considering Inventory
Level Requirements)
This example uses the following planning parameters:
Lead time: 2 days
Planning horizon: July 1 to July 4
Warehouses: W1 and W2
Inventory Level:
W1: 10
W2: 10
The table below demonstrates how the MRP plans for inventory transfer request and orders when considering inventory level as a
demand.
 Note
In the MRP result report, the application does not show the inventory level requirements in the Demands column. The MRP
automatically calculates the inventory level requirements and reflects the demands in order recommendation quantities.
July 1 July 2 July 3 July 4 July 5 July 6
Future Future
W1 W2 W1 W2 W1 W2 W1 W2 W1 W2 W1 W2
Order 16 10 2 3
Recommendations
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:10 AM
|                    | July 1 | July 2 | July 3 | July 4 | July 5 | July 6 |
| ------------------ | ------ | ------ | ------ | ------ | ------ | ------ |
|                    |        |        |        |        | Future | Future |
| Initial Inventory  | 10 1   | -4 0   | -1 0   | 10 10  | 10 11  | 10 10  |
| Demands            | 15     |        | 5      | 15     | 3      | 3      |
| Receipts           |        | 3      |        | 16     |        |        |
| Inventory Transfer | 1 -1   | 3 -3   |        | 15 -15 | 1 -1   |        |
| Receipts from      |        |        | 16 10  |        | 2      | 3      |
Recommendations
| Final Inventory | -4 0 | -1 0 | 10 10 | 10 11 | 10 10 | 10 10 |
| --------------- | ---- | ---- | ----- | ----- | ----- | ----- |
July 1
Warehouse W1 needs 5 items to stay balanced. The MRP first considers inventory transfer from W2 to W1, because
inventory transfers are not confined to lead time requirements. Now W2 only has 1 items to be transferred, therefore, the
final inventory on July 1 is -4 for W1 and 0 for W2.
  Note
Though there are inventory level requirements for W2, the MRP gives order demands higher priority. Therefore, within
the lead time period, the MRP first transfers available inventory from W2 to W1 to catch up with the demands for W1 that
is due on July 1.
July 2
Warehouse W2 receives 3 items on July 2. The MRP recommends to transfer these 3 items to W1 so that the final inventory
on July 2 is -1 for W1 and 0 for W2.
July 3
No extra items from W2 can be transferred, yet there is a demand for 6 items to keep the inventory from falling negative
numbers. Considering the inventory level requirements, the MRP recommends 16 items for W1 and 10 items for W2 on July
1, the first day of the planning horizon, so that the both warehouses have receipts from recommendations to fulfill order
demands as well as inventory level requirements.
July 4
Warehouse W1 has a demand of 15. W2 has 16 items received this day. Therefore the MRP recommends to transfer 15 items
from W2 to W1, so that the final inventory is 10 for W1 and 11 for W2.
July 5
Considering the inventory level requirements for both warehouses, W1 is in short of 3 items while W2 only has 1 item to
offer. Therefore the MRP first transfers this 1 item to W1, then schedules an order recommendation on July 3, 2 days prior to
July 5, to fulfill the demand of W1 for another 2 items.
July 6
Considering the inventory level requirements for both warehouses, W1 is in short of 3 items while W2 has no item to offer.
The MRP can only recommend orders for W1 on July 4 to fulfill the demand on July 6.
Generating Documents from Saved Recommendations
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:10 AM
Prerequisites
You have executed an MRP run and saved the order recommendations for this scenario.
Procedure
1. To view saved order recommendations, choose MRP Order Recommendation .
The Order Recommendation – Selection Criteria window appears.
2. Filter the order recommendations you want to process and choose OK.
For more information, see Order Recommendation - Selection Criteria.
3. The Order Recommendation window appears, displaying the filtered recommendations of the selected MRP scenario.
For more information about the fields in this window, see Order Recommendation.
4. You can view a list of reports for the recommended item if necessary. To do so, select a recommendation, right-click in the
Item Code column, and choose a report.
Qty in All Warehouses
Use this report to view the Available, In Stock, Committed, and Ordered quantities of the selected item. To change
the warehouse for receiving the quantities to be procured, select the alternative warehouse and choose the Choose
button. To cancel your operation and go back to the Order Recommendation window, choose Cancel.
Alternative Items
Use this report to view the alternative items for the selected item. To replace the recommended item, select an
alternative item and choose the Choose button. To cancel your operation and go back to the Order
Recommendation window, choose Cancel.
Preferred Vendors List
Use this report to view and compare preferred vendors. To replace the recommended vendor, select an alternative
vendor and choose the OK button. To cancel your operation and go back to the Order Recommendation window,
choose Cancel.
List of Bills of Materials
Last Prices
If you have specified a vendor code for the selected recommendation, the report displays the latest prices for the
selected vendor. Otherwise, the report displays the latest prices for all vendors. You can use the selection criteria to
filter last prices information, if necessary. For more information, see Last Prices Report.
Special Prices
To view the special prices report, make sure you have specified a vendor for the selected recommendation. If you do
not specify a vendor, the following error message appears:
No special prices found; specify vendor code.
Discount Groups
To view the discount groups report, make sure you have specified a vendor for the selected recommendation. If you
do not specify a vendor, the following error message appears:
No discount group found; specify vendor code.
5. Make necessary changes to the recommendation.
Different recommendation types have different ranges of editable fields. Cells in white indicate that you can change the
value for this grid.
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:10 AM
6. To create documents from the recommendations, select the Create checkbox for recommendation lines from which you
want to generate documents.
7. To consolidate the documents to be generated, from the toolbar, choose .
In the Form Settings window, select the General tab.
To group recommendations that share common attributes into one document, select the Consolidate Recommendations
checkbox. The application groups recommendations according to the following rules:
For purchase orders and purchase quotations, group recommendations with the same vendor into one purchase
order or purchase quotation.
The consolidated document may contain multiple lines due to different warehouses, items, due dates, and delivery
dates.
For production orders, group recommendations with the same due date into one production order.
You can manually change the Due Date for recommendations. After you make the changes, the application takes the
changed due date into calculation.
For inventory transfer requests, group the recommendations with the same From Warehouse and Due Date.
Order Recommendation - Selection Criteria Window
Use this window to specify selection criteria to filter the recommendations generated and saved in MRP runs. If you have run a
scenario and saved the recommendations for several times, the application stores the results of the latest MRP run and deletes the
results of the previous run.
To open this window, choose MRP Order Recommendation .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Order Recommendation - Selection Criteria Fields
Order Type
Select the order recommendation type:
All
Production Orders
Purchase Orders
Purchase Quotations
Inventory Transfer Requests
Scenario
Select the MRP scenario whose recommendations you want to process.
 Note
Simulation scenarios are not displayed in this list.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:10 AM
Due Date From... To...
Enter the range of due dates for the production orders, or delivery dates for purchase orders. Recommendations are displayed for
the selected date range.
Items: Properties
Opens the Properties window, proceeds as follows:
Select Ignore Properties.
Deselect Ignore Properties and select one or more Items Property checkboxes.
Vendors: Properties
Opens the Properties window.
In the Properties window, proceeds as follows:
Select Ignore Properties.
Select one or more Business Partners Property checkboxes.
This option is available only when you select Purchase Orders, Purchase Quotations, or All for order types.
More Information
Generating Orders from Saved Recommendations
Order Recommendation
Order Recommendation Window
This window displays the order recommendation according to your defined selection criteria.
This window is very similar to the Recommendation tab in the MRP Results window. But you can access, update and change
almost all the fields in this window. For more information, see Generating Orders from Saved Recommendations.
You can:
View the list of MRP recommendations, according to defined selection criteria
Make necessary changes to the recommendation, fore examples, order types, quantities, items, vendors, warehouses, and
so on.
Create documents from saved order recommendations
Delete recommendations
 Caution
You can delete one or several lines in the Order Recommendation window; however, you cannot restore deleted lines
until the next MRP run.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:10 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Order Recommendation Fields
Find Item No.
Enter an item number to locate the item in the window.
Create
To create documents from recommendations, select the checkbox and choose the Update button.
To select all recommendations, double-click the column header.
Order Type
MRP recommendation type.
You can
Change a production order to a purchase order, if a production Bill of Materials exists for the item.
Change a purchase order to a production order, if you can specify a vendor for the order.
Change a purchase order to purchase quotation, and create the purchase order based on the vendor's quotes.
 Note
If you create a purchase quotation from the order recommendation, the application creates quotations for all the
preferred vendors listed in item master data. If you have not specified any preferred vendor, you receive a message that
No records found; maintain preferred vendors list for item.
Change purchase orders and production orders to inventory transfer requests, so as to satisfy the demands using the
existing inventory in other warehouses.
 Note
If you create an inventory transfer request from the order recommendation, make sure that you specify the From
Warehouse and the To Warehouse fields.
Branch
Displays the branch of the order.
 Note
This field is available only if you have enabled multiple branches.
Quantity
Quantity recommended by the MRP report. You can update the value.
UoM Code, UoM Name
Unit of measurement (UoM) for purchase order recommendations and production order recommendations:
For purchase orders and purchase quotations: use the purchasing UoM defined in the Item Master Data window,
Purchasing Data tab.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:10 AM
You can manually change this default UoM to any purchasing UoM before generating the recommendation.
For production orders and inventory transfer requests: use the inventory UoM defined in the Item Master Data window,
Inventory Data tab.
MOQ
Displays the minimum order quantity for the item defined in the item master data.
Release Date
Date on which each recommended document should be released to meet its due date, depending on the lead time of the item;
cannot be earlier than today.
Due Date
Delivery date suggested for the purchase order or the due date for the production order.
Vendor Code
Select the vendor for the order.
Vendor Name
Display the name of the vendor for the order.
Price Mode
Appears only if you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System
Initialization Company Details Basic Initialization tab.
Price mode of the order. By default, it is the price mode of the selected vendor. If required, select a different mode.
 Note
This field is not available for the Brazil, India, and Israel localizations.
Price
Price from the price list linked to the preferred vendor. If special prices are defined for the linked preferred vendor, these are
displayed instead (depending on the standard behavior of prices in SAP Business One). You can update the price manually.
If you have selected the checkbox Enable Separate Net and Gross Price Mode in Administration System Initialization
Company Details Basic Initialization tab, the unit price displayed here agrees with the mode you have defined in the Price
Mode field.
 Note
The checkbox Enable Separate Net and Gross Price Mode is not available for the Brazil, India, and Israel localizations.
Discount
Specify discount percentage to be granted when creating the purchase order.
From Whse
Displays the warehouse that issues the inventory in an inventory transfer. This field is valid and editable only for recommendations
with the Order Type of Inventory Transfer Request.
To Whse
Displays the warehouse that receives the procured quantity. You can change the warehouse if necessary.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:10 AM
For production order recommendations, by default.the application displays the warehouse defined in Bill of Materials for
this parent item.
For purchase order recommendations, by default the application displays the warehouse according to your warehouse
definition in MRP Wizard, Step 5: Documents Data Source.
If you choose to Generate to Default Warehouse for Item, the application displays the item's default warehouse as
defined in item master data.
If you choose to Generate to Warehouse with the Demand the application displays the warehouse that has the
demand to procure this item.
For inventory transfer request recommendations, the application displays the receiving warehouse in the inventory transfer.
Exception
Past Due message for items whose recommendation was created with a due date in the past, or where the length of the lead time
precludes meeting the due date.
In addition, to display fields such as Item Group, Manufacturer, Total, and Origin choose in the toolbar.
This is custom documentation. For more information, please visit SAP Help Portal. 53