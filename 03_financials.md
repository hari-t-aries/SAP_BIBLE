6/8/26, 6:03 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:03:27 GMT+0000
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

6/8/26, 6:03 AM
Journal Voucher Report
This report provides comprehensive information on existing journal vouchers. Use the report to get a list of the journal vouchers to
be approved, or to save one or all of the open journal vouchers as permanent financial documents.
Use this window to specify selection criteria for the Journal Voucher report.
To open the window, choose Financials Journal Voucher Report .
After defining the report, you can view it in the Journal Voucher Report Window.
Selection Criteria
Date
Specify the range of posting dates of the journal vouchers.
Journal Voucher No.
Specify the range of the journal voucher group numbers.
Trans. No.
Specify the range of the transaction numbers of a journal voucher.
Display Open Journal Vouchers
Report includes journal vouchers that have not been approved or saved as permanent documents.
Display Closed Journal Vouchers
Report includes journal vouchers that have been approved or saved as permanent documents.
Journal Voucher Report Window
This window displays the Journal Voucher report according to the selected criteria.
Use the first column to select the journal vouchers for the report:
The document level checkboxes are activated for manual editing, while the checkboxes on the G/L account level are not.
Selecting a certain document automatically selects the related G/L accounts.
The checkboxes of the closed journal vouchers are inactive.
Once selected journal vouchers are posted as journal entries, their checkboxes become inactive.
 Note
To display the Remarks field, from the SAP Business One Main Menu, choose Tools Form Settings . In the Remarks
column, select the Visible checkbox.
The data in the Remarks field from the journal vouchers is displayed in the lower matrix of the Journal Vouchers
window.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:03 AM
Journal Voucher Report
Currency
Specify the currency type for displaying the amount.
From Date, To Date
Displays the range of the posting dates you defined for the report. Changing the dates updates the display of the journal vouchers
accordingly.
Gr.-No.
Journal Voucher Number - Transaction Number
Date
Posting date of the transaction.
G/L Acc./BP Code, G/L Acc./BP Name
Code/name of the account or business partner for which the journal voucher was recorded.
Debit, Credit
Debit/credit values of the journal voucher.
Post
Saves the selected journal vouchers as journal entries.
Working with Fixed Assets
With SAP Business One, you can now manage your fixed assets from both the tax and accounting perspectives in a more efficient
manner. The fixed assets function provides you with both physical and financial control over the complete asset life cycle, from
acquisition through depreciation, revaluation, and disposal.
The diagrams below show the topics covered in this section. Choose each topic for more information.
Use the following to manage your fixed assets in SAP Business One.
Please note that image maps are not interactive in PDF outputs.
Use the following to learn about the fixed assets add-on and virtual fixed assets.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:03 AM
Please note that image maps are not interactive in PDF outputs.
Use the following to evaluate and process the fixed asset-related data.
Please note that image maps are not interactive in PDF outputs.
More Information
Account Determination
Depreciation Types
Depreciation Areas
Asset Classes
Asset Master Data
Upgrade of Fixed Assets Add-On
If you were using SAP Business One 8.82 or lower versions with the Fixed Assets add-on installed, the upgrade process has the
following results:
The add-on is not available.
No data in the add-on is upgraded. Instead, all data in the add-on is stored in the database after upgrade.
Migration of Fixed Assets Data
In order to make the data available in SAP Business One 9.0, you must use the fixed assets data migration wizard.
With the wizard, you can only migrate the asset values at the beginning of a fiscal year from the add-on to SAP Business One. No
asset transactions can be migrated.
 Example
You have been using SAP Business One 8.82 with the Fixed Assets add-on since 2010. In March 2013, you upgrade to SAP
Business One 9.0.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:03 AM
After the upgrade, you migrate the data from the add-on using the fixed assets data migration wizard. As a result, all the asset
master data with their accumulated values as of January 1st, 2013, are migrated. Any depreciations or transactions posted
after January 1st, 2013 are not migrated.
Therefore, to make sure all fixed asset-related data are correctly migrated, we recommend that you upgrade when you close a
fiscal year and are ready to open a new fiscal year.
In case the upgrade must be executed in the middle of a fiscal year, you must do the following in the add-on before the upgrade to
ensure the data migration afterwards achieves the expected results:
If there are asset depreciations in the fiscal year, cancel the corresponding journal entries.
After the upgrade, you must carry out these depreciations again.
If there are asset transactions, such as capitalization and retirement, in the fiscal year, cancel the transactions and their
corresponding journal entries.
After the upgrade, you must create these transactions again.
More Information
Importing Data from Fixed Assets Add-On
Enabling Fixed Assets
To manage fixed assets in SAP Business One, you must enable the fixed assets function.
 Note
If you have not enabled fixed assets, you cannot access fixed asset-related menus or windows.
After you have enabled bin locations, you can find fixed asset-related menu entries in the following paths from the SAP
Business One Main Menu:
Administration Setup Financials Fixed Assets
Financials Fixed Assets
Procedure
1. From the SAP Business One Main Menu, choose Administration System Initialization Company Details .
The Company Details window opens.
2. On the Basic Initialization tab of the Company Details window, select the Enable Fixed Assets checkbox.
3. In the Calculate Depreciation By field, specify whether you want the system to calculate the depreciation of your fixed
assets by month or day.
For more information about the field, see Company Details: Basic Initialization Tab.
 Recommendation
After enabling fixed assets for your company, set up the following before you create asset master data:
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:03 AM
Account determination
Depreciation types
Depreciation areas
Attribute groups
Asset classes
More Information
Working with Fixed Assets
Defining and Assigning Asset Classes
In SAP Business One, you can define your fixed assets by different classes. In each asset class, you can assign multiple
depreciation areas and depreciation methods. By assigning an asset class to an asset, you can link the depreciation areas and
methods to the asset.
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
You have defined the following:
Account determination
Depreciation types
Depreciation areas
Attribute groups
Procedure
Defining Asset Classes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Asset Classes .
The Asset Classes - Setup window opens.
2. Specify the general information and the following parameters:
Asset type
Attribute group
Depreciation area
Account determination
Depreciation type
Useful life
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:03 AM
3. Choose Add.
Assigning Asset Classes to Fixed Assets
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
2. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
 Note
You cannot change the asset class of an asset having the status Active.
Once you specify the asset class, the associated depreciation parameters are copied to the asset. If required, you can also
change these parameters for the asset.
More Information
Asset Classes
Asset Master Data
Asset Classes
With SAP Business One, you can use asset classes to classify fixed assets according to business and legal requirements. For each
asset class, you can assign various depreciation areas and depreciation types. After you assign an asset class to an asset, the
depreciation areas and depreciation types are taken to the asset master data as defaults.
More Information
Asset Classes - Setup Window
Defining and Assigning G/L Accounts
In SAP Business One, you can define multiple sets of G/L accounts. After defining the G/L account sets, you can assign them to
asset classes and, therefore, link them to fixed assets.
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
Procedure
Defining G/L Accounts
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Account
Determination .
The Account Determination - Setup window opens.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:03 AM
2. Specify the code, description, and G/L accounts and choose Add.
Assigning G/L Accounts to Fixed Assets
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Asset Classes .
The Asset Classes - Setup window opens.
2. Specify the general information, select the depreciation areas, and specify the account determination in each area.
3. Choose Add.
4. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
5. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
 Note
You cannot change the asset class of an asset having the status Active.
Once you specify the asset class, the associated account determination is assigned to the asset.
More Information
Account Determination
Asset Classes
Asset Master Data
Account Determination
Account determination enables the system to automatically determine the relevant general ledger accounts for a fixed asset when
an asset transaction takes place.
SAP Business One lets you define multiple account determination sets. For each asset, you can apply more than one set of G/L
accounts, so that the asset value and transactions can be posted to more than one accounting area at the same time.
Related Information
Defining and Assigning G/L Accounts
Account Determination - Setup Window
Account Determination - Setup Window
Use this window to define and view different sets of G/L accounts for your fixed assets.
To open this window, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Account Determination .
Account Determination - Setup Window Fields
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:03 AM
Code
Enter a unique code for the set of G/L accounts you are defining.
Description
Enter a description for the set of G/L accounts you are defining.
Asset Balance Sheet Account
Specify the account for the acquisition and production costs of fixed assets.
Acquisition Clearing Account
Specify the clearing account for the acquisition and production costs of the fixed assets.
Revaluation Account
Specify the offset account for the revaluation reserve account. The default value is the same as the asset balance sheet account.
Revaluation Reserve
Specify the account to which the increase in the asset's value, as a result of revaluation, is posted.
Revaluation Reserve Clearing
Specify the clearing account to which the increase in the asset's value as a result of revaluation is posted temporarily when an
asset is sold.
Ordinary Depreciation
Specify the expense account for the ordinary, planned, annual depreciation of fixed assets.
Accumulated Ordinary Depr.
Specify the account on the liability side for the accumulated value of ordinary, planned depreciation. This account is the offsetting
account for ordinary, planned depreciation.
Unplanned Depreciation
Specify the expense account for the unplanned annual depreciation of fixed assets.
Accumulated Unplanned Depr.
Specify the account for the accumulated unplanned depreciation of fixed assets.
Special Depreciation
Specify the expense account for the special depreciation of fixed assets.
Accumulated Special Depr.
Specify the account for the accumulated special depreciation of fixed assets.
Revenue from Asset Sales (Net)
Specify the account for the net revenues from asset sales before tax. This account is the offsetting account for the revenue
account from asset sales that is specified for sales from the customer account. The net book value and the profits or losses are
posted to this account when a sale is made.
Retirement with Expense (Net)
Specify the account to which the net losses resulting from asset sales are posted.
Retirement with Revenue (Net)
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:03 AM
Specify the account to which the net profits gained from asset sales are posted.
NBV Retirement Expense Account (Gross)
Specify the expense account for recording the net book value of an asset during retirement.
When an asset with the gross posting method retires with losses, the account records the net book value of the asset during
retirement.
NBV Retirement Revenue Account (Gross)
Specify the revenue account for recording the net book value of an asset during retirement.
When an asset with the gross posting method retires with profits, the account records the net book value of the asset during
retirement.
Revenue Account for Retirement
Specify the account for the revenue resulting from asset retirement.
Revenue Clearing Account
Specify the clearing account for the revenue resulting from asset sales.
Revaluation Loss
Specify an account to record the difference loss between the new net book value (NBV) and the current net book value (NBV).
More Information
Account Determination
Defining and Assigning Depreciation Methods
In SAP Business One, you can define various depreciation methods, such as the following:
Straight line
Straight line period control
Declining balance
Multilevel
Immediate write-off
Special depreciation
Manual depreciation
After defining the depreciation methods, you can assign them to asset classes and, therefore, link them to fixed assets.
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:03 AM
Procedure
Defining Depreciation Methods
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Depreciation
Types .
The Depreciation Types - Setup window opens.
2. Select the depreciation methods and specify other depreciation related parameters.
3. Choose Add.
Assigning Depreciation Methods to Fixed Assets
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Asset Classes .
The Asset Classes - Setup window opens.
2. Specify the general information, select the depreciation areas, and specify the depreciation type in each area.
3. Choose Add.
4. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
5. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
 Note
You cannot change the asset class of an asset having the status Active.
Once you specify the asset class, the associated depreciation types are copied to the asset. Therefore, the depreciation
methods are assigned to the asset. If required, you can also change the depreciation types for the asset.
More Information
Depreciation Types
Asset Classes
Asset Master Data
Depreciation Types
In SAP Business One, you can use depreciation types to define different depreciation calculation methods for your fixed assets.
After you create a depreciation type, you can assign it to a specific depreciation area of an asset class. Then, by assigning the asset
class to a fixed asset, the depreciation calculation methods are finally applied to the asset.
In general, SAP Business One lets you use the following depreciation methods:
Straight Line Method
Straight Line Period Control Method
Declining Balance Method
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:03 AM
Multilevel Method
Immediate Write-Off Method
Special Depreciation Method
Manual Depreciation Method
More Information
Depreciation Types - Setup Window
Depreciation Types - Setup Window: General Tab
Depreciation Types - Setup Window: Calculation Tab
Depreciation Types - Setup Window
Use this window to create, display, or change depreciation types.
To access the general area, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Depreciation Types .
General Area Fields
Code
Enter a unique code for the depreciation type.
Description
Enter a description about the depreciation type.
Method
From the dropdown list, select one of the following depreciation methods:
No Depreciation
Straight Line – A method of distributing an asset's value evenly across its useful life. That is, the asset is depreciated by the
same amount in each period.
Straight-Line Period Control – A method that entails defining different factors used in depreciation calculation for different
periods of an asset's useful life.
Declining Balance – A method that entails applying a depreciation rate against the non-depreciated balance of an asset.
Instead of spreading the cost of the asset evenly over its useful life, the method depreciates the asset at a constant rate,
which results in declining depreciation charges each successive period.
Multilevel – A method of applying different depreciation rates to an asset for different stages of an asset's useful life.
Immediate Write-Off – A method generally applied to low-value assets whose full value can be depreciated in the
acquisition year.
Special Depreciation – A method of carrying out automatic special depreciation.
Manual Depreciation – A method of carrying out manual special depreciation.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:03 AM
Calculation Base
Specify whether you want to calculate the depreciation of assets with one of the following bases:
Yearly – Calculates the depreciation of the year first, and then uses the yearly depreciation as the base to calculate the
depreciation of each period.
Monthly – Calculates the depreciation of the month first, and then uses the monthly depreciation as the base to calculate
the depreciation of each period.
When you use the two different kinds of calculation bases, the rounding of depreciation values can be different.
 Note
For depreciation types with the Declining Balance method, the percentage you define can be annual or monthly, according to
your selection here.
 Example
Asset X
Acquisition and Production Costs: 5500 USD
Useful Life: 48 Months
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
If the asset has the yearly calculation base, the system calculates the depreciation of the year as follows:
5500 USD / 48 * 12 = 1375 USD
If the asset has the monthly calculation base, the system first calculates the depreciation of the month as follows:
5500 USD / 48 = 114.5833 USD
Then, the system rounds 114.5833 to 114.58 and calculates the depreciation of the year as follows:
114.58 USD * 12 = 1374.96 USD
More Information
Depreciation Types - Setup Window: General Tab
Depreciation Types - Setup Window: Calculation Tab
Depreciation Types - Setup Window: General Tab
Use this tab to define the general parameters for depreciation types.
To access this tab, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Depreciation Types and select the General tab.
General Tab Fields
Minimum Depreciated Value
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:03 AM
Specify the minimum book value of an asset after depreciation.
 Note
If you have specified a minimum depreciated value and a salvage value percentage at the same time, the salvage value has
higher priority. That is, the system depreciates an asset till the asset value is reduced to the salvage value.
Maximum Depreciable Value
 Note
The field is available only for depreciation types having the Straight Line or Declining Balance method.
Enter the maximum depreciable value of an asset.
The system takes the maximum depreciable value into account when calculating the depreciation charges for an asset. For more
information, see the examples below.
 Example
Asset X
Acquisition and Production Costs: 80,000 USD
Useful Life: 60 Months
Maximum Depreciable Value: 60,000 USD
Salvage Value Percentage: None
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
Calculation Base: Monthly
As the maximum depreciable value is 60,000 USD, the system calculates the monthly depreciation as follows:
60000 USD / 60 = 1000 USD
At the end of the useful life, the asset still holds the value of 20,000 USD.
Asset Y
Acquisition and Production Costs: 30,000 USD
Useful Life: 60 Months
Maximum Depreciable Value: 60,000 USD
Salvage Value Percentage: None
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
Calculation Base: Monthly
As the acquisition and production costs are less than the maximum depreciable value, the asset can be depreciated
until its acquisition and production costs reach zero. Therefore, the monthly depreciation charge is calculated as follows:
30000 USD / 60 = 500 USD
At the end of the useful life, the asset's book value is zero.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:03 AM
Asset Z
Acquisition and Production Costs: 15,000 USD
Useful Life: 60 Months
Maximum Depreciable Value: 9,000 USD
Salvage Value Percentage: 20%
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
Calculation Base: Monthly
The system calculates the salvage value of the asset as follows:
15000 USD * 20% = 3000 USD
Though the asset's maximum depreciable value is 9,000 USD, its actual depreciable value is only 6000 USD,
considering the salvage value.
Therefore, the asset's monthly depreciation charge is calculated as follows:
Include Salvage Value in Depreciation Calculation checkbox: Selected
9000 USD / 60 = 150 USD
After 40 months, the asset's accumulated depreciation charges reach 6,000 USD and the depreciation stops.
Include Salvage Value in Depreciation Calculation checkbox: Unselected
(9000 USD – 3000 USD) / 60 = 100 USD
Round Year End Book Value
Rounds the net book values of assets at the end of each fiscal year.
Once you select the checkbox, you can select a rounding method from the following:
Truncate to Integer： SAP Business One truncate the depreciation amounts to an integer.
 Example
The net book value of an asset calculated by the system amounts to 28,123.82 USD at the end of the year. If you have
selected this option, the system rounds this amount to 28,123.00 USD. The depreciation amount of the asset in the year
is therefore increased by 0.82 USD.
Round Up to Integer： SAP Business One rounds the depreciation amounts up to an integer.
 Example
The net book value of an asset calculated by the system amounts to 28,123.82 USD at the end of the year. If you have
selected this option, the system rounds this amount to 28,124.00 USD. The depreciation amount of the asset in the year
is therefore decreased by 0.18 USD.
Round Down to Integer: SAP Business One rounds the depreciation amounts down to an integer.
 Example
The net book value of an asset calculated by the system amounts to 28,123.82 USD at the end of the year. If you have
selected this option, the system rounds this amount to 28,123.00 USD. The depreciation amount of the asset in the year
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:03 AM
is therefore increased by 0.82 USD.
Salvage Value Percentage
Enter a salvage value percentage.
 Note
If you have specified a minimum depreciated value and a salvage value percentage at the same time, the salvage value has
higher priority. That is, the system depreciates an asset till the asset value is reduced to the salvage value.
Include Salvage Value in Depreciation Calculation
Includes the salvage value in the calculation of an asset's depreciation.
 Example
Asset X
Acquisition and Production Costs: 6,000 USD
Useful Life: 60 Months
Depreciation Method: Straight Line
Calculation Base: Yearly
Calculation Method: Acquisition Value / Total Useful Life
Salvage Value Percentage: 10%
If you have not selected the checkbox, the system calculates the asset's monthly depreciation as follows:
(6000 USD – 6000 USD * 10%) / 60 = 90 USD
In this case, the asset is depreciated by 90 USD per month, and the salvage value is 600 USD after its 60 months useful
life.
If you have selected the checkbox, the system calculates the asset's monthly depreciation as follows:
6000 USD / 60 = 100 USD
In this case, the asset is depreciated by 100 USD per month in the first 4 years, and 50 USD per month in the last year of
its useful life so that its salvage value remains 600 USD.
Acquisition
Specify how the acquisition of an asset determines the asset's depreciation start date. From the dropdown list, select one of the
following conventions:
Pro Rata Temporis – If you select this, the PR Temporis Type field appears. From the dropdown list, you can select one of
the following options to determine the depreciation start date:
Exact Daily Base – The depreciation of the asset starts from the day of the asset acquisition.
First Day of Current Period – The depreciation of the asset starts from the first day of the posting period within
which the asset acquisition takes place.
First Day of Next Period – The depreciation of the asset starts from the first day of the posting period that follows
the period of asset acquisition.
First Year Convention – Determines the depreciation start date as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:03 AM
When your fiscal year matches a calendar year:
If the asset acquisition takes place before July 1st, the depreciation starts from January 1st.
If the asset acquisition takes place after July 1st, the depreciation starts from July 1st.
When your fiscal year does not match a calendar year:
If the asset acquisition takes place in the first half of the fiscal year, the depreciation starts from the first day
of the first half of the year.
If the asset acquisition takes place in the second half of the fiscal year, the depreciation starts from the first
day of the second half of the year.
Half Year – The depreciation of the asset always starts from the first day of the second half of the fiscal year during which
the asset acquisition takes place.
Full Year – The depreciation of the asset always starts from the first day of the fiscal year during which the asset acquisition
takes place.
Subsequent Acquisition
Specify how an asset's subsequent acquisition affects the asset's depreciation. From the dropdown list, select one of the following
conventions:
Pro Rata Temporis – If you select this, the field PR Temporis Type appears. From the dropdown list, you can select one of
the following options:
Exact Daily Base – Recalculates the asset depreciation from the very day when the subsequent acquisition takes
place.
First Day of Current Period – Recalculates the asset depreciation from the first day of the posting period within
which the subsequent acquisition takes place.
First Day of Next Period – Recalculates the asset depreciation from the first day of the posting period that follows
the period of subsequent acquisition.
Half Year Convention – Recalculates the asset depreciation as one of the following:
If an asset's subsequent acquisition takes place in the fiscal year of acquisition, the system recalculates the asset
depreciation from the very day when the depreciation starts.
If an asset's subsequent acquisition takes place in years that follow the fiscal year of acquisition, the system
recalculates the asset depreciation from the first day of the fiscal year during which the subsequent acquisition
occurs.
Full Year – Recalculates the asset depreciation as one of the following:
If an asset's subsequent acquisition takes place in the fiscal year of acquisition, the system recalculates the asset
depreciation from the very day when the depreciation starts.
If an asset's subsequent acquisition takes place in years that follow the fiscal year of acquisition, the system
recalculates the asset depreciation from the first day of the fiscal year during which the subsequent acquisition
occurs.
Retirement
Specify how an asset's retirement affects the asset's depreciation. From the dropdown list, select one of the following conventions:
Pro Rata Temporis – If you select this, the field PR Temporis Type appears. From the dropdown list, you can select one of
the following options:
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:03 AM
Exact Daily Base – Calculates the asset depreciation till the very day of retirement.
Last Day of Prior Period – Calculates the asset depreciation till the last day of the posting period prior to the period
of retirement.
Last Day of Current Period – Calculates the asset depreciation till the last day of the posting period in which the
retirement takes place.
Half Year Convention – Calculates the asset depreciation as one of the following:
If the asset retirement takes place in the first half of the fiscal year, the system calculates the depreciation till the
last day of the first half of the year.
If the asset retirement takes place in the second half of the fiscal year, the system calculates the depreciation till the
last day of the second half of the year.
Transfer From Source Asset, PR Temporis Type
Specify how the transfer of an asset determines the depreciation of the source asset.
Transfer from Source Asset field is non-editable and displays Pro Rata Temporis.
In the PR Temporis dropdown list, you can select one of the following options:
Exact Daily Base - As the source asset, calculates the depreciation of the transferred asset until the very day of the
transfer.
First Day of Prior Period - As the source asset, calculates the depreciation of the transferred asset until the first day of the
posting period prior to the period within which the asset transfer takes place.
First Day of Current Period - As the source asset, calculates the depreciation of the transferred asset until the first day of
the posting period within which the asset transfer takes place.
Transfer to Target Asset, PR Temporis Type
Specify how the transfer of an asset determines depreciation start date of the target asset.
The Transfer to Source Asset field is non-editable and displays Pro Rata Temporis.
In the PR Temporis dropdown list, you can select one of the following options:
Exact Daily Base - As the target asset, the depreciation of the transferred asset starts from the very day of the transfer.
First Day of Prior Period - As the target asset, the depreciation of the transferred asset starts from the first day of the
posting period prior to the period within which the asset transfer takes place.
First Day of Current Period - As the target asset, the depreciation of the transferred asset starts from the first day of the
posting period within which the asset transfer takes place.
Include Depreciation of Previous Periods in Capitalization Period
Moves depreciation of previous periods in the fiscal year to the capitalization period.
If the capitalization of an asset does not take place at the beginning of a year, you can calculate the depreciation for the entire year
and then select the checkbox to move the depreciation of the previous periods to the capitalization period.
 Example
Asset X
Acquisition and Production Costs: 10,000 USD
Useful Life: 60 Months
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:03 AM
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
Capitalization Date: April 1st, 2012
It is required to deduct the depreciation in the first year by 50%.
The system first calculates the depreciation in the first year as follows:
(10000 USD / 60 * 12) * 50% = 1000 USD
Then, the depreciation per month is calculated as follows:
1000 USD / 12 = 83.33 USD
If you have selected this checkbox, the asset depreciation in 2012 is as follows:
| Jan. Feb. | Mar. | Apr.   | May   | Jun.  | Jul.  | Aug.  | Sep.  |     | Oct. Nov.   | Dec.  |
| --------- | ---- | ------ | ----- | ----- | ----- | ----- | ----- | --- | ----------- | ----- |
|           |      | 333.32 | 83.33 | 83.33 | 83.33 | 83.33 | 83.33 |     | 83.33 83.33 | 83.33 |
If you have not selected this checkbox, the asset depreciation in 2012 is as follows:
| Jan. Feb. | Mar. | Apr. | May Jun. | Jul. | Aug. | Sep. | Oct. | Nov. | Dec. |     |
| --------- | ---- | ---- | -------- | ---- | ---- | ---- | ---- | ---- | ---- | --- |
83.33 83.33 83.33 83.33 83.33 83.33 83.33 83.33 83.33 83.33 83.33 83.33
Stop Depreciation at End of Last Full Fiscal Year
Stops an asset's depreciation at the end of the last full fiscal year of the asset's useful life.
  Example
Asset X
Acquisition and Production Costs: 3,600 USD
Useful Life: 36 Months
Depreciation Method: Straight Line
Calculation Base: Monthly
Calculation Method: Acquisition Value / Total Useful Life
Capitalization Date: April 1st, 2010
If you have selected this checkbox, the asset depreciation is as follows:
|   Jan.   | Feb. Mar. | Apr. | May | Jun. | Jul. Aug. | Sep. | Oct. | Nov. | Dec. |     |
| -------- | --------- | ---- | --- | ---- | --------- | ---- | ---- | ---- | ---- | --- |
| 2010     |           | 100  | 100 | 100  | 100 100   | 100  | 100  | 100  | 100  |     |
| 2011 100 | 100 100   | 100  | 100 | 100  | 100 100   | 100  | 100  | 100  | 100  |     |
| 2012 100 | 100 100   | 100  | 100 | 100  | 100 100   | 100  | 100  | 100  | 400  |     |
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:03 AM
If you have not selected this checkbox, the asset depreciation is as follows:
|      | Jan. Feb. | Mar. Apr. | May Jun. | Jul. Aug. | Sep. Oct. | Nov. Dec. |
| ---- | --------- | --------- | -------- | --------- | --------- | --------- |
| 2010 |           | 100       | 100 100  | 100 100   | 100 100   | 100 100   |
| 2011 | 100 100   | 100 100   | 100 100  | 100 100   | 100 100   | 100 100   |
| 2012 | 100 100   | 100 100   | 100 100  | 100 100   | 100 100   | 100 100   |
| 2013 | 100 100   | 100       |          |           |           |           |
Percentage of Depreciation to Reverse in Retirement Year
Enter the amount (in percentage) of depreciation you want to reverse for an asset in the retirement year.
After you specify the percentage, the system decreases the asset's planned depreciation in the retirement year, and adjusts its net
book value accordingly.
  Note
The percentage you specify here applies to an asset only when it is fully retired.

 Example
Asset X
Acquisition and Production Costs: 48,000 USD
Useful Life: 48 Months
Depreciation Method: Straight Line
Calculation Method: Acquisition Value / Total Useful Life
Percentage of Depreciation to Reverse in Retirement Year: 40%
Capitalization Date: January 1st, 2010
Retirement Date: July 1st, 2012
The system calculates the asset depreciation as follows:
|   Jan. | Feb. Mar. | Apr. May | Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| ------ | --------- | -------- | --------- | --------- | --------- | ---- |
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
| 2012 1000 | 1000 1000 | 1000 1000 | 1000   |     |     |     |
| --------- | --------- | --------- | ------ | --- | --- | --- |
| 2013      |           |           |        |     |     |     |
Then, the system calculates the depreciation to reverse in 2012 as follows:
1000 USD * 6 * 40% = 2400 USD
And the deprecation in 2012 is updated as follows:
(6000 USD – 2400 USD) / 6 = 600 USD
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:03 AM
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2012 600 600 600 600 600 600
The net book value of the asset on July 1st, 2012 is 20,400 USD.
Valid From To
Specify the valid period of the depreciation type.
More Information
Depreciation Types - Setup Window
Depreciation Types - Setup Window: Calculation Tab
Depreciation Types - Setup Window: Calculation Tab
Use this tab to define the calculation methods for depreciation types.
To access this tab, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Depreciation Types and select the Calculation tab.
You can specify the depreciation calculation details, depending on the depreciation methods you select from among the following
in the general area of the Depreciation Types - Setup Window:
No depreciation: No calculation is carried out and you do not need to enter any data.
Straight Line Method
Straight Line Period Control Method
Declining Balance Method
Multilevel Method
Immediate Write-Off Method
Special Depreciation Method
Manual Depreciation Method
More Information
Depreciation Types - Setup Window: General Tab
Straight Line Method
Straight line depreciation is the simplest and most commonly used depreciation method, which assumes an asset loses an equal
amount of value each year over its estimated useful life. This means that the acquisition and production costs are distributed
evenly across the entire useful life of the asset.
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:03 AM
Generally, straight line depreciation is calculated by subtracting the salvage value of the asset from the acquisition and production
costs, and then dividing this amount by the useful life of the asset. SAP Business One provides two additional calculation methods.
For more information, see the Calculation Method field in the section that follows.
 Note
Subsequent acquisitions lead to an increment in the value of an asset; therefore, the depreciation is usually increased by the
amount that would have been necessary to fully depreciate the increment over the useful life of the asset.
Straight Line Method
Calculation Method
Select one of the following depreciation calculation methods:
Acquisition Value/Useful Life
Percentage of Acquisition Value
If you select this method, you must specify a percentage in the Annual Percentage field.
Net Book Value/Remaining Life
Annual Percentage
Enter the annual percentage rate for the depreciation calculation.
 Note
The field is available only if you have selected Percentage of Acquisition Value in the Calculation Method field.
 Example
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Straight Line
Calculation Base: Yearly
Capitalization Date: January 1st, 2010
The asset depreciation is calculated in different ways, depending on the different calculation methods.
Acquisition Value/Total Useful Life
The system calculates the monthly depreciation as follows:
60000 USD / 60 * 12 / 12 = 1000 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:03 AM
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
Percentage of Acquisition Value
Annual Percentage = 20%
The system calculates the monthly depreciation as follows:
60000 USD * 20% / 12 = 1000 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
Net Book Value/Remaining Life
The system calculates the monthly depreciation for each year as follows:
2010
60000 USD / 60 * 12 / 12 = 1000 USD
2011
(60000 USD – 1000 USD * 12) / (60 – 12) = 1000 USD
2012
(60000 USD – 1000 USD * 12 * 2) / (60 – 12 * 2) = 1000 USD
...
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:03 AM
If there is a subsequent acquisition of the asset, the system recalculates the depreciation so that the asset can still be fully
depreciated over its useful life.
To determine when the asset depreciation is recalculated, select a convention in the Subsequent Acquisition field on the
Depreciation Types - Setup Window: General Tab.
Assume a subsequent acquisition, with a worth of 15,000 USD, takes place on October 1st, 2010, and the depreciation is
recalculated from the same day using the Acquisition Value/Total Useful Life method; the system updates the depreciation
amounts as follows:
2010: October – December
The system calculates the monthly depreciation as follows:
(60000 USD + 15000 USD) / 60 = 1250 USD
2011, 2012, 2013
The system calculates the monthly depreciation as follows:
(60000 USD + 15000 USD) / 60 = 1250 USD
2014
In order to fully depreciate the asset, the system calculates the monthly depreciation in the last year of its useful life as
follows:
[60000 USD + 15000 USD – 1250 USD * (12 * 3 + 3) – 1000 USD * (12 – 3)] / (60 – 12 * 4) = 1437.50 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1250 1250 1250
2011 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250
2012 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250
2013 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250 1250
2014 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50 1437.50
More Information
Depreciation Types - Setup Window: Calculation Tab
Straight Line Period Control Method
Straight line period control is a depreciation method that involves exercising control over the depreciation amount of each
individual period in an asset's useful life. The method calculates an asset's depreciation in a period by multiplying the straight line
depreciation amount in the period by a factor you define.
SAP Business One provides the following two kinds of period control:
Standard – You can apply the same factor for depreciation calculation to all periods in an asset's useful life.
To define the factor, on the Calculation tab of the Depreciation Types - Setup window, enter a value in the Factor field.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:03 AM
Individual – You can apply different factors for depreciation calculation to different periods in an asset's useful life.
SAP Business One lets you define a factor for each month. To do so, open the Depreciation Period Control window by
choosing the Period Control pushbutton in the asset master data.
Straight Line Period Control Method
Calculation Method
Select one of the following depreciation calculation methods:
Acquisition Value/Useful Life
Percentage of Acquisition Value
If you select this method, you must specify a percentage in the Annual Percentage field.
Net Book Value/Remaining Life
Annual Percentage
Enter the annual percentage rate for the depreciation calculation.
 Note
The field is available only if you have selected Percentage of Acquisition Value in the Calculation Method field.
Depreciation Period
Select one of the following:
Standard – Enables you to specify a factor for depreciation calculation that can be applied to all periods of an asset's
useful life.
To specify the factor, enter a value in the Factor field.
Individual – Enables you to specify multiple factors for depreciation calculation that can be applied to different periods of
an asset's useful life.
To specify the factors, open the Depreciation Period Control window by choosing the Period Control pushbutton in the
Asset Master Data window.
To define a default factor for all periods, enter a value in the Factor field.
Factor
Do one of the following:
If you have selected Standard in the Depreciation Period field, enter a factor for depreciation calculation that is applied to
all periods of an asset's useful life.
If you have selected Individual in the Depreciation Period field, enter a factor for depreciation calculation that is taken as
the default factor for all periods. You can change the factor in the Depreciation Period Control window opened from the
asset master data.
 Note
With the straight line period control method, the factor also has an effect on the remaining life of an asset.
For example, one asset has a planned useful life of 60 months and depreciates using the standard period control method with a
factor of 1.5. After the first year, the asset is considered having passed 18 months (12 * 1.5) of its useful life and its remaining life
is 42 months instead of 48 months.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:03 AM
For more information, refer to the two examples below.
Factor Only Relevant to First Fiscal Year
 Note
The checkbox is available only if you have selected Standard in the Depreciation Period field.
Indicates that the factor you specified is effective only in the first fiscal year of an asset's useful life.
Once you select the checkbox, the system calculates the asset depreciation in the first year of its useful life with the specified
factor. In the following years, the system does not consider the factor when calculating the asset depreciation.
 Example
Standard Period Control
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Straight Line Period Control
Calculation Base: Yearly
Depreciation Period: Standard
Factor: 2
Capitalization Date: January 1st, 2010
The asset depreciation is calculated in different ways, depending on the different calculation methods.
Acquisition Value/Total Useful Life
The system calculates the monthly depreciation as follows:
60000 USD / 60 * 12 * 2 / 12 = 2000 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
2011 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
2012 2000 2000 2000 2000 2000 2000
2013
2014
Percentage of Acquisition Value
Annual Percentage = 20%
The system calculates the monthly depreciation as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:03 AM
60000 USD * 20% * 2 / 12 = 2000 USD
|   Jan. | Feb. Mar. | Apr. May | Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| ------ | --------- | -------- | --------- | --------- | --------- | ---- |
2010 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
2011 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
| 2012 2000 | 2000 2000 | 2000 2000 | 2000   |     |     |     |
| --------- | --------- | --------- | ------ | --- | --- | --- |
| 2013      |           |           |        |     |     |     |
| 2014      |           |           |        |     |     |     |
Net Book Value/Remaining Life
The system calculates the monthly depreciation for each year as follows:
2010
60000 USD / 60 * 12 * 2 / 12 = 2000 USD
2011
As the depreciation amount in 2010 equals two years' depreciation amount calculated with the straight line
method, the asset is considered having passed two years of its useful life at the end of 2010. Therefore, the
monthly depreciation of year 2011 is calculated as follows:
(60000 USD – 2000 USD * 12) * 2 / (60 – 12 * 2) = 2000 USD
2012
As the depreciation amount in the first two years equals four years' depreciation amount calculated with the
straight line method, the asset is considered having passed four years of its useful life at the end of 2011.
Therefore, the monthly depreciation of year 2012 is calculated as follows:
(60000 USD – 2000 USD * 12 * 2) * 2 / (60 – 12 * 4) = 2000 USD
At this rate, the asset is fully depreciated after the first six months in 2012.
|     | Jan. Feb. | Mar. Apr. | May Jun. | Jul. Aug. | Sep. Oct. | Nov. Dec. |
| --- | --------- | --------- | -------- | --------- | --------- | --------- |
2010 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
2011 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
| 2012 | 2000 2000 | 2000 2000 | 2000 2000 |     |     |     |
| ---- | --------- | --------- | --------- | --- | --- | --- |
| 2013 |           |           |           |     |     |     |
| 2014 |           |           |           |     |     |     |
With all the above calculation methods, the asset depreciates twice as quickly as with the straight line method, and the overall
useful life of the asset is shortened to 30 months as a result.
  Example
Individual Period Control
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:03 AM
Asset Y
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Straight Line Period Control
Depreciation Period: Individual
Capitalization Date: January 1st, 2010
Depreciation Period Control
|              | Jan. Feb. | Mar. Apr. | May Jun. | Jul. Aug. | Sep. | Oct. Nov. Dec. |
| ------------ | --------- | --------- | -------- | --------- | ---- | -------------- |
| Depreciation | Yes       | Yes       | Yes      | Yes       | Yes  |   Yes          |
| Factor       | 2         | 2         | 2        | 2         | 2    |   2            |
The asset depreciation is calculated in different ways, depending on the different calculation bases and methods.
Calculation Base: Yearly
Calculation Method: Acquisition Value/Total Useful Life
The system calculates the yearly depreciation as follows:
60000 USD / 60 * (2 + 2 + 2 + 2 + 2 + 2) = 12000 USD
Each year, the 12,000 USD is allocated to the six months as follows:
|      | Jan. Feb. | Mar. Apr. May | Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| ---- | --------- | ------------- | --------- | --------- | --------- | ---- |
| 2010 | 2000      | 2000   2000   |   2000    |   2000    |   2000    |      |
| 2011 | 2000      | 2000   2000   |   2000    |   2000    |   2000    |      |
| 2012 | 2000      | 2000   2000   |   2000    |   2000    |   2000    |      |
| 2013 | 2000      | 2000   2000   |   2000    |   2000    |   2000    |      |
| 2014 | 2000      | 2000   2000   |   2000    |   2000    |   2000    |      |
Calculation Base: Monthly
Calculation Method: Percentage of Acquisition Value
Annual Percentage = 20%
The system first calculates the monthly percentage as follows:
20% / 12 = 1.67%
Then, the depreciation for the months with a factor of 2 is calculated as follows:
60000 USD * 1.67% * 2 = 2004 USD
To make sure the depreciation does not cause the asset's book value to fall below zero, the depreciation in the last
month of the asset's useful life is calculated as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:03 AM
60000 USD – [2004 USD * (6 * 4 + 5)] = 1884 USD
|   Jan.    | Feb. Mar. | Apr. May | Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| --------- | --------- | -------- | --------- | --------- | --------- | ---- |
| 2010 2004 |   2004    |   2004   |   2004    |   2004    |   2004    |      |
| 2011 2004 |   2004    |   2004   |   2004    |   2004    |   2004    |      |
| 2012 2004 |   2004    |   2004   |   2004    |   2004    |   2004    |      |
| 2013 2004 |   2004    |   2004   |   2004    |   2004    |   2004    |      |
| 2014 2004 |   2004    |   2004   |   2004    |   2004    |   1884    |      |
Calculation Base: Monthly
Calculation Method: Net Book Value/Remaining Life
The system calculates the depreciation for each month as follows:
2010: January
60000 USD / 60 * 2 = 2000 USD
2010: March
As the depreciation amount in January equals two months' depreciation amount calculated with the straight line
method, the asset is considered having passed two months of its useful life in March. Therefore, the depreciation
of March is calculated as follows:
(60000 USD – 2000 USD) / (60 – 1 * 2) * 2 = 2000 USD
2010: May
As the depreciation amount in January and March equals four months' depreciation amount calculated with the
straight line method, the asset is considered having passed four months of its useful life in May. Therefore, the
depreciation of May is calculated as follows:
(60000 USD – 2000 USD * 2) / (60 – 1 * 4) * 2 = 2000 USD
...
|   Jan.    | Feb. Mar. | Apr. May | Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| --------- | --------- | -------- | --------- | --------- | --------- | ---- |
| 2010 2000 |   2000    |   2000   |   2000    |   2000    |   2000    |      |
| 2011 2000 |   2000    |   2000   |   2000    |   2000    |   2000    |      |
| 2012 2000 |   2000    |   2000   |   2000    |   2000    |   2000    |      |
| 2013 2000 |   2000    |   2000   |   2000    |   2000    |   2000    |      |
| 2014 2000 |   2000    |   2000   |   2000    |   2000    |   2000    |      |
More Information
Depreciation Types - Setup Window: Calculation Tab
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:03 AM
Depreciation Period Control Window
Declining Balance Method
The declining balance method entails higher depreciation charges at the beginning of an asset's useful life and gradually
decreasing charges in subsequent periods. Each year, the depreciation is calculated using the same constant percentage rate. In
the first year, the system calculates the depreciation based on the asset's acquisition and production costs. In the following years,
the calculation is based on the asset's remaining net book value.
As you can never reach a net book value of zero using this method, the system can switch to straight line depreciation towards the
end of the useful life.
The depreciation amount determined in this way must not exceed a specified upper limit. This limit is the depreciation amount
that is calculated with the straight line method, multiplied by a factor.
Percentage
Do one of the following:
If you have selected Yearly in the Calculation Base field, enter the annual percentage rate for the depreciation calculation.
If you have selected Monthly in the Calculation Base field, enter the monthly percentage rate for the depreciation
calculation.
Factor
Enter the factor for calculating the upper limit of an asset's depreciation amount in each period. The upper limit is calculated using
the straight-line method and multiplied by this factor. For example, the upper limit of an asset's annual depreciation is calculated
with the following formula:
(Net Book Value – Salvage Value) * [1 / (Total Useful Life / 12)] * Factor
 Note
If an asset's depreciation amount exceeds the upper limit, SAP Business One uses the upper limit as the depreciation amount
instead.
 Example
Asset X
Acquisition and Production Costs: 1,000 USD
Useful Life: 120 Months
Depreciation Method: Declining Balance
Calculation Base: Yearly
Percentage: 20%
Factor: 2.5
Automatically Change To: Depreciation Type 01 (Method = Straight Line, Calculation Method = Net Book Value/Remaining Life)
Capitalization Date: April 1st, 2010
Subsequent Acquisition: October 1st, 2010 with 500 USD
The system calculates the depreciation in the first year of the asset's useful life as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:03 AM
April 1st, 2010 – September 30th, 2010
The system first calculates the standard depreciation amount according to the declining balance method as follows:
1000 USD * 20% / 12 * 6 = 100 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor as follows:
1000 USD * 10% * 2.5 / 12 * 6 = 125 USD
Since the standard depreciation amount does not exceed the upper limit, the system takes 100 USD as the asset's
depreciation amount in the first half year of its useful life.
October 1st, 2010 – March 31, 2011
 Note
When an asset transaction takes place after the depreciation starts and the asset uses the yearly calculation base, SAP
Business One recalculates the standard depreciation amount and the upper limit using different criteria as follows:
For the calculation of the standard depreciation amount, SAP Business One does not subtract the depreciation
of the periods prior to the asset transaction in the same fiscal year.
For the calculation of the upper limit, SAP Business One subtracts the depreciation of the periods prior to the
asset transaction in the same fiscal year.
For more information, see the calculations below, which resulted from the asset's subsequent acquisition.
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
(1000 USD + 500 USD) * 20% / 12 * 6 = 150 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
(1000 USD + 500 USD – 100 USD) / * 10% * 2.5 / 12 * 6 = 175 USD
Since the standard depreciation amount does not exceed the upper limit, the system takes 150 USD as the asset's
depreciation amount in the second half year of its useful life.
As a result, the asset's depreciation in year 2010 is as follows:
100 USD + 150 USD = 250 USD
Automatically Change to
If required, specify a depreciation type with the straight line method as the alternative depreciation type.
After you specify a depreciation type with the straight line method, the system compares the depreciation amounts between the
declining balance and straight line methods. When the depreciation amount calculated with the declining balance method falls
below the straight line depreciation amount in a point of an asset's life, SAP Business One automatically switches to the straight
line depreciation from that point on.
If you leave the field empty, SAP Business One depreciates the asset according to the declining balance method till the stopping
point.
 Recommendation
Do not specify a depreciation type that does not use the straight line method. If you do so, SAP Business One always calculates
the depreciation of an asset as zero.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:03 AM
Declining Balance Depreciation Without Alternative Method
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Declining Balance
Calculation Base: Yearly
Percentage: 40%
Factor: 2
Automatically Change To: None
Capitalization Date: January 1st, 2010
The system calculates the depreciation for each year as follows:
2010
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
60000 USD * 40% = 24000 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
60000 USD * [1 / (60 / 12)] * 2 = 24000 USD
Since the standard depreciation amount is equal to the upper limit, the system takes 24,000 USD as the asset's
depreciation amount in 2010.
Therefore, the monthly deprecation in 2010 is 2,000 USD.
2011
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
(60000 USD – 24000 USD) * 40% = 14400 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
(60000 USD – 24000 USD) * [1 / (60 / 12)] * 2 = 14400 USD
Since the standard depreciation amount is equal to the upper limit, the system takes 14,400 USD as the asset's
depreciation amount in 2011.
Therefore, the monthly depreciation in 2011 is 1,200 USD.
2012
The system calculates the standard depreciation amount and the upper limit, and gets the same result, as follows:
(60000 USD – 24000 USD – 14400 USD) * 40% = 8640 USD
Therefore, the monthly depreciation in 2012 is 720 USD.
2013
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:03 AM
The system calculates the standard depreciation amount and the upper limit, and gets the same result as follows:
(60000 USD – 24000 USD – 14400 USD – 8640 USD) * 40% = 5184 USD
Therefore, the monthly depreciation in 2013 is 432 USD.
2014
In order to fully depreciate the asset in the last year of its useful life, the system calculates the depreciation as follows:
60000 USD – 24000 USD – 14400 USD – 8640 USD – 5184 USD = 7776 USD
Therefore, the monthly depreciation in 2014 is 648 USD.
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000 2000
2011 1200 1200 1200 1200 1200 1200 1200 1200 1200 1200 1200 1200
2012 720 720 720 720 720 720 720 720 720 720 720 720
2013 432 432 432 432 432 432 432 432 432 432 432 432
2014 648 648 648 648 648 648 648 648 648 648 648 648
 Example
Declining Balance Depreciation With an Alternative Method
Asset Y
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Declining Balance
Calculation Base: Monthly
Percentage: 3%
Factor: 5
Automatically Change To: Depreciation Type 01 (Method = Straight Line; Calculation Base = Monthly; Calculation Method =
Acquisition Value/Total Useful Life)
Capitalization Date: January 1st, 2010
According to the alternative method, the monthly depreciation amount is 1,000 USD (60000 USD/60). Therefore, once the
standard depreciation amount falls below 1,000 USD, the system automatically switches to the alternative method.
Starting from January 1st, 2010, the asset depreciates as follows:
2010: January
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
60000 USD * 3% = 1800 USD
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:03 AM
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
60000 USD * (1 / 60) * 5 = 5000 USD
Since the standard depreciation amount is less than the upper limit, the system takes 1,800 USD as the asset's
depreciation amount in January.
2010: February
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
(60000 USD – 1800 USD) * 3% = 1746 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
(60000 USD – 1800 USD) * (1 / 60) * 5 = 4850 USD
Since the standard depreciation amount is less than the upper limit, the system takes 1,746 USD as the asset's
depreciation amount in February.
2010: March
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
(60000 USD – 1800 USD – 1746 USD) * 3% = 1693.62 USD
Then, the system calculates the upper limit using the straight line depreciation multiplied by the factor, as follows:
(60000 USD – 1800 USD – 1746 USD) * (1/60) * 5 = 4704.50 USD
Since the standard depreciation amount is less than the upper limit, the system takes 1,693.62 USD and rounds it to
1694 USD as the asset's depreciation amount in March.
...
2011: September
The system first calculates the standard depreciation amount according to the declining balance method, as follows:
(60000 USD – 27372 USD) * 3% = 978.84 USD
As the depreciation amount falls below 1,000 USD, which is calculated with the alternative straight line method, the
system switches to straight line depreciation from this month.
...
2014: May
At the beginning of May 2014, the asset's accumulated depreciation has reached 59,372 USD, and its net book value is
only 628 USD. Therefore, the asset can only depreciates 628 USD in May.
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1800 1746 1694 1643 1594 1546 1499 1454 1411 1368 1327 1288
2011 1249 1211 1175 1140 1106 1072 1040 1009 1000 1000 1000 1000
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 1000 1000 1000 1000 628
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:03 AM
More Information
Depreciation Types - Setup Window: Calculation Tab
Multilevel Method
With the multilevel method, you can view an asset's useful life as several phases and depreciate the asset by a defined rate for
each phase. This way, the asset can have a course of depreciation that changes in levels over time. SAP Business One lets you
break down an asset's useful life into multiple phases, for each of which you can specify a depreciation rate and a validity period.
Multilevel Method
Level
Displays the level of depreciation. SAP Business One lets you specify multiple levels, with each level representing a phase in an
asset's useful life.
Base
Select one of the following as the base for the depreciation calculation in each phase:
Acquisition Value
The annual depreciation in each phase is calculated using the following formula:
(Acquisition Value – Salvage Value) * Annual Percentage
Net Book Value
The annual depreciation in each phase is calculated using the following formula:
(Net Book Value – Salvage Value) * Annual Percentage
Number of Years
Enter the number of years in each phase.
You can enter integers only.
Annual Percentage
Enter the annual percentage rate for the depreciation calculation that is valid for each phase.
 Example
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Multilevel
Calculation Base: Yearly
Capitalization Date: January 1st, 2010
Calculation
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:03 AM
| Level | Base              |     | Number of Years | Annual Percentage |     |     |
| ----- | ----------------- | --- | --------------- | ----------------- | --- | --- |
| 1     | Acquisition Value |     | 2               | 35                |     |     |
| 2     | Acquisition Value |     | 3               | 10                |     |     |
The system calculates the depreciation as follows:
2010 – 2011
Each year, the depreciation is calculated as follows:
60000 USD * 35% = 21000 USD
Therefore, the monthly deprecation is 1,750 USD.
2012 – 2014
Each year, the depreciation is calculated as follows:
60000 USD * 10% = 6000 USD
Therefore, the monthly depreciation is 500 USD.
|   Jan. | Feb. Mar. | Apr. | May Jun. Jul. | Aug. Sep. | Oct. Nov. | Dec. |
| ------ | --------- | ---- | ------------- | --------- | --------- | ---- |
2010 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750
2011 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750 1750
| 2012 500 | 500 500 | 500 | 500 500 500 | 500 500 | 500 500 | 500 |
| -------- | ------- | --- | ----------- | ------- | ------- | --- |
| 2013 500 | 500 500 | 500 | 500 500 500 | 500 500 | 500 500 | 500 |
| 2014 500 | 500 500 | 500 | 500 500 500 | 500 500 | 500 500 | 500 |
  Example
Asset Y
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Multilevel
Calculation Base: Monthly
Capitalization Date: January 1st, 2010
Calculation
| Level | Base           |     | Number of Years | Annual Percentage |     |     |
| ----- | -------------- | --- | --------------- | ----------------- | --- | --- |
| 1     | Net Book Value |     | 2               | 35                |     |     |
| 2     | Net Book Value |     | 3               | 10                |     |     |
The system calculates the depreciation as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:03 AM
2010: January
60000 USD * 35% / 12 = 1750 USD
2010: February
(60000 USD – 1750 USD) * 35% / 12 = 1698.95 USD
The amount is then rounded to 1699 USD.
 Note
In the above formula, the system recalculates the annual depreciation based on the new book value in February, thereby
dividing the amount by 12 instead of 11 to get the depreciation amount of this month.
2011: March
(60000 USD – 1750 USD – 1699 USD) * 35% / 12 = 1649.40
The amount is then rounded to 1649 USD.
...
2014: December
At the beginning of December 2014, the asset's accumulated depreciation has reached 38,003 USD, and its net book
value is still 21,997 USD. Therefore, to fully depreciate the asset at the end of its useful life, the depreciation amount in
December is 21,997 USD.
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1750 1699 1649 1601 1555 1509 1465 1423 1381 1341 1302 1264
2011 1227 1191 1156 1123 1090 1058 1027 997 968 940 912 886
2012 246 244 242 240 238 236 234 232 230 228 226 224
2013 222 220 219 217 215 213 211 210 208 206 204 203
2014 201 199 198 196 194 193 191 190 188 186 185 21997
More Information
Depreciation Types - Setup Window: Calculation Tab
Immediate Write-Off Method
Immediate write-off is a depreciation method that completely writes off the depreciable value of an asset in the period when the
asset is acquired. Usually, this method is applied to low value assets.
In SAP Business One, based on different calculation bases, a low value asset can be completely written off in the acquisition month
or year. For more information, see the examples below:
 Example
Asset X
Acquisition and Production Costs: 100 USD
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:03 AM
Useful Life: 1 Month
Depreciation Method: Immediate Write-Off
Calculation Base: Yearly
Capitalization Date: January 1st, 2010
As the total useful life of the asset is 1 month, the asset must be completely written off in this month. Therefore, the
depreciation amount in January is 100 USD.
 Example
Asset Y
Acquisition and Production Costs: 100 USD
Useful Life: 2 Months
Depreciation Method: Immediate Write-Off
Capitalization Date: January 1st, 2010
The asset depreciation can be different based on different calculation bases, as follows:
Calculation Base – Yearly
The asset must be completely written off in year 2010. Therefore, the asset is depreciated by 50 USD each month in
January and February.
Calculation Base – Monthly
The asset must be completely written off in the first month of its useful life. Therefore, the asset is depreciated by 100
USD in January.
More Information
Depreciation Types - Setup Window: Calculation Tab
Special Depreciation Method
In many countries, you are allowed to carry out special depreciations for your fixed assets. Usually, a certain percentage of the
asset value can be depreciated in addition to the normal depreciation amount. The percentage allowed for the special
depreciation, as well as the period over which you can carry out the special depreciation, are dependent on national legislation.
 Note
In SAP Business One, special depreciation is always carried out in the first period of the concession years. For more
information, see the examples below.
Special Depreciation Method
Calculation Method
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:03 AM
Displays Additional, which suggests that special depreciation is always calculated in addition to the standard depreciation
amount.
Pool of Depreciation Type
From the dropdown list, select a pool to which you want to assign the depreciation type.
You must assign a special or manual depreciation type to a pool.
Normal Depreciation
Specify a depreciation type that is used for the regular automatic depreciation of an asset.
You must specify a depreciation type whose method is not special depreciation.
Alternative Depreciation
To compare different depreciation calculations, specify a second depreciation type here. The system calculates the depreciation
for this depreciation type in parallel. The result of the alternative calculation is for reference only, and no bookings are carried out
in the general ledger.
 Recommendation
You can specify the same depreciation type for the normal and alternative depreciation. This way, you can compare the asset
depreciation with and without the special depreciation.
Concession Period (Years)
Enter the number of years during which the special depreciation is legally permitted.
You can enter integers only.
Maximum Percentage
If required, enter the percentage rate for calculating the maximum depreciation amount allowed in addition to the normal
depreciation. National legislation specifies this value.
The system calculates the maximum special depreciation amount as follows:
(Acquisition and Production Costs – Salvage Value) * Maximum Percentage
Maximum Amount
If required, enter the maximum depreciation amount allowed in addition to the normal depreciation. The maximum amount is an
alternative to the maximum percentage.
To optimize depreciation from a tax point of view, you can split the concession period into multiple sub-periods and freely
distribute the maximum percentage over these periods.
Number of Years
Specify the number of years in each period.
You can enter integers only.
 Note
The total number of years you enter must not exceed the concession period.
Annual Percentage
Enter the annual percentage rate for the special depreciation calculation.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:03 AM
 Note
The total percentage rate of all periods must not exceed the maximum percentage.
Amount
Enter the annual special depreciation amount.
 Note
The total amount for all periods must not exceed the maximum amount.
 Example
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Type: Special Depreciation
Calculation Base: Yearly
Normal Depreciation: Depreciation Type 02 (Method = Straight Line; Calculation Base = Yearly; Calculation Method = Net Book
Value/Remaining Life)
Capitalization Date: January 1st, 2010
Concession Period: 2 Years
Maximum Percentage: 30
Level Number of Years Annual Percentage
1 2 15
The system calculates the asset depreciation as follows:
2010–2011
The system first calculates the normal depreciation in 2010 and 2011 as follows:
2010: 60000 USD / 60 * 12 = 12000 USD
2011: (60000 USD – 12000 USD) / (60 – 12) * 12 = 12000 USD
Then, the special depreciation in each year is calculated as follows:
60000 USD * 15% = 9000 USD
Assuming your company's posting periods are months, SAP Business One carries out the special depreciation in the
first month of 2010 and 2011, respectively.
2012–2014
The system calculates the depreciation from 2012 to 2014 as follows:
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:03 AM
Within the concession period, the special depreciation amount does not affect the calculation of the net book value.
However, after the concession period, the calculation of the net book value takes into account the special depreciation
amount.
2012
(60000 USD – 12000 USD * 2 – 9000 USD * 2) / (60 – 12 * 2) * 12 = 6000 USD
2013
(60000 USD – 12000 USD * 2 – 9000 USD * 2 – 6000 USD) / (60 – 12 * 3) * 12 = 6000 USD
2014
60000 USD – 12000 USD * 2 – 9000 USD * 2 – 6000 USD * 2 = 6000 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 10000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 10000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2012 500 500 500 500 500 500 500 500 500 500 500 500
2013 500 500 500 500 500 500 500 500 500 500 500 500
2014 500 500 500 500 500 500 500 500 500 500 500 500
 Example
Asset Y
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Type: Special Depreciation
Calculation Base: Yearly
Normal Depreciation: Depreciation Type 02 (Method = Straight Line; Calculation Base = Yearly; Calculation Method = Net Book
Value/Remaining Life)
Capitalization Date: January 1st, 2010
Concession Period: 2 Years
Maximum Amount: 20,000 USD
Level Number of Years Amount
1 2 10000
The system calculates the asset depreciation as follows:
2010–2011
The system calculates the normal depreciation in 2010 and 2011 as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:03 AM
2010: 60000 USD / 60 * 12 = 12000 USD
2011: (60000 USD – 12000 USD) / (60 – 12) * 12 = 12000 USD
The special depreciation in each year is 10,000 USD.
Assuming your company's posting periods are months, SAP Business One carries out the special depreciation in the
first month of 2010 and 2011, respectively.
2012–2014
The system calculates the depreciation from 2012 to 2014 as follows:
 Note
Within the concession period, the special depreciation amount does not affect the calculation of the net book value.
However, after the concession period, the calculation of the net book value takes into account the special depreciation
amount.
2012
(60000 USD – 12000 USD * 2 – 10000 USD * 2) / (60 – 12 * 2) * 12 = 5333.33 USD
The system rounds 5,333.33 USD to 5,333 USD.
2013
(60000 USD – 12000 USD * 2 – 10000 USD * 2 – 5333 USD) / (60 – 12 * 3) * 12 = 5333.33 USD
The system rounds 5,333.33 USD to 5,333 USD.
2014
60000 USD – 12000 USD * 2 – 10000 USD * 2 – 5333 USD * 2 = 5334 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 11000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 11000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2012 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.38
2013 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.42 444.38
2014 444.50 444.50 444.50 444.50 444.50 444.50 444.50 444.50 444.50 444.50 444.50 444.50
More Information
Depreciation Types - Setup Window: Calculation Tab
Manual Depreciation Method
Use this depreciation method for one-off depreciations.
With this depreciation method, you do not need to specify any calculation methods. Instead, you enter the depreciation amount
directly when you create the manual depreciation documents. For more information, see Manual Depreciation.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:03 AM
 Note
You cannot assign depreciation types with the manual depreciation method to any asset or asset class.
SAP Business One lets you use these depreciation types only when you create manual depreciations.
Manual Depreciation Method
Reduce Depreciation Base
To let manual depreciation affect the calculation of an asset's planned depreciation, select this checkbox.
After you select the checkbox, the system automatically reduces the depreciation base by the manual depreciation amount.
The reduction of the depreciation base only applies to the fiscal year during which the manual depreciation takes place. For more
information, see the examples below.
 Note
The reduction applies to an asset only when the asset uses the acquisition and production costs as the base for the planned
depreciation calculation. If the asset uses the net book value as the base, the manual depreciation amount is deducted anyway.
In addition, the reduction only takes places in the fiscal year during which the manual depreciation occurs.
For more information, see the examples below.
Pool of Depreciation Type
From the dropdown list, select a pool to which you want to assign the depreciation type.
You must assign a special or manual depreciation type to a pool.
Example
Asset X
Acquisition and Production Costs: 60,000 USD
Useful Life: 60 Months
Depreciation Method: Straight Line
Calculation Base: Yearly
Calculation Method: Acquisition Value/Total Useful Life
Capitalization Date: January 1st, 2010
On January 1st, 2011, you created a manual depreciation for the asset with a worth of 2,000 USD.
The system calculates the depreciation differently, depending on the settings of the manual depreciation type.
Reduce Depreciation Base checkbox: Selected
2010
60000 USD / 60 * 12 = 12000 USD
2011
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:03 AM
In January, the asset was manually depreciated by 2,000 USD. In this case, the depreciation base (the acquisition
and production costs) of this year is reduced by 2,000 USD as follows:
60000 USD – 2000 USD = 58000 USD
Therefore, the standard depreciation in this year is calculated as follows:
58000 USD / 60 * 12 = 11600 USD
2012
As the manual depreciation amount only affects the depreciation base in 2011, the depreciation in 2012 is still
calculated as follows:
60000 USD / 60 * 12 = 12000 USD
2013
60000 USD / 60 * 12 = 12000 USD
2014
The system calculates the book value of the asset as follows:
60000 USD – 12000 USD * 3 – 2000 USD – 11600 USD = 10400 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 2966.67 966.67 966.67 966.67 966.67 966.67 966.67 966.67 966.67 966.67 966.67 966.63
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 866.67 866.67 866.67 866.67 866.67 866.67 866.67 866.67 866.67 866.67 866.67 866.63
Reduce Depreciation Base checkbox: Unselected
2010
60000 USD / 60 * 12 = 12000 USD
2011
The system still calculates the standard depreciation in this year as follows:
60000 USD / 60 * 12 = 12000 USD
In addition, in January, the asset was manually depreciated by 2,000 USD.
2012
60000 USD / 60 * 12 = 12000 USD
2013
60000 USD / 60 * 12 = 12000 USD
2014
The system calculates the book value of the asset as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:03 AM
60000 USD – 12000 USD * 4 – 2000 USD = 10000 USD
Jan. Feb. Mar. Apr. May Jun. Jul. Aug. Sep. Oct. Nov. Dec.
2010 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2011 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2012 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2013 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000 1000
2014 833.33 833.33 833.33 833.33 833.33 833.33 833.33 833.33 833.33 833.33 833.33 833.37
More Information
Depreciation Types - Setup Window: Calculation Tab
Defining and Assigning Depreciation Areas
In SAP Business One, you can define the following types of depreciation areas:
Posting to G/L
Additional area
Derived area
For each asset class, you can assign multiple depreciation areas and these depreciation areas will then be taken to all assets in the
class. With multiple depreciation areas, you can carry out different depreciation calculations for a single asset.
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
Procedure
Defining Depreciation Areas
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Depreciation
Areas .
The Depreciation Areas - Setup window opens.
2. Enter the code and description, select the type, and specify other parameters.
3. Choose Add.
Assigning Depreciation Areas to Fixed Assets
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Asset Classes .
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:03 AM
The Asset Classes - Setup window opens.
2. Specify the general information, select the depreciation areas, and specify other required fields.
3. Choose Add.
4. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
5. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
 Note
You cannot change the asset class of an asset having the status Active.
Once you specify the asset class, the associated depreciation areas are copied to the asset.
More Information
Depreciation Areas
Asset Classes
Asset Master Data
Depreciation Areas
In SAP Business One, you can use different depreciation areas for showing the value of fixed assets for a specific purpose.
 Example
Balances for tax purposes or management accounting values
SAP Business One supports the following types of depreciation areas:
Posting to G/L – The area for posting asset depreciations in the general ledger accounts.
Derived Area – The derived area of the main depreciation area. Generally, you use this area when carrying out special
depreciations.
In special depreciation, you can specify the same depreciation type for both the normal and alternative depreciation. This
way, the main depreciation area carries out the normal depreciation and the special depreciation while the derived area
carries out the normal depreciation only. You can then compare the asset depreciation with and without the special
depreciation.
The derived area is used only for information purposes, and there is no posting in the general ledger.
Additional Area – The area in addition to the posting depreciation areas. You can use this area to compare the effects of
using different depreciation areas. You can carry out an additional depreciation calculation for a different depreciation area
in parallel to the actual calculation. The parallel calculation is for information purposes only, and no posting is carried out in
the general ledger.
More Information
Depreciation Areas - Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:03 AM
Depreciation Areas - Setup Window
Use this window to create, update, and view depreciation areas.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Depreciation Areas .
Depreciation Areas - Setup Window Fields
Code
Enter a unique code for the depreciation area.
Description
If required, enter a description of the depreciation area.
Type
Select one of the following types for the depreciation area:
Posting to G/L – In this area, the asset depreciation is posted to the general ledger accounts.
Additional Area – In this area, the asset depreciation is not posted to the general ledger accounts. The depreciation carried
out in this area is for information purposes only.
Derived Area – The derived area of the main depreciation area. Generally, you use this area when carrying out special
depreciations.
In special depreciation, you can specify the same depreciation type for both the normal and alternative depreciation. This
way, the main depreciation area carries out the normal depreciation and the special depreciation, while the derived area
carries out the normal depreciation only. You can then compare the asset depreciation with and without the special
depreciation. For more information, see Special Depreciation Method.
The derived area is used only for information purposes, and there is no posting in the general ledger.
 Note
SAP Business One lets you create only one depreciation area with the Derived Area type.
Main Depreciation Area
Select the checkbox to indicate that the depreciation area is the main depreciation area.
 Note
SAP Business One lets you create one main depreciation area only.
Derived Depreciation Area
 Note
The field is available only if the following conditions are met:
The depreciation area has the Posting to G/L type.
The depreciation area is the main depreciation area.
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:03 AM
From the dropdown list, select the derived depreciation area of the main depreciation area.
Posting of Depreciation
 Note
The field is available only for the depreciation areas with the Posting to G/L type.
Select one of the following depreciation posting methods:
Direct Posting – The system posts the asset depreciation directly in the asset balance sheet account.
Indirect Posting – The system posts the asset depreciation in the accumulated depreciation accounts and transfers the
depreciation to the revaluation account only when the asset is retired.
Posting of Retirement
 Note
The field is available only for the depreciation areas with the Posting to G/L type.
Select one of the following retirement posting methods:
Gross – The system does not post the profits or losses during asset retirement to any general ledger accounts.
Net – The system posts the profits and losses during asset retirement to corresponding general ledger accounts.
More Information
Depreciation Areas
Defining and Assigning Asset Attributes
In SAP Business One, you can define different groups of attributes for your fixed assets. By assigning an attribute group to an asset
class, you can, therefore, link the attributes to your fixed assets.
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
Procedure
Defining Attributes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Attribute Groups
.
The Attribute Groups - Setup window opens.
2. Enter the description, activate the attributes that you want to use, and enter the attribute names and default values.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:03 AM
If you want to adjust the order of the attributes, use the Move Up orMove Down pushbutton.
3. Choose Add.
Assigning Attributes to Fixed Assets
1. From the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets Asset Classes .
The Asset Classes - Setup window opens.
2. Specify the general information and select the attribute group that you want to assign to the asset class.
3. Choose Add.
4. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
5. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
 Note
You cannot change the asset class of an asset having the status Active.
Once you specify the asset class, the associated attribute group is linked to the asset. As a result, the active attributes in
the group are copied to the Attributes subtab, displayed in the order that was specified in the Attribute Groups - Setup
window.
More Information
Attribute Groups - Setup Window
Asset Classes
Asset Master Data
Attribute Groups - Setup Window
Use this window to set up different groups of attributes for your fixed assets.
In each group, you can define up to 64 attributes of different types, as follows:
Type Number of Attributes
Text 32
Numeric 10
Date 5
Amount 7
Price 5
Quantity 5
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:03 AM
By assigning an attribute group to an asset class, you can, therefore, link the attribute group to your fixed assets. The active
attributes in the group will then be displayed in Asset Master Data Window - Fixed Assets Tab: Attributes Subtab.
To open this window, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Attribute Groups .
Attribute Groups - Setup Window Fields
Name
Enter a name of up to 100 characters for the attribute group.
Attribute Name
 Note
The field is editable only if you have selected the Active checkbox in the row.
Enter a name of up to 100 characters for the attribute.
Attribute Value
 Note
The field is editable only if you have selected the Active checkbox in the row.
If required, enter an attribute value of up to 100 characters.
The value you enter here is taken to the asset master data as the default attribute value.
 Example
Attribute Name – Color
Attribute Value – Black
If you assign the asset group to an asset class, the attribute Color and the default value Black will be taken to the master data
of all assets in the class.
Field Type
Displays the predefined type of the attribute field.
You cannot change the type.
Active
Activates the attribute.
You can then specify the attribute name and value.
 Note
Once you assign the attribute group to an asset class, the active attributes in the group are taken to the master data of all
assets in the class.
Move Up, Move Down
Use these two pushbuttons to adjust the order of the attributes.
To move an attribute upward in the list, select the attribute row and choose the Move Up pushbutton.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:03 AM
Likewise, to move an attribute downward in the list, select the attribute row and choose the Move Down pushbutton.
SAP Business One lets you select multiple rows with the Shift or Ctrl key on your keyboard.
 Note
Once you assign the attribute group to an asset class, the active attributes in the group are taken to the asset master data,
displayed in the order specified in the Attribute Groups - Setup window.
More Information
Asset Classes - Setup Window
Asset Master Data Window - Fixed Assets Tab: Attributes Subtab
Asset Classes - Setup Window
Use this window to create, update and view asset classes.
To open this window, from the SAP Business One Main Menu, choose Administration Setup Financials Fixed Assets
Asset Classes .
General Area Fields
Code
Enter a unique code for the asset class.
Description
If required, enter a description of the asset class.
Asset Type
Select one of the following asset types:
General – Select this option for regular assets.
Low Value Asset – Select this option for low value assets.
Value Limit From
 Note
The field is available only if you have selected Low Value Asset in the Asset Type field.
Enter the lower limit for low value assets.
Value Limit To
 Note
The field is available only if you have selected Low Value Asset in the Asset Type field.
Enter the upper limit for low value assets.
Attribute Group
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:03 AM
From the dropdown list, select the attribute group that you want to assign to the asset class.
By default, Default Attribute Group is selected. The default attribute group contains the following four predefined attributes:
Remark 1
Remark 2
Amount 1
Amount 2
Table Area Fields
Depreciation Area
Specify the depreciation areas for the asset class.
 Note
You must specify at least one main depreciation area.
Active
Select the checkbox to indicate that the depreciation area is active for the asset class.
The system calculates the asset depreciation in all active depreciation areas.
 Note
At least one depreciation area must be active.
Account Determination
Specify the account determination for the Posting to G/L type of depreciation areas.
Depreciation Type
Specify the depreciation type in the depreciation area.
Later, when you assign the asset class to an asset, you can still change the depreciation type in the asset master data.
 Note
For the derived depreciation area, you cannot specify a depreciation type.
Useful Life (Months)
Enter the useful life in months for the assets in this asset class.
Later, when you assign the asset class to an asset, you can still change the useful life in the asset master data.
 Note
For the derived depreciation area, you cannot specify a useful life.
More Information
Asset Classes
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:03 AM
Creating Fixed Assets
Prerequisites
1. You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
2. You have defined the following:
Account determination
Depreciation types
Depreciation areas
Attribute groups
Asset classes
Procedure
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
The Asset Master Data window opens.
2. To switch to Add mode, do one of the following:
Press Ctrl + A on your keyboard.
In the toolbar, choose .
From the menu bar, choose Data Add .
3. In the general area of the Asset Master Data window, specify the item number and other required information.
4. On the Fixed Assets tab, Overview subtab, specify the asset class to which the asset belongs.
Once you specify the asset class, the following depreciation parameters of the asset class are copied to the asset as the
default:
Depreciation area
Depreciation type
Useful life
5. If required, specify other information related to the asset on the Fixed Assets tab.
6. Choose Add.
 Note
The asset is created successfully with the status New. To change its status to Active, you must capitalize the asset. For
more information, see Capitalization.
Related Information
Account Determination
Depreciation Types
Depreciation Areas
Asset Classes
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:03 AM
Asset Master Data
SAP Business One lets you manage all fixed assets in the asset master data.
You can create, update, and delete a fixed asset using the asset master data. After an asset is capitalized, you can view and
maintain the asset depreciation details in the asset master data.
More Information
Asset Master Data Window - General Area
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
Asset Master Data Window - General Area
The general area of the Asset Master Data window has the same fields as the general area of the Item Master Data window, except
for the following fields.
Virtual Item
 Note
This checkbox is available only if you use numbering series for asset master data. By default, this checkbox is unselected.
Select the checkbox to indicate the asset is a virtual item used for bulk purchase.
Virtual items can be capitalized by A/P invoices only. Once you have used a virtual item in an A/P invoice, the checkbox becomes
non-editable.
Enforce Serial Numbers
 Note
This checkbox is available only if you have selected the Virtual Item checkbox. By default, this checkbox is unselected.
Select the checkbox to enforce the use of serial numbers for fixed assets generated by virtual items. This means, when you
purchase assets by using virtual items in A/P invoices, you must specify a serial number for each generated asset.
Asset Master Data Window - Fixed Assets Tab
Use this tab to view and maintain the asset data.
To access the tab, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data and select
the Fixed Assets tab.
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:03 AM
The Fixed Assets tab contains the following subtabs:
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
More Information
Asset Master Data
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
This subtab provides an overview of the most important data for a fixed asset and its depreciation parameters.
To access the subtab, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data . Select
the Fixed Assets tab and then the Overview subtab.
General Area Fields
Status
Displays the asset's status as one of the following:
New – Indicates the asset has been manually created and has not yet been capitalized.
Active – Indicates the asset has been capitalized and is active.
Inactive – Indicates the asset has been retired and is now inactive.
When you create an asset, the system automatically marks the asset as New. After you capitalize the asset, the status changes
from New to Active. After the asset is retired, either by sales or scrapping, the status automatically changes from Active to
Inactive.
Asset Class
Specify the asset class to which the asset belongs.
After you assign an asset class to the asset, the following depreciation parameters of the asset class are copied to the asset as the
defaults:
Depreciation area
Depreciation type
Useful life
To view the details of the asset class, click to the left of the field.
Asset Group
Specify the asset group to which the asset belongs.
To define new asset groups, open the Asset Groups - Setup window by selecting Define New from the dropdown list.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:03 AM
Inventory No.
If required, enter the inventory number of the asset.
You can use the inventory number as an alternative to the asset number. This enables you to retain previously used numbers when
transferring legacy fixed asset data, for example, from the Fixed Assets add-on.
 Example
If a fixed asset has a specific number in the add-on, you can assign a new number to the asset while keeping the old number as
the inventory number in SAP Business One.
Serial Number
If required, enter the serial number of the asset.
Location
If required, select the location of the asset from the dropdown list.
To define new locations, open the Locations - Setup window by selecting Define New from the dropdown list.
Technician
If required, assign an employee for maintenance of the asset.
Employee
If required, specify an employee to whom the asset is physically assigned.
Capitalization Date
Specify the date on which the asset is capitalized.
You can manually specify and update the date before the capitalization actually takes place. Alternatively, SAP Business One can
automatically fill the date when you capitalize the asset upon the creation of either of the following documents:
Capitalization
A/P invoice
The system takes the asset value date from the document and uses it as the asset's capitalization date.
Statistical Asset
Select the checkbox to indicate the asset is only a statistical asset that is not owned by your company.
Cession
Select the checkbox to indicate the asset is owned by your company but financed by a bank mortgage.
Depreciation Area
Select the depreciation area in which you want to view the asset depreciation details.
You can view the depreciation only in the areas that are defined in the asset class.
Fiscal Year
Select the fiscal year for which you want to view the asset depreciation details.
The default value is the current fiscal year. Once you change the fiscal year, the system automatically recalculates the depreciation
and updates the asset-relevant values.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:03 AM
 Note
SAP Business One lets you view the asset depreciation details of each year throughout the asset's useful life. However, the
system carries forward the depreciation values of a fiscal year only when the fiscal year change has taken place. If no values are
displayed for the fiscal year you select, you must perform a fiscal year change.
When you change the depreciation area and fiscal year, SAP Business One automatically updates the values in the non-editable
fields from among the following:
Historical APC
If required, enter the asset's historical acquisition and production costs.
 Note
The field is not editable if either of the following situations arises:
The asset does not exist in the fiscal year you select.
You have not performed a fiscal year change for the fiscal year you select.
Acquisition and Production Costs
Displays the asset's acquisition and production costs at the end of the selected fiscal year.
Net Book Value
Displays the asset's net book value at the end of the selected fiscal year.
Historical NBV
Displays the asset's historical net book value at the end of the selected fiscal year.
Different from the net book value, the historical net book value is the net book value of the asset that is calculated without taking
into account any unplanned depreciation, appreciation, or write-up.
Ordinary Depreciation
Displays the asset's ordinary depreciation for the selected fiscal year.
Unplanned Depreciation
Displays the asset's unplanned depreciation for the selected fiscal year.
Special Depreciation
Displays the asset's special depreciation for the selected fiscal year.
Write-Up
Displays the asset's write-up for the selected fiscal year.
Salvage Value
 Note
The field is editable only when the following conditions are met:
The asset has the Active status.
You have performed the fiscal year change for the selected fiscal year, and the asset exists in the fiscal year.
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:03 AM
In the selected depreciation area, the corresponding depreciation type has a defined salvage value percentage.
Specify the asset's salvage value.
If the field is not editable, it displays the asset's salvage value.
Quantity
If the asset is planned for quantity maintenance, the field displays the quantity. Otherwise, the field is empty.
IFRS Posting for Revaluation
Indicates that this fixed asset is available for revaluation postings according to International Financial Reporting Standards (IFRS).
When you are revaluating assets, the IFRS status of the fixed asset and its revaluation must be the same. That is, if you select the
IFRS Posting checkbox in a revaluation, you can only add assets for which the IFRS Posting for Revaluation checkbox ( Asset
Master Data Fixed Assets Overview ) is selected; and vice versa.
Table Area Fields
Depreciation Area
Displays the depreciation areas you have specified in the asset class.
To view the details of the depreciation area, open the Depreciation Areas - Setup window by clicking to the left of the
depreciation area code.
Depreciation Start Date
 Note
The field is editable when the following conditions are met:
The asset has been capitalized.
The fiscal year you select is the year during which the capitalization takes place.
The depreciation area is not a derived area.
Specify the asset's depreciation start date.
Once you change the date, the system automatically recalculates the depreciation and updates the asset-relevant values.
If you do not want to manually specify the depreciation start date, SAP Business One can calculate the date for you based on the
capitalization date and the depreciation convention you specified for the depreciation type. For more information, see Depreciation
Types - Setup Window: General Tab.
Depreciation End Date
Displays the depreciation end date, which is calculated based on the depreciation start date and the useful life.
The field is not editable.
Useful Life
Enter the asset's useful life, in months.
By default, the system copies the useful life from the asset class.
Once you change the useful life value, the system automatically recalculates the depreciation and updates the asset-relevant
values.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:03 AM
Remaining Life (Months)
Displays the asset's remaining life, which is calculated based on the useful life and the depreciation start date.
The field is not editable.
 Note
The field always displays the remaining life at the start of the fiscal year you select.
 Example
Asset X
Useful Life: 60 Months
Capitalization Date: January 1st, 2012
Depreciation Start Date: July 1st, 2012
Current System Date: December 1st, 2012
In this case, if you select fiscal year 2012, the remaining life of the asset is displayed as 60 months, as the system calculates the
remaining life in January of fiscal year 2012.
However, if you change the fiscal year to 2013, the remaining life is displayed as 54 (60 – 6) months, as the system calculates
the remaining life in January of fiscal year 2013.
Depreciation Type
Specify the depreciation type in the depreciation area.
By default, the system copies the depreciation type from the asset class.
Once you change the depreciation type, the system automatically recalculates the depreciation and updates the asset-relevant
values.
Period Control
To define the depreciation calculation factors for different periods, choose the pushbutton to open the Depreciation Period
Control window.
 Note
The pushbutton is enabled only if you have selected a row where the depreciation type meets the following conditions:
The depreciation type has the Straight Line Period Control method.
For more information, see Straight Line Period Control Method.
The depreciation period of the depreciation type is Individual.
More Information
Depreciation Period Control Window
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:03 AM
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
Depreciation Period Control Window
Use this window to define the depreciation calculation factors for different periods when you depreciate an asset using the straight
line period control method with individual period control.
For more information, see Straight Line Period Control Method.
To access the window, do the following:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data and select the Fixed
Assets tab.
2. On the Overview subtab of the Fixed Assets tab, select the row with the intended depreciation type in the Depreciation
Parameters table and choose the Period Control pushbutton.
Depreciation Period Control Window Fields
Fiscal Year
Displays the fiscal year you have selected in the Fiscal Year field in the Asset Master Data window.
Depreciation
Select the checkbox to depreciate the asset in the period.
Factor
Enter a factor for the calculation of depreciation in the period.
By default, the system displays the factor you have specified for the depreciation type.
More Information
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Straight Line Period Control Method
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Use this subtab to monitor the changes in the value of an asset over the course of one year.
The current depreciation area and the fiscal year are displayed in the upper right corner of the subtab. You can change them
manually to display the values for a different depreciation area or fiscal year.
To access the subtab, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data . Select
the Fixed Assets tab and then the Values subtab.
Values Subtab Fields
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:03 AM
Transaction
Displays the following:
Beginning of Year – The asset values displayed in this row are the accumulated values at the beginning of the selected
fiscal year.
Acquisition, Retirement, Transfer, Write-Up, Ordinary Depreciation, Unplanned Depreciation, Special Depreciation –
These are the different types of asset transactions, and the values in these rows are the amounts incurred in the selected
fiscal year as a result of the different transactions.
End of Year – The asset values displayed in this row are the accumulated values at the end of the selected fiscal year.
Acquisition and Production Costs
Displays the asset's acquisition and production costs at the beginning and end of the year, and shows how the value changes over
the course of the year.
Quantity
If the asset is planned for quantity maintenance, the field displays the quantity at the beginning and end of the year, and shows
how the quantity changes over the course of the year.
Depreciation
Displays the asset's depreciation amount at the beginning and end of the year, and shows how the value changes over the course
of the year.
Write-Up
Displays the asset's write-up amount at the beginning and end of the year, and shows how the value changes over the course of the
year.
In SAP Business One, write-up is the increase in an asset's value as a result of manual appreciation or revaluation.
Net Book Value
Displays the asset's net book value at the beginning and end of the year, and shows how the value changes over the course of the
year.
More Information
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation
Subtab
Use this subtab to view an asset's planned and posted depreciations at different periods of each year.
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:03 AM
The current depreciation area and the fiscal year are displayed in the upper right corner of the subtab. You can change them
manually to display the values for a different depreciation area or fiscal year.
To access the subtab, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data . Select
the Fixed Assets tab and then the Depreciation subtab.
Depreciation Subtab Fields
Planned Depreciation
Displays the depreciation amount planned for the asset in each period.
The planned depreciation includes all depreciations planned for the asset, both automatic and manual.
Posted Depreciation
Displays the depreciation amount that has already been posted to the general ledger accounts for the asset in each period.
The following formula shows the relations between the posted, automatic and manual depreciation:
Planned Depreciation = Automatic Depreciation + Manual Depreciation
To post depreciation to the general ledger accounts, use the depreciation run. For more information, see Depreciation Run.
Automatic Depreciation
Displays the automatic depreciation amount that has been posted to the general ledger accounts for the asset in each period.
The automatic depreciation refers to the depreciation automatically carried out by the system.
Manual Depreciation
Displays the manual depreciation amount that has been posted to the general ledger accounts for the asset in each period.
The manual depreciation refers to all depreciations that you have carried out manually using the Manual Depreciation documents.
More Information
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting
Subtab
Use this subtab to assign projects and distribution rules to an asset to facilitate cost accounting.
For asset transactions that create journal entries, SAP Business One carries forward the relevant projects and distribution rules to
the journal entries.
To access the subtab, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data . Select
the Fixed Assets tab and then the Cost Accounting subtab.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:03 AM
Project Assignment Fields
Valid From, Valid To
Specify the period during which you want to assign the asset to a project.
The Valid From field is mandatory, while the Valid To field is optional in the last row. If you do not specify a Valid To date, SAP
Business One regards it as 31.12.2099.
Project
Specify the projects to which you want to assign the asset.
 Note
In the chart of accounts, you can also assign a project to a profit and loss account that is used by the asset. However, the
project you assign here takes priority over the project assigned to the account.
Distribution Rule Assignment Fields
Valid From, Valid To
Specify the period during which you want to assign a distribution rule to the asset.
The Valid From field is mandatory, while the Valid To field is optional in the last row. If you do not specify a Valid To date, SAP
Business One regards it as 31.12.2099.
Distribution Rule
Specify the distribution rules that you want to assign to the asset.
 Note
In the chart of accounts, you can also assign distribution rules to a profit and loss account that is used by the asset. However,
the distribution rules you assign here take priority over the distribution rules assigned to the account.
More Information
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Additional Information Subtab
Consolidation of Journal Entry Rows by Projects and Distribution Rules
Consolidation of Journal Entry Rows by Projects and Distribution
Rules
In SAP Business One, you can assign a fixed asset to multiple projects and distribution rules. When you create a transaction for the
asset, the projects and distribution rules are then displayed in the corresponding journal entries.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:03 AM
To consolidate the journal entry rows by projects and distribution rules, you can select the Consolidate Journal Entry Rows by
Projects and Consolidate Journal Entry Rows by Distribution Rules checkboxes in, for example, the retirement and manual
depreciation documents.
Scenario 1
If you select the checkbox Consolidate Journal Entry Rows by Distribution Rules, the system consolidates the journal entry rows
by both G/L accounts and distribution rules.
Sample Data
| JE # | Amount | G/L Account |     | Distribution Rule | Project |
| ---- | ------ | ----------- | --- | ----------------- | ------- |
| 1    | $ 30   | 100         |     | D1                | P2      |
| 2    | $ 20   | 300         |     | D3                | P1      |
| 3    | $ 450  | 300         |     | D3                | P2      |
| 4    | $ 32   | 300         |     | D1                | P1      |
| 5    | $ 12   | 200         |     | D4                | P1      |
| 6    | $ 80   | 100         |     | D2                | P3      |
| 7    | $ 43   | 200         |     | D1                | P3      |
| 8    | $ 23   | 100         |     | D1                | P2      |
| 9    | $ 21   | 100         |     | D1                | P3      |
| 10   | $ 45   | 100         |     | D2                | P2      |
|      | $ 756  |             |     |                   |         |
Summary Output
| JE # | Amount | G/L Account | Distribution |     |     |
| ---- | ------ | ----------- | ------------ | --- | --- |
| 1    | $ 74   | 100         | D1           |     |     |
| 2    | $ 125  | 100         | D2           |     |     |
| 3    | $ 43   | 200         | D1           |     |     |
| 4    | $ 12   | 200         | D4           |     |     |
| 5    | $ 32   | 300         | D1           |     |     |
| 6    | $ 470  | 300         | D3           |     |     |
|      | $ 756  |             |              |     |     |
Scenario 2
If you select the checkbox Consolidate Journal Entry Rows by Projects, the system consolidates the journal entry rows by both
G/L accounts and projects.
Sample Data
| JE # | Amount | G/L Account |     | Distribution Rule | Project |
| ---- | ------ | ----------- | --- | ----------------- | ------- |
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:03 AM
| 1   | $ 30  | 100 |     | D1  | P2  |
| --- | ----- | --- | --- | --- | --- |
| 2   | $ 20  | 300 |     | D3  | P1  |
| 3   | $ 450 | 300 |     | D3  | P2  |
| 4   | $ 32  | 300 |     | D1  | P1  |
| 5   | $ 12  | 200 |     | D4  | P1  |
| 6   | $ 80  | 100 |     | D2  | P3  |
| 7   | $ 43  | 200 |     | D1  | P3  |
| 8   | $ 23  | 100 |     | D1  | P2  |
| 9   | $ 21  | 100 |     | D1  | P3  |
| 10  | $ 45  | 100 |     | D2  | P2  |
|     | $ 756 |     |     |     |     |
Summary Output
| JE # | Amount | G/L Account | Project |     |     |
| ---- | ------ | ----------- | ------- | --- | --- |
| 1    | $ 78   | 100         | P1      |     |     |
| 2    | $ 101  | 100         | P3      |     |     |
| 3    | $ 12   | 200         | P1      |     |     |
| 4    | $ 43   | 200         | P3      |     |     |
| 5    | $ 52   | 300         | P1      |     |     |
| 6    | $ 450  | 300         | P3      |     |     |
|      | $ 756  |             |         |     |     |
Scenario 3
If you select both checkboxes, the system consolidates the journal entry rows by both G/L accounts, projects, and distribution
rules.
Sample Data
| JE # | Amount | G/L Account |     | Distribution Rule | Project |
| ---- | ------ | ----------- | --- | ----------------- | ------- |
| 1    | $ 30   | 100         |     | D1                | P2      |
| 2    | $ 20   | 300         |     | D3                | P1      |
| 3    | $ 450  | 300         |     | D3                | P2      |
| 4    | $ 32   | 300         |     | D1                | P1      |
| 5    | $ 12   | 200         |     | D4                | P1      |
| 6    | $ 80   | 100         |     | D2                | P3      |
| 7    | $ 43   | 200         |     | D1                | P3      |
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:03 AM
| 8   | $ 23  | 100 | D1  | P2  |
| --- | ----- | --- | --- | --- |
| 9   | $ 21  | 100 | D1  | P3  |
| 10  | $ 45  | 100 | D2  | P2  |
|     | $ 756 |     |     |     |
Summary Output
| JE # | Amount | G/L Account | Distribution Rule | Project |
| ---- | ------ | ----------- | ----------------- | ------- |
| 1    | $ 53   | 100         | D1                | P2      |
| 2    | $ 20   | 300         | D3                | P1      |
| 3    | $ 450  | 300         | D3                | P2      |
| 4    | $ 32   | 300         | D1                | P1      |
| 5    | $ 12   | 200         | D4                | P1      |
| 6    | $ 80   | 100         | D2                | P3      |
| 7    | $ 43   | 200         | D1                | P3      |
| 8    | $ 23   | 100         | D1                | P2      |
| 9    | $ 21   | 100         | D1                | P3      |
| 10   | $ 45   | 100         | D2                | P2      |
|      | $ 756  |             |                   |         |
Scenario 4
If you do not select either checkbox, the system consolidates the journal entry rows by G/L accounts only.
Sample Data
| JE # | Amount | G/L Account | Distribution Rule | Project |
| ---- | ------ | ----------- | ----------------- | ------- |
| 1    | $ 30   | 100         | D1                | P2      |
| 2    | $ 20   | 300         | D3                | P1      |
| 3    | $ 450  | 300         | D3                | P2      |
| 4    | $ 32   | 300         | D1                | P1      |
| 5    | $ 12   | 200         | D4                | P1      |
| 6    | $ 80   | 100         | D2                | P3      |
| 7    | $ 43   | 200         | D1                | P3      |
| 8    | $ 23   | 100         | D1                | P2      |
| 9    | $ 21   | 100         | D1                | P3      |
| 10   | $ 45   | 100         | D2                | P2      |
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:03 AM
|     | $ 756 |     |     |     |
| --- | ----- | --- | --- | --- |
Summary Output
| JE # | Amount | G/L Account |     |     |
| ---- | ------ | ----------- | --- | --- |
| 1    | $ 199  | 100         |     |     |
| 2    | $ 55   | 200         |     |     |
| 3    | $ 502  | 300         |     |     |
|      | $ 756  |             |     |     |
More Information
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Master Data Window - Fixed Assets Tab: Attributes Subtab
Use this subtab to manage the attributes of an asset.
To access the subtab, from the SAP Business One Main Menu, choose  Financials   Fixed Assets   Asset Master Data . Select
the Fixed Assets tab and then the Additional Information subtab.
Additional Information Subtab Fields
Attribute Name
Displays the names of the active attributes in the attribute group that you assigned to the asset class of the asset.
Attribute Value
Enter an attribute value of up to 100 characters.
By default, the field displays the attribute value you specified in the Attribute Groups - Setup window.
More Information
Asset Master Data Window - Fixed Assets Tab
Asset Master Data Window - Fixed Assets Tab: Overview Subtab
Asset Master Data Window - Fixed Assets Tab: Values Subtab
Asset Master Data Window - Fixed Assets Tab: Depreciation Subtab
Asset Master Data Window - Fixed Assets Tab: Cost Accounting Subtab
Asset Transactions
With SAP Business One, you can carry out a series of transactions for your fixed assets as follows:
Capitalization
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:03 AM
Capitalization Credit Memo
Retirement
Transfer
Manual Depreciation
Depreciation Run
Asset Revaluation
To facilitate the management of fixed assets, SAP Business One also lets you acquire, sell and retire an asset using the following
types of marketing documents:
A/P Invoice
A/P Credit Memo
A/P Correction Invoice
A/P Correction Invoice Reversal
A/R Invoice
More Information
Capitalization
Capitalization Credit Memo
Retirement
Transfer
Manual Depreciation
Depreciation Run
Asset Revaluation
Fiscal Year Change Window
Capitalization
Capitalization is the process of recording an acquisition and production cost as a fixed asset (written off as depreciation over
several accounting periods) instead of an expense (charged against earnings in one accounting period). When you acquire an
asset, SAP Business One automatically capitalizes it.
To create asset acquisitions, you can use any of the following documents:
Capitalization
 Note
When you acquire an asset for the first time using a capitalization document, you must create the document for all
depreciation areas. For subsequent acquisitions, you can create the document for a specific depreciation area.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:03 AM
SAP Business One lets you create a capitalization document for multiple assets. Once you add the document, the system
creates a journal entry for each Posting to G/L depreciation area associated with the assets. In the journal entry, the asset
balance sheet accounts are debited and the acquisition clearing accounts are credited.
A/P invoice
A/P correction invoice
 Note
If you acquire an asset using an A/P invoice or A/P correction invoice, the system automatically generates a
capitalization document. The capitalization affects all of the asset's associated depreciation areas.
After you acquire an asset for the first time, you can still create subsequent acquisitions.
More Information
Capitalization Window
Capitalization Window
Use this window to create asset acquisitions.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Capitalization .
General Area Fields
Origin
Displays one of the following:
AC – The abbreviation for the transaction type Capitalization. It indicates the capitalization document is manually created.
PU – The abbreviation for the transaction type A/P Invoice. It indicates the capitalization document is automatically
generated as a result of the creation of an A/P invoice with fixed assets.
CU – The abbreviation for the transaction type A/P Correction Invoice. It indicates the capitalization document is
automatically generated as a result of the creation of an A/P correction invoice with fixed assets.
When the capitalization document is in Add mode, the field is blank.
Origin No.
Displays one of the following:
If the capitalization document is created manually, the field displays the document number according to the definition in
the Document Numbering - Setup window.
If the capitalization document is automatically generated, the field displays the document number of the source A/P
invoice or A/P correction invoice document.
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Status
Displays one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:03 AM
Posted – Indicates the capitalization document is created.
Cancelled – Indicates the capitalization document is cancelled.
Posting Date
Specify the date on which the journal entry is posted.
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date on which the asset is capitalized.
By default, the date is the same as the posting date.
 Note
If you have not specified the capitalization date for an asset in the asset master data, the date you specify here is copied to the
asset master data as the capitalization date.
Cancellation Date
 Note
The field is available only if you have canceled the capitalization document.
If a capitalization document is automatically generated upon the creation of an A/P invoice or A/P correction invoice, you must
cancel the invoice in order to cancel the capitalization document.
Displays the cancellation date.
Depreciation Area
Select the depreciation area in which the capitalization takes effect.
 Note
You must create the capitalization document for all depreciation areas.
By default, * – All Areas is selected.
Reference
If required, specify additional information about the capitalization.
Currency
From the dropdown list, select which currency (local, system, or foreign) you want to use for the capitalization.
If you select foreign currency, specify the currency and the exchange rate.
Total
Displays the total amount of the document.
Contents Tab Fields
Asset No.
Specify the asset you want to acquire.
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:03 AM
Selecting the same asset twice displays an error message.
Asset Description
You can select an asset by the asset description, as an alternative to the asset number.
G/L Account
 Note
The field is available only if you have selected a specific depreciation area instead of all areas in the Depreciation Area field.
Specify the clearing account for the acquisition and production costs of the fixed assets.
By default, the Acquisition Clearing Account you have specified for the asset is displayed.
Total
Enter the acquisition cost of the asset.
Quantity
If the asset is planned for quantity maintenance, enter the acquired quantity.
Distr. Rule, Project
Enter the distribution rule and project for the asset.
For automatically-created capitalizations, the distribution rules and projects are retrieved from the base documents. For
capitalizations with no base documents, the distribution rules and projects are automatically filled with the information from the
fixed asset master data.
Remark
If required, enter remarks about the asset.
Accounting Tab Fields
Depreciation Area
Displays all Posting to G/L depreciation areas that are associated with the selected assets in this document.
One journal entry is generated for each depreciation area.
Journal Remark
If required, enter the remark about the journal entry generated in each depreciation area.
By default, the journal remark is Capitalization.
Cancellation Journal Remark
If required, enter the remark about the journal entry generated upon the cancellation of the capitalization document.
 Note
The field is available only if you have canceled the capitalization document.
If a capitalization document is automatically generated upon the creation of an A/P invoice or A/P correction invoice, you must
cancel the invoice in order to cancel the capitalization document.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:03 AM
Capitalization
A/P Invoice
Capitalization Credit Memo
A capitalization credit memo, which reduces the acquisition and production costs of an asset, essentially represents the opposite
of an invoice for a purchased asset.
To reduce the acquisition and production costs of an asset, you can use any of the following documents:
Capitalization credit memo
When you reduce the acquisition and production costs of an asset using a capitalization credit memo, you can apply the
reduction to any depreciation area associated with the asset. If the depreciation area you specify is not a Posting to G/L
area, no journal entry is generated.
SAP Business One lets you create a capitalization credit memo for multiple assets. If you select all depreciation areas, the
system creates a journal entry for each Posting to G/L depreciation area associated with the assets. In the journal entry,
the asset balance sheet accounts are credited and the acquisition clearing accounts are debited.
A/P credit memo
A/P correction invoice
 Note
If you reduce an asset's acquisition and production costs using an A/P credit memo or A/P correction invoice, the
system automatically generates a capitalization credit memo.
A/P correction invoice reversal
 Note
If you have acquired an asset using an A/P correction invoice, you can reverse the acquisition by creating an A/P
correction invoice reversal. With the reversal, the system cancels the original capitalization document generated upon
the creation of the A/P correction invoice.
When you create a capitalization credit memo for an asset, the credit memo always affects the asset's planned depreciation for the
whole year, no matter when in the year the credit memo occurs. If the credit memo occurs in the year of the first acquisition, the
asset's depreciation is decreased as of the depreciation start date. If the credit memo occurs in a subsequent fiscal year,
depreciation for the asset is decreased as of the beginning of this subsequent fiscal year.
 Note
SAP Business One considers the asset value date of the capitalization credit memo document as the date when the credit
memo actually occurs.
More Information
Capitalization Credit Memo Window
Capitalization Credit Memo Window
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:03 AM
Use this window to create capitalization credit memos for assets.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Capitalization .
General Area Fields
Origin
Displays one of the following:
AM – The abbreviation of the transaction type Capitalization Credit Memo. It indicates that the capitalization credit memo
is manually created.
PC – The abbreviation of the transaction type A/P Credit Memo. It indicates that the capitalization credit memo is
automatically generated as a result of the creation of an A/P credit memo with fixed assets.
CU – The abbreviation of the transaction type A/P Correction Invoice. It indicates that the capitalization credit memo is
automatically generated as a result of the creation of an A/P correction invoice with fixed assets.
When the capitalization credit memo is in Add mode, the field is blank.
Origin No.
Displays one of the following:
If the capitalization credit memo is created manually, the field displays the document number according to the definition in
the Document Numbering - Setup window.
If the capitalization credit memo is automatically generated, the field displays the document number of the source A/P
credit memo or A/P correction invoice document.
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Status
Displays one of the following:
Posted – Indicates that the capitalization credit memo is created.
Cancelled – Indicates that the capitalization credit memo is cancelled.
Posting Date
Specify the date on which the journal entry is posted.
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date on which the assets' acquisition and production costs are reduced.
By default, the date is the same as the posting date.
Cancellation Date
 Note
The field is available only if you have canceled the capitalization credit memo.
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:03 AM
If a capitalization credit memo is automatically generated upon the creation of an A/P credit memo, you must cancel the A/P
credit memo in order to cancel the capitalization credit memo.
In addition, if a capitalization credit memo is automatically generated upon the creation of an A/P correction invoice, you must
create an A/P correction invoice reversal to cancel the capitalization credit memo.
Displays the cancellation date.
Depreciation Area
Select the deprecation area in which the reduction of the assets' acquisition and production costs applies.
By default, * – All Areas is selected.
Reference
If required, specify any additional information about the capitalization credit memo.
Currency
From the dropdown list, select which currency (local, system, or foreign) you want to use for the credit memo.
If you select foreign currency, specify the currency and the exchange rate.
Total
Displays the total amount of the document.
Contents Tab Fields
Asset No.
Specify the asset for which you want to reduce acquisition and production costs.
You cannot select the same asset twice; otherwise, an error message appears.
Asset Description
You can select an asset by its asset description, as an alternative to its asset number.
G/L Account
 Note
The field is available only if you have selected a specific depreciation area instead of all areas in the Depreciation Area field.
Specify the clearing account for the acquisition and production costs of the fixed assets.
By default, the Acquisition Clearing Account you have specified for the asset is displayed.
Total
Enter the amount that you want to reduce from the asset's acquisition and production costs.
Quantity
If the asset is planned for quantity maintenance, enter the quantity you want to reduce.
Distr. Rule, Project
Enter the distribution rule and project for the asset.
For automatically-created capitalization credit memos, the distribution rules and projects are retrieved from the base documents.
For capitalization credit memos with no base documents, the distribution rules and projects are automatically filled with the
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:03 AM
information from the fixed asset master data.
Remarks
If required, enter the remarks about the asset.
Accounting Tab Fields
Depreciation Area
Displays one of the following:
If you have selected a specific depreciation area in the Depreciation Area field in the general area, the field displays this
depreciation area.
Only when this depreciation area is a Posting to G/L area can the system generate a journal entry.
If you have selected * – All Areas in the Depreciation Area field in the general area, the field displays all Posting to G/L
depreciation areas that are associated with the selected assets in this document.
In this case, for each depreciation area, one journal entry is generated.
Journal Remark
If required, enter the remark about the journal entry generated in each depreciation area.
By default, the journal remark is Capitalization Credit Memo.
Cancellation Journal Remark
 Note
The field is available only if you have canceled the capitalization credit memo.
If a capitalization credit memo is automatically generated upon the creation of an A/P credit memo, you must cancel the A/P
credit memo in order to cancel the capitalization credit memo.
In addition, if a capitalization credit memo is automatically generated upon the creation of an A/P correction invoice, you must
create an A/P correction invoice reversal to cancel the capitalization credit memo.
If required, enter the remark about the journal entry generated upon the cancellation of the capitalization credit memo.
More Information
Capitalization Credit Memo
Retirement
In accounting, retiring a fixed asset means removing it from a corporate balance sheet and operating activities.
In SAP Business One, you can retire an asset in the following ways:
Retirement through Sale
A fixed asset is sold with a profit or loss. If you want to specify the customer information for the asset sale, you can create
an A/R invoice to retire the asset. Upon the creation of the A/R invoice, a retirement document is generated automatically.
However, if you do not want to specify the customer information, you can directly create a retirement document using the
Sales type.
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:03 AM
Retirement through Scrapping
If a fixed asset leaves the asset portfolio without any profit or loss being made, you can retire the asset by creating a
retirement document with the scrapping type. In this case, the system posts the remaining book value of the asset during
retirement as an expense.
Complete or Partial Retirement
A retirement can refer to an entire asset (complete retirement) or part of an asset (partial retirement). You can trigger the
partial retirement of an asset by entering the retired acquisition and production costs or the retired quantity. When you
enter the retired acquisition and production costs or quantity, the system determines the percentage that is deducted from
the asset.
When you create a partial retirement for an asset, the retirement reduces the asset's acquisition and production costs and
thereby affects the planned depreciation. The date on which the partial retirement reduces the assets's acquisition and
production costs is calculated based on the asset value date in the retirement document and the retirement convention
you specified for the asset's depreciation type.
When you retire an asset completely, the asset becomes inactive and you can no longer carry out any transactions with it.
More Information
Retirement Window
Retirement Window
Use this window to create retirement for assets.
To open this window, from the SAP Business One Main Menu, choose Financials Fixed Assets Retirement .
General Area Fields
Origin
Displays one of the following:
RT – The abbreviation for the transaction type Retirement. It indicates the retirement document is manually created.
IN – The abbreviation for the transaction type A/R Invoice. It indicates the retirement document is automatically
generated as a result of the creation of an A/R invoice with fixed assets.
When the retirement document is in Add mode, the field is blank.
Origin No.
Displays one of the following:
If the retirement document is created manually, the field displays the document number according to the definition in the
Document Numbering - Setup window.
If the retirement document is automatically generated, the field displays the document number of the source A/R invoice
document.
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Status
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:03 AM
Displays one of the following:
Posted – Indicates the retirement is created.
Cancelled – Indicates the retirement is cancelled.
Posting Date
Specify the date on which the journal entry is posted.
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date of the retirement.
By default, the date is the same as the posting date.
Cancellation Date
Displays the cancellation date.
 Note
The field is available only if you have canceled the retirement document.
If a retirement document is automatically generated upon the creation of an A/R invoice, you must cancel the A/R invoice in
order to cancel the retirement document.
Transaction Type
Select one of the following retirement types:
Sales – Indicates an asset sold with a profit or loss. If you do not need to specify the customer information, use this type;
otherwise, use an A/R invoice.
Scrapping – Indicates a scrapped asset, with no revenue earned. SAP Business One posts the asset's remaining book value
at the time of retirement as an expense.
Depreciation Area
Select the depreciation area in which an asset's retirement takes effect.
If an asset is retired completely, the retirement is effective in all depreciation areas. In this case, you must select * – All Areas in
this field.
By default, * – All Areas is selected.
Reference
If required, specify any additional information about the retirement.
Currency
From the dropdown list, select the currency (local, system or foreign) you want to use for the retirement.
If you select foreign currency, specify the currency and the exchange rate.
Use Projects/Use Distributions Rules
Select the checkbox to make the Project/Distr. Rule column in the table effective and editable for the fixed assets in the displayed
depreciation area.
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:03 AM
Total
Displays the total amount of the document.
Contents Tab Fields
Asset No.
Specify the asset that you want to retire.
Selecting the same asset twice displays an error message.
Asset Description
You can select an asset by the asset description, as an alternative to the asset number.
G/L Account
 Note
The field is available only if the following conditions are met:
You have selected Sales in the Transaction Type field.
You have selected a specific depreciation area instead of all areas in the Depreciation Area field.
Specify the general ledger account to record the revenue from asset sales. The account cannot be a control account.
By default, the Revenue Account for Retirement you have specified for the asset is displayed.
For an asset that retires through scrapping, you cannot specify the general ledger account. Depending on the Posting of
Retirement method you have specified for the asset in the Depreciation Areas - Setup window, the retirement is posted to one of
the following accounts:
If the asset's retirement posting method is Gross, the asset's retired value is posted to the Leave with Expense NBV
(Gross) account.
If the asset's retirement posting method is Net, the asset's retired value is posted to the Retirement with Expense (Net)
account.
Total
Enter the total revenue resulting from an asset sale.
Based on the asset's sales revenue and its net book value on the retirement date, the system determines whether the asset retires
with profit or loss.
 Note
The field is available only if you have selected Sales in the Transaction Type field.
Partial
Select the checkbox to indicate the asset retirement is partial, for example. Only part of the asset quantity or value is removed
from the portfolio.
Quantity
 Note
The field is editable only if you have selected the Partial checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:03 AM
If you want to retire an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to retire. In
this case, if you enter the acquisition and production costs, the value you enter is not effective.
 Note
After you enter the quantity, the system calculates the retired net book value as follows:
Retired Net Book Value = Net Book Value on Retirement Date * Retired Quantity / Available Quantity on Retirement Date
APC
If you want to retire an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are retired. In this case, if you enter the quantity, it is not effective.
 Note
The field is editable only if you have selected the Partial checkbox.
 Note
After you enter the quantity, the system calculates the retired net book value as follows:
Retired Net Book Value = Net Book Value on Retirement Date * Retired Acquisition and Production Costs / Acquisition and
Production Costs on Retirement Date
Project/Distr. Rule
Displays the project/distribution rule for each asset.
 Note
The Project/Distr. Rule column is effective and editable only if you have selected the Use Project/Use Distr. Rule checkbox.
Remarks
If required, enter the remarks about the asset.
Accounting Tab Fields
Depreciation Area
Displays one of the following:
If you have selected a specific depreciation area in the Depreciation Area field in the general area, the field displays this
depreciation area.
Only when this depreciation area is a Posting to G/L area can the system generate a journal entry.
If you have selected * – All Areas in the Depreciation Area field in the general area, the field displays all Posting to G/L
depreciation areas that are associated with the selected assets in this document.
In this case, for each depreciation area, one journal entry is generated.
Journal Remark
If required, enter the remark about the journal entry generated in each depreciation area.
Depending on whether the retirement type is sales or scrapping, the default journal remark is Retirement – Sales or Retirement –
Scrapping, respectively.
Cancellation Journal Remark
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:03 AM
 Note
The field is available only if you have canceled the retirement document.
If a retirement document is automatically generated upon the creation of an A/R invoice, you must cancel the A/R invoice in
order to cancel the retirement document.
If required, enter the remark about the journal entry generated upon the cancellation of the retirement document.
More Information
Retirement
Transfer
In SAP Business One, you can transfer a fixed asset to a different asset class or a different asset master data record. This may be
necessary if you want to do any of the following:
Assign a different set of G/L accounts to an asset
If you want to change the G/L accounts for a certain asset, transferring the asset offers an alternative to creating a
completely new asset. Once you transfer the asset, the system copies all depreciation data to the target asset. You only
need to assign the new set of G/L accounts to the target asset. After the transfer, the system continues carrying out the
asset's depreciation and transactions with the new set of G/L accounts.
After you completely transfer an asset to another asset, the system deactivates the source asset and carries out the
depreciation calculation for the target asset with its own depreciation types.
Create different asset master records for the same asset
If you use a certain type of asset in multiple locations, it may be necessary to maintain different master data records for
this asset. Transferring the asset enables you to create and store different master records for an asset, and you do not need
to create a completely new asset in the system.
Change the asset class of an asset for which bookings have already been carried out
Change the asset class when an asset construction has been completed
For an asset under construction, it is often necessary to reflect the asset at the year end in the asset history sheet. To
achieve this, as well as monitor the construction progress, you may need to create a specific asset class for this asset. After
the construction is completed and the asset is ready to be used, you can move the asset to a designated asset class by
creating a transfer of the Asset Class Transfer transaction type.
 Note
Fixed assets that already have posted special depreciation cannot be transferred to another asset. A valid workaround is to
cancel the manual depreciation posting (if any), cancel the acquisition, and then post the correct values to the new fixed asset.
To keep a link between the two fixed assets, you might want to enter the old fixed asset number in the description field. This link
is for information purposes only. Another solution is to retire the old fixed asset and then do the new acquisition.
More Information
Transfer Window
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:03 AM
Transfer Window
Use this widow to transfer an asset to a new asset or asset class.
To open this window, from the SAP Business One Main Menu, choose Financials Fixed Assets Transfer .
General Area Fields
Origin
Displays FT, which is the abbreviation for the transaction type Transfer. It indicates the transfer document is always manually
created.
When the transfer document is in Add mode, the field is blank.
Origin No.
Displays the document number according to the definition in the Document Numbering - Setup window.
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Status
Displays one of the following:
Posted – Indicates the transfer is created.
Cancelled – Indicates the transfer is cancelled.
Posting Date
Specify the date on which the journal entry is posted.
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date on which the transfer takes place.
By default, the date is the same as the posting date.
Cancellation Date
Displays the cancellation date of a transfer document.
 Note
The field is available only if you have canceled the transfer document.
The field is not available for an asset class transfer document, as you cannot cancel such a document.
Transaction Type
Select one of the following transfer types:
Asset Transfer – Transfers an asset to another asset. You can create an asset transfer only if the following conditions are
met:
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:03 AM
The transfer date is on the first day of a fiscal year. That is, you must specify an asset value date that is the first day
of a fiscal year.
The source asset does not have special depreciation, either automatic or manual.
You have performed fiscal year change for the year during which the transfer takes place.
In asset transfer, the target asset can be a new or capitalized asset.
If the target asset is a new asset, the system capitalizes it upon the creation of the transfer document and the capitalization
date is copied from the source asset. However, the target asset's depreciation start date is determined by the transfer date
and the acquisition convention you specified for the depreciation type.
After the transfer, the system brings the remaining life of the source asset to the new asset as its useful life and remaining
life. In addition, the system keeps a record of the source asset's useful life for the depreciation calculation of the new asset.
In case the source asset's remaining life has decimals, which can happen if the asset uses the straight line period control
depreciation method, the system first rounds the number and then brings it to the new asset.
Asset Class Transfer – Transfers an asset to a new asset class. You can perform the asset class transfer only if the asset
uses the depreciation types with the No Depreciation method in all areas during the transfer period.
Depreciation Area
Select the depreciation area in which the asset's transfer takes effect.
By default, * – All Areas is selected.
 Note
You must select * – All Areas for either of the following conditions:
The transfer is an asset class transfer.
The transfer is an asset transfer in which the target asset has not been capitalized.
Reference
If required, specify any additional information about the transfer.
Contents Tab Fields
Asset No.
Specify the asset that you want to transfer.
If you select the same asset twice, an error appears.
Asset Description
You can select an asset by the asset description, as an alternative to asset number.
Target Asset No.
 Note
The field is available only if you have selected Asset Transfer in the Transaction Type field.
Specify the target asset to which you want to transfer the asset.
Note that the target asset must have the same depreciation areas as the source asset.
Target Asset Description
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:03 AM
 Note
The field is available only if you have selected Asset Transfer in the Transaction Type field.
You can select the asset by the asset description, as an alternative to the asset number.
Note that the target asset must have the same depreciation areas as the source asset.
Target Asset Class
Specify the new asset class for the asset.
Note that the new asset class must have the same depreciation areas as the current asset class.
 Note
The field is available only if you have selected Asset Class Transfer in the Transaction Type field.
Partial
 Note
The checkbox is available only if you have selected Asset Transfer in the Transaction Type field.
Select the checkbox to indicate the asset transfer is partial, for example, only part of the asset quantity or value is transferred to
the target asset.
Quantity
 Note
The field is available only if you have selected Asset Transfer in the Transaction Type field.
In addition, the field is editable only if you have selected the Partial checkbox.
If you want to transfer an asset partially and the asset is planned for quantity maintenance, enter the quantity you want to transfer.
In this case, if you enter the acquisition and production cost, it is not effective.
 Note
After you enter the quantity, the system calculates the transferred net book value as follows:
Transferred Net Book Value = Net Book Value on Transfer Date * Transferred Quantity / Available Quantity on Transfer Date
APC
 Note
The field is available only if you have selected Asset Transfer in the Transaction Type field.
In addition, the field is editable only if you have selected the Partial checkbox.
If you want to transfer an asset partially and the asset is not planned for quantity maintenance, specify how much of the asset's
acquisition and production costs are transferred. In this case, if you enter the quantity, it is not effective.
 Note
After you enter the acquisition and production costs, the system calculates the transferred net book value as follows:
Transferred Net Book Value = Net Book Value on Transfer Date * Transferred Acquisition and Production Costs / Acquisition and
Production Costs on Transfer Date
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:03 AM
Distr. Rule, Project
Enter the distribution rule and project for the transfer.
Remarks
If required, enter a remark about the asset.
Accounting Tab Fields
Depreciation Area
Displays either of the following:
If you have selected a specific depreciation area in the Depreciation Area field in the general area, the field displays this
depreciation area.
Only when this depreciation area is a Posting to G/L area can the system generate a journal entry.
If you have selected * – All Areas in the Depreciation Area field in the general area, the field displays all Posting to G/L
depreciation areas that are associated with the selected assets in this document.
In this case, for each depreciation area, one journal entry is generated.
Journal Remark
If required, enter a remark about the journal entry generated in each depreciation area.
Depending on whether the transfer type is asset transfer or asset class transfer, the default journal remark is Transfer – Asset
Transfer or Transfer – Asset Class Transfer respectively.
Cancellation Journal Remark
 Note
The field is available only if you have canceled the transfer document.
The field is not available for an asset class transfer document, as you cannot cancel such a document.
If required, enter the remark about the journal entry generated upon the cancellation of the transfer document.
More Information
Transfer
Manual Depreciation
SAP Business One can use depreciation types to automatically determine the planned depreciation for an asset in a particular
fiscal year. However, you may want to manually depreciate the asset in case one of the following situations arises:
There is an unexpected permanent reduction in the value of the asset caused, for example, by an accident.
You want to manually trigger the special depreciation of the asset.
You are using the unit-of-production depreciation method and want to manually plan the asset's depreciation.
SAP Business One lets you create the following types of manual depreciation documents:
Ordinary Depreciation – Refers to the manual ordinary depreciation.
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:03 AM
Generally, ordinary depreciation includes the planned ordinary depreciation and the manual ordinary depreciation. The
former is the depreciation calculated and carried out automatically by the system based on the depreciation type you
assign to the asset. The latter is the depreciation you manually perform using the manual depreciation document. You can
view the sum of both depreciation amounts in the Ordinary Depreciation row on the Values subtab in the asset master
data.
Unplanned Depreciation – Refers to the unplanned depreciation, usually carried out when there is an unexpected
reduction in the value of an asset resulting, for example, from an accident.
Special Depreciation – Refers to the manual special depreciation.
SAP Business One can carry out the special depreciation automatically for an asset, which is known as the automatic
special depreciation. You can assign a depreciation type with the Special Depreciation method to an asset, and the system
automatically calculates the special depreciation when it is due. For more information, see Special Depreciation Method.
If you want to manually carry out the special depreciation, use the manual depreciation document and assign a
depreciation type with the Manual Depreciation method. For more information, see Manual Depreciation Method.
You can view the sum of both depreciation amounts in the Special Depreciation row on the Values subtab in the asset
master data.
Appreciation – Refers to the increase in an asset's book value to offset the asset's unplanned depreciation.
Usually a revaluation of an asset can also result in the increase of the asset's value in the book. SAP Business One regards
the two kinds of value increase in an asset as a write-up. To view an asset's write-up information, see the Write-Up row on
the Values subtab in the asset master data.
More Information
Manual Depreciation Window
Manual Depreciation Window
Use this window to create manual depreciations for assets.
To open this window, from the SAP Business One Main Menu, choose Financials Fixed Assets Manual Depreciation .
General Area Fields
Origin
Displays MD, which is the abbreviation for the transaction type Manual Depreciation. It indicates that the manual depreciation
document is always manually created.
When the manual depreciation document is in Add mode, the field is blank.
Origin No.
Displays the document number according to the definition in the Document Numbering - Setup window.
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Status
Displays one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:03 AM
Posted – Indicates the manual depreciation is created.
Cancelled – Indicates the manual depreciation is cancelled.
Posting Date
Specify the date on which the journal entry is posted.
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date on which the special depreciation takes place.
By default, the date is the same as the posting date.
Cancellation Date
Displays the cancellation date.
 Note
The field is available only if you have canceled the manual depreciation document.
Transaction Type
Select one of the following types for manual depreciation:
Ordinary Depreciation – Refers to the manual ordinary depreciation in this case.
Generally, ordinary depreciation includes the planned ordinary depreciation and the manual ordinary depreciation. The
former is the depreciation calculated and carried out automatically by the system based on the depreciation type you
assign to the asset. And the latter is the depreciation you manually perform using the manual depreciation document. You
can view the sum of both depreciation amounts in the Ordinary Depreciation row on the Values subtab in the asset master
data.
Unplanned Depreciation – Refers to the unplanned depreciation, usually carried out when there is an unexpected
reduction in the value of an asset resulting, for example, from an accident.
Special Depreciation – Refers to the manual special depreciation.
SAP Business One can carry out the special depreciation automatically for an asset, known as the automatic special
depreciation. You can assign a depreciation type to an asset with the Special Depreciation method, and the system
automatically calculates the special depreciation when it is due. For more information, see Special Depreciation Method.
If you want to manually carry out the special depreciation, use the manual depreciation document and assign a
depreciation type with the Manual Depreciation method. For more information, see Manual Depreciation Method.
You can view the sum of both depreciation amounts in the Special Depreciation row on the Values subtab in the asset
master data.
Appreciation – Refers to the increase in an asset's book value to offset the asset's unplanned depreciation.
Usually a revaluation of an asset can also result in the increase of the asset's value in the book. SAP Business One regards
the two kinds of value increase in an asset as a write-up. To view an asset's write-up information, see the Write-Up row on
the Values subtab in the asset master data.
Depreciation Area
Select the depreciation area in which an asset's manual depreciation takes effect.
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:03 AM
By default, * – All Areas is selected.
Reference
If required, specify any additional information about the manual depreciation.
Use Projects/Use Distribution Rules
Select the checkbox to make the Project/Distr. Rule column in the table effective and editable for the fixed assets in the displayed
depreciation area.
Contents Tab Fields
Asset No.
Specify the asset for which you want to create manual depreciations.
Selecting the same asset twice displays an error message.
Asset Description
You can select an asset by the asset description, as an alternative to the asset number.
Total
Enter the total depreciation amount.
If it is an appreciation, the total must not exceed the difference between the asset's NBV and historical NBV.
 Note
If the total you enter in this field causes the asset's net book value to fall below zero in any period, the system displays an error.
For example, asset X is capitalized on January 1, 2012 and its acquisition and production costs are 100 USD. You create a
capitalization credit memo for the asset with the amount of 40 USD on 2012 October 1st.
On May 1, 2012 you want to create a manual depreciation of 70 USD for the asset. In this case, the system blocks you from the
creation of the manual depreciation document.
Project/Distr. Rule
Displays the project/distribution rule for each asset.
 Note
The Project/Distr. Rule column is effective and editable only if you have selected the Use Project/Use Distr. Rule checkbox.
Remarks
If required, enter remarks about the asset.
Accounting Tab Fields
Depreciation Area
Displays one of the following:
If you have selected a specific depreciation area in the Depreciation Area field in the general area, the field displays this
depreciation area.
Only when this depreciation area is a Posting to G/L area can the system generate a journal entry.
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:03 AM
If you have selected * – All Areas in the Depreciation Area field in the general area, the field displays all Posting to G/L
depreciation areas that are associated with the selected assets in this document.
In this case, one journal entry is generated for each depreciation area.
Journal Remark
If required, enter the remark about the journal entry generated in each depreciation area.
Depending on the transaction type, the default journal remark can be any of the following:
Manual Depreciation – Ordinary Depreciation
Manual Depreciation – Unplanned Depreciation
Manual Depreciation – Special Depreciation
Manual Depreciation – Appreciation
Cancellation Journal Remark
If required, enter the remark about the journal entry generated upon the cancellation of the manual depreciation document.
 Note
The field is available only if you have canceled the manual depreciation document.
More Information
Manual Depreciation
Depreciation Run
Each single asset transaction leads to a change in planned depreciation, but not to a posting to the relevant general ledger
accounts. Only when you execute a depreciation run does the system carry out all depreciations planned up to the specified date.
The depreciation run only covers automatic depreciation.
 Note
When you create manual depreciations, the associated values are immediately posted to the general ledger accounts.
 Note
For more information about canceling a depreciation run, see SAP Note 3358686 .
To trigger the posting of planned depreciation, it is usually sufficient to start one depreciation run for several posting periods.
However, it is possible to execute several depreciation runs for the same depreciation period. A repeat run might be necessary, for
example, if the depreciation terms have been changed for individual assets in connection with the year-end closing.
In depreciation runs, unposted planned depreciation is always posted using the catch-up method. In the catch-up method, the
system gathers any planned depreciation that has not been posted yet for the entire depreciation period and then creates a
collective posting. Therefore, the posting can also include planned depreciation from several periods.
 Example
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:03 AM
A planned depreciation of 1,200 USD for the current fiscal year has been calculated for an asset. The depreciation run is
executed for the first time in March. The system proportionally posts a depreciation amount of 300 USD for the months from
January to March. This means the depreciation for January and February is done in March in general ledger accounting.
A depreciation run can be repeated as often as necessary, provided no depreciation run has been executed for the following
periods. A repeat depreciation run may be necessary if the asset values have changed once again after posting planned
depreciation. When repeating a depreciation run, only the value differences to the posting of the last depreciation run are
considered.
 Caution
You can execute a depreciation run only when no depreciation run has been executed for the following periods. Within one
period you can execute as many depreciation runs as required.
 Note
In order to keep the number of financial documents to a minimum, we recommend that you carry out only one depreciation run
per fiscal year.
SAP Business One lets you preview the details of the depreciation run before you execute it.
More Information
Depreciation Run Window
Depreciation Run - Preview/Results Window
Depreciation Run Window
Use this window to enter the desired data for a depreciation run and view previous depreciation runs.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Depreciation Run .
General Area Fields
Depreciation Area
Select the depreciation area for which the depreciation run is carried out.
Depreciate To
Select the period until which the depreciation run is carried out.
By default, the current period is displayed.
After you specify the period, the system carries out the posting for the depreciation from the first day of the fiscal year to the last
day of the selected period.
 Example
You select May 2012 as the Depreciate To period.
After you execute the depreciation run, the system posts all assets' planned depreciation from January 1st, 2012 to May 31,
2012.
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:03 AM
If you have not posted the depreciation for year 2011, you must post the depreciation for 2011 before you execute the
depreciation run for 2012.
No.
Select the numbering series for which you want to execute the depreciation run.
 Note
When the multiple branch functionality is enabled, you can only execute the depreciation run for the default numbering series,
and the No. field is not available in the Depreciation Run window.
Branch
This field is available when the multiple branch functionality is enabled. Choose the Browse button to open the Branch
Assignment window. In the Branch Assignment window, select the branches for which you want to execute the depreciation run.
Table Area Fields
Run
Displays the previously executed depreciation runs.
To view the details about a depreciation run, choose to open the Depreciation Run - Results window.
Status
Displays one of the following statuses of the executed depreciation runs:
Depreciation Posted – Indicates that the depreciation has been posted to the general ledger accounts.
No Depreciation Posted – Indicates that no depreciation has been posted to the general ledger accounts, which can
happen in any of the following situations:
You have selected a non-posting depreciation area for the depreciation run.
There is no planned depreciation in the specified period.
You repeat a previously executed depreciation run, and the depreciation has not changed in the interval.
Depreciation Area
Displays the depreciation area for which the depreciation run is carried out.
Depreciate To
Displays the end date of the depreciation run.
Posting Date
Displays the posting date of the depreciation run.
Depreciation
Displays the total depreciation amount posted during the depreciation run.
Remarks
Displays the remarks, if any, about the depreciation run.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:03 AM
Depreciation Run
Depreciation Run - Preview/Results Window
Depreciation Run - Preview/Results Window
Use the Depreciation Run - Preview window to preview the details of the depreciation run before you execute it.
Use the Depreciation Run - Results window to view the details of the depreciation runs that you have executed.
To access the Depreciation Run - Preview window, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Depreciation Run .
2. In the Depreciation Run window, specify the depreciation area and the Depreciate To date, and choose Preview.
The Depreciation Run – Preview window opens.
To access the Depreciation Run - Results window, choose the Execute button in the Depreciation Run – Preview window opened
in step 2 above.
General Area Fields
Depreciation Area
Displays the depreciation area for which the depreciation run is carried out.
Depreciate To
Displays the end date of the depreciation run.
Posting Date
Specify the date for the journal entry posting.
By default, the posting date is the last day of the selected Depreciate To period.
Remarks
If required, enter the remarks about the depreciation run.
Consolidate Journal Entry Rows by Projects/Distribution Rules
Select the checkboxes to consolidate the journal entry rows by projects and distribution rules.
Depending on your selection, the journal entry layout can be one of the following:
Consolidate Journal Entry Rows by Projects – the system consolidates the journal entry rows with the same G/L account
and project.
Consolidate Journal Entry Rows by Distribution Rules – the system consolidates the journal entry rows with the same G/L
account and distribution rule.
If you select both, the system consolidates the journal entry rows with the same G/L account, project, and distribution rule.
If you leave the two checkboxes unselected, the system consolidates only the journal entry rows with the same G/L
account.
For more information, see the examples in Consolidation of Journal Entry Rows by Projects and Distribution.
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:03 AM
Status
 Note
The field is blank in preview mode.
Displays either of the following statuses of the executed depreciation runs:
Depreciation Posted – Indicates that the depreciation has been posted to the general ledger accounts.
No Depreciation Posted – Indicates that no depreciation has been posted to the general ledger accounts, which can
happen in any of the following situations:
You have selected a non-posting depreciation area for the depreciation run.
There is no planned depreciation in the specified period.
You repeat a previously executed depreciation run, and the depreciation has not changed in the interval.
Table Area Fields
Asset Class
Displays the asset class to which the asset is assigned.
Journal Entry
 Note
The field is blank in preview mode.
Displays the journal entry for the posted depreciation in the Depreciation Run - Results window.
Cancellation Journal Entry
Displays the journal entry for the canceled depreciation run.
 Note
This column is available only if the depreciation run has been canceled.
Asset No.
Displays the assets for which the planned depreciation is to be posted.
Asset Description
Displays the description of each asset.
Ordinary Depreciation
Displays each asset's planned ordinary depreciation in the specified period.
Special Depreciation
Displays each asset's automatic special depreciation in the specified period.
More Information
Depreciation Run Window
Depreciation Run
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:03 AM
Asset Revaluation
Asset revaluation is a technique used to revaluate a company's assets to take into account inflation or changes in value since the
assets were acquired. Usually, revaluations are carried out for an asset whenever there is a difference between the asset's current
market value and its value on the company's balance sheet.
A revaluation reserve arises when the value of an asset becomes greater than the value at which it was previously carried on the
balance sheet. However, not every increase in the asset value is added to the revaluation reserve. The exact treatment depends on
the history of the asset – whether the asset has been impaired, that is, whether the asset has had unplanned depreciation carried
out.
In the case of an asset having unplanned depreciation, the value increase resulting from the revaluation is used to reverse the
planned depreciation. And if there is any surplus, it is added to the revaluation reserve.
Similarly, a value decrease resulting from the revaluation is used to reduce the revaluation reserve, with any excess treated as
unplanned depreciation and taken as a loss.
You can find more information in this blog .
More Information
Asset Revaluation Window
Asset Revaluation Window
Use this window to revaluate assets.
To access the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset Revaluation .
General Area Fields
Depreciation Area
Select the depreciation area in which the asset revaluation takes effect.
Reference
If required, specify the additional information about the revaluation.
Revaluation Percentage
If required, enter the revaluation percentage.
The percentage you enter here is copied to the Revaluation Percentage field in the table area as the default.
With the revaluation percentage, the system calculates the new net book value of the assets as follows:
New NBV = NBV * Revaluation Percentage
No.
Displays the document series and number according to the definition in the Document Numbering - Setup window.
Posting Date
Specify the date on which the journal entry is posted.
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:03 AM
Document Date
Specify the document date. By default, the document date is the same as the posting date.
Asset Value Date
Specify the date on which the revaluation takes place.
 Note
If a fixed asset is assigned a depreciation type whose calculation base is Monthly, the date you specify must be the last day of a
month. If a fixed asset is assigned a depreciation type whose calculation base is Yearly, the date you specify must be the last
day of a fiscal year.
By default, the date is the same as the posting date.
Journal Remark
If required, enter the remark about the journal entry generated upon the creation of the revaluation document.
The default journal remark is Fixed Asset Revaluation.
IFRS Posting
With this checkbox, you can post asset revaluations according to International Financial Reporting Standards (IFRS) for
depreciation areas whose Posting of Depreciation is Indirect Posting. Journal entries of retirements for such assets are also
posted according to IFRS.
When you are revaluating assets, the IFRS status of the fixed asset and its revaluation must be the same. That is, if you select the
IFRS Posting checkbox in a revaluation, you can only add assets for which the IFRS Posting for Revaluation checkbox ( Asset
Master Data Fixed Assets Overview ) is selected; and vice versa.
Table Area Fields
Asset No.
Specify the asset that you want to revaluate.
Selecting the same asset twice displays an error message.
Asset Description
Displays the description of the asset.
NBV
Displays the asset's net book value on the asset value date you specified.
Revaluation Percentage
If required, specify the revaluation percentage.
By default, the value is copied from the Revaluation Percentage field in the header.
After you specify the revaluation percentage, the system calculates the new net book value of the asset as follows:
New NBV = NBV * Revaluation Percentage
New NBV
Specify the new net book value of the asset after the revaluation.
By default, the system calculates the net NBV according to the NBV and revaluation percentage with the following formula:
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:03 AM
New NBV = NBV * Revaluation Percentage
Difference
Displays the difference between the net book value and the new net book value.
Distr. Rule, Project
Enter the distribution rule and project for the revaluation.
Remarks
If required, enter the remarks about the asset.
More Information
Asset Revaluation
Executing a Fiscal Year Change
Prerequisites
You have enabled fixed assets.
For more information, see Enabling Fixed Assets.
Context
In fixed asset management, you must execute a fiscal year change when a fiscal year ends. With the change, SAP Business One
transfers all the asset depreciations and balances seamlessly from the current fiscal year to the continuous new fiscal year.
Procedure
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Fiscal Year Change .
The Fiscal Year Change window opens.
2. In the From Fiscal Year field, select the fiscal year from which you want to execute the change.
SAP Business One automatically adds the next fiscal year in the To Fiscal Year field, to which the change is to be made.
 Note
If the next fiscal year, to which you want to change, is not yet defined in SAP Business One, you receive an error
message.
To define the next fiscal year, do the following:
a. From the SAP Business One Main Menu, choose Administration System Initialization Posting Periods .
The Posting Periods window opens.
b. Choose the New Period pushbutton and add the desired fiscal year.
3. In the Fiscal Year Change window, choose the Execute pushbutton.
The system prompts a system message for you to confirm the change.
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:03 AM
4. In the message dialog box, choose OK.
Related Information
Fiscal Year Change Window
Fiscal Year Change Window
Use this window to start a fiscal year change. When you change a fiscal year, SAP Business One performs the following
calculations:
For each asset, SAP Business One calculates the year-end values of all asset transactions. These values are saved in the
asset master data and serve as start values for the new fiscal year.
For each asset, SAP Business One recalculates the planned depreciation for the new fiscal year.
Fiscal Year Change Window Fields
From Fiscal Year
Select the fiscal year you want to change.
To Fiscal Year
Displays the fiscal year to which the change is made. The system always selects the subsequent fiscal year.
Asset Depreciation Forecast Report
To help you plan the value development of your fixed assets from both the management and accounting perspectives, SAP
Business One provides you with the depreciation forecast report to forecast and simulate an assets's future depreciations.
More Information
Asset Depreciation Forecast Report - Selection Criteria
Asset Depreciation Forecast Report Window
Asset Depreciation Forecast Report - Selection Criteria
Use this window to specify the selection criteria for the asset depreciation forecast report.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset
Depreciation Forecast Report .
Selection Criteria
Asset No. From ... To
Specify the range of assets that you want to include in the depreciation forecast report.
 Note
The following assets are not displayed in the report:
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:03 AM
New assets which have not been capitalized
Assets which retired in fiscal years before the forecast period
Balance Sheet Account
Select the balance sheet account for the assets you want to include in the report.
The assets which use the specified account are displayed in the report.
 Note
If you select a balance sheet account and a non-posting depreciation area at the same time, the system prompts an error as
there is no balance sheet account in a non-posting depreciation area.
Depreciation Area
Select the depreciation area in which the depreciation forecast is carried out.
 Note
If you select a balance sheet account and a non-posting depreciation area at the same time, the system prompts an error as
there is no balance sheet account in a non-posting depreciation area.
Forecast Date From ... To
Specify the period for which you want to carry out the depreciation forecast.
By default, the From field displays one of the following:
If you have executed the fiscal year change, the From date displays the first day of the fiscal year to which the last change is
executed.
If you have not executed a fiscal year change, the From date displays the first day of the current fiscal year.
In the To field, you must specify a date that is the last day of a fiscal year. Otherwise, the system automatically changes it to the
last day of the fiscal year according to the From date.
Summarize By
Select one of the following options to split the forecast period for assets in the report:
Project – The system splits the forecast period according to the validity periods of the projects assigned to the assets.
Distr. Rule – The system splits the forecast period according to the validity periods of the distribution rules assigned to the
assets.
Project and Distr. Rule – The system splits the forecast period according to the validity periods of the projects and
distribution rules assigned to the assets.
If you do not select any of the above options, the system splits the forecast period by fiscal years.
 Note
If you select Distr. Rule or Project and Distr. Rule, you can also specify the dimension.
Dimension
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:03 AM
The field is available only if you have selected Distr. Rule or Project and Distr. Rule.
Select the dimension to which the distribution rules are assigned.
Once you select a dimension, the system displays only the distribution rules relevant to this dimension in the report.
More Information
Asset Depreciation Forecast Report Window
Asset Depreciation Forecast Report
Asset Depreciation Forecast Report Window
Use this window to view the details of an asset's depreciation forecast.
To open the window, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset Depreciation
Forecast Report .
2. In the Asset Depreciation Forecast Report - Selection Criteria window, specify the selection criteria and choose OK.
The Asset Depreciation Forecast Report window opens.
Asset Depreciation Forecast Report Window Fields
Asset No.
Displays the asset number.
Asset Description
Displays the description of the asset.
Year
Displays the fiscal years in the forecast period in separate rows.
Project
 Note
The field is hidden unless you choose to summarize the report by projects in the report selection criteria.
Displays the projects assigned to each asset.
Distr. Rule
 Note
The field is hidden unless you choose to summarize the report by distribution rules in the report selection criteria.
Displays the distribution rules assigned to each asset.
Period Start Date
Displays the start date of each period.
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:03 AM
If you choose to summarize the report by projects or distribution rules, the system splits the forecast period according to the
validity periods of the projects or distribution rules assigned to the assets.
If you do not choose to summarize the report, the system splits the forecast period by fiscal years.
Period End Date
Displays the end date of each period.
If you choose to summarize the report by projects or distribution rules, the system splits the forecast period according to the
validity periods of the projects or distribution rules assigned to the assets.
If you do not choose to summarize the report, the system splits the forecast period by fiscal years.
APC
Displays the asset's acquisition and production costs at the end of each period.
Accum. Ordinary Depr.
Displays the asset's accumulated ordinary depreciation at the beginning of each fiscal year in the forecast period.
Accum. Unplanned Depr.
Displays the asset's accumulated unplanned depreciation at the beginning of each fiscal year in the forecast period.
Accum. Special Depr.
Displays the asset's accumulated special depreciation at the beginning of each fiscal year in the forecast period.
Accum. Write-Up
Displays the asset's accumulated write-up at the beginning of each fiscal year in the forecast period.
Ordinary Depr.
Displays the asset's ordinary depreciation in each period.
Unplanned Depr.
Displays the asset's unplanned depreciation.
Special Depr.
Displays the asset's special depreciation.
Write-Up
Displays the asset's write-up.
NBV
Displays the asset's net book value at the end of each fiscal year in the forecast period.
Historical NBV
Displays the asset's historical net book value at the end of each fiscal year in the forecast period.
The historical net book value is the net book value of the asset that is calculated without taking into account any unplanned
depreciation, appreciation or write-up.
More Information
Asset Depreciation Forecast Report - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:03 AM
Asset Depreciation Forecast Report
Asset History Sheet
The asset history sheet is the most important supplement to the balance sheet from the fixed asset point of view. The report
shows all the changes to the asset portfolio in a fiscal year or a specific period of a fiscal year.
You can create the report for all assets, assets using the same balance sheet account, or a specific asset.
More Information
Asset History Sheet - Selection Criteria
Asset History Sheet Window
Asset History Sheet - Selection Criteria
Use this window to specify the selection criteria for the asset history sheet.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset
History Sheet .
Selection Criteria
Asset Class From ... To
Specify the asset classes of the assets you want to include in the asset history sheet.
 Note
The following assets are not displayed in the report:
New assets which have not been capitalized
Assets which retired in fiscal years before the reported period.
Balance Sheet Account
Select the balance sheet account for the assets you want to include in the report.
 Note
If you select a balance sheet account and a non-posting depreciation area at the same time, the system prompts an error as
there is no balance sheet account in a non-posting depreciation area.
Depreciation Area
Select the depreciation area in which you want to see the asset values.
 Note
If you select a balance sheet account and a non-posting depreciation area at the same time, the system prompts an error as
there is no balance sheet account in a non-posting depreciation area.
Period
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:03 AM
Select the fiscal year in which you want to view the asset value changes. You can select from all fiscal years defined in SAP
Business One.
Subperiod From ... To
To view the asset value changes in a sub period in the selected fiscal year, specify the period range.
Template
Select a template for the asset history sheet.
To define a template for the asset history sheet, go to the Financial Report Templates window.
Project From … To …, Distribution Rule From … To...
To include the assets that are assigned to specific projects and distribution rules, specify the ranges.
More Information
Asset History Sheet Window
Asset History Sheet
Asset History Sheet Window
Use this window to view the asset value changes over the course of a fiscal year or a specific period of a fiscal year.
The assets displayed in this window are grouped by balance sheet accounts and asset classes.
To access the window, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset History Sheet
.
2. In the Asset History Sheet - Selection Criteria window, specify the selection criteria and choose OK.
The Asset History Sheet window opens.
Asset History Sheet Window Fields
Balance Account
 Note
The field is available only if you have selected a Posting to G/L depreciation area in the report selection criteria.
Displays the asset's balance sheet account in the depreciation area selected in the report selection criteria.
Account Name
 Note
The field is available only if you have selected a Posting to G/L depreciation area in the report selection criteria.
Displays the name of the asset balance sheet account.
Asset Class
Displays the asset class of the assets.
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:03 AM
Asset No.
Displays the asset number of each asset.
Asset Description
Displays the description of the asset.
Historical APC
Displays the asset's historical APC as specified in the asset master data.
Capitalization Date
Displays the asset's capitalization date.
Useful Life (Months)
Displays the asset's total useful life in months.
Remaining Life (Months)
Displays the asset's remaining life in months at the end of the reported period.
Depr. Type
Displays the asset's depreciation type assigned to the depreciation area selected in the report selection criteria.
APC on Start Date
Displays the asset's acquisition and production costs on the first day of the reported period.
Accum. Depr. on Start Date
Displays the asset's accumulated depreciation on the first day of the reported period.
Accum. Write-Up on Start Date
Displays the asset's accumulated write-up on the first day of the reported period.
NBV on Start Date
Displays the asset's net book value on the first day of the reported period.
Capitalization
Displays the asset's capitalization amount in the reported period.
Retired APC
Displays the asset's retired acquisition and production costs in the reported period.
Retired NBV
Displays the asset's retired net book value in the reported period.
For more information about how the system calculates retired net book value, see Retirement Window.
Transferred APC
Displays the asset's transferred acquisition and production costs in the reported period.
Transferred NBV
Displays the asset's transferred net book value in the reported period.
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:03 AM
For more information about how the system calculates transferred net book value, see Transfer Window.
Write-Up
Displays the asset's write-up in the reported period.
Depreciation
Displays the asset's depreciation in the reported period.
APC on End Date
Displays the asset's acquisition and production costs on the last day of the reported period.
NBV on End Date
Displays the asset's net book value on the last day of the reported period.
Accum. Depr. on End Date
Displays the asset's accumulated depreciation on the last day of the reported period.
Project, Distribution Rule
Displays the asset's project and distribution rule in the reported period.
More Information
Asset History Sheet - Selection Criteria
Asset History Sheet
Asset Status Report
In SAP Business One, you can use the asset status report to view an asset's overall information, such as the asset class, useful life,
and depreciation type. The report provides you with easy access to an overview of all your fixed assets.
You can create the report for specific asset classes, and you can also filter the assets by their statuses.
More Information
Asset Status Report - Selection Criteria
Asset Status Report Window
Asset Status Report - Selection Criteria
Use this window to specify the selection criteria for the asset status report.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset
Status Report .
Selection Criteria
Asset No. From ... To
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:03 AM
Specify the range of assets that you want to include in the asset status report.
Asset Class From ... To
To narrow down the asset range, specify the range of asset classes of the assets you want to include in the asset status report.
Period
Select the fiscal year for which you want to view the asset data.
Display New Fixed Assets
To display new fixed assets in the report, select the checkbox.
Display Active Fixed Assets
To display active fixed assets in the report, select the checkbox.
Display Inactive Fixed Assets
To display inactive fixed assets in the report, select the checkbox.
More Information
Asset Status Report Window
Asset Status Report
Asset Status Report Window
Use this window to view the overall information of an asset.
To access the window, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset Status Report
.
2. In the Asset Status Report - Selection Criteria window, specify the selection criteria and choose OK.
The Asset Status Report window opens.
Asset Status Report Window Fields
Asset No.
Displays the asset number.
Asset Description
Displays the description of the asset.
Asset Class
Displays the asset class to which the asset is assigned.
Status
Displays the asset's current status – New, Active or Inactive.
Asset Group
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:03 AM
Displays the asset group to which the asset belongs.
Depreciation Area
Displays the asset's associated depreciation areas.
Depreciation Start Date
Displays the asset's depreciation start date.
Depreciation End Date
Displays the asset's depreciation end date.
Useful Life (Months)
Displays the asset's total useful life, in months.
Remaining Life (Months)
Displays the asset's remaining life at the beginning of the fiscal year selected in the report selection criteria.
Depreciation Type
Displays the depreciation type assigned to the asset in each depreciation area.
More Information
Asset Status Report - Selection Criteria
Asset Status Report
Asset Transaction Report
The asset transaction report provides you with a list of all transactions relevant to an asset.
SAP Business One lets you view the following types of transactions in the report:
Acquisition – The first acquisition of an asset.
Subacquisition – The subsequent acquisitions of an asset.
Credit Memo – The credit memo created to reduce an asset's acquisition and production costs.
Full Retirement – The full retirement of a regular asset with a method of sales.
Full Scrapping – The full retirement of a regular asset using the scrapping method.
Partial Retirement – The partial retirement of a regular asset using the sales method.
Partial Scrapping – The partial retirement of a regular asset using the scrapping method.
Low Value Asset Full Retirement – The full retirement of a low value asset using the sales method.
Low Value Asset Full Scrapping – The full retirement of a low value asset using the scrapping method.
Full Transfer – The full transfer of an asset to another asset.
Partial Transfer – The partial transfer of an asset to another asset.
Asset Class Transfer – The transfer of an asset from one asset class to another asset class.
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:03 AM
Manual Ordinary Depreciation – The manual depreciation document created for an asset of the Ordinary Depreciation
type.
Manual Unplanned Depreciation – The manual depreciation document created for an asset of the Unplanned
Depreciation type.
Manual Special Depreciation – The manual depreciation document created for an asset with the Special Depreciation
type.
Appreciation – The manual depreciation document created for an asset of the Appreciation type.
Revaluation – The revaluation of an asset.
Change of Depreciation Type – The change of an asset's depreciation type in the asset master data.
Change of Useful Life – The change of an asset's useful life in the asset master data.
Change of Depreciation Start Date – The change of an asset's depreciation start date in the asset master data.
Change of Salvage Value – The change of an asset's salvage value in the asset master data.
Change of Period Control – The change of an asset's period control settings in the asset master data if the asset uses the
individual straight line period control depreciation method.
More Information
Asset Transaction Report - Selection Criteria
Asset Transaction Report Window
Asset Transaction Report - Selection Criteria
Use this window to specify the selection criteria for the asset transaction report.
To open the window, from the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset
Transaction Report .
Selection Criteria
Asset Class From ... To
Specify the asset classes of the assets you want to include in the asset transaction report.
Asset No. From ... To
Specify the range of assets that you want to include in the asset transaction report.
 Note
The report does not display new fixed assets as they do not have any transactions yet.
Posting Date From ... To
Specify the posting date range of the transactions that you want to include in the asset transaction report.
Document Date From ... To
Specify the document date range of the transactions that you want to include in the asset transaction report.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:03 AM
Asset Value Date From ... To
Specify the asset value date range of the transactions that you want to include in the asset transaction report.
Transaction Type
Acquisition The first acquisition of an asset
Subacquisition The subsequent acquisitions of an asset
Credit Memo The credit memo created to reduce an asset's acquisition and production costs
Full Retirement The full retirement of a regular asset with a method of sales
Full Scrapping The full retirement of a regular asset with a method of scrapping
Partial Retirement The partial retirement of a regular asset with a method of sales
Partial Scrapping The partial retirement of a regular asset with a method of scrapping
Low Value Asset Full Retirement The full retirement of a low value asset with a method of sales
Low Value Asset Full Scrapping The full retirement of a low value asset with a method of scrapping
Full Transfer The full transfer of an asset to another asset
Partial Transfer The partial transfer of an asset to another asset
Asset Class Transfer The transfer of an asset from one asset class to anther asset class
Manual Ordinary Depreciation The manual depreciation document created for an asset with the Ordinary
Depreciation type
Manual Unplanned Depreciation The manual depreciation document created for an asset with the Unplanned
Depreciation type
Manual Special Depreciation The manual depreciation document created for an asset with the Special
Depreciation type
Appreciation The manual depreciation document created for an asset with the Appreciation type
Revaluation The revaluation of an asset
 Note
The following five options are not document or transaction types. Instead, they are user actions which result in the changes of asset
values. SAP Business One lists them as transaction types here so that you can view the detailed change log in the report.
Change of Depreciation Type The change of an asset's depreciation type in the asset master data
Change of Useful Life The change of an asset's useful life in the asset master data
Change of Depreciation Start Date The change of an asset's depreciation start date in the asset master data
Change of Salvage Value The change of an asset's salvage value in the asset master data
Change of Period Control The change of an asset's period control settings in the asset master data if the asset
uses the individual straight line period control depreciation method
More Information
Asset Transaction Report Window
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:03 AM
Asset Transaction Report
Asset Transaction Report Window
Use this window to view assets' transaction details.
To access the window, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Fixed Asset Reports Asset Transaction
Report .
2. In the Asset Transaction Report - Selection Criteria window, specify the selection criteria and choose OK.
The Asset Transaction Report window opens.
Asset Transaction Report Window Fields
Asset No.
Displays the asset number.
Asset Description
Displays the description of the asset.
Doc. No.
Displays the asset transaction document number.
To view the details about the transaction, choose to open the corresponding document.
 Note
If the transaction type is any of the following, there is no document number as none of the following is an actual document in
the system:
Change of Depreciation Type
Change of Useful Life
Change of Depreciation Start Date
Change of Salvage Value
Change of Period Control
Posting Date
Displays the posting date of the document.
 Note
If the transaction type is any of the following, the field displays the date when you made the change:
Change of Depreciation Type
Change of Useful Life
Change of Depreciation Start Date
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:03 AM
Change of Salvage Value
Change of Period Control
Document Date
Displays the document date.
 Note
If the transaction type is any of the following, the field displays the date when you made the change:
Change of Depreciation Type
Change of Useful Life
Change of Depreciation Start Date
Change of Salvage Value
Change of Period Control
Asset Value Date
Displays the asset value date of the document.
 Note
If the transaction type is any of the following, the field displays the first day of the fiscal year selected in the asset master data
when you made the change:
Change of Depreciation Type
Change of Useful Life
Change of Depreciation Start Date
Change of Salvage Value
Change of Period Control
Transaction Type
Displays the type of the transaction.
For more information about each transaction type, see Asset Transaction Report.
Depreciation Area
Displays in which depreciation areas the transaction takes effect.
Amount
Displays the amount in each transaction.
Cancelled
Indicates whether the transaction has been cancelled.
Remarks
Displays the change log for the following transaction types:
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:03 AM
Change of Depreciation Type
Change of Useful Life
Change of Depreciation Start Date
Change of Salvage Value
Change of Period Control
More Information
Asset Transaction Report - Selection Criteria
Asset Transaction Report
Importing Fixed Asset Master Data from Microsoft Excel
After you enable fixed assets, you can import the fixed asset master data from Microsoft Excel into SAP Business One.
Before you start importing, you can prepare the asset-related values in the Microsoft Excel sheet. Note that all asset values must
be the values at the beginning of a fiscal year. During the import, you can specify the fiscal year, and then the system transfers all
values to the asset master data in SAP Business One as the beginning values of the specified fiscal year.
Prerequisites
You have specified the following information in the Microsoft Excel sheet for the different types of assets you want to
import:
New Assets – Assets that do not have a depreciation start date
For new assets, you have specified the following:
Item no.
Asset class
Depreciation area
Useful life
Remaining life
Depreciation type
Active Assets – Assets that have a depreciation start date and do not have a retirement date
For active assets, you have specified the following:
Item no.
Asset class
Depreciation area
Useful life
Remaining life
Depreciation type
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:03 AM
Acquisition and production costs
Accumulated ordinary depreciation
Inactive Assets – Assets that have a retirement date and the net book value of which is zero
For inactive assets, you have specified the following:
Item no.
Asset class
Depreciation area
The following values in the Microsoft Excel sheet already exist in SAP Business One:
Asset class
Depreciation area
Depreciation type
Pool of depreciation type
Asset group
Depreciation group
Sales tax definition
Purchase tax definition
Procedure
1. From the SAP Business One Main Menu, choose Administration Data Import/Data Export Data Import Import
Fixed Asset Master Data from Excel .
2. In the Import Fixed Asset Master Data from Excel window, select the fiscal year of which you want to import the asset
related values.
 Note
The system copies the asset values from the Microsoft Excel sheet to SAP Business One as the beginning asset values
of the selected fiscal year.
3. To map the Microsoft Excel sheet columns with the SAP Business One fields, do either of the following:
If you have saved a data mapping template, load the template by choosing in the Use Data Template field.
If you do not have a data mapping template yet, specify the data mapping method by using the Column and Field
columns.
To save the mapping method as a template, choose the Save As pushbutton.
4. Choose OK.
After the import is completed, you can find the assets in the asset master data.
More Information
Import Fixed Asset Master Data from Excel Window
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:03 AM
Import Fixed Asset Master Data from Excel Window
Use this window to map the Microsoft Excel sheet columns to the fixed asset data in SAP Business One.
You can save the data mapping method as a template to use directly for future imports.
To access the window, from the SAP Business One Main Menu, choose Administration Data Import/Data Export Data
Import Import Fixed Asset Master Data from Excel .
General Area Fields
Import to Fiscal Year
Select the fiscal year of which you want to import the asset values.
The system copies the asset values from the Excel sheet to the asset master data in SAP Business One as the values at the
beginning of the specified fiscal year.
Use Data Template
If you have saved a data mapping template, you can load the template by choosing .
To save the data mapping method as a template, choose the Save As pushbutton.
Save As
Lets you save the data mapping method as a template for future imports.
Table Area Fields
Column
Displays the columns in the Microsoft Excel sheet.
Field
Select the SAP Business One field to which each column in the Microsoft Excel sheet corresponds.
You can select among the following:
Item Description – The Item Description field in the asset master data.
Description in Foreign Lang. – The Foreign Name field in the asset master data.
Bar Code – The Bar Code field in the asset master data.
Sales Tax Definition – The Tax Group field on the Sales Data tab in the asset master data.
Purchase Tax Definition – The Tax Group field on the Purchasing Data tab in the asset master data.
Asset Class – The Asset Class field in the asset master data.
Capitalization Date – The Capitalization Date field on the Overview subtab of the Fixed Assets tab in the asset master
data.
Retirement Date – The date on which an asset retires completely. The value is stored in the database.
Asset Group – The Asset Group field on the Overview subtab of the Fixed Assets tab in the asset master data.
Depreciation Group – The Depreciation Group field on the Overview subtab of the Fixed Assets tab in the asset master
data.
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:03 AM
Inventory Number of Asset – The Inventory No. field on the Overview subtab of the Fixed Assets tab in the asset master
data.
Asset Serial Number – The Serial Number field on the Overview subtab of the Fixed Assets tab in the asset master data.
Depreciation Area – The Depreciation Area field on the Overview subtab of the Fixed Assets tab in the asset master data.
Depreciation Start Date – The Depreciation Start Date field on the Overview subtab of the Fixed Assets tab in the asset
master data.
Useful Life – The Useful Life field on the Overview subtab of the Fixed Assets tab in the asset master data.
Remaining Life – The Remaining Life field on the Overview subtab of the Fixed Assets tab in the asset master data.
Depreciation Type – The Depreciation Type field on the Overview subtab of the Fixed Assets tab in the asset master data.
APC – The Acquisition and Production Costs field on the Overview subtab of the Fixed Assets tab in the asset master
data.
Historical APC – The Historical APC field on the Overview subtab of the Fixed Assets tab in the asset master data.
Asset Quantity – The Quantity field on the Overview subtab of the Fixed Assets tab in the asset master data.
Salvage Value – The Salvage Value field on the Overview subtab of the Fixed Assets tab in the asset master data.
Accumulated Ordinary Depr. – The accumulated ordinary depreciation of an asset. The value is stored in the database.
Accumulated Unplanned Depr. – The accumulated unplanned depreciation of an asset. The value is stored in the database.
Special Depreciation 01, 02, 03 – The special depreciation of an asset in depreciation pool 01, 02, and 03. The values are
stored in the database.
Accumulated Special Depr. 01, 02, 03 – The accumulated depreciation of an asset in depreciation pool 01, 02, and 03. The
values are stored in the database
Accumulated Write-Up – The accumulated write-up of an asset. The value is stored in the database.
More Information
Importing Fixed Asset Master Data from Microsoft Excel
Working with Fixed Assets Data Migration Wizard
Prerequisites
You have data in the Fixed Assets add-on to be migrated.
You have backed up the company database.
You are the only user that is logged on to the company database.
Context
You can import data from the Fixed Assets add-on to SAP Business One with the Fixed Asset Data Migration wizard if you are
working with the add-on before it was integrated into SAP Business One 9.0. From the SAP Business One Main Menu, choose
Administration Utilities Fixed Assets Data Migration Wizard .
You can migrate the following data from the Fixed Assets add-on to SAP Business One:
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:03 AM
Account determination
Depreciation areas
Depreciation types
Asset classes
Asset master data
When importing the asset master data, the system can only copy the asset values at the beginning of a fiscal year from the add-on
to SAP Business One. Usually, this is the year to which the last fiscal year change is carried out in the add-on. If asset transactions
take place during the fiscal year, you must manually create these transactions in SAP Business One as the transactions cannot be
imported.
For example, in the Fixed Assets add-on, asset X has a net book value of 5000 USD on January 1st, 2012. On October 1st, 2012, the
asset retires completely and becomes inactive.
In November, you import the asset-related data from the add-on into SAP Business One. After the import is completed, you can
find asset X in SAP Business One with a net book value of 5,000 USD at the beginning of fiscal year 2012. There is no record of its
retirement and the asset is still in active status. In this case, you must create the asset retirement transactions in SAP Business
One all over again.
Start a New Migration Run
The interactive graphics below help you navigate through this section. Choose the highlighted areas for more information.
Please note that image maps are not interactive in PDF outputs.
Load Executed Migration Runs
The interactive graphics below help you navigate through this section. Choose the highlighted areas for more information.
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:03 AM
Please note that image maps are not interactive in PDF outputs.
Step 1: Selecting Wizard Options
On the Wizard Options page, specify whether you want to start a new migration run or load an executed migration run.
Wizard Options Fields
Start a New Migration Run
Select the option to create a new migration run.
Load Executed Migration Runs
Select this option to view the details of previously executed migration runs.
 Note
The following fields are available only if you have selected the Load Executed Migration Runs option.
Find
Enter the name of the executed migration run for which you want to view the details.
Migration Run Name
Displays the names of the previously executed migration runs.
Date
Displays the date on which each migration run is carried out.
Status
Displays one of the following:
Successful – Indicates all the objects are successfully migrated.
Partially Successful – Indicates some objects are successfully migrated while some are not.
Failed – Indicates no objects are migrated.
Remarks
Displays the remarks of each depreciation run.
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:03 AM
Related Information
Working with Fixed Assets Data Migration Wizard
Step 2: Specifying Migration Parameters
On the Migration Parameters page, specify the migration run name and migration options.
 Note
If you chose to view an executed migration run in step 1, you can only view the detailed parameters of the migration run in this
step.
Migration Parameters Fields
Migration Run Name
Enter the name of the migration run.
Migrate Data for Fiscal Year
Displays one of the following:
If you have executed fiscal year changes in the add-on, the field displays the fiscal year to which the last change was made.
If you have not executed fiscal year changes in the add-on, the field displays the last year in which the values of the
migrated assets were calculated in the add-on.
 Note
During the migration, the system migrates the asset values at the beginning of the fiscal year from the add-on to SAP Business
One.
If asset transactions that took place during the year exist in the add-on, you must manually create these transactions in SAP
Business One as you cannot migrate asset transactions using this wizard.
Remarks
If required, enter remarks about the migration run.
Fixed Asset Data
Displays the fixed asset-related data that are migrated from the add-on to SAP Business One.
Account determination records, depreciation areas, depreciation types, asset classes, and asset master data must all be migrated.
You cannot change the selection.
Migration Options
Select one of the following migration options:
Skip if Data Already Exists – If the data you want to migrate already exists in SAP Business One, the data is not migrated.
Overwrite Existing Data – If the data you want to migrate already exists in SAP Business One, the system overwrites the
data.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:03 AM
Working with Fixed Assets Data Migration Wizard
Step 3: Viewing Summary Report or Migration Results
Viewing Summary Report
 Note
If you selected Start a New Migration Run in step 1, this is the last step of the wizard.
On the Summary Report page, you view the summary report of the migration run. The report displays all error, warning, and
information messages.
To see the detailed results of the migration run, return to the first step of the wizard and select the Load Executed Migration Runs
option.
Viewing Migration Results
 Note
If you selected Load Executed Migration Runs in step 1, this is the last step of the wizard.
On the Migration Results page, view the detailed results of a previously executed migration run.
Migration Results Fields
Object Type
Displays the different types of fixed asset data that are migrated from the add-on.
Object Code
Displays the code of each migrated object.
To view the details about the migrated object, open the object window by clicking before the code.
Object Name
Displays the name or description of the migrated object.
Result
Indicates whether the object was migrated successfully.
Remarks
If the object is successfully migrated, the field displays Create Object. Otherwise, it displays an error message.
Related Information
Working with Fixed Assets Data Migration Wizard
Working with Virtual Fixed Assets
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:03 AM
With SAP Business One, you can now manage fixed assets with the virtual fixed asset function. That is, when your company needs
to purchase identical fixed assets in large quantities, you can purchase a virtual fixed asset in a certain quantity, and then SAP
Business One automatically creates the same quantity of asset master data records, and capitalizes them for you.
Using this function can free you from having to manually enter large amounts of repeated information; hence helping to improve
your company’s efficiency in managing fixed assets.
Working with Virtual Fixed Assets in SAP Business One includes the following:
Creating a Virtual Fixed Asset
Capitalizing Assets by Virtual Fixed Assets
Canceling Capitalization of Virtual Fixed Assets
Creating a Virtual Fixed Asset
Prerequisites
You have enabled the numbering series, and used a non-manual series for Items.
To set up the document numbering series, from the SAP Business One Main Menu, choose Administration System
Initialization Document Numbering .
Procedure
1. From the SAP Business One Main Menu, choose Financials Fixed Assets Asset Master Data .
2. In the dropdown list of the Item No. field in the general area, choose the predefined numbering series.
The Virtual Item checkbox appears in the general area.
3. Select the Virtual Item checkbox.
The Enforce Serial Number checkbox appears under the Virtual Item checkbox.
4. [Optional] If you want to manage assets that are generated by virtual fixed assets by serial number, select the Enforce
Serial Number checkbox.
5. Specify the required information for the asset that you want to purchase in bulk.
 Note
Once you have purchased the virtual fixed asset by A/P invoice, identical asset master data will be automatically created
by SAP Business One. Make sure you have entered all necessary information in the master data of the virtual fixed asset.
Related Information
Working with Virtual Fixed Assets
Capitalizing Assets by Virtual Fixed Assets
Canceling Capitalization of Virtual Fixed Assets
Capitalizing Assets by Virtual Fixed Assets
Prerequisites
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:03 AM
You have created asset master data with the Virtual Item checkbox selected.
To access the Asset Master Data window, from the SAP Business One Main Menu, choose Financials Fixed Assets Asset
Master Data .
Procedure
1. From the SAP Business One Main Menu, choose Purchasing A/P A/P Invoice .
2. In the A/P invoice, specify relevant information in the header.
3. In the table on the Contents tab, perform the following:
a. In the Item No. field, choose the virtual item.
b. In the Quantity field, specify the amount of the asset that you want to purchase in bulk.
c. [Optional] If you want to maintain quantity for the created asset master data, select the Consider Quantity
checkbox.
4. [Optional] If you have selected the Enforce Serial Number checkbox for the virtual fixed asset, perform the following:
a. In the A/P invoice, right click and choose Asset Serial Numbers. The Asset Serial Numbers – Setup window opens.
b. In the Asset Serial Numbers – Setup window, create a serial numbers for each asset purchased through the A/P
invoice.
5. In the A/P invoice, choose the Add button.
Results
SAP Business One automatically creates asset master data results as follows:
The information in the asset master data of the virtual fixed asset is completely copied to the newly created asset master
data, except the Virtual Item checkbox is unselected.
The quantity of the newly created asset master data is the same as the quantity you have specified in the A/P invoice.
The item numbers are automatically assigned to newly created asset master data, according to the rules you have defined
for the series used in the master data of the virtual fixed asset.
 Note
You can include multiple virtual fixed assets in the same A/P invoice, but you cannot include both virtual fixed assets
and normal fixed assets in the same A/P invoice.
To capitalize assets by virtual assets, you can use A/P invoices only; capitalization documents are not allowed for virtual
fixed assets.
Related Information
Working with Virtual Fixed Assets
Creating a Virtual Fixed Asset
Canceling Capitalization of Virtual Fixed Assets
Canceling Capitalization of Virtual Fixed Assets
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:03 AM
Prerequisites
You have capitalized fixed assets by purchasing a virtual fixed asset with an A/P invoice.
The credited amount is no greater than the total NBV of credited assets.
In the following scenarios, none of the assets were subsequently capitalized.
Scenario 1: Cancel A/P Invoices
Procedure:
In the A/P invoice with which you purchased the virtual fixed asset , right-click and choose Cancel.
Result:
The purchased assets become inactive. That is, in the Asset Master Data window of each asset, the Inactive radio button is
automatically selected.
Scenario 2: All Purchased Assets Are Fully Credited
Procedure:
1. In the A/P invoice with which you purchased the virtual fixed asset , choose the Copy To button; then choose A/P Credit
Memo.
2. The target A/P credit memo opens. Do not change either the quantity or the total amount.
3. Choose the Add button.
Result:
The APC and the net book values of all assets become zero. That is, for all relevant assets, in the Net Book Value field on the
Overview subtab of the Fixed Assets tab of the Asset Master Data window, the value becomes zero.
Scenario 3: All Purchased Assets Are Credited with Partial Amount
Procedure:
1. In the A/P invoice with which you purchased the virtual fixed asset , choose the Copy To button; then choose A/P Credit
Memo. The target A/P credit memo opens.
2. In the A/P Credit Memo window, change the total amount to a smaller value.
3. Choose theAdd button.
Result:
The credited amount is distributed equally to each asset. The APC and the net book value of each asset decrease by the
distributed amount.
Scenario 4: Partial Assets Are Credited
Procedure:
1. In the A/P invoice with which you purchased the virtual fixed asset , choose the Copy To button; then choose A/P Credit
Memo. The target A/P credit memo opens.
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:03 AM
2. In the A/P Credit Memo window, change both the quantity and the total amount to a smaller value.
3. In the table area, right-click and choose Asset Selection.
4. In the Asset Selection window, select the assets that you want to credit, and choose OK .
5. In the A/P Credit Memo window, choose the Add button.
Result:
One of the following happens:
If the credited amount is equal to the total NBV of all credited assets:
The net book value of each credited asset becomes zero.
The APC of each credited asset decreases by the NBV amount, or becomes zero.
If the credited amount is less than the total NBV of all credited assets:
The credited amount is distributed equally to each credited asset.
The APC and the net book value of each credited asset decrease by the distributed amount.
More Information
Working with Virtual Fixed Assets
Creating a Virtual Fixed Asset
Capitalizing Assets by Virtual Fixed Assets
Cost Accounting
In addition to their regular bookkeeping, many businesses perform expense and revenue analysis that measure the profitability of
each of their business activities or departments.
The cost accounting function in SAP Business One enables you to define sets of cost centers and distribution rules and apply them
in almost all marketing documents. Generating respective reports provides important cost-related information.
SAP Business One provides two cost accounting methods: distribution rules and projects.
 Note
You can set cost accounting-relevant configurations on the Cost Accounting tab of the General Settings window under
Administration System Initialization General Settings .
The diagram below shows the topics covered in this section. Choose each topic for more information.
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:03 AM
Please note that image maps are not interactive in PDF outputs.
For more information about cost accounting windows and cost accounting reports, choose the topics below.
Please note that image maps are not interactive in PDF outputs.
More Information
General Settings: Cost Accounting Tab
Working with Dimensions
Dimensions configured in the system provide customers with multiple views of an expense and revenue analysis.
Authorization is required for viewing and defining dimensions.
To define dimensions, choose Financials Cost Accounting Dimensions .
 Note
This window appears only after you select the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
More Information
General Settings: Cost Accounting Tab
Dimensions Window
Working with Cost Centers and Distribution Rules
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:03 AM
A cost center is a company unit or division that performs a specific business function.
For expenses and revenues that can be assigned directly to a cost center, you define a direct distribution rule. When you create a
cost center, SAP Business One automatically creates a distribution rule. You cannot change this distribution rule. The default
values of the distribution rule are as follows:
Values in the Code and Description fields are the same as they appear in the Cost Center and Name fields, respectively, of
the corresponding cost center.
The dimension and effective period are the same as those of the corresponding cost center.
The Active and Direct Allocation checkboxes are automatically selected.
The value of the corresponding cost center is 100, for a total value of 100.
More Information
Working with Cost Centers
Working with Distribution Rules
Working with Cost Centers
A cost center is a company unit or division that performs a specific business function, such as manufacturing specific products or
providing a specific service. The cost center you define here represents the respective division or department, and is used to
consolidate the expenses and revenues resulting from the ongoing activity of the specific organizational unit.
Authorization is required for viewing and defining cost centers.
To define cost centers, choose Financials Cost Accounting Cost Centers .
 Note
A distribution rule is automatically created for each cost center you create.
More Information
Working with Cost Centers and Distribution Rules
Allocating Expenses/Revenues to Cost Centers
Assigning Cost Centers to Expense/Revenue and COGS Accounts
Cost Centers – Setup Window
Allocating Expenses/Revenues to Cost Centers
This example illustrates how to allocate two amounts from an accounting document to two cost centers as follows: amount 1 to
cost center CC1, and amount 2 to cost center CC2.
Prerequisites
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:03 AM
You have defined cost centers CC1 and CC2 in Financials Cost Accounting Cost Centers .
You have prepared the relevant accounting document, but have not yet added it to the database.
Procedure
If you did not select the Use Multidimensions checkbox on the Cost Accounting tab of the General Settings window under
Administration System Initialization General Settings , in the Distr. Rule field of the row with amount 1/amount 2,
specify distribution rule CC1/CC2.
If you selected the Use Multidimensions checkbox, do the following:
If you selected the In a Unified Column radio button, then in the Distr. Rule field of the row with amount 1/amount 2,
specify distribution rule CC1/CC2 for the required dimension.
If you selected the In Separate Columns radio button, then in the XXX field (XXX is the description of the required
dimension) of the row with amount 1/amount 2, specify distribution rule CC1/CC2.
 Note
SAP Business One automatically creates distribution rules CC1 and CC2 once you create cost centers CC1 and CC2.
Result
When you add the document to the database, amount 1 is allocated to cost center CC1, and amount 2 is allocated to cost center
CC2.
More Information
Working with Cost Centers
General Settings: Cost Accounting Tab
Assigning Cost Centers to Expense/Revenue and COGS
Accounts
 Note
COGS accounts are relevant only to A/R documents.
When you create an accounting document that involves expense/revenue and cost of goods sold (COGS) accounts (such as
deliveries, A/R invoices, returns, A/R invoices + payments, and A/R credit memos), the transaction amounts are:
Posted to the default expense/revenue or COGS accounts
Allocated to the cost centers that are linked to these accounts through distribution rules
The following procedure illustrates how to link different cost centers to the expense/revenue and COGS accounts for all/specific
document rows.
Prerequisites
You have defined the required cost centers in Financials Cost Accounting Cost Centers .
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:03 AM
You have prepared the relevant accounting document, but have not yet added it to the database.
Procedure
1. On the Table Format tab of the Form Settings window for the accounting document, select the Visible and Active
checkboxes for the Distr. Rule and COGS Distr. Rule columns.
 Note
If you selected the In Separate Columns radio button on the Cost Accounting tab of the General Settings window in
Administration System Initialization General Settings , select the two checkboxes for the XXX and COGS XXX
columns, where XXX is the description of active dimensions.
The two columns appear on the Contents tab of the accounting document.
2. Assign cost centers to expense/revenue and COGS accounts.
To assign cost centers for all document rows, proceed as follows:
a. In the Form Settings window for the accounting document, choose Document Table .
b. In the Distr. Rule field, assign to the expense/revenue account the distribution rule that is automatically
created for the required cost center.
c. In the COGS Distr. Rule field (such as deliveries, A/R invoices, returns, A/R invoices + payments, and A/R
credit memos), assign to the COGS account the distribution rule that is automatically created for the
required cost center.
d. Choose the OK button.
A system message appears asking whether you want to apply your selections to document table rows.
e. Choose the Yes button.
Your selections are applied to all document table rows.
To assign cost centers for specific document rows, proceed as follows:
a. In the Distr. Rule field or the XXX field of the row (XXX being the description of the required dimension),
assign to the expense/revenue account the distribution rule that is automatically created for the required
cost center.
b. In the COGS Distr. Rule field or the COGS XXX field of the row (XXX being the description of the required
dimension), assign to the COGS account the distribution rule that is automatically created for the required
cost center.
3. When the accounting document is complete, choose the Add button.
 Note
If most of the document rows have the same distribution rule, you can first assign the distribution rule to all document rows
and then assign a distribution rule to the exceptional rows.
Result
In the accounting document you created, the selected distribution rules appear in the Distr. Rule and COGS Distr. Rule
columns (or XXX and COGS XXX columns, where XXX is the description of the required dimension).
The cost centers are linked to the amounts posted to the expense/revenue and COGS accounts through distribution rules.
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:03 AM
These amounts are reflected in cost accounting reports.
More Information
Working with Cost Centers
General Settings: Cost Accounting Tab
Working with Distribution Rules
A distribution rule is a cost accounting method used to allocate direct and indirect expenses and revenues to one or more cost
centers. It contains information regarding the portion or the fixed amounts of the expenses or revenues to be allocated to each
cost center.
 Example
To distribute the indirect expenses incurred by rent, you can specify the portion of the total rented space that a specific cost
center uses. If one store uses 150 square yards of the total rented floor space of 200 square yards, and the other uses only 50
square yards, you can distribute the expenses incurred by rent and professional cleaning services proportionately between the
stores on the basis of the space they occupy. To achieve this, you can assign the distribution rules to the appropriate expense
accounts and revenue accounts.
Another way of defining such a distribution rule would involve expressing the number of employees belonging to a cost center
as a proportion of the total head count in the company.
 Example
Sometimes fixed amounts are required to be allocated to specific cost centers. For example, the front-office employees are in
the field a lot; however, the back-office employees are not. So, the company wants to allocate a fixed amount of the electric
expense to the finance department and the HR department. To achieve this, in the table you can define USD 50.00 for Cost
Center Fin Dep. and USD 30.00 for Cost Center HR Dep.
If you want to allocate the rest (the difference between the exact bill amount and the defined total amount of USD 80.00) to the
sales department, select Cost Center Sales Dep. in the table, but do not define any value for it. If you want to allocate the rest to
the zero cost center (Centr_z), which is only used in reports, keep only Cost Center Fin Dep. and Cost Center HR Dep. in the
table.
You can link distribution rules to the respective expenditure and sales G/L accounts of the business. As a result, the amount of
each accounting transaction that is posted to these accounts is recorded in the respective cost centers according to the ratio
defined in the distribution rules.
SAP Business One provides the following three kinds of distribution rules:
Distribution rules that SAP Business One creates when you create cost centers. This kind of distribution rule has a one-to-
one relationship with the corresponding cost centers.
Distribution rules that you create as master data. This kind of distribution rule is the most common one. You create it to
allocate direct and indirect expenses and revenues to one or more cost centers.
Distribution rules that you create manually for individual transactions. This kind of distribution rule is defined for particular
transactions and does not affect the distribution rule master data.
Authorization is required for viewing and defining distribution rules.
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:03 AM
To define distribution rules, choose Financials Cost Accounting Distribution Rules .
More Information
Working with Cost Centers and Distribution Rules
Displaying and Editing Distribution Rules
Defining Cost Accounting Methods for G/L Accounts
Updating Distribution Rules in Accounting Documents and Manual Journal Entries
Specifying One-Time Distribution Rules
Distribution Rules – Setup Window
Displaying and Editing Distribution Rules
Context
 Note
You can only display (not edit) a direct distribution rule that is automatically created for a cost center. You can display and edit
other distribution rules.
Procedure
1. From the SAP Business One Main Menu, choose Financials Cost Accounting Distribution Rules .
The Distribution Rules – Setup window appears.
2. In Find mode, use the search functions to find the required distribution rule.
You can edit a distribution rule by, for example, adding new cost centers to it, or changing the factors used to allocate
expenses and revenues.
For more information about the fields in this window, see Distribution Rules - Setup Window.
3. To save your changes, choose the Update button.
Related Information
Working with Distribution Rules
Defining Cost Accounting Methods for G/L Accounts
SAP Business One provides two cost accounting methods: distribution rules and projects.
SAP Business One provides two types of cost accounting method settings for G/L accounts:
Checking the cost accounting method assignment of G/L accounts
Assigning default cost accounting methods to G/L accounts
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:03 AM
Prerequisites
You have defined the required projects in Administration Setup Financials Projects .
You have defined the required distribution rules in Financials Cost Accounting Distribution Rules .
You have defined the required G/L accounts in Financials Chart of Accounts .
Procedure
1. From the SAP Business One Main Menu, choose Financials Chart of Accounts .
The Chart of Accounts window appears.
2. Select the required G/L account for which you want to define cost accounting methods.
3. Select the Project checkbox, which sets the G/L account as relevant to project. You can also specify a default project for
the account.
For G/L accounts relevant to project, SAP Business One performs actions defined on the Cost Accounting tab of the
General Settings window, in Administration System Initialization General Settings , for postings in which such G/L
accounts are without project assignment.
4. In the Distribution Rule section, select one or more checkboxes to set the G/L account as relevant to distribution rules of
corresponding dimensions. You can also specify default distribution rules for corresponding dimensions.
 Note
Distribution rule fields are editable only for G/L accounts of type Sales or Expenditure.
For G/L accounts relevant to distribution rules, SAP Business One performs actions defined on the Cost Accounting tab of
the General Settings window for postings in which such G/L accounts have no distribution rule assigned to the selected
dimensions.
5. In the Chart of Accounts window, choose the Update button.
 Note
The cost accounting methods assigned to G/L accounts in this procedure function as the default methods when you post
different transactions in SAP Business One. You might have transactions or documents in which you are required to assign
different cost accounting methods to a specific account. In such cases, the default cost accounting methods can be changed in
most windows.
More Information
Working with Distribution Rules
Chart of Accounts Window
General Settings: Cost Accounting Tab
Specifying One-Time Distribution Rules
Updating Distribution Rules in Accounting Documents and
Manual Journal Entries
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:03 AM
Context
An accounting document is a logistics document recording a business transaction that generates journal entries, that is, postings
to accounts.
If you add accounting documents or manual journal entries to SAP Business One, transaction amounts are posted to various cost
centers according to the distribution rules defined for the G/L accounts.
At times, you may want to use a different distribution rule for a transaction. For example, if you have some cleaning work done that
also involves renovation, you might want to post the expenses not to your usual cleaning expense account, but to a different
account. In such a case, you need to change the distribution rule specified in the accounting document or manual journal entry.
Procedure
1. On the Table Format tab of the Form Settings window for the accounting document or manual journal entry, select the
Visible and Active checkboxes for the Distr. Rule column.
 Note
If you selected the In Separate Columns radio button on the Cost Accounting tab of the General Settings window in
Administration System Initialization General Settings , select the two checkboxes for the XXX column, where
XXX is the description of active dimensions.
The column appears on the Contents tab of the accounting document or in the Journal Entry window.
2. In the Distr. Rule or XXX field of the row for which you want to change the distribution rule, specify a different distribution
rule.
3. To save your changes, choose the Update button.
Related Information
General Settings: Cost Accounting Tab
Working with Distribution Rules
Specifying One-Time Distribution Rules
The following is a list of transactions and documents in SAP Business One where you can assign distribution rules to G/L accounts
that are involved in a specific transaction/document or a series of transactions/documents. This might be required in the following
cases:
You have assigned a default distribution rule to the G/L account, but in a specific transaction/document or series of
transactions/documents, you need to assign a different distribution rule.
You have not assigned a default distribution rule to the G/L account, but in a specific transaction/document or a series of
transactions/documents, you need to assign to it a distribution rule.
Features
In all places listed below, the distribution rules can be changed at any time (before and after the transaction/document is added),
unless otherwise stated.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:03 AM
If you specify distribution rules at both the row level and the document level, SAP Business One takes the distribution rule
information from the row level.
Financials Module
Journal entries / journal voucher entries – the Distr. Rule field is active at both the row level and the document level. You
can access the field in the expanded editing mode, or in the table directly, or on the Table subtab of the Document tab in
the Form Settings window. Use the last option to assign distribution rules at the document level.
Posting templates / recurring postings – the Distr. Rule column is active at the row level. Assign to each row the required
distribution rule. Journal entries that are created from posting templates / recurring postings automatically record
distribution rules in the posting templates / recurring postings as default distribution rules.
Sales and Purchasing Documents
In sales and purchasing documents, the Distr. Rule column is active at both the row level and the document level.
In sales documents of type Item, you can specify distribution rules for the cost of goods sold (COGS) account. The COGS
Distr. Rule column is active at both the row level and the document level.
Freight
In the Freight – Setup window in Administration Setup General Freight , the Distr. Rule column is active at the row
level. The distribution rule you specify here is used by default, at both the row level and the document level, whenever
freight is used.
In all sales and purchasing documents, the Distr. Rule column for freights is active at both the row level and the document
level.
To specify distribution rules for freight at the row level, on the Table Format tab of the Form Settings window, select
the Visible and Active checkboxes for the columns Freight 1 Distr. Rule, Freight 2 Distr. Rule, and Freight 3 Distr.
Rule, and specify a required distribution rule for each freight item.
To specify distribution rules for freight at the document level, in the Freight field, choose . In the Freight Charges
window, specify a required distribution rule for each freight item.
Banking Module
Incoming and outgoing payments – the Distr. Rule column is active at the row level.
Payment wizard – the Distr. Rule column is active at the row level in the recommendation report.
Commission – the Distr. Rule field is active for commissions.
Inventory Module
Inventory documents – in goods receipts, goods issues, and inventory transfers, the Distr. Rule column is active at the row
level.
Inventory revaluation, inventory opening balances, inventory tracking, and inventory posting – the Distr. Rule column is
active at the row level.
Production Module
Production orders – the Distr. Rule column is active at the row level.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 130

6/8/26, 6:03 AM
Working with Distribution Rules
Working with Accrual Types
An accrual type is a set of conditions used to represent the differences between cost accounting and financial accounting.
 Example
The legal life of a machine is 50 years, but in the company’s point of view, the estimated useful life is 60 years. This causes the
monthly depreciation expenses to be different in financial accounting and cost accounting. In this case, you need to define an
accrual type and record the cost accounting depreciation using two additional accounts. The difference then appears in the
cost accounting reconciliation report.
 Note
Accrual types are defined only for use in the cost accounting reconciliation report. They do not impact other reports.
Authorization is required for viewing and defining accrual types.
To define accrual types, choose Financials Cost Accounting Accrual Type .
More Information
Cost Accounting Reconciliation Report
Accrual Types – Setup Window
Recording Differences Between Financial Accounting and Cost Accounting – Example
Recording Differences Between Financial Accounting and Cost
Accounting – Example
This example illustrates how to record differences between financial accounting and cost accounting using accrual types.
In the example, a machine costs USD 9,000, and its legal life is 3 years (that is, the monthly depreciation is USD 250 in financial
accounting), but in the company's point of view, the estimated useful life is 5 years (that is, the monthly depreciation is USD 150 in
cost accounting).
The current monthly posting is as follows:
Debit Credit
111000 - Plant and Machinery USD 250
645010 - Plant and Machinery Depreciation USD 250
Expense
Procedure
To record the differences between financial accounting and cost accounting, proceed as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 131

6/8/26, 6:03 AM
1. In the Edit Chart of Accounts window, create two G/L accounts of type Expenditure:
645011 - Calculation Machinery Depr and 645012 - Calculation Interim Machinery Depr.
2. In the Accrual Types – Setup window, create an accrual type as follows:
Code Name Posting Acct Accrual Calculation Accrual Calculation
|     |     |                |     |        |     | Acct   | Interim Acct |     |
| --- | --- | -------------- | --- | ------ | --- | ------ | ------------ | --- |
| 01  |     | Machinery Depr |     | 645010 |     | 645011 | 645012       |     |
3. For cost accounting correction postings, you can create a monthly recurring posting, or you can manually create a journal
entry every month.
| G/L Acct/BP Code |     | G/L Acct/BP Name              |     |     | Debit   |     | Credit  |     |
| ---------------- | --- | ----------------------------- | --- | --- | ------- | --- | ------- | --- |
| 645011           |     | Calculation Machinery Depr    |     |     | USD 150 |     |         |     |
| 645012           |     | Calculation Interim Machinery |     |     |         |     | USD 150 |     |
Depr
Result
In financial accounting, the depreciation expense is USD 250, while in cost accounting, the depreciation expense is USD 150. The
difference between financial accounting and cost accounting is USD 100.
In the cost accounting reconciliation report, you can find the following records:
| Financial Accounting |     |     | Cost Accounting |     |     |     |     |     |
| -------------------- | --- | --- | --------------- | --- | --- | --- | --- | --- |
P/L Company-Related Cost Accounting Correction Cost Accounting P/L
Accounts Expense(LC) Revenue(LC) Expense(LC) Revenue(LC) Expense(LC) Revenue(LC) Expense(LC) Revenue(LC
| 645010- | USD 250 |     | USD 0 |     | USD 250 |     | USD 0 |     |
| ------- | ------- | --- | ----- | --- | ------- | --- | ----- | --- |
Plant and
Machinery
Depreciation
Expense
| 645011- | USD 150 |     | USD 0 |     | USD 0 |     | USD 150 |     |
| ------- | ------- | --- | ----- | --- | ----- | --- | ------- | --- |
Calculation
Machinery
Depr
| 645012- | USD -150 |     | USD 0 |     | USD -150 |     | USD 0 |     |
| ------- | -------- | --- | ----- | --- | -------- | --- | ----- | --- |
Calculation
Interim
Machinery
Depr
|       | USD 250 | USD 0    | USD 0 | USD 0 | USD 100 | USD 0    | USD 150 | USD 0    |
| ----- | ------- | -------- | ----- | ----- | ------- | -------- | ------- | -------- |
| Total |         | USD -250 |       | USD 0 |         | USD -100 |         | USD -150 |
This is custom documentation. For more information, please visit SAP Help Portal. 132

6/8/26, 6:03 AM
Financial Accounting Cost Accounting
P/L Company-Related Cost Accounting Correction Cost Accounting P/L
Accounts Expense(LC) Revenue(LC) Expense(LC) Revenue(LC) Expense(LC) Revenue(LC) Expense(LC) Revenue(LC
Financial USD -250 Non- USD -100 Cost USD -150
P/L Operating Accounting
P/L P/L
More Information
Accrual Types – Setup Window
Cost Accounting Reconciliation Report
Cost Accounting Reports
The following reports provide cost accounting information in your company.
Cost center report – provides information about expenses and revenues that are credited to or debited from cost centers.
Distribution report – provides information about total overhead expenses and the expenses in each cost center, according
to distribution rules.
Cost accounting summary report – provides information about transactions related to cost accounting.
Budget versus cost accounting – provides information about budget and cost accounting for budget relevant G/L
accounts.
Cost accounting reconciliation report – provides an overview of financial accounting and cost accounting in your company.
Cost Center Report
This report provides comprehensive information about expenses and revenues that are credited to or debited from cost centers.
Use the report to analyze the financial situation of cost centers in detail.
Authorization is required for viewing this report.
Use this window to specify selection criteria for the cost center report.
To open the window, choose Financials Cost Accounting Cost Center Report .
After defining the report, you can view it in the Cost Center Report window (see Cost Center Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Dimension
This is custom documentation. For more information, please visit SAP Help Portal. 133

6/8/26, 6:03 AM
From the dropdown list, select a dimension to view its related cost centers.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Template
If required and you’ve defined a cost center hierarchy, select the radio button, and from the dropdown list, select a hierarchy
template to display the cost centers in the hierarchy.
 Note
Selecting the radio button hides the Sort Code From…To… and the Summary by Sort Code fields.
Cost Center From...To...
If required, specify a range of cost centers to include in the report.
Sort Code From...To...
If required, specify a range of sort codes to include in the report only cost centers with selected sort codes.
 Note
This field appears only when you selected the Cost Center radio button.
Due Date / Posting Date / Document Date From…To…
If required, specify ranges of due dates, posting dates, or document dates to include specific postings in the report.
Summary of
From the dropdown list, select to include summaries of each cost center by distribution rules, linked accounts, or months.
Project
If required, select the checkbox and choose specific projects to further narrow down the cost centers to be displayed in the report.
Display by Posting Date / Due Date
Select the way of displaying when the report is summarized by months.
 Note
This field appears only when you selected Months in the Summary of dropdown list.
Summary by Sort Code
If required, select the checkbox to include summaries by sort codes in the report.
 Note
This field appears only when you selected the Cost Center radio button.
Exclude Closing Balance JEs
This is custom documentation. For more information, please visit SAP Help Portal. 134

6/8/26, 6:03 AM
Select the checkbox to exclude journal entries created by the period-end closing function. It is deselected by default.
Hide Cost Centers with No Postings
Hides cost centers with no postings in the cost center report. The checkbox is selected by default.
Hide Distribution Rules with No Postings
Hides distribution rules with no postings in the cost center report. The checkbox is selected by default. It appears only when you
select Distribution Rules in the Summary of dropdown list.
Distribution Report
This report provides comprehensive information about total overhead expenses and the expenses in each cost center, according to
distribution rules. Use the report to get a clear picture of overhead expenses posted by specific transactions and the distributed
amounts in each cost center.
Authorization is required for viewing this report. The report excludes confidential G/L accounts for users who are set as No
Authorization for Access to Confidential Accounts.
Use this window to specify selection criteria for the distribution report.
To open the window, choose Financials Cost Accounting Distribution Report .
After defining the report, you can view it in the Distribution Report window (see Distribution Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Dimension
From the dropdown list, select a dimension to view its related distribution rules.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Distr. Rule From...To...
If required, specify a range of distribution rules to include in the report.
Posting Date / Due Date / Document Date From...To...
If required, specify ranges of posting dates, due dates, or document dates to include specific postings in the report.
Project
This is custom documentation. For more information, please visit SAP Help Portal. 135

6/8/26, 6:03 AM
If required, select the checkbox and choose specific projects to further narrow down the distribution rules to be displayed in the
report.
Scenario
Select the budget scenario that you want to display in the report.
 Note
Only valid budget scenarios in the selected date range appear in the dropdown list.
Display LC / SC / LC and SC
Select to display the report in local currency, system currency, or both local currency and system currency.
Hide Cost Centers with No Values
If required, select to hide cost centers with no values in the report.
Exclude Closing Balance JEs
Select the checkbox to exclude journal entries created by the period-end closing function. It is deselected by default.
Cost Accounting Adjustment
Click this button to open the Journal Entry for Cost Accounting Adjustment window.
Cost Accounting Summary Report
This report provides information on transactions related to cost accounting.
Authorization is required for viewing this report. The report excludes confidential G/L accounts for users who are set as No
Authorization for Access to Confidential Accounts.
Use this window to specify selection criteria for the cost accounting summary report.
To open the window, choose Financials Cost Accounting Cost Accounting Summary Report .
After defining the report, you can view it in the Cost Accounting Summary Report window (see Cost Accounting Summary Report
Window).
You can find more information in this blog .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Dimension
From the dropdown list, select a dimension to view its related cost centers.
 Note
Only active dimensions appear in the dropdown list.
This is custom documentation. For more information, please visit SAP Help Portal. 136

6/8/26, 6:03 AM
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Hierarchy Template
If required and you’ve defined a cost center hierarchy, select the radio button, and from the dropdown list, select a hierarchy
template to display the cost centers in the hierarchy.
 Note
Selecting the radio button disables the Cost Center Type From…To… and the Sort Code From...To… fields.
Cost Center
If required, select the radio button, and choose the icon to select specific cost centers in the Cost Center Selection window.
By default, all cost centers are selected.
 Note
In the Cost Center Selection window, you can choose the Find button to specify a range of cost centers to include in the report.
Cost Center Type / Sort Code From…To…
If required, specify a range of cost center types or sort codes to include in the report only cost centers with selected types or sort
codes.
 Note
These fields are enabled only when you selected the Cost Center radio button.
Date From…To…
Specify a range of posting dates, due dates, or document dates to include specific postings in the report.
G/L Accounts
If required, select the checkbox, and choose the icon to select specific G/L accounts in the Accounts – Selection Criteria
window.
 Note
In the Accounts – Selection Criteria window, you can choose the Find button to select specific G/L accounts using the
selection criteria in the Find G/L Accounts window.
Project
If required, select the checkbox and choose specific projects to further narrow down the cost centers to be displayed in the report.
Add Journal Vouchers
If required, select the checkbox to include journal vouchers in the report as potential postings.
Exclude Closing Balance JEs
Select the checkbox to exclude journal entries created by the period-end closing function. It is deselected by default.
Annual / Quarterly / Monthly Report
Select to display an annual, quarterly, or monthly report for the selected fiscal year.
This is custom documentation. For more information, please visit SAP Help Portal. 137

6/8/26, 6:03 AM
Display LC / SC / LC and SC
Select to display the report in local currency, system currency, or both local currency and system currency.
Budget versus Cost Accounting
This report provides comprehensive information on budget and cost accounting for budget relevant G/L accounts. Use the report
to get information on G/L accounts for which budget amounts have been entered in the Budget Scenarios – Setup (Scenario –
XXX) window.
Authorization is required for viewing this report.
Use this window to specify selection criteria for the budget versus cost accounting report.
To open the window, choose Financials Cost Accounting Budget versus Cost Accounting .
After defining the report, you can view it in the Budget versus Cost Accounting window (see Budget versus Cost Accounting
Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Dimension
From the dropdown list, select a dimension to view its related cost accounting information.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
G/L Accounts
If required, select specific G/L accounts to be included in the report. You can choose the Find button to specify a range of account
codes in the Accounts – Selection Criteria window.
 Note
Only G/L accounts appear here for which you selected the Relevant to Budget checkbox in its G/L Account Details window.
Scenario
From the dropdown list, select a budget scenario.
 Note
Only valid budget scenarios in the selected date range appear in the dropdown list.
Date From…To…
This is custom documentation. For more information, please visit SAP Help Portal. 138

6/8/26, 6:03 AM
Specify a range of posting dates, due dates, or document dates to include specific postings in the report.
Exclude Closing Balance JEs
Select the checkbox to exclude journal entries created by the period-end closing function. It is deselected by default.
Display LC / SC / LC and SC
Select to display the report in local currency, system currency, or both local currency and system currency.
Hide Accounts with No Postings
Hides accounts with no postings in the budget versus cost accounting report. The checkbox is selected by default.
Cost Accounting Reconciliation Report
To make sure that expenses and revenues are posted to the correct period, define accrual types to reflect the differences between
financial accounting and cost accounting, and then use the report to get an overview of financial accounting and cost accounting
in your company.
Authorization is required for viewing this report.
Use this window to specify selection criteria for the cost accounting reconciliation report.
To open the window, choose Financials Cost Accounting Cost Accounting Reconciliation Report .
After defining the report, you can view it in the Cost Accounting Reconciliation Report window (see Cost Accounting
Reconciliation Report Window).
 Note
To get the current data (for example, you want the report to reflect the latest change made by other users), close the selection
criteria window, and run the report by opening the window again.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Dimension
From the dropdown list, select a dimension to view its related cost accounting information.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
G/L Accounts
This is custom documentation. For more information, please visit SAP Help Portal. 139

6/8/26, 6:03 AM
If required, select specific G/L accounts to be included in the report. You can choose the Find button to specify a range of account
codes in the Accounts – Selection Criteria window.
 Note
Only G/L accounts whose account type is Expenditure or Sales appear here.
Posting Date / Due Date / Document Date From…To…
Specify ranges of posting dates, due dates, or document dates to include specific postings in the report.
Exclude Closing Balance JEs
Select the checkbox to exclude journal entries created by the period-end closing function. It is deselected by default.
Display LC / SC / LC and SC
Select to display the report in local currency, system currency, or both local currency and system currency.
Hide Accounts with No Postings
Hides accounts with no postings in the cost accounting reconciliation report. The checkbox is selected by default.
More Information
Working with Accrual Types
Recording Differences Between Financial Accounting and Cost Accounting – Example
Cost Accounting Windows
Use the following windows to set up the cost accounting function:
Dimensions Window
Cost Centers – Setup Window
Distribution Rules – Setup Window
Cost Center Hierarchy Window
Accrual Types – Setup Window
Use the following windows to work with the cost accounting function:
Distribution Rule History Window
Table of Cost Centers and Distribution Rules Window
Cost Center Report Window
Distribution Report Window
Cost Accounting Summary Report Window
Budget versus Cost Accounting Window
This is custom documentation. For more information, please visit SAP Help Portal. 140

6/8/26, 6:03 AM
Cost Accounting Reconciliation Report Window
Dimensions Window
Use this window to define and view dimensions used in cost accounting.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Dimensions Window Fields
Name
Displays the default names of the five dimensions.
Act.
Select the checkbox to activate a dimension (the checkbox for Dimension 1 is selected by default).
 Note
Once you assign a dimension to cost centers or distribution rules, the checkbox of this dimension is disabled.
Description
If required, specify the name of the dimension. Default values are the same as they appear in the Name field.
Values you entered here appear as field or column names for corresponding dimensions.
More Information
Working with Dimensions
Cost Centers - Setup Window
Use this window to define and view cost centers in your company.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cost Centers – Setup Window Fields
Cost Center
Specify a code for the cost center.
Name
If required, specify a name or short description for the cost center.
Owner
This is custom documentation. For more information, please visit SAP Help Portal. 141

6/8/26, 6:03 AM
Define an employee as the owner of the cost center.
Sort Code
If required, specify a sort code for the cost center, for selection by future reports and analyses.
 Example
A company manufactures 10 different products, for each of which you defined a cost center. The products are divided among
three different categories, and the company management wants to know which category is the most profitable. You can assign
to each cost center a sort code that represents the relevant product category. Generating the cost center report summarized
by sort code provides the answer.
Dimension
From the dropdown list, select the dimension to relate to the cost center.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Cost Center Type
If required, from the dropdown list, select a cost center type, for selection by future reports and analyses.
You can select Define New to open the Cost Center Type – Setup window, in which you can specify the code and name of the cost
center type.
Effective From…To…
Specify the effective period of the cost center.
 Note
You cannot update the Effective From and Effective To dates for inactive cost centers.
Active
If required, select the checkbox to activate the cost center. By default, the checkbox is selected.
 Note
In SAP Business One, you can only use active cost centers.
Open Table
Choose to open the Table of Cost Centers and Distribution Rules window.
More Information
Working with Cost Centers
Table of Cost Centers and Distribution Rules Window
This is custom documentation. For more information, please visit SAP Help Portal. 142

6/8/26, 6:03 AM
Distribution Rules - Setup Window
Use this window to define and view distribution rules.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Distribution Rules – Setup Window
Code, Description
Specify a code and a description for the distribution rule.
Effective From…To…
For reporting purposes, specify the effective periods of the distribution rule. The effective periods cannot overlap each other. For
manually created distribution rules, you can update the current Effective From date in the Date window. To open this window,
choose Define New in the Effective From dropdown list. You cannot update the Effective From and Effective To dates for inactive
distribution rules
 Note
When you assign a distribution rule in a transaction, SAP Business One lists out only the distribution rules that are effective on
the transaction posting date.
 Example
There is a transaction with a posting date of 01.07.2009, and you have assigned to it a distribution rule whose effective
period is from 01.06.2009 onwards. You updated the effective period of the distribution rule as from 01.06.2009 to
30.06.2009. SAP Business One still includes the distribution information in reports by comparing the posting date with the
latest Effective From date.
However, for new transactions, if the posting date is not within June 2009, SAP Business One does not list out the above
distribution rule for you to choose.
 Example
There is a distribution rule whose effective period is from 01.06.2009 onwards, and you add the following effective periods:
The new effective period is from 01.07.2009 onwards: SAP Business One updates the original effective period as from
01.06.2009 to 30.06.2009.
The new effective period is from 01.04.2009 to 30.04.2009: SAP Business One does not change the original
effective period.
The new effective period is from 01.04.2009 onwards: the new and original effective periods overlap each other, SAP
Business One does not save the new effective period and displays an error message.
Dimension
From the dropdown list, select the dimension to relate to the distribution rule.
 Note
Only active dimensions appear in the dropdown list.
This is custom documentation. For more information, please visit SAP Help Portal. 143

6/8/26, 6:03 AM
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Active
If required, select the checkbox to activate the distribution rule. By default, the checkbox is selected.
 Note
In SAP Business One, you can only use active distribution rules.
Total
Specify the reference value to be used for defining factors.
Direct Allocation
For reporting purposes, specify whether the amounts based on this distribution rule is allocated directly or indirectly.
 Example
A company consists of four departments, each of which is a cost center. The electricity bill covers the consumption of the entire
company for a defined period. Since the company cannot calculate the exact amount of electricity consumed by each
department, the global amount is distributed among the departments according to each department's office size. The
distribution rule used in this case is not Direct Allocation, as it is impossible to relate a specific amount of the electricity bill
directly to a specific department.
The Direct Allocation distribution rule is used for allocating amounts that are directly related to specific cost centers, such as raw
material expenses for a production division.
Allocate By Fixed Amounts
Select the checkbox to indicate that fixed amounts will be allocated to cost centers when the current distribution rule is used.
 Note
Once you have added the distribution rule in the application, the selection status of this checkbox cannot be changed any
longer.
Center Code, Center Name
Specify the code of the cost center.
 Note
You can only choose the cost centers:
That are effective throughout the effective period of the distribution rule, and
That are related to the selected dimension.
Value
If you have entered a value in the Total field
Specify the portion of the expenses or revenues to be debited from/credited to the cost center.
If you have selected the Allocate by Fixed Amounts checkbox
This is custom documentation. For more information, please visit SAP Help Portal. 144

6/8/26, 6:03 AM
Specify in local currency the fixed amount of the expenses or revenues to be debited from/credited to the cost center.
Table Total
Total of all values entered in the table.
When you have entered a value in the Total field
Table total value is not necessarily the same as the total value specified in the Total field above.
To distribute expenses and revenues as percentages, enter 100 in the Total field above, and enter the percentages for the
individual cost centers as whole numbers in the table.
 Note
If the values you enter in the table do not add up to the total value, SAP Business One automatically allocates the
difference to the zero cost center (Centr_z), which is only used in reports.
When you have selected the Allocate by Fixed Amounts checkbox
It is not necessarily that the transaction amount always equals the table total amount. The difference between the
transaction amount and the table total amount will be allocated according to the following rules:
If you have selected one cost center in the table with no defined value, the difference amount will be allocated to this
cost center.
In this case, only one cost center can have no defined value, and at least one of the selected cost centers must have
a defined value.
If you have not selected any cost center in the table with no defined value, then the difference amount will be
allocated to the zero cost center (Centr_z), which is only used in reports.
 Example
1. You have selected one cost center in the table with no defined value
Cost Center Code Cost Center Name Value
CC01 Cost Center 1 USD 50.00
CC02 Cost Center 2 USD 30.00
CC03 Cost Center 3
Table Total: USD 80.00
a. When the transaction amount is USD 100.00, allocation using this distribution rule is:
CC01: USD 50.00 CC02: USD 30.00 CC03: USD 20.00
b. When the transaction amount is USD 70.00, allocation using this distribution rule is:
CC01: USD 50.00 CC02: USD 30.00 CC03: USD -10.00
2. You have not selected any cost center in the table with no defined value
This is custom documentation. For more information, please visit SAP Help Portal. 145

6/8/26, 6:03 AM
Cost Center Code Cost Center Name Value
CC01 Cost Center 1 USD 50.00
CC02 Cost Center 2 USD 30.00
Table Total: USD 80.00
a. When the transaction amount is USD 100.00, allocation using this distribution rule is:
CC01: USD 50.00 CC02: USD 30.00 zero cost center (Centr_z): USD
20.00
b. When the transaction amount is USD 70.00, allocation using this distribution rule is:
CC01: USD 50.00 CC02: USD 30.00 zero cost center (Centr_z): USD
-10.00
Distribution Rule History
Displays the Distribution Rule History window, which provides an overview of the changes made to the distribution rule based on
different effective periods.
You can edit the effective periods of the distribution rule.
More Information
Working with Distribution Rules
Distribution Rule History Window
Distribution Rule History Window
This window provides an overview of the changes made to a specific distribution rule. The changes are displayed according to
different effective periods.
 Example
A sweets factory produces chocolate, cookies, and ice cream. In the spring and summer periods (01.03.2010 – 31.08.2010) the
sugar consumption of the factory is distributed among the three cost centers as follows:
30% - chocolate
30% - cookies
40% - ice cream
However, between 01.09.2010 and 28.02.2011, the factory does not produce ice cream, and the sugar consumption is
distributed as follows:
40% - chocolate
This is custom documentation. For more information, please visit SAP Help Portal. 146

6/8/26, 6:03 AM
60% - cookies
The Distribution Rule History window displays the following rows:
Effective From Effective To Chocolate Cookies Ice Cream Center_z
01.03.2010 31.08.2010 30 30 40
01.09.2010 28.02.2011 40 60
Table of Cost Centers and Distribution Rules Window
This window provides an overview of the cost centers and distribution rules defined in SAP Business One.
Authorization is required for viewing this window.
To open the window, choose Financials Cost Accounting Table of Cost Centers and Distribution Rules .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Table of Cost Centers and Distribution Rules Window Fields
Dimension
From the dropdown list, select a dimension to view its related distribution rules and cost centers.
 Note
Only active dimensions appear in the dropdown list.
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Distr. Rule/Cost Center
Displays all distribution rules related to the selected dimension.
To open the Distribution Rules – Setup window and to view the distribution rule, choose the icon.
If the distribution rule is created automatically from a cost center, it has the same name as the cost center and you cannot change
the distribution rule.
Allocate By Fixed Amounts
Indicate whether transactions using this distribution rule are allocated by fixed amounts.
Effective From, Effective To
Displays the effective periods of the distribution rule.
If the distribution rule is created automatically from a cost center, it has the same effective period as the cost center.
This is custom documentation. For more information, please visit SAP Help Portal. 147

6/8/26, 6:03 AM
 Note
For effective period that includes the current system date, the corresponding distribution row is marked bold.
Total
Displays the total value of each distribution rule.
Centr_z
Displays the portion allocated to the zero cost center. If the total value if allocated in its entirety to individual cost centers, the
value in this column is 0.
Additional columns
Displays all cost centers related to the selected dimension. The appropriate distribution rule for distributing expenses among the
cost centers is displayed for each distribution rule.
New Cost Center
Opens the Cost Centers – Setup window.
New Distribution Rule
Opens the Distribution Rules - Setup window.
Cost Accounting Adjustment
Click this button to open the Journal Entry for Cost Accounting Adjustment window.
More Information
Cost Centers - Setup Window
Distribution Rules - Setup Window
Cost Center Hierarchy Window
Use this window to define and view cost accounting report templates according to company needs.
To open the window, choose Financials Cost Accounting Cost Center Hierarchy .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cost Center Hierarchy Window Fields
Dimension
From the dropdown list, select a dimension to define and view its related cost accounting report templates.
 Note
Only active dimensions appear in the dropdown list.
This is custom documentation. For more information, please visit SAP Help Portal. 148

6/8/26, 6:03 AM
 Note
This field appears only when you selected the Use Multidimensions checkbox on the Cost Accounting tab of the General
Settings window under Administration System Initialization General Settings .
Template
To view or update existing hierarchy templates, from the dropdown list, select a template.
To define new hierarchy templates, from the dropdown list, select Define New. After specifying the name and updating the Cost
Center Hierarchy Templates – Setup window, return to the Cost Center Hierarchy window to define the new hierarchy template.
Item Name
Displays the name of the selected hierarchy item. If required, specify a new name.
Item Location
Displays the parent article and the location on the tree of the selected hierarchy item. If required, specify a new location.
Text Title
Selecting the checkbox:
Defines the selected item as a text title that appears in reports without statistics
Hides the Subtotal checkbox
Subtotal
Selecting the checkbox:
Defines the selected item as a subtotal calculated according to the defined formula
Displays the Formula button
Add Same-Level Cost Center
Choose to add a new cost center that is of the same level as the selected cost center.
Add Child Cost Center
Choose to add a new cost center that is one level lower than the selected cost center.
Accrual Types - Setup Window
Use this window to define and view accrual types used for cost accounting correction.
Use either of the following to open the Recurring Postings window:
Right-click a selected row and choose Recurring Postings.
Select a row and in the menu bar, choose Data Advanced Recurring Postings .
The default values of the recurring posting are as follows:
Code: code of the accrual type
Description: name of the accrual type
This is custom documentation. For more information, please visit SAP Help Portal. 149

6/8/26, 6:03 AM
G/L Acct/BP Code, G/L Account/BP Name: the accrual calculation account and the accrual calculation interim account
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Accrual Types – Setup Window Fields
Code, Name
Specify the code and name of the accrual type.
Posting Acct
Specify a financial posting account for the accrual type.
Amounts posted to this account appear in both the Financial Accounting and the Cost Accounting Correction sections of the cost
accounting reconciliation report.
Accrual Calculation Acct
Specify a cost accounting calculation account for the accrual type.
Amounts posted to this account appear in both the Financial Accounting and the Cost Accounting P/L sections of the cost
accounting reconciliation report.
Accrual Calculation Interim Acct
Specify a cost accounting calculation interim account for the accrual type.
Amounts posted to this account appear in both the Financial Accounting and the Cost Accounting Correction sections of the cost
accounting reconciliation report.
 Note
You can select only those G/L accounts whose account type is Expenditure or Sales.
 Note
You can specify one G/L account only once in the window.
More Information
Working with Accrual Types
Cost Accounting Reconciliation Report
Recurring Posting
Cost Center Report Window
This window displays the cost center report according to the defined selection criteria (see Cost Center Report).
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 150

6/8/26, 6:03 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cost Center Report
Cost Center Hierarchy, Cost Center
Displays the cost center hierarchy if you selected the Template radio button, or cost centers if you selected the Cost Center radio
button in the selection criteria window.
Trans. No., Origin
Displays the transaction number and origin type of the transaction that have postings to the particular cost center. If required,
choose the icon to open the Journal Entry window.
 Example
IN is displayed for a transaction created by an A/R invoice.
 Note
These fields appear only when you selected Linked Accounts in the Summary of dropdown list of the selection criteria window.
Direct Allocation, Indirect Allocation
Displays amounts referring to direct or indirect allocation, divided into expenses and revenues.
 Note
You can define the allocation to be direct or indirect in the Distribution Rules – Setup window.
Total
Displays the total amount in cost centers for each row.
Distribution Report Window
This window displays the distribution report according to the defined selection criteria (see Distribution Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Distribution Report
Distr. Rule
Displays the distribution rule codes. If required, choose the icon to open the Distribution Rules – Setup window.
G/L Acct
Displays the code and name of the G/L account for which you selected the distribution rule in a posting.
Trans. No., Origin
This is custom documentation. For more information, please visit SAP Help Portal. 151

6/8/26, 6:03 AM
Displays the transaction number and origin type of the transaction. If required, choose the icon to open the Journal Entry
window.
 Example
IN is displayed for a transaction created by an A/R invoice.
Remarks
Displays the remarks of the transaction row.
Total Costs
Displays the total expenses posted to the distribution rule.
Distribution Total
Displays the total distribution amount.
Budget
Displays the budget amount defined for this distribution rule and this account.
Total Costs vs. Budget
Displays the result of total costs minus the budget amount.
Cost Centers
Displays the distribution amounts for each cost center.
Cost Accounting Summary Report Window
This window displays the cost accounting summary report according to the defined selection criteria (see Cost Accounting
Summary Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cost Accounting Summary Report
Cost Center Hierarchy
Displays the cost center hierarchy only if you selected the Hierarchy Template radio button in the selection criteria window.
Cost Center
Displays the cost center codes.
G/L Acct
Displays the code and name of the G/L account that have postings to the particular cost center.
Trans. No., Origin
Displays the transaction number and origin type of the transaction. If required, choose the icon to open the Journal Entry
window.
This is custom documentation. For more information, please visit SAP Help Portal. 152

6/8/26, 6:03 AM
 Note
IN is displayed for a transaction created by an A/R invoice.
Remarks, Amount, Distr. Rule
Displays the remarks, amount, and distribution rule of the transaction row. If required, choose the icon to open the Distribution
Rules – Setup window.
Cost Total
Displays the amount allocated to the cost center calculated based on the transaction amount and distribution rule.
Budget versus Cost Accounting Window
This window displays the budget versus cost accounting report according to the defined selection criteria (see Budget versus Cost
Accounting).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Budget versus Cost Accounting
Financial Accounting Section
G/L Account
Displays the code and name of the G/L accounts according to the defined selection criteria.
Budget
Displays the budget amount of the G/L account in the selected date range and the selected budget scenario.
Actual
Displays the actual posting amount of the G/L account in the selected date range.
Difference
Displays the difference between the budget and actual amounts. It is calculated as the value in the Budget field minus that in the
Actual field of the financial accounting section.
Diff. in %
Displays the difference in percentage. It is calculated as: value in the Difference field of the financial accounting section / value in
the Budget field * 100%.
Cost Accounting Section
Distr. Rule Code, Distr. Rule Name
Displays the code and name of the distribution rule that you assigned to the specific G/L account in postings of the selected date
range.
Actual
Displays the actual posting amount based on the distribution rule and the G/L account in the selected date range.
This is custom documentation. For more information, please visit SAP Help Portal. 153

6/8/26, 6:03 AM
Difference
Displays the difference between the budget and actual amounts. It is calculated as the value in the Budget field minus that in the
Actual field of the cost accounting section.
Diff. in %
Displays the difference in percentage. It is calculated as: value in the Difference field of the cost accounting section / value in the
Budget field * 100%.
Budget
Displays the budget amount defined for this distribution rule and this account.
Actual vs. Budget
Displays the result of cost accounting actual amount minus the budget amount.
Cost Accounting Reconciliation Report Window
This window displays the cost accounting reconciliation report according to the defined selection criteria (see Cost Accounting
Reconciliation Report).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Cost Accounting Reconciliation Report
Financial Accounting Section
P/L (Accounts, Expense, Revenue)
Displays the selected G/L account codes and names, as well as their corresponding expense and revenue totals from all journal
entries.
For Expenditure type G/L accounts, displays their totals (amounts on the debit side minus that on the credit side) as
Expense.
For Sales type G/L accounts, displays their totals (amounts on the credit side minus that on the debit side) as Revenue.
Cost Accounting Section
Company-Related (Expense, Revenue)
Displays the expense and revenue totals of G/L accounts that are both:
Not entered in the Accrual Types – Setup window
From postings that have no distribution rule assignment in the selected dimension.
Cost Accounting Correction (Expense, Revenue)
Displays the expense and revenue totals of the corresponding G/L accounts that are set as Posting Acct or Accrual Calculation
Interim Acct in the Accrual Types – Setup window.
This is custom documentation. For more information, please visit SAP Help Portal. 154

6/8/26, 6:03 AM
For Expenditure type G/L accounts, displays their totals (amounts on the debit side minus that on the credit side) as
Expense.
For Sales type G/L accounts, displays their totals (amounts on the credit side minus that on the debit side) as Revenue.
Cost Accounting P/L (Expense, Revenue)
Displays the expense and revenue totals of G/L accounts that meet one or both of the following criteria:
The accounts are set as Accrual Calculation Acct in the Accrual Types – Setup window.
The accounts are both not relevant to accrual types and from postings that have distribution rule assignment in the
selected dimension.
Total
Displays totals (revenue totals minus expense totals) of financial accounting, company-related, cost accounting correction, and
cost accounting amounts.
Financial P/L
Displays totals (revenue totals minus expense totals) of financial accounting amounts.
Non-Operating P/L
Displays totals (revenue totals minus expense totals) of company-related and cost accounting correction amounts.
Cost Accounting P/L
Displays totals (revenue totals minus expense totals) of cost accounting amounts.
Journal Entry for Cost Accounting Adjustment Window
Use this window to display cost accounting adjustment journal entries. To open this window, choose Financials Cost
Accounting Cost Accounting Windows Journal Entry for Cost Accounting Adjustment .
This window is identical to the Journal Entry Window except for the following rules:
Numbering series: must be “Cost Accounting Adjustment Only”
G/L account:
default “Cost Accounting Adjustment Only” will be used automatically
must use “Cost Accounting Adjustment Only”
must use the same G/L account in JE
JE origin is “Manual”
JEs are excluded from financial reports, but included in accounting reports
Tax relevant functions are not available in this window
Recurring template is not available in this window
Postings are in LC only
Must specify distribution rule
Related Information
Journal Entry Window
This is custom documentation. For more information, please visit SAP Help Portal. 155

6/8/26, 6:03 AM
Voucher Entry for Cost Accounting Adjustment
Use this window to add a cost accounting adjustment journal entry to a cost accounting adjustment journal voucher.
This window is identical to the Journal Entry for Cost Accounting Adjustment Window except for the following fields:
Voucher No.
Number of the voucher to which the cost accounting adjustment journal entry is added.
Related Information
Journal Entry for Cost Accounting Adjustment Window
Financial Reports
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
Electronic Reports
Use Electronic Reports to generate reports in electronic formats. Before generating electronic reports, you must have set up the
electronic file formats using the electronic file manager.
Depending on the definition of Module from the Electronic File Manager: Format Definition add-on, the available electronic
formats are listed in Electronic Reports under the reports menu entry of the specific SAP Business One module.
 Example
In the Electronic File Manager: Format Definition add-on, the module of EU Sales Report has been defined as Financials. In
SAP Business One, you have imported the electronic format EU Sales Report using the electronic file manager. To generate this
report, choose Financials Financial Reports Electronic Reports EU Sales Reports . Alternatively, choose Reports
Financials Electronic Reports EU Sales Report .
Generating Electronic Reports
This is custom documentation. For more information, please visit SAP Help Portal. 156

6/8/26, 6:03 AM
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
To close the wizard, choose the Finish button.
More Information
For more information about defining electronic formats, see the online help for the Electronic File Manager: Format Definition
add-on after installing it.
SAF-T
SAF-T (Standard Audit File for Tax) is an international standard file type for the electronic exchange of data between companies
and authorities. The standards are set by the Organisation for Economic Co-operation and Development (OECD).
Various authorities have adopted SAF-T and require the use of SAF-T when exchanging data with companies. SAF-T reporting
requirements exist in different localizations of SAP Business One and typically require generic electronic file format projects (GEP)
that are managed through Electronic File Manager.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 157

6/8/26, 6:03 AM
Setting Up Electronic File Formats
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
Opens the Properties window where you select the required properties. Your choices appear in the adjoining field.
G/L Accounts
Includes G/L accounts in the report.
This is custom documentation. For more information, please visit SAP Help Portal. 158

6/8/26, 6:03 AM
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
General Ledger
This report enables you to generate a list of journal entries posted to the company database according to various criteria. Use this
window to specify selection criteria for the report.
This is custom documentation. For more information, please visit SAP Help Portal. 159

6/8/26, 6:03 AM
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
Select the level of the accounts displayed in the table.
Selecting Level 1 displays the account titles on the highest level.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 160

6/8/26, 6:03 AM
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
Select this checkbox to display the opening balance of the selected BP and G/L accounts, as accumulated in the time range from
the following option date to the start date specified in the Selection options:
OB from Start of Company Activity – displays the opening balance accumulated after company activity started.
This is custom documentation. For more information, please visit SAP Help Portal. 161

6/8/26, 6:03 AM
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
If you select the checkbox, the report displays transactions with a correct historic balance due as at the specified posting
date To date as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 162

6/8/26, 6:03 AM
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
Properties
This is custom documentation. For more information, please visit SAP Help Portal. 163

6/8/26, 6:03 AM
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
Document
Specify the document.
This is custom documentation. For more information, please visit SAP Help Portal. 164

6/8/26, 6:03 AM
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
Value
Displays the index defined for the chosen month and year. Change this value if required.
This is custom documentation. For more information, please visit SAP Help Portal. 165

6/8/26, 6:03 AM
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
SAP Business One creates a general ledger report that displays only the selected accounts and prints only the totals for the
control accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 166

6/8/26, 6:03 AM
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
Cumulative Balance Due (LC)
This is custom documentation. For more information, please visit SAP Help Portal. 167

6/8/26, 6:03 AM
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
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 168

6/8/26, 6:03 AM
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
Opens the Properties window, where you can specify customer properties.
This is custom documentation. For more information, please visit SAP Help Portal. 169

6/8/26, 6:03 AM
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
This function is available only if you are using SAP Business One, version for SAP HANA.
This is custom documentation. For more information, please visit SAP Help Portal. 170

6/8/26, 6:03 AM
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
Number of Days Outstanding
The number of days between the due date and the aging date
This is custom documentation. For more information, please visit SAP Help Portal. 171

6/8/26, 6:03 AM
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
Select the checkbox in this column to create a dunning letter for that document.
Doubtful Debt
This is custom documentation. For more information, please visit SAP Help Portal. 172

6/8/26, 6:03 AM
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
Previous <Number> Rows – Choose this button to display the data in the previous page of the table. This button is
disabled if the current display is the first page.
This is custom documentation. For more information, please visit SAP Help Portal. 173

6/8/26, 6:03 AM
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
Vendor Group
This is custom documentation. For more information, please visit SAP Help Portal. 174

6/8/26, 6:03 AM
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
Hides the Future Remit column in the report and excludes transactions that have a value in this field
This is custom documentation. For more information, please visit SAP Help Portal. 175

6/8/26, 6:03 AM
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
Number of Days Outstanding
The number of days between the due date and the aging date
This is custom documentation. For more information, please visit SAP Help Portal. 176

6/8/26, 6:03 AM
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
To open the window, choose Financials Financial Reports Accounting Transaction Journal Report . Alternatively, open it
from the Reports module.
This is custom documentation. For more information, please visit SAP Help Portal. 177

6/8/26, 6:03 AM
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
Transaction number with a link to the transaction.
Creator
This is custom documentation. For more information, please visit SAP Help Portal. 178

6/8/26, 6:03 AM
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
Transaction Report by Projects Window
This is custom documentation. For more information, please visit SAP Help Portal. 179

6/8/26, 6:03 AM
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
You can save a specific set of selection criteria and generate the report accordingly whenever required. To do so press CTRL +
A , enter a meaningful name, and set all the required selection criteria for the report. Choose Save. To generate a report based on
a saved selection criteria set, click the icon. The List of Reports - Selection Criteria window appears. Highlight the required
This is custom documentation. For more information, please visit SAP Help Portal. 180

6/8/26, 6:03 AM
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
No Total: Displays all journal entries
Month (Posting Date): Displays all journal entries per month based on the posting date
This is custom documentation. For more information, please visit SAP Help Portal. 181

6/8/26, 6:03 AM
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
The calculation of the opening balance is influenced by the date range defined for the report. If you specify more than one date
range, SAP Business One calculates opening balance as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 182

6/8/26, 6:03 AM
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
Trans. No.
Transaction number and a link to the journal entry.
This is custom documentation. For more information, please visit SAP Help Portal. 183

6/8/26, 6:03 AM
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
This window displays a list of cash flow relevant transactions that may or may not have been assigned a cash flow line item within a
certain period. With the exception of the report reference period, you cannot modify the fields in this report.
This is custom documentation. For more information, please visit SAP Help Portal. 184

6/8/26, 6:03 AM
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
Abbreviation Journal Type
OB Opening Balance
JE Journal Entry
This is custom documentation. For more information, please visit SAP Help Portal. 185

6/8/26, 6:03 AM
Abbreviation Journal Type
IN A/R Invoice
CN A/R Credit Memo
PU A/P Invoice
PC A/P Credit Note
RC Incoming Payment
PS Payments to Vendors
DP Deposits
CP Checks for Payment
DN Delivery
RE A/R Returns
PD Goods Receipt PO
SI Goods Receipt
SO Goods Issue
MI Inventory Posting
WO Work Order
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
This is custom documentation. For more information, please visit SAP Help Portal. 186

6/8/26, 6:03 AM
possible.
Series
Opens the Series Selection window where you can choose to view only journal entries related to specific numbering series.
Clear Sel.
Clears all selections made in this window.
Related Information
Series Selection
Series Selection
This window appears when you specify selection criteria for the General Ledger.
To access the window, choose Financials Financial Reports Accounting General Ledger . In the General Ledger –
Selection Criteria window, choose Expanded, and in the Expanded Selection Criteria window, choose Series.
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Series Selection
Document
Specify the document.
Series
Numbering series defined in the Document Numbering window for documents available in the Expanded Selection Criteria
window.
Related Information
General Ledger
Tax
This menu option includes tax reports according to the company's localization. The same tax reports are available in multiple
localizations if the localizations fall under wider reporting regions, such as the European Union.
Information about tax reports that are specific to a country/region is available in the localization-specific online help file in: Help
Documentation Localization-Specific Information or by choosing F1 while the relevant tax report is the active window in
SAP Business One.
To create tax reports, choose Financials Financial Reports Accounting Tax . Alternatively, create them from the Reports
module.
This is custom documentation. For more information, please visit SAP Help Portal. 187

6/8/26, 6:03 AM
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
Accounts with Balance of Zero – report displays accounts with a balance of zero.
Foreign Name – report displays the foreign names defined for G/L accounts.
Nothing is displayed for accounts for which a foreign name was not defined.
External Code – report displays external codes defined for G/L accounts.
Add Journal Vouchers
Includes transactions that are recorded in Open journal vouchers, but not yet permanently saved in the database.
This is custom documentation. For more information, please visit SAP Help Portal. 188

6/8/26, 6:03 AM
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
Balance Sheet Revaluation
Use this window to set criteria according to which the balance sheet is revaluated.
To open the window, choose Financials Financials Reports Financial Balance Sheet. In the Balance Sheet – Selection
Criteria window choose the Revaluation button.
Alternatively, open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 189

6/8/26, 6:03 AM
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
Revaluate All Currencies G/L Account/BP
All currency accounts and business partners must have their values converted to one currency before they can be revaluated.
Select whether to revaluate all currency G/L accounts or business partners by local currency or by system currency.
Index Tab
To
Choose the required month and year of the index.
Value
Displays the index defined for the chosen month and year. Change this value if required.
Revaluation Method
Choose whether to calculate the revaluation according to the index defined for the Posting Date or the Due Date of the
transaction.
More Information
Balance Sheet - Selection Criteria
Balance Sheet Window
This window displays the Balance Sheet report according to the defined selection criteria.
Balance Sheet Window
Up to
Date specified in the To field in the selection criteria.
Display Subtotals
Displays a subtotal opposite each title.
Hide Titles
This is custom documentation. For more information, please visit SAP Help Portal. 190

6/8/26, 6:03 AM
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
To sort the accounts alphanumerically in descending order, double-click the column header again.
Balance
Balance of the drawer, title, or G/L account, according to the display level.
Foreign Currency
Balance in foreign currency for foreign currency G/L accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 191

6/8/26, 6:03 AM
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
Specify the number of days for calculating an average rate in case an exchange rate was not defined for a specific date.
Refer to Rates in Journal Entry
Select this checkbox to use the rate defined in the journal entries, if it is different from the rate defined in the Exchange Rates and
Indexes window.
Revaluate All Currency G/L Account/BP
All currency accounts and business partners must have their values converted to one currency before they can be revaluated.
This is custom documentation. For more information, please visit SAP Help Portal. 192

6/8/26, 6:03 AM
Select whether to revaluate All currency G/L accounts or business partners by local currency or by system currency.
Index Tab
To
Choose the required month and year of the index.
Value
Displays the index defined for the chosen month and year. Change this value if required.
Revaluation Method
Choose whether to calculate the revaluation according to the index defined for the Posting Date or the Due Date of the
transaction.
Related Information
General Ledger
General Ledger
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
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 193

6/8/26, 6:03 AM
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
OB from Start of Company Activity – Displays the opening balance accumulated since the company’s activity
started.
OB from Start of Fiscal Year – Displays the opening balance accumulated from the start of the current fiscal year.
This is custom documentation. For more information, please visit SAP Help Portal. 194

6/8/26, 6:03 AM
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
Period-end closing journal entries of posting periods prior to the selected period are included in the Opening Balance
column.
This is custom documentation. For more information, please visit SAP Help Portal. 195

6/8/26, 6:03 AM
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
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 196

6/8/26, 6:03 AM
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
This column is displayed only when the Disp.Opening Balance for Period checkbox is selected in the Selection Criteria
window.
This is custom documentation. For more information, please visit SAP Help Portal. 197

6/8/26, 6:03 AM
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
The transition to a higher level of detail will conform to the levels you defined in the Chart of Accounts.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 198

6/8/26, 6:03 AM
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
Monthly Report to calculate the profit and loss statement separately for each month
Periodic Report
This is custom documentation. For more information, please visit SAP Help Portal. 199

6/8/26, 6:03 AM
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
Select this option and choose the required parameters to generate a revaluated report.
Expanded
This is custom documentation. For more information, please visit SAP Help Portal. 200

6/8/26, 6:03 AM
Opens the Expanded Selection Criteria window, where you can define additional parameters for the report.
Related Information
Expanded Selection Criteria
Profit and Loss Statement Revaluation
Use this window to set criteria according to which the profit and loss statement is revaluated.
To open the window, choose Financials Financials Reports Financial Profit and Loss Statement. In the Profit and Loss
Statement – Selection Criteria window choose the Revaluation button.
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
Revaluate All Currencies G/L Account/BP
All currency accounts and business partners must have their values converted to one currency before they can be revaluated.
Select whether to revaluate all currency G/L accounts or business partners by local currency or by system currency.
Index Tab
To
Choose the required month and year of the index.
Value
Displays the index defined for the chosen month and year. Change this value if required.
Revaluation Method
This is custom documentation. For more information, please visit SAP Help Portal. 201

6/8/26, 6:03 AM
Choose whether to calculate the revaluation according to the index defined for the Posting Date or the Due Date of the
transaction.
More Information
Profit and Loss Statement - Selection Criteria
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
If the selected date range is not from the beginning of work in the company, there will be a difference in the data displayed in the
Balance and Current Year columns.
This is custom documentation. For more information, please visit SAP Help Portal. 202

6/8/26, 6:03 AM
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
Specify a date range. The report includes documents and transactions with due dates within this range.
This is custom documentation. For more information, please visit SAP Help Portal. 203

6/8/26, 6:03 AM
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
Opening Balance/Calculate Opening Balance
This is custom documentation. For more information, please visit SAP Help Portal. 204

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 205

6/8/26, 6:03 AM
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
Parent topic: Cash Flow
Parent topic: Cash Flow
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 206

6/8/26, 6:03 AM
Cash Flow - Selection Criteria
Cash Flow - Selection Criteria
Cash Flow Report
The Cash Flow report is a standard financial statement. It details information relating to cash relevant income and expenses, and
cash equivalents within a defined period.
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
This is custom documentation. For more information, please visit SAP Help Portal. 207

6/8/26, 6:03 AM
Specify a template for displaying the report.
Cash Flow Report Window
This window displays the Cash Flow Report according to your defined selection criteria. The report details information relating to
cash relevant income and expenses and cash equivalents within a defined period. In order to generate this report, you must assign
pre-defined cash flow line items to cash relevant transactions.
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
This is custom documentation. For more information, please visit SAP Help Portal. 208

6/8/26, 6:03 AM
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Creating a Cash Flow Report
Context
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
This is custom documentation. For more information, please visit SAP Help Portal. 209

6/8/26, 6:03 AM
Budget Comparison: this report mode displays the expenses, the budgets, and their deviations in the posting period
you selected and the current fiscal year YTD.
Monthly Comparison: this report mode displays the expenses in each month of the fiscal year that includes the
posting period you selected.
Yearly Comparison: this report mode displays the expenses in the posting period you selected, the corresponding
one of its previous fiscal year, the current fiscal year YTD, and the corresponding period of the previous fiscal year.
 Note
In the report, you can choose a line to display a list of related journal entries, and also choose link arrows to display
specific journal entries directly from the report.
Comparison
These reports let you review the results of business activities of two posting periods, or compare two companies.
Balance Sheet Comparison
Trial Balance Comparison
Profit and Loss Statement Comparison - Selection Criteria
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
This is custom documentation. For more information, please visit SAP Help Portal. 210

6/8/26, 6:03 AM
Database Name
Name of the database to which the figures of the current company should be compared. By default, the database of the current
company is displayed.
Change
Opens a window in which you can choose the company to which the figures of the current company should be compared.
 Note
You can only select companies that are located on the same database server as the current company.
Posting Date/Document Date
Specify whether to generate the report according to a posting or a document date range.
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
This is custom documentation. For more information, please visit SAP Help Portal. 211

6/8/26, 6:03 AM
Choose Segments
Opens the Find G/L Accounts window where you can choose the accounts to include in the report, according to segments.
 Note
Only available if the company maintains a chart of accounts based on segments.
Revaluation
Opens the Balance Sheet Revaluation window where you can make additional selection criteria for revaluation.
Balance Sheet Comparison Window
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
This is custom documentation. For more information, please visit SAP Help Portal. 212

6/8/26, 6:03 AM
 Note
You can distinguish between the various display levels by color: drawers in red, titles in blue, and accounts in black.
Difference Amount
Difference between compared periods / Companies according to this accounting formula:
Difference Amount = Current Period / Company - Comparison Period/company
Percentage Difference
Difference between the current period/company and the compared period/company according to the accounting formula:
Percentage Difference = Difference Amount / Compared Period x 100
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
This is custom documentation. For more information, please visit SAP Help Portal. 213

6/8/26, 6:03 AM
In this section, define the periods to be compared by the report:
Current, Comparison – Click and select whether to generate the report according to posting date, due date, or document
date.
From, To, – Define the current period and comparison period by entering the required date ranges. Click to define the
date ranges according to posting periods.
Display in Report
You can select the following options to display in the report:
Hide Zero Balanced Acct – Select this checkbox to exclude zero balanced accounts from the report.
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
This is custom documentation. For more information, please visit SAP Help Portal. 214

6/8/26, 6:03 AM
Includes closing balances in the report.
Revaluation
Opens the Trial Balance Revaluation window. After the revaluation is made, the option next to this button is selected.
Expanded
Opens the Expanded Selection Criteria window, where you can use a project range and a distribution rule range as selection
criteria for this report.
Related Information
Revaluation - Selection Criteria
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
This is custom documentation. For more information, please visit SAP Help Portal. 215

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 216

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 217

6/8/26, 6:03 AM
This window displays the Profit and Loss Statement Comparison report according to your defined selection criteria.
Profit and Loss Statement Comparison Window
Account Name
Displays the names of the drawers (Revenues, Cost of Sales, Expenses, and so on), titles and accounts, according to the display
level you selected, and the selections made in the Profit and Loss Statement Comparison – Selection Criteria window.
Current Period
Displays the balance of the drawer, title, or account (according to the selected display level) to the requested date of the Current
Period in the current database.
Comparison Period
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
This is custom documentation. For more information, please visit SAP Help Portal. 218

6/8/26, 6:03 AM
Budgets
If your company manages budgets, you can create a budget report to review business activities from a budget perspective.
Budget Report
This report analyzes the business activities that took place during a defined period, with reference to a selected budget scenario.
Use this window to specify its selection criteria.
To open the window, choose Financials Financial Reports Budget Setup Budget Report . Alternatively, open it from the
Reports module.
After defining the report, you can view it in the Budget Report window.
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
This is custom documentation. For more information, please visit SAP Help Portal. 219

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 220

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 221

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 222

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 223

6/8/26, 6:03 AM
This window displays the Trial Balance Budget report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Trial Balance Budget Report Window
From Date To
Displays the dates you entered in the range of dates in the Trial Balance Budget Report – Selection Criteria window.
Budget
The planned amount for each account as specified in the Define Budget window.
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
This is custom documentation. For more information, please visit SAP Help Portal. 224

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 225

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 226

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 227

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 228

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 229

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 230

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 231

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 232

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 233

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 234

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 235

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 236

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 237

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 238

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 239

6/8/26, 6:03 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 240

6/8/26, 6:04 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:04:01 GMT+0000
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
Financials
This module:
Includes all functions and reports required for the accounting and financial operations of the company
Includes all tax-related reports according to the regulations in each country/region
Enables you to document all financial and accounting-related transactions
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Basic Settings
Please note that image maps are not interactive in PDF outputs.
Basic Operations
Please note that image maps are not interactive in PDF outputs.
Additional Operations
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
Report Management
Please note that image maps are not interactive in PDF outputs.
Basic Functions
Please note that image maps are not interactive in PDF outputs.
Chart of Accounts
The setting up of financial accounting occurs when SAP Business One is first implemented. During implementation, your partner,
tax advisor, and accountant follow GAAP and country/region or state regulations to set up financial accounting.
Once you have determined your financial or posting periods and account segments, if any, you create your chart of accounts. A
chart of accounts lists all of a company's general ledger (G/L) accounts and is the basis for its reporting and posting activities.
Drawers, Titles, and Active Accounts
Accounts are organized hierarchically according to drawers, titles, and active accounts. The organization of the chart of accounts
follows GAAP in which there is a separate “drawer” for accounts representing assets, liabilities, equity, revenues, cost of sales,
expenses, financing, and other revenues and expenses (see level 1 in the figure). Within each drawer, you organize your accounts by
level in a logical fashion appropriate to your financial accounting processes. Drawers are the organizational units on the top level.
You cannot change the predefined drawers provided with SAP Business One, but you can rename them as needed. To rename the
drawers, proceed as follows:
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:04 AM
1. From the SAP Business One Main Menu, choose Financials Chart of Accounts . The Chart of Accounts window
opens.
2. On the right side of the window, select the drawer you want to rename.
3. In the chart of account list in the middle of the window, select the top line that represents the drawer.
4. On the left side of the window, in the Name field, specify a new name and update.
Every G/L account is defined as either a title account or an active account. A title account groups together all of the active
accounts below it (see level 2, 3, and 4 in the figure). In financial reports, a title summarizes all of the balances of each active
account below it. Active accounts contain postings of transactions (see level 4 and 5 in the figure). You can differentiate titles and
active accounts by their text color: titles appear in blue, active accounts appear in either green or black. Green accounts are
control accounts that have been defined as default G/L accounts for automatic posting of transactions in SAP Business One. Black
accounts are those active accounts that have not been selected in G/L account determination. For more information, see G/L
Account Determination.
The number of levels in your chart of accounts may depend on your localization and common business practices. Some
countries/regions have legally required number of levels.
SAP Business One provides predefined charts of accounts for individual countries/regions based on local requirements. Discuss
with your partner which predefined chart of accounts to use, and what additions and adjustments are necessary for your company.
Example of a Chart of Accounts Structure
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:04 AM
Setting Up and Working with G/L Accounts
Setting Up and Working with G/L Accounts
The diagram below shows the topics covered in this section. Hover over each topic for a description. Choose each topic for more
information.
Please note that image maps are not interactive in PDF outputs.
Related Information
Chart of Accounts
Chart of Accounts Windows
Use the following windows to set up and work with the chart of accounts:
Chart of Accounts Window
G/L Account Details Window
Edit Chart of Accounts - Selection Criteria Window
Edit Chart of Accounts Window
Account Code Generator Window
Segment Codes - Selection Criteria Window
Account Code List Window
Chart of Accounts Window
Use this window to define a chart of accounts for your company or organization.
To open the window, choose Financials Chart of Accounts .
Chart of Accounts Window
Title, Active Account
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:04 AM
After you have defined the G/L account code, you classify each G/L account as either Title or Active Account. An active account
contains postings of transactions. A title account groups together all the active accounts below it.
For an active account to be summarized at title level in financial reporting, it must be assigned accordingly in the chart of accounts
hierarchy.
You can differentiate titles and active accounts by their text color: titles appear in blue, active accounts appear in either green or
black. Green accounts are control accounts or accounts that have been defined as default G/L accounts for automatic posting of
transactions in SAP Business One. Black accounts are those active accounts that have neither been selected in G/L account
determination nor control accounts.
G/L Account
Enter an alphanumeric code of up to fifteen characters (letters, numbers or a combination of both) for the account.
Name
Specify an account name of up to 100 characters.
External Code
Define an additional code for sorting purposes. The additional code is informational only and allows you to refine queries
(customized reports).
Currency
The account currency is the currency in which all journal entries for that account are recorded. By default, the currency is defined
as All Currencies.
In an all currencies account, transactions can be executed in a foreign currency without the account’s foreign currency balance
having any significance. Therefore, the account can accept journal entries in different currencies.
 Example
A foreign sales account can be used for every sale abroad, even though the sales are in different currencies. Accounts are then
settled with these customers in their account currency (an American customer buys in US dollars). However, the revenue
account accumulates revenue from all the various currencies. Since this account is not a debit/credit account, its updated
foreign currency balance is not relevant, and you refer only to its LC (local currency) balance.
If you work with a number of countries but use only one revenue account, define this account as All Currencies.
If the account currency is defined as a foreign currency, all postings in this account are recorded in both the local currency (as
required by law) and in the defined foreign currency.
If you define a foreign currency account and record transactions for it, you cannot later change the account currency or perform
transactions in any currency other than the defined account currency.
Accounts defined as foreign currency accounts are usually foreign bank accounts, and so on.
A foreign currency account has two balances: a local currency balance and the account currency balance.
Confidential
Defines certain accounts as confidential, preventing unauthorized users (according to defined permissions) from using them or
viewing their activities in the system.
Level
Define the level of the account.
Level 1 is the drawer level, so you cannot define an account or a title as Level 1.
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:04 AM
Level 2 to 9 are for either titles or accounts.
Level 10 is for active accounts only.
The number of levels in your chart of accounts may depend on your localization and common business practices. Some countries
have a legally required number of levels.
Balance
The account balance displayed in the currency defined for the account, after various journal entries have been recorded.
 Note
If the account is defined in a foreign currency, select LC from the field dropdown list to display the balance in local currency.
Account Type
You can define the account as a revenue account or as an expense account or as a different type of account (“other”).
Control Account
Defines this account as a control account. Control accounts are linked to business partners and reflect their activities in the
financial reports. Only accounts defined in the Assets and Liabilities drawers can be defined as control accounts. Control accounts
appear in the chart of accounts in green.
 Note
Once the account has any transaction posted to it, you cannot change the status by selecting or deselecting the checkbox.
Cash Account
This checkbox appears in the first three drawers that include the balance sheet accounts, and defines an account as a monetary
account.
Cash flow statements refer only to monetary accounts. SAP Business One defines the following as monetary accounts: cash funds
and bank accounts (current and short-term deposits).
 Note
An account cannot be defined as indexed and monetary at the same time. Therefore, selecting the Indexed Account option
automatically clears the Monetary Account option and vice versa.
Indexed
Defines an account as indexed.
SAP Business One revalues only indexed accounts when performing valuations of financial statements to an index. Indexes are
defined in Administration Exchange Rates and Indexes .
Reval. (Currency)
Select this box for companies whose defined currency is not the local currency.
Selecting this box enables you to:
Generate a conversion differences report for the account.
Produce an automatic differences reconciliation to adjust the balance of the account in the system currency to the balance
in the account currency.
Primary Closing Account
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:04 AM
Assign an account as the primarily selected period-end closing account.
 Note
This feature is not available in the following localizations: Austria, Belgium, Chile, Costa Rica, Czech Republic, Spain, France,
Guatemala, Hungary, Italy, Mexico, Portugal, Slovakia, Argentina and Turkey.
 Note
This field appears only for those accounts related to the P/L accounts that are included in the Period-End Closing - Selection
Criteria window.
Cash Flow Relevant
Specify G/L accounts that are cash flow relevant. The objective of the assignment process is to generate the Cash Flow report.
 Note
This field is visible only for active accounts at the asset level.
Project
If required, select the checkbox to set the G/L account as relevant to project. If required, you can further choose , and in the List
of Projects window, select a default project.
You can change the checkbox status and the default project field at any time.
 Note
For G/L accounts relevant to project, SAP Business One performs actions, defined on the Cost Accounting tab of the General
Settings window, under Administration System Initialization General Settings , for postings in which such G/L
accounts are without project assignment.
Distribution Rule
If you did not select the Use Multidimensions checkbox on the Cost Accounting tab of the General Settings window, under
Administration System Initialization General Settings , the section displays one checkbox and one default
distribution rule field.
If you selected the Use Multidimensions checkbox, the section displays checkboxes and their default distribution rule
fields for the active dimensions.
Only active dimensions are displayed. You can set the active status of dimensions in the Dimensions window under
Financials Cost Accounting Dimensions .
If required, select one or more checkboxes to set the G/L account as relevant to distribution rules of corresponding dimensions. If
required, you can further choose , and in the List of Distribution Rules window, select a default distribution rule for the
corresponding dimension.
You can change the checkbox status and the default distribution rule field at any time.
 Note
Distribution rule fields are displayed only for G/L accounts of type Sales or Expenditure.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:04 AM
For G/L accounts relevant to distribution rules, SAP Business One performs actions, defined on the Cost Accounting tab of the
General Settings window, for postings in which such G/L accounts have no distribution rule assigned to the selected
dimensions.
Account Details
Opens the G/L Account Details window in which you can define and add more information pertaining to the account.
Block Manual Posting
Select to block manual postings to the selected account in the following transactions:
Journal vouchers
Posting templates
Recurring postings
This checkbox does not apply to the following transactions:
Conversion difference
Exchange rate difference
Opening balance
Period end closing
You can deselect the checkbox at any time and manual postings will no longer be blocked for the account.
More Information
Chart of Accounts
Setting Up and Working with G/L Accounts
G/L Account Details Window
G/L Account Details Window
Use this window to display or change the data of a specific account.
To open the window, choose Financials Chart of Accounts . Then select the required account and choose Account Details.
G/L Account Details
G/L Account, Account Name
Read-only account code and name, as defined in the Chart of Accounts window.
Foreign Name
Name that appears in several reports (on screen and in printed reports) when Display Foreign Names is selected in the selection
criteria window of the report.
Code for Exporting
Additional code for the account, used only when exporting transactions from SAP Business One to another software.
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:04 AM
Project
Specify whether to relate the account to one of the projects defined in SAP Business One.
Details
Specify additional details regarding the account.
Default Tax Posting Account
Select default account for tax posting. The options are:
Sales Tax Account
Purchase Tax Account
Default Tax Code
Specify the tax code to be used by default when a manual journal entry is created (including any journal entry that is based on a
posting template or a recurring posting). If you have left the Default Tax Posting Account field empty, this field is disabled.
Category
The Category fields are available for active accounts only. If required, specify the category of the account.
1. In the first field, from the dropdown list, choose the category of the account, as follows:
Balance Sheet – Specify the account as a Balance Sheet account.
Profit and Loss – Specify the account as a Profit and Loss account.
Trial Balance – Specify the account as a Trial Balance account (predefined and closed list of options available only).
Other – Specify the account category as Other if it is neither a Balance Sheet account nor a Profit and Loss
account.
If the field is left empty, the account does not belong to any category and you cannot specify a subcategory for it.
2. In the second field, from the dropdown list, choose the subcategory of the account. Proceed as follows:
If there is no relevant subcategory in the dropdown list, define a new one to which you want to assign the account.
If there are relevant subcategories in the dropdown list, specify one for the account.
If the field is left empty, the account does not belong to any subcategory.
For certain countries/regions you may find additional information in the localization-specific online help file under: Help
Documentation Localization-Specific Info .
Planning Level
If required, specify the planning level for use in the B1iSN integration scenario Liquidity Forecasting. The planning level is a source
of planning data used to process the liquidity forecasting report in SAP ERP.
Branch
Select a branch to which you want to assign the account.
 Note
This field is available only if you have enabled multiple branches.
Active
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:04 AM
Enables you to determine an active date range for the account:
From...To... – Specify the date range.
Remarks – Specify a relevant comment.
 Note
If a user tries to add a journal entry, for example, on a date that exceeds the defined range, the remark appears in an
error message.
Account Balance Allowed
Defines in local currency the amount range of the account balance for any G/L account. (You can define only the highest amount,
only the lowest amount, both amounts, or neither amount.)
Remarks Template
You can predefine texts here as templates for remarks in journal entries either manually created or generated by documents
whose remarks are defined in the Reference Field Links setup form.
On Hold
Enables you to deactivate an account for a determined period of time.
From...To... – Specify the date range during which the account cannot be used.
Remarks – Specify a relevant comment.
 Note
If you try to add a journal entry on a date within the defined range, the remark appears in an error message.
Cost Accounting Adjustment Only
Available only when the account category is not Other.
If the checkbox is selected, the G/L account can be used in the Journal Entry for Cost Accounting Adjustments
only.
Allow Multiple Linking to Financial Templates
Lets you link this account more than once within the same financial template. This is useful, for example, if you need to include the
debit and the credit sides of an account rather than the overall balance, one side in the assets section and the other side in the
liabilities section of the balance sheet.
If you do not select this checkbox, the application issues a warning message but you are not prevented from including the account
more than once.
Relevant to Budget
Enables you to define budgets for the account.
 Note
Only available if Budget Initialization is selected in Administration System Initialization General Settings Budget .
Exchange Rate Differences
Includes the account in the automatic creation of exchange rate differences transactions.
Rate Conversion
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:04 AM
Includes the account in the automatic creation of rate conversion transactions.
More Information
Chart of Accounts
Setting Up and Working with G/L Accounts
Chart of Accounts Window
Balance Sheet Categories - Setup Window
Use this window to define new subcategories that can be linked to Balance Sheet accounts.
To open the window, choose Financials Chart of Accounts Account Details . In the Category fields, choose Balance Sheet
in the first field, and then in the second field, choose Define New.
More Information
G/L Account Details
Profit and Loss Categories - Setup Window
Use this window to define new subcategories that can be linked to Profit and Loss accounts.
To open the window, choose Financials Chart of Accounts Account Details . In the Category fields, choose Profit and Loss
in the first field, and then in the second field, choose Define New.
More Information
G/L Account Details
Other Categories - Setup Window
Use this window to define new subcategories that can be linked to accounts other than the Balance Sheet or Profit and Loss
accounts.
To open the window, choose Financials Chart of Accounts Account Details . In the Category fields, choose Other in the
first field, and then in the second field, choose Define New.
More Information
G/L Account Details
Edit Chart of Accounts - Selection Criteria Window
Use this window to specify the selection criteria for an account or accounts you want to add or edit.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:04 AM
To open the window, choose Financials Edit Chart of Accounts .
After selecting the drawers in which the accounts are located (or are to be located), you maintain them in the Edit Chart of
Accounts window.
Edit Chart of Accounts Window
Use this window to maintain an account or accounts you filtered in the Edit Chart of Accounts - Selection Criteria window.
Edit Chart of Accounts Window
G/L Account Details
The account type (title or active), code, name, and level, for the selected account.
G/L Account Location
Location in the chart of accounts, according to:
Drawer - Name of the drawer(s) in which the account resides
Parent Article - Immediate level under which the account is found
You can view all items on this level that are found in this drawer.
Loc. in Drawer - First, last, or after another account in the drawer.
Add Sub-Level Acct
Adds a lower-level account under the marked account.
 Example
Select a Level 3 account, and choose Add Sub-Level Account to create a new account on Level 4 or 5. The selected account
becomes the parent article of the new account.
 Note
This button displays only if the option Use Segmentation Accounts is not selected on the Basic Initialization tab in
Administration System Initialization Company Details .
Add Same-Level Acct
Adds an account on the same level as a selected account, under the same parent article.
 Note
This button exists only if the option Use Segmentation Accounts is not selected on the Basic Initialization tab in
Administration System Initialization Company Details .
More Information
Chart of Accounts
Setting Up and Working with G/L Accounts
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:04 AM
Account Code Generator Window
Use this window to have active accounts generated automatically from a combination of different segments. These segments
represent the specific business units or activities that you want to track.
The following prerequisites must be fulfilled:
Account segmentation is allowed for your country/region or state.
The option Use Segmentation Accounts is selected in Administration System Initialization Company Details on
the Basic Initialization tab.
To open the window, choose Financials Account Code Generator .
Account Code Generator Window
G/L Account Details
For all G/L accounts to be created, define the following:
Natural Account – Number of characters is limited to the value of the Size field in the Account Segmentation - Setup
window for the first segment: Natural Account
Account Name – String you enter here, plus a suffix from the short name of every segment
Currency – Specify the appropriate currency
Level – Specify the level in the chart of accounts
G/L Account Location
Drawer: Specify the chart of accounts drawer to which to add the G/L accounts.
Parent Article: If you create G/L accounts in Levels 3 to 5, you can set the appropriate title in the drawer to which the
accounts are added. The drop-down box displays titles from one level below the value you set in Level of G\L Account
Details.
 Example
When you select 3 in the Level field, the Parent Article field displays titles from Level 2 of the selected drawer.
G/L Account Properties
The fields from the Chart of Accounts window appear according to the selected drawer.
Division, Region, Department
Choose the button for each segment to open the Segment Code – Selection Criteria window, where you select the required codes
from each segment to be included.
 Note
You must use all the segments defined in SAP Business One when you create new G/L accounts.
More Information
Creating G/L Accounts
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:04 AM
Segment Codes - Selection Criteria Window
Account Code List Window
Segment Codes - Selection Criteria Window
Use this window to specify selection criteria for the segment codes from which you want to generate active accounts. Segment
codes are numbers that represent the specific business units or activities you want to track.
The following prerequisites must be fulfilled:
Account segmentation is allowed for your country/region or state.
The option Use Segmentation Accounts is selected in Administration System Initialization Company Details on
the Basic Initialization tab.
To open the window, choose Financials Account Code Generator , and then choose the button next to the Division,
Region, or Department option.
Selection Criteria
Choose
Includes the accounts defined under this segment in your selection criteria.
Code
These columns display identifying details regarding the segments defined in SAP Business One.
More Information
Creating G/L Accounts
Account Code Generator Window
Account Code List Window
Account Code List Window
This window displays accounts that you can create in the chart of accounts, according to the parameters you set in the Account
Code Generator Window.
 Note
The prerequisites for using this window are that account segmentation is allowed for your country/region or state, and that the
option Use Segmentation Accounts is selected in Administration System Initialization Company Details on the Basic
Initialization tab. If these two conditions are not true, you cannot use this window.
Account Code List Window
Add
Select the accounts you would like to create.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:04 AM
G/L Account
Code that will be assigned for each new account.
Name
Combination of the specified account name and the short name for the selected segment codes. Change the name if required.
Currency
Currency code. You can change the currency if required.
Parent Article
Drawer in the chart of accounts. All the accounts will be created according to the level set in the Account Code Generator window,
under the selected title.
Add
Adds the selected accounts to the chart of accounts.
More Information
Creating G/L Accounts
Account Code Generator Window
Segment Codes - Selection Criteria Window
Creating G/L Accounts
You can create G/L accounts manually or, if you use account segments, you can generate them automatically. You create most
accounts during initialization and setup, often as additions to a predefined chart of accounts. However, you may wish to add a new
account from time to time. For example, if your company incurs a new kind of operating cost due to the introduction of new
technology, you will add a new expenses account. Or if your company opens a new bank account, you will need to reflect this in
your chart of accounts.
Use automatic generation for the following purposes:
To create active accounts from a combination of different segments
Active accounts are accounts in the chart of accounts to which journal entries are posted.
Segments represent the specific business units, such as company, division, region, department, group, or categories, such
as travel expense, box office revenue, product line, and so on, that you want to track.
Automatically generated accounts are based on a combination of different segments.
To create a specific G/L account simultaneously in several different account groups, for example, departments
Procedure
Manually Creating a Title or an Active Account
1. From the SAP Business One Main Menu, choose Financials Chart of Accounts .
The Chart of Accounts window appears.
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:04 AM
2. Select the drawer to which you want to add the account.
3. In the list of accounts, click at the level where you want to add the account.
4. In the menu bar, switch to Add mode by choosing Data Add .
5. In the G/L Account field, enter a valid code and then specify all other relevant data.
6. Choose Add.
The new account is added at the specified level of the selected drawer, as the last account on that level. If you have not
specified a default, it is created as an active account at level two.
 Note
As long as no transactions have been posted, you can change any details/parameters in the Edit Chart of Accounts
window.
You can also create an account in the Edit Chart of Accounts window.
More Information
Chart of Accounts
Chart of Accounts Window
Edit Chart of Accounts Window
Automatically Generating a G/L Account
Prerequisites
- Account segmentation is allowed for your country/region or state.
- The option Use Segmentation Accounts is selected in Administration System Initialization Company Details on the
Basic Initialization tab.
 Note
Once a single journal entry has been posted, you can no longer change the selection for this option.
Procedure
1. From the SAP Business One Main Menu, choose Financials Account Code Generator .
2. In the Account Code Generator window, specify the required information.
3. In the Segment Codes – Selection Criteria window, specify the selection criteria for the segment codes.
4. In the Account Code List window, make the necessary settings and choose Add.
More Information
Account Code Generator Window
Segment Codes - Selection Criteria Window
Account Code List Window
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:04 AM
Changing, Moving, and Deleting G/L Accounts
In the normal course of business, it is not uncommon to have to adjust the chart of accounts from time to time. In SAP Business
One, you can make changes to the chart of accounts, and change, regroup, or delete existing accounts.
Examples
One of your banks changes its name, so you update its name in the corresponding G/L account.
You originally created an account that was then never used, so you decide to delete it.
You need to reorganize your subsidiary’s accounts, based on new instructions from the mother company.
Procedure
Changing a G/L Account
1. From the SAP Business One Main Menu, choose Financials Edit Chart of Accounts .
2. In the Chart of Accounts window, select the account and make your changes.
3. To save these changes, choose Update.
4. If required, choose Account Details, make changes in the G/L Account Details window, and choose Update.
More Information
Chart of Accounts Window
G/L Account Details Window
Moving a G/L Account
 Note
Moving a parent account also moves its sublevel accounts.
1. From the SAP Business One Main Menu, choose Financials Edit Chart of Accounts .
2. Do one of the following, and choose OK.
To change the location of accounts within a drawer, select the relevant drawer.
To move accounts between drawers, select the relevant drawers.
The Edit Chart of Accounts window appears, listing the accounts included in the selected drawer(s).
3. Select the account you want to move.
 Note
To find an account, press CTRL + F , enter its code and/or name in the Find Account window, and choose OK.
The G/L Account Location section displays the current location parameters.
4. In the Drawer, Parent Article, and Loc. in Drawer fields, specify the target location of the account.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:04 AM
The options in the G/L Account Location fields depend on the selections made in the Edit Chart of Accounts –
Selection Criteria window.
The account moves to the specified location.
5. To save the change, choose Update.
More Information
Edit Chart of Accounts - Selection Criteria Window
Edit Chart of Accounts Window
Deleting G/L Accounts
Prerequisites
- No transactions have been posted to the account, including the opening balance.
- The opening balance has not been posted to the account.
- The account is not defined as a control account.
- The account is not included in G/L account determination.
Procedure
1. From the SAP Business One Main Menu, choose Financials Edit Chart of Accounts .
2. In the Edit Chart of Accounts - Selection Criteria window, select the required drawers and choose OK.
3. Select the account you want to delete.
4. From the menu bar, choose Data Advanced Delete Account .
Checking G/L Account Balances
Procedure
1. From the SAP Business One Main Menu, choose Financials Chart of Accounts .
2. Choose an account and click the arrow next to Balance.
The Account Balance – <account title> window appears.
3. To display the codes and names of business partners or G/L accounts in the account balance, choose and select the
Visible option for the BP/Account Code and BP/Account Name columns.
 Note
You can also check the account balance of an individual business partner from the Business Partner Master Data window.
More Information
Chart of Accounts Window
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:04 AM
Journal Entry
Use this function to manually create journal entries for accounts and business partners.
 Note
Manual entries are recorded directly in the database and cannot be deleted. To cancel a journal entry, create a correction
journal entry (storno).
You can view and create journal entries in expanded or reduced editing mode.
For more information about the abbreviated transaction types in the Origin field in the Journal Entry window, see Transaction Type
Abbreviations Legend.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Creating Journal Entries Manually
Context
 Caution
You cannot delete a journal entry after it has been added manually to the database.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Entry .
The Journal Entry window opens in Add mode.
2. In the header fields, enter the relevant transaction information, such as reference number, dates, and so on.
3. In the table area, enter accounting information, including amounts and additional details, using a separate row per G/L
account or business partner.
4. After inserting all the rows, ensure that the debit and credit total amounts are balanced, in local currency, foreign currency
and system currency.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:04 AM
To enable creating unbalanced transactions in foreign currency, choose Form Settings Document General , and
select Allow Unbalanced Transaction in FC.
5. Choose Add.
Results
The transaction is recorded in the database and affects financial and accounting reports.
Related Information
Journal Entry
Changing the BP Control Account in Journal Entries
Prerequisites
You have defined all accounts you want used as control accounts for a specific business partner (see Business Partners
Business Partner Master Data Accounting General Control Accounts Control Accounts – Accounts Payable/Receivable
).
Context
Whenever a journal entry is posted to a business partner, it is also automatically posted to a control account defined for the
business partner. This enables SAP Business One to reflect in the accounting system and the financial reports all business
activities carried on with business partners.
The control account to which a journal entry is posted is defaulted, but can be changed. To achieve more detailed reports, you can
change the control account. This procedure:
Explains how to change the control account for a business partner when you create manual journal entries
Is also relevant for the journal entries that are first recorded as journal vouchers
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Entry .
The Journal Entry window appears.
2. Open the Journal Entry – Form Settings window.
3. On the Table Format tab, select the options Visible and Active for the Control Acct column, and choose OK.
The Control Acct column appears in the table area of the Journal Entry window.
4. Create the journal entry.
Notice that once you choose a G/L account or business partner code, the defaulted control account is recorded in the
Control Acct column. Move to the Control Acct column in the business partner row and delete the control account you
want to replace.
5. To view the available control accounts, press TAB and choose the required account.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:04 AM
It is not possible to change the control account in the G/L account row.
6. Choose Add.
Results
The system posts the journal entry to the selected control account.
Related Information
Journal Entry
Cancelling Journal Entries
Prerequisites
The transaction is a manual journal entry of type JE (displayed in the Origin field of the Journal Entry window).
Context
You cannot delete journal entries from the database, but you can create a reversal journal entry that voids the original transaction.
Use this procedure to cancel manual journal entries.
 Note
You can reverse journal entries created by documents by creating the opposite document or a manual journal entry that
reflects the reversal.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Entry.
2. Display the journal entry you want to cancel.
3. From the menu bar, choose Data Cancel .
The following message appears: Create reversal for this transaction?
4. To continue, choose Yes.
 Note
If the selected journal entry has been reconciled, a notification appears and you can decide whether to continue or not.
The Journal Entry window displays the reversed transaction. The dates of the new transaction are the same as in the
original transaction. If required, you can change the dates.
 Note
The reversed transaction format is determined by the selection made in the Company Details. If Use Negative Amount
for Reverse Transaction is selected, the amounts in the reversed transaction appear on the same sides as in the original
transaction, but with a minus sign. If the option is not selected, the same amounts appear on opposite sides.
5. Choose Add.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:04 AM
Results
The reversed transaction is added to the database. SAP Business One automatically adds the text (Reversal) – original trans. no.
to the transaction details for reporting purposes.
Journal Entry Window
Use this window to display journal entries. The fields in the General Area section are relevant for the entire journal entry, while the
fields in the Expanded Editing Mode section reflect the data relevant to the selected row in the journal entry.
To open the window, choose Financials Journal Entry .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
Series
Displays the default numbering series of the journal entries. Choose another series if required.
Number
Entry number allocated by the system according to the selected numbering series.
Due Date, Posting Date, Doc. Date
By default, the posting date is the current date. Change it if necessary. The due date is the date on which the entry takes place. The
document date is the journal entry date for tax reporting purposes.
Ref. 1, Ref. 2
Specify relevant references for the journal entry, or leave these fields blank.
Trans. Code
Select a transaction sort code from a previously defined list of codes to help you find a particular transaction. Choosing a code
automatically inserts the code description as the default setting in the Details field.
Remarks
Enter any relevant information regarding the journal entry.
 Note
If the transaction is an incoming payment that has been generated by the payment wizard, the default display is
Incoming Payments - <business partner code> — <payment run name>.
If the transaction is an outgoing payment that has been generated by the payment wizard, the default display is
Outgoing Payments - <business partner code> — <payment run name>.
The payment run name is copied from the Payment Wizard, General Parameters window.
Origin, Origin No., Trans. No.
The Origin field displays the abbreviated name of the original document. If the journal entry was created when you added an A/R
invoice, the abbreviation IN is displayed.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:04 AM
The Origin No. field displays the number of the document that generated the journal entry transaction.
Choose (Link Arrow) to display the document.
The Trans. No. field displays the automatically assigned number of the journal entry.
Template Type, Template
You can record transactions according to one of the defined posting templates.
Choose Template Type (percentage or recurring) and in the Template Code field, select the appropriate template code.
Indicator
Select the relevant indicator code from a list of previously defined codes to help you find a particular transaction.
Project
You can link a transaction to a previously defined project and use it as a selection criterion in reports.
Click the icon to link the transaction to a project in the list of projects defined for the company.
Revaluation Reporting Exch. Rate
In reports, if you want to revalue the postings in foreign currency with an exchange rate other than the one defined in the Exchange
Rate and Indexes window, select this checkbox to define the foreign currency and the exchange rate.
The revaluation is for reporting purposes only and does not affect the postings values.
Reverse
Enables you to create a reversal transaction for the current journal entry and define the date on which the reversal transaction
should be created.
Adj. Trans. (Period 13)
Enables you to mark the closing entries. If required, you can exclude closing entries when generating a report.
Branch
Select the branch for which you want to create the journal entry.
 Note
This field is available only if you have enabled multiple branches.
Automatic Tax
If this option is selected, once you create a row in the journal entry for a G/L account for which a default tax group was defined,
SAP Business One automatically creates a row for the tax transaction. The checkbox is not editable once the journal entry is
added.
This option is selected by default if the option Use Automatic Tax in Administration System Initialization Document
Settings Per Document tab Journal Entry is selected.
Manage WTax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox:
The WTax Amount field and the WTax Liable column are displayed.
You can enter only one business partner in the journal.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:04 AM
Manage Deferred Tax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox, you can enter only one business partner in the journal.
Display in FC, Display in SC
By default, journal entry amounts are displayed in local currency. Select these options to display the amounts in foreign and/or
system currency.
Clear Template
Disconnects a journal entry based on a specific posting template, from that template.
A message asking whether to clear the table appears. To have all rows of the journal entry deleted, choose Yes. To keep the journal
entry rows while clearing the Template Type and Template fields, choose No.
Expanded Editing Mode
G/L Acc./BP Code, G/L Acc./BP Name
Selecting the G/L Account/BP Code in the table automatically inserts the G/L account/business partner name.
Ref. 1
 Note
You can configure the values through Administration Setup General Reference Field Links . The values described here
are the default ones.
Displays the document number for all the rows in the journal entry, if the entry resulted from a document such as an A/R invoice,
incoming payment, and so on.
Displays for all the rows, the data specified by the user in the header field Ref. 1, if the journal entry was created manually.
Ref. 2
 Note
You can configure the values through Administration Setup General Reference Field Links . The values described here
are the default ones.
Displays different information, depending on the document through which the journal entry was created:
Displays the customer/vendor reference number assigned to the document, if the journal entry resulted from an A/R
Invoice, Incoming Payment, and so on.
Displays the number of the base document, if the journal entry resulted from a reversing document (A/R Credit Memo
based on A/R Invoice).
Displays the data specified in the document header Ref. 2 field, if the journal entry resulted from an inventory transaction
document, such as Goods Receipt.
Displays the data specified in the Ref. 2 field of the Opening Balance or Period-End Closing Settings window, if the journal
entry was created through one of these windows.
Displays data specified by the user, if the journal entry was created manually.
Ref. 3
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:04 AM
You can configure the values through Administration Setup General Reference Field Links . The values described here
are the default ones.
The information displayed here depends on the document through which the journal entry was created:
A/R and A/P Invoice, A/R and A/P Credit Memo, A/R and A/P Down Payment Invoice, A/R and A/P Reserve Invoice:
Business partner row: sequential installment number
Withholding tax row: sequential number of the last installment
Incoming and Outgoing Payments:
Business partner row: document number
Check payment: check number
Credit card payment: credit card voucher number
Bank transfer payment: reference number specified by the user
In the case of a cash payment, nothing is displayed.
When cancelling an incoming or outgoing payment, the document number of the cancelled document is displayed.
When creating an incoming or outgoing payment on account (not based on selected transactions), the document
number is displayed in the Ref. 3 field in the tax line.
When creating an incoming or outgoing payment to account, the document number is displayed in the Ref. 3 field of
the account rows.
Deposits:
Check deposit: check number
Credit card voucher deposit: credit card voucher number
Cash deposit: deposit number
Receipt from Production, Issue for Production and closing a production order: production order number
The production order number is copied to Ref. 3 only when the value of the Reference 3 - BP Row field in the Reference
Field Links - Setup window is set to Not Defined. To access the Reference Field Links - Setup window, from the SAP
Business One Main Menu, choose Administration Setup General Reference Field Links .
Offset Account
Automatically specifies the offset account of the posting.
You can specify any account from those that were posted in this document. The offset account is then displayed in accounting
reports.
Debit (FC), Credit (FC), Debit, Credit, Debit (SC), Credit (SC)
Display the credit or debit amount of every row in the transaction currency, foreign currency, and system currency.
Due Date, Posting Date, Doc. Date
By default, the posting date is the current date. Change it if necessary.
The due date is the date on which the entry takes place.
The document date is the journal entry date for tax reporting purposes.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:04 AM
Project
If required, specify the project to which the G/L account or business partner is allocated.
Tax Group
Tax group connected to the G/L account or business partner that appears in the selected row.
Distr. Rule
If required, specify a distribution rule for the selected row.
If you did not select the Use Multidimensions checkbox on the Cost Accounting tab of the General Settings window, under
Administration System Initialization General Settings , select a distribution rule from the dropdown list.
If you selected the Use Multidimensions checkbox, click , and in the Select Distr. Rule window, choose distribution rules
for the dimensions.
In the List of Distribution Rules window, you can choose the Define Manual Distribution Rule button to define a
distribution rule for the specific row.
 Note
Only active dimensions appear in the Select Distr. Rule window.
Remarks
Specify row details.
The default entry consists of details for the entire transaction.
 Note
If the transaction is an incoming payment that has been generated by the payment wizard, the default display is
Incoming Payments - <business partner code> — <payment run name>.
If the transaction is an outgoing payment that has been generated by the payment wizard, the default display is
Outgoing Payments - <business partner code> — <payment run name>.
The payment run name is copied from the Payment Wizard, General Parameters window.
Contents Tab Fields
G/L Acc./BP Code, G/L Acc./BP Name
Business partners and/or accounts involved in the transaction. When creating the journal entry manually, to choose a G/L account
from list, press the TAB key; To choose a business partner from list, press CTRL + TAB .
Federal Tax ID
Displays the federal tax ID in the rows of business partner accounts as follows:
If the journal entry is automatically generated by a purchasing or sales document, the field value is copied from the
document and refreshes accordingly in case of changes in the document. Here, the value is not editable.
If the journal entry is automatically generated by a document of other types, the field value is copied from the document
only if the value in the document is editable. Otherwise, the value remains blank.
If you manually create the journal entry, the following conditions apply:
If the business partner you selected is a customer, the default value in the field is copied from the Federal Tax ID
field in the Ship-To Address table in the business partner master data.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:04 AM
If the value in the Ship-To Address is empty, the default value is copied from the Federal Tax ID field on the header of
the business partner master data.
If the business partner you selected is a vendor, the default value in the field is copied from the Federal Tax ID field
on the header of the business partner master data.
You can update the field at any time, even after the journal entry is added.
Tax Amount
Gross Value
Payment Block
In manual journal entries, you can specify whether a business partner row should be blocked from payment by selecting Y or N.
Block Reason
If the row should be blocked from payment (that is, you selected Y in the Payment Block dropdown list), you can select a reason
from this dropdown list.
Payment Order Run
If the checkbox is selected, it indicates that this manual journal entry row is included in a payment order run. The checkbox is
deselected in the following situations:
The payment order row that includes this manual journal entry is removed from the payment order run.
To remove a payment order row, in Payment Wizard: Step 6 - Recommendation Report, right-click the payment order row
and choose Remove. The checkbox for this payment order row is deselected in the selection column.
The payment order row that includes this manual journal entry is closed in the payment order run.
To close payment order rows in which all the documents are fully paid, in Payment Wizard: Step 6 - Recommendation
Report, choose the Close Payment Order Rows button. The Payment Order Status column displays C for the closed
payment order rows.
The payment order run that includes this manual journal entry is executed into a payment run.
To execute a payment run, in Payment Wizard: Step 6 - Recommendation Report, choose the Next button. In Payment
Wizard: Step 7 - Save Options, choose the Next button and choose Yes in the system message.
 Note
When this checkbox is selected, you cannot change the value in the Due Date field in the expanded editing area.
 Note
The above-mentioned fields appear in the table section by default. Use the Form Settings window to add more columns to the
table.
Control Account
You can specify the control account for this journal entry after selecting a business partner.
 Note
If you cannot find this field in the table, in the Form Settings window, set the Control Account field to Active and Visible.
Due Date
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:04 AM
Due date of each line in the transaction.
Expected Account Balance (LC, SC, FC)
Display the expected balance of the account in local, system, and foreign currencies. Before you add the journal entry, the values in
the fields refresh accordingly if you perform one of the following:
Enter or change the amount in the Debit or Credit field
Create or update documents which trigger changes in the account balance, for example, A/P invoices
 Note
These fields are available only when the Journal Entry window is in Add mode.
Source of Posting
Indicates the source of the current posting line. A journal entry source is a data table that records information and data related to
journal entries. If the source is not supported, this field is empty.
The values are presented in the <Origin - Source (Source Table Name)> format. For example, if the journal entry is posted due to
the creation of an A/R invoice, and the current journal entry line is posted due to the freight in the A/R invoice lines, then the value
of the Source of Posting field will be [A/R Invoice – Freight on Rows (INV3)].
Currently, the following sources are supported:
A/R Invoice (OINV): represents the origin document as a whole
A/R Invoice – Rows (INV1): represents the origin document lines
A/R Invoice – Freight – Rows (INV2): represents the freight defined in the origin document lines
A/R Invoice – Freight (INV3): represents the freight defined on the origin document header
A/R Invoice Rows – Distributed Freights (INV13): represents the distributed freight on the origin document header
A/R Invoice – Installments (INV6): represents the installment in the origin document
A/R Invoice – Drawn Dpm Detail (INV11): represents the down payment in the origin document
Source Line Internal ID
Indicate the internal ID of the line in the source of the current posting line.
The internal ID is the internal numeric key automatically assigned to the source line by SAP Business One at the time of creation.
The combination of the Source of Posting and the Source Line Internal ID values can identify the specific and unique data record
line that causes the current posting line.
For example, if the journal entry is posted due to the creation of an A/R invoice, the Source of Posting is [A/R Invoice – Freight on
Rows (INV3)], and the Source Line Internal ID of the current posting line is 3. This means that the current journal entry line is
posted due to the freight in the A/R invoice line, and the Int. Line No. of the freight line is 3.
 Note
To enable the line internal ID in marketing documents, choose Form Settings Table Format , and select the Visible
checkbox for the Int. Line No. column.
Import from Excel
You can import certain data from a Microsoft Excel file to a company in SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:04 AM
The data is copied from the cells of the Microsoft Excel table and written to the corresponding fields in SAP Business One.
 Note
If some data is manually added on the form before import, the imported lines will be added at the end of the existing
lines and will not override the existing data.
After performing the import from Excel, you must choose the Add button in the Journal Entry window to finish the data
import.
You can import only a single journal entry (for example, a header with several lines). If you intend to import several
journal entries at one time (for example, two headers with several lines), you can go to the Import from Excel window (
Main Menu Administration Data Import/Export Data Import Import from Excel ) and select Journal Entry
from the Data Type to Import dropdown list.
 Note
You can update the Ref. 1, Ref. 2, Ref. 3 fields and Remarks fields in the header and rows, and any user-defined fields, on journal
entries with locked posting periods if the Allow Updating of References, Remarks, and UDFs on Journal Entries with Locked
Posting Periods checkbox is selected in the Document Settings window ( Administration System Initialization
Document Settings Per Document tab Journal Entry document ).
Related Information
Journal Entry
Posting Templates
Reverse Transactions
Preparing a Microsoft Excel Import File for Journal Entry
Journal Entry: Attachments Tab
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
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:04 AM
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
Form Settings - Journal Entry Window, Document Tab
Define in this tab default settings to apply whenever you create a manual journal entry. In the General tab, you define settings
related to the general area of the Journal Entry window, and in the Table tab you define settings related to the journal entry rows.
Convert Amounts According to Rate Upon Exit:
Define if a recalculation has to take place when exiting the respective field, after changing amounts in local currency or foreign
currency:
From LC Field — when selected, if you change an amount in the Debit or Credit field and exit the field, SAP Business One
recalculates the amount in the respective Debit (FC) or Credit (FC) field accordingly. This checkbox is deselected by default
From FC Field — when selected, if you change an amount in the Debit (FC) or Credit (FC) field and exit the field, SAP
Business One recalculates the amount in the respective Debit or Credit field accordingly. This checkbox is selected by
default.
Transaction Type Abbreviations Legend
The following table lists the transaction types and their abbreviations. The abbreviated transaction types appear in the Origin field
in the Journal Entry window, as well as in other windows in SAP Business One.
Transaction Type Abbreviations Legend
Transaction Type Abbreviation
Opening Balance OB
Closing Balance BC
Journal Entry JE
Delivery DN
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:04 AM
Return RE
A/R Invoice IN
A/R Invoice + Payment IN
A/R Reserve Invoice IN
A/R Debit Memo IN
A/R Invoice Exempt IN
A/R Bill IN
A/R Exempt Bill IN
A/R Export Invoice IN
A/R Down Payment Invoice DT
A/R Credit Memo CN
A/R Correction Invoice CS
A/R Correction Invoice Reversal CE
Goods Receipt PO PD
Goods Return PR
A/P Invoice PU
A/P Reserve Invoice PU
Internal Invoice in Israel PU
A/P Debit Memo PU
A/P Down Payment Invoice DT
A/P Credit Memo PC
A/P Correction Invoice CU
A/P Correction Invoice Reversal CV
Landed Costs IF
Incoming Payment RC
Deposit DP
Postdated Credit Voucher Deposit / Postdated Check Deposit DD
Outgoing Payment PS
Checks for Payment CP
Bill of Exchange BT
Goods Issue SO
Goods Receipt SI
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:04 AM
Inventory Transfer IM
Inventory Posting ST
Inventory Revaluation MR
Production Order PW
Receipt from Production SI
Issue for Production SO
Internal Reconciliation JR
Correction Invoice CI
Incoming Excise Invoice in India IE
TDS Adjustment in India AD
Outgoing Excise Invoice in India OE
Self Invoice SF
Self Credit Memo SC
Fixed Asset Capitalization AC
Fixed Asset Capitalization Credit Memo AM
Depreciation Run DR
Fixed Asset Manual Depreciation MD
Fixed Asset Revaluation AR
Fixed Asset Transfer FT
Fixed Asset Retirement RT
Item IT
Sales Order OR
Purchase Order PO
Sales Quotation QU
Work Order WO
Equipment Card RI
Inflation Wizard IW
A/P and A/R Tax Invoice TI
Resources RS
Personal Data Management Wizard GW
Data Archive Wizard DA
Return Request RR
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:04 AM
Goods Return Request GR
VAT Exemptions for Business Partners VE
E-Books in Greece EP
Tax Wizard in Brazil TW
Tax Adjustment in Brazil TA
Systems for Value Mapping SM
Value Mapping VM
Value Mapping Communication VC
BP for Immediate Supply of Information (IIS) Annual Reporting in BW
Spain
Customs Cargo Declaration (CCD) Log in Russia CL
Transportation Document TO
Input Service Distribution in India IS
Input Service Invoice in India II
Input Service Recipient Invoice in India IV
ISD Credit Memo in India IC
ISD Recipient Credit Memo in India RM
Purchase Quotation PQ
Inventory Transfer Request TR
Blanket Agreement BA
Purchase Request IQ
Gross Profit Adjustment GP
Preparing a Microsoft Excel Import File for Journal Entry
Context
The following fields for journal entry can be imported into SAP Business One and, therefore, can be contained in a Microsoft Excel
file.
 Note
The maximum length of a numeric value is expressed in the form of <Maximum Digits>.<Maximum Digits>. For
example, "19.6" means that, at most, 19 digits are allowed before the decimal separator, while, at most, 6 digits are
allowed after the decimal separator.
Value options of a field must be in upper case.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:04 AM
The value in the fields could be empty.
| Field Name | Max. Length | Data Type | Remark |
| ---------- | ----------- | --------- | ------ |
Record Type (H for Header and 1 Value options: Predefined column A.
L for Line)
H - create a new header
L – create a new line
that is affiliated with the
latest header
| Series | 8   | Alphanumeric | Field in Header. |
| ------ | --- | ------------ | ---------------- |
Predefined column B.
| Posting Date | 8   | Date                  | Field in Header.     |
| ------------ | --- | --------------------- | -------------------- |
|              |     | Format: YYYY-MM-DD or | Predefined column C. |
YYYY/MM/DD
| Due Date | 8   | Date                  | Field in Header.     |
| -------- | --- | --------------------- | -------------------- |
|          |     | Format: YYYY-MM-DD or | Predefined column D. |
YYYY/MM/DD
| Document Date | 8   | Date                  | Field in Header.     |
| ------------- | --- | --------------------- | -------------------- |
|               |     | Format: YYYY-MM-DD or | Predefined column E. |
YYYY/MM/DD
| Remarks | 50  | Alphanumeric | Field in Header. |
| ------- | --- | ------------ | ---------------- |
Predefined column F.
| Indicator Code | 2   | Alphanumeric | Field in Header. |
| -------------- | --- | ------------ | ---------------- |
Predefined column G.
| Project Code | 20  | Alphanumeric | Field in Header. |
| ------------ | --- | ------------ | ---------------- |
Predefined column H.
| Transaction Code | 4   | Alphanumeric | Field in Header. |
| ---------------- | --- | ------------ | ---------------- |
Predefined column I.
| Reference 1 | 100 | Alphanumeric | Field in Header. |
| ----------- | --- | ------------ | ---------------- |
Predefined column J.
| Reference 2 | 100 | Alphanumeric | Field in Header. |
| ----------- | --- | ------------ | ---------------- |
Predefined column K.
| Reference 3 | 27  | Alphanumeric | Field in Header. |
| ----------- | --- | ------------ | ---------------- |
Predefined column L.
| VAT Date | 8   | Date                  | Field in Header.      |
| -------- | --- | --------------------- | --------------------- |
|          |     | Format: YYYY-MM-DD or | Predefined column (if |
|          |     | YYYY/MM/DD            | applicable)           |
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:04 AM
| Field Name | Max. Length | Data Type      | Remark                |
| ---------- | ----------- | -------------- | --------------------- |
| EU Report  | 1           | Value options: | Checkbox in Header    |
|            |             | Y – Yes        | Predefined column (if |
applicable)
N – No
| ECD Posting Type | 1   | Value options: | Field in Header |
| ---------------- | --- | -------------- | --------------- |
N – Normal
Predefined column (if
applicable)
E - Statement
| Contract Code Identification | 11  | Numeric | Field in Header |
| ---------------------------- | --- | ------- | --------------- |
(CIG)
Predefined column (if
applicable)
| Unique Code of Project (CUP) | 11  | Numeric | Field in Header |
| ---------------------------- | --- | ------- | --------------- |
Predefined column (if
applicable)
Generate Excise Reg No. or Not 1 Value options: Field in Header
Y – Yes
Predefined column (if
applicable)
N – No
| Material Type | 11  | Numeric | Field in Header |
| ------------- | --- | ------- | --------------- |
Predefined column (if
applicable)
| Residence Number Type | 1   | Value options: | Field in Header |
| --------------------- | --- | -------------- | --------------- |
(Multiple Excise Register
1 – Spanish Fiscal ID
Predefined column (if
Number)
applicable)
2 – VAT Registration
Number
3 – Passport
4 – Fiscal ID Issued by
the County of Residence
5 – Certificate of Fiscal
Residence
6 – Other Document
| Creator Name | 155 | Alphanumeric | Field in Header |
| ------------ | --- | ------------ | --------------- |
Predefined column (if
applicable)
| Approver Name | 155 | Alphanumeric | Field in Header |
| ------------- | --- | ------------ | --------------- |
Predefined column (if
applicable)
Account Type (GL or BP)
|     | 2   | Value options: | Field in Line. |
| --- | --- | -------------- | -------------- |
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:04 AM
| Field Name | Max. Length | Data Type         | Remark             |
| ---------- | ----------- | ----------------- | ------------------ |
|            |             | GL – G/L accounts | Predefined column. |
involved in the
transaction
BP – Business partners
involved in the
transaction
| Account Code/BP Code | 15  | Alphanumeric | Field in Line. |
| -------------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Debit Amount | 19.6 | Numeric | Field in Line. |
| ------------ | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Credit Amount | 19.6 | Numeric | Field in Line. |
| ------------- | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Debit Amount (FC) | 19.6 | Numeric | Field in Line. |
| ----------------- | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Credit Amount (FC) | 19.6 | Numeric | Field in Line. |
| ------------------ | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Foreign Currency | 3   | Alphanumeric | Field in Line. |
| ---------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Debit Amount (SC) | 19.6 | Numeric | Field in Line. |
| ----------------- | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Credit Amount (SC) | 19.6 | Numeric | Field in Line. |
| ------------------ | ---- | ------- | -------------- |
Predefined option in dropdown
list.
| Row Details | 50  | Alphanumeric | Field in Line. |
| ----------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Reference 1 (in Lines) | 100 | Alphanumeric | Field in Line. |
| ---------------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Reference 2 (in Lines) | 100 | Alphanumeric | Field in Line. |
| ---------------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:04 AM
| Field Name             | Max. Length | Data Type    | Remark         |
| ---------------------- | ----------- | ------------ | -------------- |
| Reference 3 (in Lines) | 27          | Alphanumeric | Field in Line. |
Predefined option in dropdown
list.
| Due Date (in Lines)      | 8   | Date                  | Field in Line.                |
| ------------------------ | --- | --------------------- | ----------------------------- |
|                          |     | Format: YYYY-MM-DD or | Predefined option in dropdown |
|                          |     | YYYY/MM/DD            | list.                         |
| Document Date (in Lines) | 8   | Date                  | Field in Line.                |
|                          |     | Format: YYYY-MM-DD or | Predefined option in dropdown |
|                          |     | YYYY/MM/DD            | list.                         |
| Project Code (in Lines)  | 20  | Alphanumeric          | Field in Line.                |
Predefined option in dropdown
list.
| Payment Reference No. | 27  | Alphanumeric | Field in Line. |
| --------------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Distribution Rule | 8   | Alphanumeric | Field in Line. |
| ----------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Costing Code 2 | 8   | Alphanumeric | Field in Line. |
| -------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Costing Code 3 | 8   | Alphanumeric | Field in Line. |
| -------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Costing Code 4 | 8   | Alphanumeric | Field in Line. |
| -------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Costing Code 5 | 8   | Alphanumeric | Field in Line. |
| -------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list.
| Payment Block | 1   | Value options: | Field in Header       |
| ------------- | --- | -------------- | --------------------- |
|               |     | Y – Yes        | Predefined column (if |
applicable)
N – No
| Payment Block Abs Entry | 11  | Numeric | Field in Line. |
| ----------------------- | --- | ------- | -------------- |
Predefined option in dropdown
list.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:04 AM
| Field Name                      | Max. Length | Data Type | Remark         |
| ------------------------------- | ----------- | --------- | -------------- |
| Cash Flow Line Item ID (Primary | 11          | Numeric   | Field in Line. |
Form Item)
Predefined option in dropdown
list (if applicable).
You can import only one Cash
Flow Line Item for each line.
| Contract Code Identification | 11  | Numeric | Field in Line. |
| ---------------------------- | --- | ------- | -------------- |
(CIG)(in lines)
Predefined option in dropdown
list (if applicable).
| Unique Code of Project (CUP) | 11  | Numeric | Field in Line. |
| ---------------------------- | --- | ------- | -------------- |
(in lines)
Predefined option in dropdown
list (if applicable).
| System Currency | 3   | Alphanumeric | Field in Line. |
| --------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list (if applicable).
| Posting Date (in lines) | 8   | Date                  | Field in Line.                |
| ----------------------- | --- | --------------------- | ----------------------------- |
|                         |     | Format: YYYY-MM-DD or | Predefined option in dropdown |
|                         |     | YYYY/MM/DD            | list (if applicable).         |
| Federal Tax ID (RFC)    | 32  | Alphanumeric          | Field in Line.                |
Predefined option in dropdown
list.
| Branch Name (in lines) | 100 | Alphanumeric | Field in Line. |
| ---------------------- | --- | ------------ | -------------- |
Predefined option in dropdown
list (if applicable).
If you do not select this option,
the branch name of each line
will be defined with the default
value.
UDFs (User Defined Fields) Depends on the UDFs length.   The UDFs defined for the
header list behind the line
column and the UDFs defined
for the lines list following the
header’s UDFs.
Procedure
You can import the journal entry by the following methods:
1. You can import the journal entry in the Import from Excel window by selecting Journal Entry from the Data Type to Import
dropdown list. It supports batch import, which means you can import simultaneously multiple journal entries that contain
multiple headers. Each header starts behind the previous line.

 Example
Your company is in Italy and you import two journal entries via the Import from Excel window.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:04 AM
Record Series Posting Due Document Remarks Indicator Project Transaction Reference Reference
Type Date Date Code Code Code 1 2
Date
H Primary 2016- 2016- 2016-06- Remark01 1 pr1 tr1 ref1a ref2
06-01 06- 03
02
L
L
L
L
H Primary 2016- 2016- 2016-06- Remark01 1 pr1 tr1 ref1a ref2
06-01 06- 03
02
L
L
L
L
2. You can import the data from the Journal Entry window. Via this window, you can import only a single journal entry, which
contains only one header, at a time.
 Note
The import process is not finished until you click the Add button in the Journal Entry window.
If you have changed the description of a field in the Journal Entry window ( Ctrl + double-click), the field name
in the Import from Excel window will show the description as you defined it originally.
With this import method, the field names are consistent with the description defined in the journal entry. So
when you import the data from the Journal Entry window, you may find that some field names are different from
the field names listed in the previous method; for example, <Unique Code of Project> is described as <CIG>.
 Example
Your company is in Italy and you import one journal entry via the Journal Entry window.
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:04 AM
Record Series Posting Due Document Remarks Indicator Project Transaction Reference Reference R
Type Date Date Code Code Code 1 2 3
Date
H Primary 2016- 2016- 2016-06- Remark01 1 pr1 tr1 ref1a ref2 r
06-01 06- 03
02
L
L
L
L
 Note
You define your data import template in two parts:
a. The predefined columns are mandatory fields.
b. The predefined option in a dropdown list are optional fields.
 Note
Some fields apply only to the specific countries and/or specific system settings.
 Example
You can see the <System Currency> in the object fields only if you have specified a system currency for your
company.
 Example
You can see the <ECD Posting Type> in the object fields only if your company’s location is in Brazil.
 Example
You can see the <VAT Date> in the object fields only if your company’s location is in Belgium or Israel and,
simultaneously, you have enabled the <VAT Date> on marketing documents and the journal entry form.
The below fields in the header cannot be imported from Excel, and so you must manually specify these fields in
the form:
<Template>
<Template Type>
All checkboxes in the header (for example, <Automatic Tax>), except <EU Report> (if applicable). <EU
Report> can be imported from Excel.
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:04 AM
During the import process, even an error caused by one of the lines will result in failure of the whole import
operation. You must cancel the entire import operation (for example, stop importing the data and remove the
data that has been imported from the file) and, after correcting the error, execute the whole import process from
the beginning.
You must ensure that one of the following fields has a value in the Excel file.
<Debit Amount>
<Credit Amount>
<Debit Amount (FC)>
<Credit Amount (FC)>
<Debit Amount (SC)>
<Credit Amount (SC)>
The authorization for importing a journal entry from an Excel operation is based on the authorization of the
Journal Entry form.
If you have full authorization for the Journal Entry form and the authorization for Import from Excel,
you can import multiple journal entries via the Import from Excel window.
If you don’t have the authorization for the Journal Entry form but you do have the authorization for
Import from Excel, you cannot import a journal entry via the import utility; however, you can still import
other objects (for example, Business Partner) via the Import from Excel window.
For importing journal entries from an Excel file, you can only add new records; you cannot update existing
records. All data is imported as new records.
Related Information
Importing Data from a Microsoft Excel File
Import from Microsoft Excel Window
Journal Entry Window
Journal Vouchers
A journal voucher is a draft stage document that creates no values in the general ledger. At this stage, the journal voucher can be
checked and completed, and then recorded. The input template is identical to that of the Journal Entry window.
To open a journal voucher, choose Financials Journal Vouchers .
The diagram below shows the topics covered in this section. Choose each topic for more information.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
Journal Vouchers Window
Use this window to view and enter journal vouchers.
To open the window, choose Financials Journal Vouchers .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Voucher-Related Fields
Find
Trace a journal voucher by its number.
Open Only
Displays only open journal vouchers.
Post Voucher
Posts the journal entries of the selected journal voucher (one that you have finished processing) to the database.
 Note
When a journal voucher is posted, its status changes to C lose d.
Date
Date when the journal voucher was created.
Total (LC)
Total value in local currency of all journal entries included in the journal voucher.
User
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:04 AM
Name of the user who created the journal voucher.
Remarks
Enter any relevant information regarding the journal voucher.
Entry-Related Fields
Trans. No.
The successive number of the journal entries for each journal voucher.
Status
Status of the journal voucher containing the journal entry.
Total (LC), Total (FC)
Total value of each journal entry, in local currency and foreign currency.
Remarks
Content of the Remarks field in the Journal Voucher Entry window.
Base Ref., Posting Date, Ref. 1, Ref. 2, Trans. Code, Project Code
Details taken from journal entries, not displayed by default.
 Note
To view these fields, choose Form Settings in the toolbar.
Add Entry to New Voucher/Add Cost Accounting Adjustment Entry to New Voucher
Opens the Journal Voucher Entry window or the Journal Entry for Cost Accounting Adjustment window where you can create a
journal entry or a cost accounting adjustment journal entry for a new journal voucher.
Add Entry to Existing Voucher
Opens the Journal Voucher Entry window where you can create a journal entry for the journal voucher selected in the upper table.
 Note
Journal entries can be added for open journal vouchers only.
More Information
Journal Voucher Entry
Journal Voucher Entry
Use this window to add a journal entry to a journal voucher.
This window is identical to the Journal Entry Window except for the following field:
Voucher No.
Number of the voucher to which the journal entry is added.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:04 AM
More Information
Journal Voucher
Adding New Journal Vouchers
Context
Use the following procedure to create a new journal voucher for temporary recording of journal entries.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Vouchers .
The Journal Vouchers window appears.
2. Choose Add Entry to New Voucher.
The Journal Voucher Entry window appears.
3. Record the journal entry you want to save in the new journal voucher.
4. Choose Add to Voucher.
Results
The system adds a new record to the upper table in the Journal Vouchers window. Selecting the record displays, in the lower table,
a row representing the journal entry you saved in the new journal voucher.
Related Information
Journal Vouchers
Adding Entries to Existing Journal Vouchers
Prerequisites
At least one journal voucher with the status Open exists in the upper table of the Journal Vouchers window.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Vouchers .
The Journal Vouchers window appears.
2. In the upper table, select the voucher to which you want to add the new entry.
 Note
You can add new entries only to vouchers with the status Open.
3. Choose Add Entry to Existing Voucher.
The Journal Voucher Entry window appears.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:04 AM
4. To record the new entry, choose Add to Voucher.
5. To return to the Journal Vouchers window, choose Close.
Results
Selecting the voucher containing the new entry displays the new record in the lower table of the window.
Related Information
Journal Vouchers
Posting Journal Vouchers
Use journal vouchers as a temporary storage facility for journal entries that cannot yet be posted to the company database. Once
you have checked and approved the journal voucher content, you save it to the database. It is then reflected in the accounting
system.
Procedure
To post journal vouchers to the database and record them as any other journal entry:
1. From the SAP Business One Main Menu, choose Financials Journal Vouchers .
The Journal Vouchers window appears.
2. In the upper table of the window, choose the journal voucher you want to post.
 Note
You can post journal vouchers as long as they have the status Open.
3. Choose Post Voucher.
A system message appears prompting you to save the voucher to the permanent file.
4. Choose Yes.
Result
The status of the posted voucher changes to Closed.
More Information
Journal Vouchers
Deleting Entries from Journal Vouchers
Prerequisites
The journal voucher from which you want to delete entries has the status Open.
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:04 AM
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Vouchers .
The Journal Vouchers window appears.
2. In the upper table of the window, choose the journal voucher from which you want to delete entries.
The lower table of the window displays the entries recorded in the selected voucher.
3. In the lower table, select the row(s) for the entries you want to delete.
4. In the menu bar, choose Data Delete Row .
5. Choose Update.
Related Information
Journal Vouchers
Removing Journal Vouchers
Prerequisites
The journal voucher has the status Open.
Context
SAP Business One saves journal vouchers as temporary files until a user posts them to the database. Until such a time, you can
remove them, along with their recorded entries. Use this procedure to remove irrelevant journal vouchers.
 Note
You can only remove one voucher at a time.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Vouchers .
The Journal Vouchers window appears.
2. In the upper table, select the voucher to remove.
3. From the menu bar, choose Data Remove Journal Voucher .
A confirmation message appears.
4. Choose the OK button.
Posting Templates
Every commercial organization has transactions presented in template format, in which only the recorded amounts vary from
transaction to transaction (for example, the separation of VAT in purchasing or sales).
SAP Business One enables you to create fixed templates for such recurrent journal entries. When recording this type of
transaction, choose the relevant template and fill in the missing items. SAP Business One separates the amounts in accordance
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:04 AM
with the account assignment template.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Posting Templates Window
This window displays Posting Templates according to your defined criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Posting Templates Window
Code
Enter a unique code of up to 8 characters for the posting template.
We recommend that you choose a meaningful code, one that will be understandable to users when they need to choose a posting
template in a journal entry.
Automatic Tax
Applies the Automatic Tax functionality on transactions you create through the Posting Templates window. This option is selected
by default if the option Use Automatic Tax in Administration System Initialization Document Settings Per Document tab
Journal Entry is selected.
Manage WTax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox:
The WTax Amount field and the WTax Liable column are displayed.
You can enter only one business partner in the journal.
Manage Deferred Tax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox, you can enter only one business partner in the journal.
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:04 AM
Control Account
You can specify the control account for this posting template after selecting a business partner.
 Note
If you cannot find this field in the table, you may need to set the Control Account field to Active and Visible in the Form
Settings window.
G/L Acct/BP Code, G/L Account/BP Name
Specify the account code or business partner code to be associated with a journal entry created with this template. The account
name or business partner name appears automatically in the G/L Account/BP Name field.
If there is no constant account or business partner associated with a specific row, or even the entire template, but you still want to
create a template for the percentage distribution, leave these fields blank.
Debit %, Credit %
Enter the appropriate percentages used to separate the amounts in the journal entry for which you are defining the template.
As in a regular journal entry, the debit and credit sides must be balanced in a posting template; otherwise, SAP Business One does
not allow you to add it.
Tax Group
Specify the tax group to which the line refers.
The drop-down list displays all the tax groups to which the account is linked. Selecting one automatically inserts the account in the
line.
If the Automatic VAT option is selected, the default tax group, if defined for the G/L account, is displayed automatically.
If the option Permit Other VAT Group is selected for the G/L account, you may select another VAT group.
Distr. Rule
Specify the distribution rule for each row in the template. When a journal entry based on this posting template is created, the
relevant amounts are posted to the respective cost centers.
 Note
If a distribution rule was defined for the account(s) that appears in the posting template, the amounts recorded in the journal
entries based on this posting template, are posted to the distribution rule(s) defined in the chart of accounts.
Project
Specify the project that you want to relate to the account. If you defined the project for the account in the Chart of Accounts
window, the field displays the project code by default.
 Note
The specified project information appears in the journal entry created using this posting template.
Total
Indicates the percentages entered in the Debit and Credit columns of the posting template.
To Balance
Indicates what percentages you need to enter in the Debit / Credit column to balance this posting.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:04 AM
More Information
Posting Templates
Creating Posting Templates
You can create a percentage-based posting template for journal entries requiring a format that:
Includes the same accounts and/or business partners
Is characterized by a specific ratio of amounts
Procedure
1. From the SAP Business One Main Menu, choose Financials Posting Templates .
The Posting Templates window appears.
2. Specify a unique code and description for the template.
3. In the table area, specify the G/L accounts and/or business partners for inclusion in the template.
 Note
The default control accounts for the business partners included in the posting template can be changed; therefore,
journal entries based on this template are posted to the selected control accounts.
4. For each G/L account/business partner, specify the ratio that reflects the debit or credit amount in the transaction.
 Note
The total percentage in the debit and credit sides must be equal, though it need not be 100%.
5. Choose Add.
Result
The posting template is saved in the database and can be updated.
Example
You can use the following posting template to create journal entries that reflect A/R Invoices:
Posting Template
G/L Account/BP Code Debit % Credit %
Customer 117
Tax Account 17
Sales Credit Account 100
Total 117 117
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:04 AM
More Information
Posting Templates
Creating Journal Entries Based on Posting Templates
Context
You can manually create journal entries by using previously defined posting templates.
Procedure
1. From the SAP Business One Main Menu, choose Financials Journal Entry .
The Journal Entry window appears.
2. In the Template Type field, select the required category:
Percentage – to use a template defined in Financials Posting Templates
Recurring Posting – to use a template defined in Financials Recurring Postings
3. In the Template field, press TAB to open a list of available templates of the selected template type.
 Note
Choosing the Recurring Posting template type displays a list of instances of the recurring posting templates.
4. Select the required posting template or instance:
Selecting Posting Template displays the G/L accounts and/or business partner codes in the table area, together
with the respective percentages representing the amounts of debit and credit.
Selecting a Recurring Posting instance displays the complete journal entry in the window, including all G/L
accounts, and/or business partners and amounts. You can change the amounts, as necessary.
5. If you selected Posting Template, enter the relevant amount in one of the rows and press TAB .
The amounts in the remaining rows are updated accordingly.
6. Enter any other details that might be required, such as reference numbers, and check the dates.
7. Choose Add.
Related Information
Journal Entry
Posting Templates
Removing Posting Templates
Context
Use this procedure to remove posting templates that are no longer relevant.
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:04 AM
Removing a posting template is irreversible. We strongly recommend that you perform this action carefully, especially when
preparing to remove complicated templates.
Procedure
1. From the SAP Business One Main Menu, choose Financials Posting Templates.
The Posting Templates window appears.
2. Display the posting template you want to remove.
3. From the menu bar, choose Data Remove .
A confirmation message appears.
4. Choose OK.
Recurring Posting
Every business has transactions that recur monthly or weekly. Although the transactions recur on predefined dates, and usually
comprise the same objects, the transaction amounts are not necessarily the same each time, nor do the percentages have to be
fixed.
 Example
Recurring journal entries can be payroll orders or standing instructions that are paid by the bank every month.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Recurring Postings Window
This window lets you define and display a recurring posting template according to your defined criteria.
To open the window, choose Financials Recurring Postings .
Recurring Postings Window
Code
Enter a unique code of up to 8 characters for the recurring posting template.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:04 AM
We recommend that you choose a meaningful code, one that will be understandable to users when they need to choose a recurring
posting template in a journal entry.
Instance
Indicates the instance of the transaction.
Description
Enter a short description of the recurring posting.
Ref. 1, Ref. 2
Use these fields to predefine the transaction details, or to specify them just before adding the transaction on the defined date.
Trans. Code
From the drop-down list, choose either the required code or Define New to open the Transaction Codes - Setup window.
The chosen code automatically appears in the Tran. Code field of the Journal Entry window.
Remarks
After you choose a code, its description is copied automatically to this field, and it then appears in the Remarks field in the Journal
Entry window.
Regardless of the chosen code, you can still manually enter the details you prefer.
Automatic Tax
Applies the Automatic Tax functionality on transactions you create through the Recurring Postings window. This option is
selected by default if the option Use Automatic Tax in Administration System Initialization Document Settings Per
Document tab Journal Entry is selected.
Manage WTax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox:
The WTax Amount field and the WTax Liable column are displayed.
You can enter only one business partner in the journal.
Manage Deferred Tax
This checkbox is enabled only if the Automatic Tax checkbox is selected.
If you select this checkbox, you can enter only one business partner in the journal.
G/L Acc./BP Code, G/L Account/BP Name
Enter the account code or business partner code to be associated to a journal entry created with this template. The account name
or business partner name appears automatically in the G/L Account/BP Name field.
Debit, Credit
Fill in the required amounts. Remember that – as for a regular journal entry – the debit and credit must be balanced; otherwise,
you will not be able to add the recurring posting template.
Tax Group
Specify the tax group to which the line refers.
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:04 AM
The drop-down list displays all the tax groups to which the account is linked. Selecting one automatically inserts the account in the
line.
Distr. Rule
Specify the distribution rule for each row in the template. When a journal entry based on this recurring posting template is created,
the relevant amounts are posted to the respective cost centers.
 Note
If a distribution rule was defined for the accounts that appear in the recurring posting template, the amounts recorded in the
journal entries resulting from this recurring posting template, are posted to the distribution rule(s) defined in the chart of
accounts.
Control Account
Displays the default control accounts defined for each business partner and/or G/L accounts included in the template. You can
change the control account in the business partner rows, if required.
To display this column in the table area, select it in the Form Settings - Recurring Posting window. For more information, click
here.
Project
Specify the project that you want to relate to the account. If you defined the project for the account in the Chart of Accounts
window, the field displays the project code by default.
 Note
The specified project information appears in the journal entry created using this recurring posting template.
Total
Indicates the sum of the amounts that were already entered in the Credit column and in the Debit column of the recurring posting
template.
To Balance
Indicates the amount you need to enter in the Debit / Credit column in order to balance this recurring posting template.
Frequency
Choose the required frequency for making the recurring posting.
If you choose Daily, Weekly or Monthly, use the drop-down list for the field to the right to specify a value, that is, the exact number
of days, the day of the week, or the day of the month the recurring posting should be made.
Choosing any other option disables the field to the right.
Choose Template to create a posting template that is not subject to any execution dates or frequency. As such, it will not appear in
the list of transactions for execution.
Next Execution
Enter the required date for the next execution of the recurring posting. This is the base date from which SAP Business One
calculates the value defined in the Frequency field. The default value for this field is the current system date.
If you chose Template for the Frequency field, this field is not shown.
Valid Until
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:04 AM
Select this option to define an expiration date for the validity of the recurring posting template. After the defined date, no further
instances of this template will be created or appear in the list of transactions for execution.
Confirmation List
Opens the Confirmation of Recurring Postings window, in which you can view all recurring postings to be executed.
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
The Ref. Doc field displays the Recurring Posting Code.
You can add only one document at a time from the Document Referenced To tab of a recurring posting.
If a recurring posting template is referenced to a document, for example, an A/R invoice, and you create a journal entry document
from the recurring posting or from another journal entry which uses the recurring posting template, the journal entry will be
referenced automatically to the document (A/R invoice) and will appear on the Document Referenced To tab of the document
(A/R invoice).
Note that if the recurring posting template is referenced to a closed production order, the automatic reference cannot be created.
This applies to all SAP Business One localizations except for Brazil.
You can change the reference documents for the recurring posting at any time. After you change the references, all newly created
journal entries will be referenced automatically to the new documents (available to all SAP Business One localizations except for
Brazil), while the reference relationships of the previously created journal entries stay as is.
 Note
Since recurring postings are not supported by the Relationship Map, you cannot view or track them in the Relationship
Map.
The Copy To functionality does not copy the reference links, as the references are specific to the document for which
they were created.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:04 AM
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
Related Information
Recurring Posting
Confirmation of Recurring Posting
Confirmation of Recurring Posting
This window displays a list of all instances of recurring posting templates. Use this window to define which instances you want
saved to the database and which can be removed from the list.
To open the window, choose Financials Recurring Postings Confirmation List .
Confirmation of Recurring Postings
Posting No.
Displays the recurring posting template code. Choose the arrow to view the recurring posting template.
Description
Displays the description of the recurring posting template.
Date
Displays the date on which each instance of the recurring posting is scheduled to be executed.
 Note
If you execute a specific instance in a date later than appears in the Date field, the date of execution is set as the posting date,
due date, and document date of the journal entry.
Value
Displays the total debit/credit in the recurring posting.
Instance
Instance number of the recurring posting; increases incrementally each time the recurring posting is executed.
Total
Displays the total debit/credit of the selected recurring postings.
Remove
Removes the selected recurring postings. Removed recurring postings cannot be executed and they are deleted from this window.
Execute
Choose to execute the selected recurring postings. Once a recurring posting is executed, a new journal entry is added. You can
view it in the Journal Entry window.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:04 AM
Number of Postings to be Executed
The number of the selected recurring postings.
More Information
Recurring Postings
Setting Templates for Recurring Postings
Context
Use this procedure to create a template for recurring postings and set its frequency and expiration date.
Procedure
1. From the SAP Business One Main Menu, choose Financials Recurring Postings .
The Recurring Postings window appears.
2. In the window header, specify a unique code, an expressive description, and other relevant details.
3. In the table area, build the transaction. Enter the accounts and/or business partners and expected amounts, and ensure
that the transaction is balanced.
 Note
You can change the amounts of each instance of the transaction before you confirm it.
4. In the footer, set the frequency according to which you want SAP Business One to create instances for the transaction. The
default frequency is Monthly.
5. To set a date after which SAP Business One should not create instances of the transaction, use the Valid Until option.
Results
SAP Business One creates the recurring posting template. The instances are created according to the frequency you set, and are
stored in the Confirmation for Recurring Posting window until you execute or remove them.
Related Information
Recurring Posting
Executing Instances of Recurring Postings
Context
Use this procedure to add instances of recurring posting templates and turn them into journal entries.
Procedure
1. From the SAP Business One Main Menu, choose Financials Recurring Postings Confirmation List .
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:04 AM
The Confirmation of Recurring Postings window appears, in which each row represents one instance of a recurring posting
template.
 Note
To set the automatic display of this window, choose Administration System Initialization General Settings
Services . For more information, see General Settings: Services Tab.
2. Deselect the rows you do not want to execute. All are selected by default.
 Note
You can display each instance and make required changes, such as updating amounts. You can also change control
accounts for business partners.
 Note
Every change you make in a specific instance is valid only for that instance and does not affect other instances of the
same template.
3. Choose Execute.
A message appears, asking whether you want to save the posting to the permanent file.
4. To complete the action and create journal entries, choose Add.
Results
The selected instances become journal entries and no longer appear in the Confirmation of Recurring Postings window.
Related Information
Recurring Posting
Removing Recurring Postings
Procedure
1. From the SAP Business One Main Menu, choose Financials Recurring Postings Confirmation List .
The Confirmation of Recurring Postings window appears.
2. Deselect instances you do not want to remove.
3. Choose Remove.
A confirmation message appears.
4. Choose Remove.
Related Information
Recurring Posting
Reverse Transactions
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:04 AM
This function displays a list of all manual journal entries scheduled for automatic reversal, which you can execute.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Reverse Transactions Window
Use this window to create reverse transactions for selected journal entries.
To open the window, choose Financials Reverse Transactions .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Reverse Transactions Window
Cancel
Deselect this option for each transaction that you do not want to reverse.
Transaction
Displays the journal entry number. Use the arrow to the left of this field to open the Journal Entry window.
Description
Displays the content of the Details field in the Journal Entry window.
Original Date
Posting date of the journal entry.
Cancellation Date
Displays the date on which the journal entry should be reversed, as defined in the Journal Entry window.
Value
Displays the debit/credit value of the journal entry.
Number of transactions to be cancelled
The number of the selected transactions.
More Information
Reverse Transactions
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:04 AM
Posting Reverse Transactions
Prerequisites
Reverse transactions can be posted only if the reverse date has already arrived.
Context
Use this procedure to post reverse transactions that are defined in the Journal Entry window.
Procedure
1. From the SAP Business One Main Menu, choose Financials Reverse Transactions . The Reverse Transactions window
appears, displaying all transactions to which a reverse date earlier than the current date was assigned.
2. Deselect transactions you do not want to reverse.
 Note
To change the date of a reverse transaction, choose in the Transaction field.
3. Choose Execute.
Results
New transactions are created, one for each selected row. The Remarks field of these transactions displays the text
(Reversal) and the number of the original transaction. The Reverse option is disabled.
In the original transactions, the Reverse option is not visible, and the word Cancelled indicates that the transactions
were cancelled.
 Note
You can reverse each journal entry only once.
Exchange Rate Differences
When you maintain foreign currency (FC) business partners and/or accounts, SAP Business One conducts all related bookkeeping
in FC. Since you also conduct the bookkeeping system in local currency (LC), SAP Business One expresses every FC transaction in
LC according to the FC exchange rate on the date of transaction. Daily fluctuations in FC exchange rates may cause mismatches
between the balances in LC and FC.
The Exchange Rate Differences function periodically recalculates the LC and FC balances according to the exchange rate on the
day the differences are calculated.
SAP Business One provides recommendations for executing automatic journal transactions for exchange rate differences in FC
business partners and accounts, correct to a given date. The Exchange Rate Differences function reconciles the FC balance and
the LC balance, considering the fluctuation in the FC exchange rate.
The diagram below shows the topics covered in this section. Choose each topic for more information.
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:04 AM
Please note that image maps are not interactive in PDF outputs.
Exchange Rate Differences Window
This window displays the Exchange Rate Differences report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Exchange Rate Differences Window
Execution Date
Date up to which the exchange rate differences are calculated.
Exchange Rate
The exchange rate of the System Currency in Local Currency for the Execution Date.
Details on Transactions
Determine the following details regarding the exchange rate differences transactions you want to execute:
Ref. 1 – Specify the details you want to display in the Ref. 1 field of the transactions.
Code – Specify the required transaction code. The description of the selected code is displayed automatically in the
Remarks field. To define a new transaction code, choose Administration Setup Financials Transaction Codes .
Remarks – Enter a remark to display in the Remarks field in the journal entry.
Auto. Remarks – Automatically displays the text Exchange rate differences for <currency name> in the
Remarks field of the journal entry.
Auto Reverse – Automatically creates a reverse transaction for the exchange rate differences transaction. In the Reversal
Date field, you can specify the date for the reverse transaction.
App.
Select the transactions you want to execute.
Balance
Balance of the G/L account or business partner, calculated in local currency.
Balance (FC)
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:04 AM
Balance of the G/L account or business partner, calculated in the G/L account/business partner currency (the mark of the
currency displayed in the next column).
Rate
Rate set for calculating the difference.
Difference
Suggested difference calculated in LC for the journal entries recorded up to the date of execution.
Save
Saves the recommendations as a draft, without creating journal entries.
More Information
Reverse Transaction
Exchange Rate Differences - Selection Criteria
Use this window to specify selection criteria for the Exchange Rate Differences report.
To open the window, choose Financials Exchange Rate Differences .
After defining the report, you can view it in the Exchange Rate Differences window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Business Partner
Calculates exchange rate differences for business partners.
If not selected, other fields pertaining to business partner selection criteria are not displayed.
Customer Group, Vendor Group
Specify whether to display business partners from a specific group, separated into customers and vendors.
 Example
To display only customers, choose None in the Vendor Group field.
Properties
Opens the Properties window where you can specify required properties. Your choices appear in the field next to the Properties
button.
G/L Accounts
Calculates exchange rate differences for G/L accounts. If not selected, all fields related to G/L accounts selection criteria are not
displayed.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:04 AM
The Account column displays the codes and the names of the accounts. In column X, specify which account or title to include by
clicking the appropriate row.
Show Level
Choose the account level to display in the table.
Level 1 displays the highest level titles for the accounts. When selecting a title in the table, you select all the accounts that appear
under this title.
Exclude Gains with Due Date After
Define a date after which you want to exclude the calculation of net realized gains.
Due Date From...To...
Define a due date range for open items.
Execution Date
Specify the cut-off date for calculating exchange rate differences. This is usually the end of the year or quarter.
Consider Recon. Date
Reflects the reconciliation status of the transactions for the selected date.
 Example
If a transaction is reconciled now but was not reconciled on the execution date, the exchange rate differences are calculated as
if the transaction has not been reconciled.
Currency
Specify the currency for which you want to calculate the exchange rate differences.
Series
Select required series for the exchange rate differences transactions.
Exch. Rate Gain Acct (A/R), Exch. Rate Gain Acct (A/P), Exch. Rate Gain Acct (G/L), Exch. Rate Loss Acct (A/R), Exch. Rate
Loss Acct (A/P), Exch. Rate Loss Acct (G/L)
Specify which of the exchange rate differences accounts should be applied when the automatic journal transaction is executed.
The accounts are divided into gain and loss accounts and used accordingly.
You can define different or identical accounts for customers, vendors, and accounts.
Data Side
Specify whether to calculate the exchange rate differences for the gain side, loss side or both sides.
Previous Report
Opens the latest saved recommendation report.
More Information
Properties
G/L Accounts Determination
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:04 AM
Properties
This window opens when you choose the Properties button in selection criteria windows.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Properties
Ignore Properties
Ignores properties as business partner selection criteria.
Link, Or, And
Specify the logic link between the selected properties:
And narrows the selection, so the selected business partners are only those containing all properties defined in the
properties window.
Or expands the selection so each business partner having at least one of the selected properties is included in the
selection.
Property
Specify required properties by selecting their boxes.
Exchange Rate Differences - Row Details
This window displays the exchange rate difference for the selected row.
Code, Name
The details of the G/L account or business partner to which this row refers.
Currency
The currency in which the exchange rate difference is calculated.
Journal ID
Entry number allocated by SAP Business One according to the selected numbering series. To display the journal entry for the
selected row, click .
Balance, Balance (FC)
The balance of the selected G/L account/business partner displayed in the system currency and the foreign currency. These fields
are maintained automatically.
Rate
Displays the rate of exchange between the system currency and the local currency on the date the transaction is carried out.
Difference
Displays the difference (in the system currency) between the amount in the (system) Balance column and the amount in the
(foreign) Balance (FC) column.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:04 AM
Due Date, Doc. Date, Posting Date
Displays the due date, document date, and posting date for the transaction.
Generating Exchange Rate Differences Report
Context
If you run business activities with foreign business partners or manage foreign currency accounts, you have to handle exchange
rate differences. You can generate a report that lists the recommended transactions pertaining to exchange rate differences.
Procedure
1. From the SAP Business One Main Menu, choose Financials Exchange Rate Differences .
The Exchange Rate Differences – Selection Criteria window opens.
2. Specify the parameters according to which you want SAP Business One to generate the recommendations for the
exchange rate differences transactions.
3. Choose Execute.
Related Information
Exchange Rate Differences
Posting Exchange Rate Differences Transactions
Prerequisites
You have created the Exchange Rate Differences report.
Context
Use this procedure to post exchange rate differences transactions according to recommendations provided by SAP Business One.
Procedure
1. In the header of the Exchange Rate Differences window, specify the relevant details.
2. The rows in the table area represent transactions. In the App. column, select the transactions you want to post.
 Note
Each row in the table can refer to more than one transaction. To view the transactions behind a specific row, double-click
the row. In the Rate Differences – Row Details window, you can include all the transactions in the exchange rate
differences posting or just part of them. Values in the recommended exchange rate differences transaction are updated
accordingly.
3. Choose Add.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:04 AM
If you are not sure whether or not to add the transactions , you can choose Save to save the modified report for later
processing.
Results
SAP Business One adds a new transaction for each row you selected. You can recognize the new transactions according to the
details you assigned to them in the header of the Exchange Rate Differences window.
 Note
If you chose to save the recommendations, no new transactions are added to the database.
Conversion Differences
This function is relevant for companies whose defined system currency is different from the local currency. SAP Business One
recommends making journal entries automatically for differences in system currency. Use the Conversion Differences function to
make adjustments between the account/business partner balance in the system currency and the balance in the local currency.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Conversion Differences Window
This window displays conversion differences templates according to your defined criteria.
Conversion Differences Window
Execution Date
Displays the date until which conversion differences are calculated. This date is entered in the selection criteria window.
Details on Transactions
Use this section to determine the following details pertaining to the conversion differences transactions you choose to execute.
Ref. 1 – Specify the details to display in the Ref. 1 field of the transactions.
Code – Choose the required transaction code. The description of the code is displayed automatically in the Remarks field.
To define a new transaction code, choose Administration Setup Financials Transaction Codes - Setup .
Remarks – Enter the remarks you want displayed in the Details field of the journal entry.
Auto. Remarks – Select to automatically display the text Conversion differences for (currency name) in the
Details field of the journal entry.
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:04 AM
Auto Reverse – Select to automatically create a reverse transaction for the conversion differences transaction, and enable
the Reversal Date field, where you specify the date for the reverse transaction.
App.
Select the checkbox of each transaction you wish to execute.
Code, Name
The details of the G/L account or business partner to which this row refers.
Balance (SC), Balance (LC)
The balance of the G/L account or business partner, displayed in the system currency and the local currency.
Converted Balance (SC)
Displays the balance of the G/L account or business partner in system currency, calculated by the following formulae:
With the Direct exchange rate posting option: Converted Balance (SC) = Balance (LC) / Exchange Rate
With the Indirect exchange rate posting option: Converted Balance (SC) = Balance (LC) * Exchange Rate
Difference
Displays the difference (in the system currency) between the amount in the Converted Balance (SC) column and the amount in
the Balance (SC) column.
This is the amount caused by the difference of the system currency exchange rate between the report execution date and the
document posting date.
Add
Creates the selected transactions and adds them to the database.
Save
Saves the recommendations displayed in this window as a draft, without creating journal entries.
Reject All, Approve All
Choose to clear the selection you made or to select all the transactions.
More Information
Conversion Differences
Conversion Differences - Selection Criteria
Use this window to specify values for a conversion differences template.
To open the window, choose Financials Conversion Differences .
After defining the template, you can view it in the Conversion Differences window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:04 AM
Selection Criteria
Business Partner
Select to calculate conversion differences for business partners. When this checkbox is cleared, all other fields pertaining to
business partner selection criteria are not displayed.
Properties
Opens the Properties window, where you specify the required selection of properties. Your choices appear in the field next to this
button.
G/L Accounts
Select to calculate conversion differences for G/L accounts. If the checkbox is cleared, the fields related to G/L accounts selection
criteria are not displayed.
The X column indicates a selected account or title.
To select/clear accounts, click in the relevant row.
To select/clear all rows, click the X appearing in the column header.
The Account column displays the codes and names of the accounts. View details of each account by using the link appearing next
to its code and name.
Show Level
Choose the account level to display in the table.
Option 1 displays the highest level titles of the accounts. If you select a row in the table you actually select all the accounts
appearing under this title.
Execution Date
Define the cut-off date for calculating conversion differences. Usually this is the end of the year or quarter.
Consider Recon. Date
Reflects the reconciliation status of the transactions for the selected date.
 Example
If a transaction is reconciled now but was not reconciled on the execution date, the exchange rate differences are calculated as
if the transaction has not been reconciled.
Series
Select required series for the conversion differences transactions.
Conv. Rate Gain Acct (A/R), Conv. Rate Loss Acct (A/R), Conv. Rate Gain Acct (A/P), Conv. Rate Loss Acct (A/P), Conv. Rate
Gain Acct (G/L), Conv. Rate Loss Acct (G/L)
Specify which of the conversion differences accounts should be applied when the automatic journal transaction is executed.
The accounts are divided into gain and loss accounts and used accordingly.
You can define different or identical accounts for customers, vendors, and accounts.
Data Side
Specify whether to calculate the conversion differences for the gain side, loss side, or both sides.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:04 AM
Previous Report
Choose to view saved recommendation report.
More Information
Conversion Differences
Properties
Conversion Differences - Row Details
This window displays the conversion difference for the selected row.
General Area Fields
Code, Name
The details of the G/L account or business partner to which this row refers.
Exchange Rate
Displays the rate of exchange between the system currency and the local currency on the date the transaction is carried out.
SC Adjustment
Select this checkbox to create journal entries to adjust the conversion difference for the selected BP or G/L account.
Total Transaction Amount (SC)
Sums up and displays the total value of all transactions of the selected BP or G/L account in the system currency.
Total Balance Due (SC)
Displays the open balance of all the open transactions of the selected BP or G/L account in the system currency.
Difference
Displays the difference between the Total Balance Due (SC) field and the Total Transaction Amount (SC) field.
Table Area Fields
Journal ID
Entry number allocated by SAP Business One according to the selected numbering series. To display the journal entry for the
selected row, click .
Balance (SC), Balance (LC)
The balance of the selected G/L account or business partner displayed in the system currency and the local currency. These fields
are maintained automatically.
Converted Balance (SC)
Displays the balance of the G/L account or business partner in system currency, calculated by the following formulae:
With the Direct exchange rate posting option: Converted Balance (SC) = Balance (LC) / Exchange Rate
With the Indirect exchange rate posting option: Converted Balance (SC) = Balance (LC) * Exchange Rate
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:04 AM
Difference
Displays the difference (in system currency) between the amount in the Converted Balance (SC) column and the amount in the
Balance (SC) column.
This is the amount caused by the difference of the system currency exchange rate between the report execution date and the
document posting date.
Due Date, Doc. Date, Posting Date
Displays the due date, document date, and posting date for the transaction.
Posting Conversion Differences Transactions
Prerequisites
You have generated the Conversion Differences report.
Context
Use the procedure to post conversion differences transactions according to the recommendations provided by SAP Business One.
Procedure
1. In the header of the Conversion Differences window, specify the relevant details.
2. In the App. column in the table area, select the rows (transactions) you want to post.
 Note
Each row can refer to more than one transaction. To view the transactions behind a row, double-click the row. In the
window that appears, you can define whether to include all the listed transactions in the conversion differences posting,
or just some of them. The values in the recommended conversion differences transaction are updated accordingly.
3. Choose Add.
 Note
If you are not sure whether or not to add transactions, you can choose Save to save the modified report for later
processing.
Results
A new transaction is added for each row selected. In the header of the Conversion Differences window, you can recognize the new
transactions according to the details you assigned to them.
If you defined the projects for the selected accounts in the Chart of Accounts window, the project codes appear in the
corresponding journal entry rows.
 Note
If you save the recommendations, no new transactions are added to the database.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:04 AM
Conversion Differences
Financial Report Templates
Use this function to create financial report templates that you can customize for your business needs.
You can create templates for the following reports:
Balance Sheet
Profit and Loss Statement
Trial Balance
Cash Flow
FA Historic Report
More Information
Financial Report Templates Window
Creating Financial Report Templates
Creating Financial Report Templates Based on Existing
Templates
Context
There are cases when it is required to create a financial report template that is similar to another financial report template that
already exists in SAP Business One.
 Example
Subsidiaries of a parent company report their activity on a daily basis. The parent company would like to create a profit and loss
report on a monthly basis to their respective subsidiaries, to show the total for each subsidiary in the books. The chart of
accounts of the parent company identifies each subsidiary using segments. The parent company creates a profit and loss
financial report template for one subsidiary, which is a slimmed down version of the parent company’s profit and loss
statement, and now has to create similar templates for the other subsidiaries.
Procedure
1. From SAP Business One Main Menu, choose: Financials Financial Report Templates . From the Report dropdown list,
select the required financial report.
2. From the Template dropdown list, choose Define New. A setup window, indicating in its name the selected report, appears.
 Example
If you have selected in step #1 the value Balance Sheet, when selecting the option Define New from the Template
dropdown list, the window Balance Sheet Templates — Setup appears.
Specify a name for the new template, and choose the Update button. Choose the OK button.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:04 AM
3. In the Financial Report Templates window, select from the Report dropdown list the financial report whose template is
going to be used as the base template, and from the Template dropdown list select the required template.
4. From the Data menu, choose: Advanced Copy to Template . The Choose Copy Template window appears.
5. From the Report dropdown list select the financial report for which you have defined the new template in step #1, and from
the Template dropdown list, select the new template. Choose the OK button.
6. In the Financial Report Templates window, choose the Update button.
Results
In the Template Details section, select the new template. You can see that it is a copy of the base template. You can now make any
adjustments if required.
Creating Financial Report Templates
Context
Financial reports are presented to different parties for various purposes, requiring customized formatting and presentation
solutions. Use this procedure to build financial report templates, without making any changes in the chart of accounts.
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Report Templates .
The Financial Report Templates window appears.
2. Choose the report for which you want to create a template.
3. Define a new template or, if you only need modifications, select an existing one.
The window displays the existing template, or a blank page to define a new one.
4. Add the required accounts and titles to the template and place them in the required hierarchy and order.
 Note
If you choose Generate Standard Chart of Accounts for a new template, the chart of accounts structure is displayed.
You can remove non-relevant accounts and rearrange the others as required.
5. To link relevant G/L accounts to an account group in the template, double-click the account.
The Account Category - Details window appears.
6. Specify the required account(s) and choose Update.
 Note
Although the chart of accounts may contain accounts at more than four levels, the financial report templates can only
include accounts of up to four levels. Accounts defined as Level 5 and lower are grouped under their Level 4 parent
article and displayed in the Account Category - Details window. The accounting data of the lower-level accounts is
reflected through the fourth-level parent article.
For information about how to specify the accounts, see Account Category - Details Window.
7. In the Financial Report Templates window, choose Update.
Results
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:04 AM
The new template is added to the database and is available in the selection criteria of the report for which the template was
created.
 Example
If you create a template for a balance sheet and name it "My Balance Sheet", the Template field in the Balance Sheet -
Selection Criteria window lists the option My Balance Sheet.
Financial Report Templates Window
Use this window to create or edit Financial Report Templates.
To open the window, choose Financials Financial Report Templates .
Financial Report Templates Window
Template Details
Report – From the dropdown menu, select the report for which you want to create a template.
Template – Specify whether to use an existing template or define a new one.
Show Missing Accounts
Displays accounts that are not included in the template.
G/L Account Details
Name and foreign name of the selected account.
 Note
You can change the name and foreign name of the account for display in the report.
G/L Account Location
Current parent article and account location in the tree.
 Note
You can change the location of the account.
Group Data
For Balance Sheet: Select whether to group the data from the Active side or the Passive side.
For Profit and Loss: Subtotal displays subtotals in the report. Select the account under which you want to locate the
subtotal, select Subtotal and specify its title in the field on the right.
Totals Formula calculates the subtotals from a formula you specify using the Formula option on the right.
Automatic Summary calculates the default subtotals.
For FA historic report: Subtotal displays subtotals in asset history sheet reports. Automatic Summary calculates the
subtotals.
Add Child Acct
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:04 AM
Enables you to create an account on a level lower than that of the selected account.
Add Same-Level Acct
Enables you to add a new account on the same level as the selected account.
Generate Standard Chart of Accounts / Generate From Cash Flow Line Items
Generates the standard chart of accounts for the temperate.
For cash flow report templates, generate the template from cash flow line items.
For fixed asset templates, generates only the assets of the standard chart of accounts.
You can add new accounts, rearrange the accounts, or remove non-relevant accounts as required.
Mock Title
Hides the selected account in the financial report.
Not available for FA history report templates.
Hide Accounts
Hides selected accounts in the report.
Not available for FA history report templates.
Cash Flow Report Template Fields
Report
Specify a report type.
Line Item
Displays the name of a selected line item.
Parent Article
Specify the title to be assigned to the line item.
Loc. on Tree
Specify the location of the line item relative to other line items under the same title.
Line Number
Specify the line item number to be displayed in the final Cash Flow report.
Indent Characters
Specify the number of character indentations to display in the final report. The default number for Level 3 is four indentations.
Text Title
Selecting this field:
Defines the selected line item as a text title that cannot have any child cash flow line items or cash flow relevant G/L
accounts
Disables the Subtotal and Reversal Sign fields
Reversal Sign
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:04 AM
Changes the cash flow line item amount to a negative number.
To display the Financial Report Templates – Expansion window, double-click the line item.
Financial Report Templates - Expansion Window
Double-click the line item to display the Financial Report Templates – Expansion window.
The Cash Flow Line Item tab is launched as the default for both primary and supplementary line items.
You can assign either a cash flow line item or a G/L account.
Cash Flow Line Item Tab
Line Item
From the Choose from List window, assign active cash flow line items to the line items created in the cash flow report template.
Delete Rows
Select a row and click Delete Rows to delete a cash flow line item.
G/L Accounts Tab
G/L Account
Specify G/L accounts to a line item in the cash flow report template.
Account Name
Displays the G/L account name.
Calculation Method
Define the period of time for which to calculate the balance of the assigned G/L accounts.
Delete Rows
Select a row and click Delete Rows to delete a G/L account.
More Information
Financial Report Templates Window
Account Category - Details Window
When you create financial report templates, the account hierarchy display is limited to 4 levels only, while in the chart of accounts
there may be up to 8 levels depending on your localization.
To display the child accounts located under a specific account, double-click this account in the Financial Report Templates
window. The Account Category – Details window appears.
Account Category – Details
G/L Account, Account Name
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:04 AM
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
If the checkbox Accounts with Balance of
Zero is selected in the Balance Sheet –
Selection Criteria window, G/L accounts
with a balance of 0 (zero) are also
included.
Debit + Debit > 0
Debit - Debit < 0
Debit Included regardless of whether the value is
positive or the value is negative
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:04 AM
| Linked | Sign |     | Included in this account group if the |
| ------ | ---- | --- | ------------------------------------- |
following applies:
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
  Note
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
  Note
If the checkbox Accounts with Balance of Zero is selected
in the Balance Sheet – Selection Criteria window, G/L
accounts with a balance of 0 (zero) are also included.
| Debit | +   | Debit < 0 |     |
| ----- | --- | --------- | --- |
| Debit | -   | Debit > 0 |     |
Balance Included regardless of whether the value is positive or the
value is negative
(Balance = Credit – Debit)
  Note
If the checkbox Accounts with Balance of Zero is selected
in the Balance Sheet – Selection Criteria window, G/L
accounts with a balance of 0 (zero) are also included.
| Credit | +   | 0 < Credit |     |
| ------ | --- | ---------- | --- |
| Credit | -   | 0 > Credit |     |
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:04 AM
Linked Sign Included in this account group if the following applies:
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
Choose Copy Template Window
Use this window to copy financial report templates.
More Information
Financial Report Templates
Financial Template - Full Display
This window provides you full display of the current financial report template. You can use it to review the complete template, and
make sure that all required accounts are included and in the right level.
To locate a specific account, choose the Find button and specify the code or name of the required account. If this account is
included in the template, it is marked in the Financial Template – Full Display window. If it is not included in the template, an error
message appears.
Document Printing
Context
Use this function to print batches of documents according to your required selection criteria. You can choose whether to print the
whole list or specific documents.
Procedure
1. From the SAP Business One Main Menu, choose one of the following:
Financials Document Printing
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:04 AM
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
Posting Date From ... To
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:04 AM
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
generates cancellation documents. For a complete list of relevant documents, see Canceling Sales and Purchasing Documents.
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:04 AM
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
Inventory transfer and inventory transfer request
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:04 AM
Production order
Service call
Service contract
Bill of exchange – receivables, bill of exchange – payables, and bill of exchange – transactions
Related Information
Document Printing - Selection Criteria: Checks for Payment
Document Printing
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
Budget
Use this function to define budgets to relevant accounts, according to selected scenarios.
To use the function, choose Financials Budget Setup Budget .
More Information
Budget Scenarios - Setup (Scenario - XXX) Window
Budget Scenarios
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:04 AM
Budget scenarios are used mainly for displaying budget reports. Using a scenario, you create a prognosis of a particular situation
for the company's budget and obtain important information about what the budgetary balance would be according to the selected
scenario.
 Note
When you set up a new company, the application provides a default scenario called Main Budget. This scenario cannot be
altered.
Related Information
Budget Scenarios - Setup Window
Budget Scenarios - Setup (Scenario - XXX) Window
Import Budget Scenarios Window
Use this window to import a budget scenario from another company database. You can also define new budget scenarios with
Budget Scenarios - Setup Window.
To open the window, choose Financials Budget Setup Budget Scenarios . In the Budget Scenarios — Setup window,
choose the Import Scenario button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Import Budget Scenarios Window
Original Data
Specify the data of the source company.
Choose Company – Opens the Choose/Create Company window, where you select the source company.
Database Name, Company Name – Displays the details of the selected source company.
Original Scenario – Specify the budget scenario you wish to import. The list displays all budget scenarios defined in the
selected company.
Destination Data
Database Name, Company Name – Displays the details of the current company.
Destination Scenario – Specify the scenario to which you want to import the original scenario.
More Information
Budget Scenarios - Setup (Scenario - XXX) Window
Copy Budget Scenarios Window
Use this window to copy an existing budget scenario to a new budget scenario in the present company.
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:04 AM
To open the window, choose Financials Budget Setup Budget Scenarios , and then choose Copy Scenario.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Copy Budget Scenarios Window
Original Data
Database Name, Company Name – your current database and company name
Original Scenario – specify the scenario you want to copy
Destination Data
Database Name, Company Name – your current database and company name.
Destination Scenario - specify the target scenario to which you want to copy the original budget scenario data.
Find
Opens the Account – Selection Criteria window where you can define a range of accounts to be selected for the copy budget
scenario procedure.
[Accounts Selection Table]
Specify the required accounts by selecting their rows in the X column. Click the column header to choose all or no accounts. In the
upper right corner, you can choose the account display level.
More Information
Budget Scenarios - Setup (Scenario - XXX) Window
Budget Distribution Methods
Use this function to define the required distribution methods for your budget(s).
 Note
This function is not relevant if you manage an annual budget (see Administration System Initialization General Settings
Budget ).
By default, each company in SAP Business One has three common methods for budget distribution:
Equal – Distributes the budget amount equally among the months of the year.
Ascending Order – Distributes the budget amount in an ascending order; can be used when you increase your budget
expenses over the course of the year.
 Example
In January you use only a small portion of your budget amount, in February you increase your expenses, and so on.
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:04 AM
Descending Order – Distributes the budget amount in a descending order; can be used when you decrease your budget
expenses over the course of the year.
 Example
In January you use the largest portion of your budget amount, in February you use a little less, and so on.
More Information
Budget Distribution Methods - Setup Window
Budget Distribution Methods - Setup Window
Use this window to specify budget distribution methods.
To open the window, choose Financials Budget Setup Budget Distribution Methods .
Budget Distribution Method – Setup Window
Method
Internal number automatically assigned to the distribution method.
Method Name
Specify a description of the distribution method.
Total
Specify the total amount to be distributed among the months. This amount must be greater than zero. The amount is in local
currency.
Month
A numerical representation of the month of the year.
Factor
Specify the proportion of the total to be distributed to each month. The factor total should match the total distribution.
Clear
Clears the definitions made in the Factor column.
Set as Default
Sets a distribution method as the default.
Defining the Budget
Prerequisites
The Budget Initialization option in Administration System Initialization General Settings Budget tab is selected.
The required budget scenario was defined in Financials Budget Setup Budget Scenarios .
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:04 AM
The required distribution methods were defined in Financials Budget Setup Budget Distribution Methods .
Procedure
1. From the SAP Business One Main Menu, choose Financials Budget Setup Budget .
The Budget Scenario Definition window appears.
2. Choose the scenario on which to base the budget and select the G/L accounts to be included.
3. Choose OK.
The Budget Scenarios – Setup window appears, with the name of the selected scenario.
4. For each account, enter the budget amount, percentage, and distribution method.
 Note
When you create a new budget that includes accounts without previous budget definition, the window does not display
any accounts. In this case, select the option Display accounts with no budget.
Results
The budget is defined for the selected accounts and you can make an analysis by comparing the defined budget with the actual
business activity.
Related Information
Budget
Budget Scenarios - Setup Window
Use this window to define new budget scenarios.
To add a new budget scenario, in the menu bar, choose Data Add Row . To delete a user-defined budget scenario, highlight any
field in that scenario, in the menu bar, choose Data Delete Row .
Budget Scenarios — Setup Window
Fiscal Year
The current fiscal year is displayed by default. Choose a different one if required.
 Example
If you are preparing for the coming year and want to define new budget scenario, choose the coming year from the dropdown
menu Note that this is available only if you have defined the respective posting period already.
Budget Name
Specify a name for the budget scenario. This name is unique to that fiscal year.
Based On
Choose the budget scenario on which to base the defined budget scenario. An independent budget scenario should be based on
itself.
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:04 AM
Initial Ratio (%)
Set the percentage of the defined budget in relation to its base budget. If the budget scenario is based on itself, the initial ratio
percentage must be 100.
Rounding Method
Select the rounding method for budget amounts in each scenario.
Copy Scenario
Opens the Copy Budget Scenarios window with which you can copy existing budget scenario into a new one.
Import Scenario
Open the Import Budget Scenarios window in which you can import budget scenario from other SAP Business One company into
new budget scenario.
Related Information
Budget Scenarios
Defining the Budget
Budget Scenarios - Setup (Scenario - XXX) Window
Use this window to specify a budget according to a specific budget scenario.
To open the window, choose Financials Budget Setup Budget . Set the required parameters in the Budget Scenario
Definition window and choose OK.
Budget Scenarios – Setup (Scenario – XXX) Window
Display Accounts with no Budget
Displays G/L accounts for which no budget amount has been entered.
Dimension
From the dropdown list, select an active dimension for which you want to define the budget.
Acct No., Acct Name
Account code and name as defined in the chart of accounts.
Parent Acct
A percentage of this account will be the budget for the account in focus.
%
Percentage of the parent account amount.
 Note
Since the amount in the parent account is not divided between the child accounts, the rate can exceed 100%.
Method
Specify the required method according to which the budget is distributed over months:
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:04 AM
Equal – The budget amount is distributed equally among 12 months.
Ascending Order – The budget is distributed in such a way that most of it is dedicated to the last months, and only a small
part is used during the first months.
Descending Series – The budget is distributed in such a way that most of it is dedicated to the first months of the year, and
the amount assigned to each month decreases as the year progresses.
Manual – Enables you to manually specify how the budget is distributed among the different months. You can, for example,
decide that the budget is distributed among two months only.
Define New – Opens the Budget Distribution Method window where you can define new budget distribution methods.
Debit
Budget amount in local currency. Budget calculation is always performed against the debit side.
Credit
Budget amount for incoming payment accounts, for reporting purposes only.
Actual
Actual amount in this account based on its journal entries.
Distr. Rule Code, Distr. Rule Name
Displays the code and name of the distribution rules to which the budget amount is distributed.
You can add cost centers by right-clicking the G/L account row and choosing Add Cost Center.
Distr. Rule Debit
Enter the budget amount, in local currency or system currency, that you want to distribute to each distribution rule. Budget
calculation is always performed against the debit side.
Distr. Rule Credit
Enter the budget amount, in local currency or system currency, that you want to distribute to each distribution rule. This is the
budget amount for incoming payment accounts, for reporting purposes only.
Distr. Rule Actual
Displays the actual amount, in local currency or system currency, accrued in this account as a result of the distribution rule.
Related Information
Budget Scenarios - Setup Window
Budget Item Details Window
This window enables you to manually change the distribution of the budget amounts, for the selected account. You can change the
total amount assigned to the account as well as the distribution of the amount within the months.
Budget Item Details Window
Account Number
The code of the selected G/L account.
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:04 AM
Account Name
The name of the selected G/L account as defined in Chart of Accounts window.
Total (Local)
The total budget amount in local currency defined for the selected G/L account. You can change this amount if required. Once you
press the TAB key, the amounts in the Total (System) field and in the table are updated accordingly.
Total (System)
The total budget amount in system currency defined for the selected G/L account. You can change this amount if required. Once
you press TAB , the amounts in the System column are updated accordingly.
Month
The month of the year.
Local
The budget amount in local currency that was distributed to each month. You can change manually the amount distributed to each
month. Once you press the TAB key, the amounts in the System column are updated accordingly, and the difference between the
original amount distributed and the updated amount appears in the For Reconciliat.: field.
System
The budget amount in system currency that was distributed to each month. You can change this amount manually. Once you press
the TAB key, the difference between the original amount in system currency and the updated one appears in the For Reconciliat.:
row, under the System column.
 Note
When changing amounts in system currency, the amounts in local currency are not updated accordingly (as opposed to a
change in local currency that results in respective change in system currency as well).
%
The proportion out of the overall budget amount that was distributed to each month. When changing the amounts distributed
among the months and pressing the TAB key, the percentage is updated accordingly.
For Reconciliation
If the total of the % column is not 100, this row displays the amount remaining to be distributed.
Remarks
Specify relevant remark for each month, if required.
 Note
The remarks are saved per month, so make sure that you click the relevant month before entering your remarks.
Update Differences
If you change the monthly budget amounts and, as a result, the total budget value is not fully allocated, choose this button to
specify the remaining value in the budget amount of the last month.
Related Information
Budget Scenarios - Setup (Scenario - XXX) Window
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:04 AM
Cash Flow Forecast Window
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
SAP Business One, version for SAP HANA provides a cash flow forecast function to let you view detailed information about your
company's incoming and outgoing cash flows.
 Recommendation
You should install Microsoft Internet Explorer 9.0 or later for best performance.
To use the cash flow forecast function, in the SAP Business One, version for SAP HANA toolbar, choose . The Cash Flow
Forecast window appears.
You can choose the Export button in the lower–right area to export the business object detail to a Microsoft Excel file.
More Information
Configuration Area
Company Overview
Business Object Details
Configuration Area
 Note
You may choose the collapse/expand button to display or hide the configuration area. In addition, some of the accounts and
measures may vary in different localizations.
The accounts are defined as follows:
A cash account is an account whose Cash Account checkbox is selected in the Chart of Accounts window.
A credit account is the account you choose when creating payments using the Credit Card payment means.
A check account is the account you choose when creating payments using the Checks payment means.
The configuration area has the following sections:
Measure provides five cash-related categories that you can choose to consider in the overview chart.
 Note
Invoices include reserve invoices.
Purchase quotations and sales quotations are not considered.
Outgoing Cash / Outgoing Transaction includes the following:
Cash account amounts in outgoing payments and manual journal entries
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:04 AM
Credit account amounts in outgoing payments and manual journal entries
Check account amounts in outgoing payments and manual journal entries
Business partner row amounts in outgoing payments and manual journal entries
A/P invoices
A/P credit memos
Incoming Cash / Incoming Transaction includes the following:
Cash account amounts in incoming payments and manual journal entries
Credit account amounts in incoming payments and manual journal entries
Check account amounts in incoming payments and manual journal entries
Business partner row amounts in incoming payments and manual journal entries
A/R invoices
A/R credit memos
Expense Forecast includes the following:
Cash account amounts in journal vouchers and recurring postings
Credit account amounts in journal vouchers and recurring postings
Check account amounts in journal vouchers and recurring postings
Business partner row amounts in journal vouchers and recurring postings
Purchase orders
Goods receipt POs
Goods returns
Blanket agreements
Drafts of purchase orders, goods receipt POs, goods returns, A/P down payments, A/P invoices, A/P credit
memos, and A/P correction invoices
Recurring transactions of A/P invoices and A/P credit memos
Sales Forecast includes the following:
Cash account amounts in journal vouchers and recurring postings
Credit account amounts in journal vouchers and recurring postings
Check account amounts in journal vouchers and recurring postings
Business partner row amounts in journal vouchers and recurring postings
Sales orders
Deliveries
Returns
Blanket agreements
Drafts of sales orders, deliveries, returns, , A/R invoices, and A/R credit memos
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:04 AM
Recurring transactions of A/R invoices and A/R credit memos
Opening Balance takes into consideration the amounts that occurred before the starting date you defined in the
time bar.
Criteria provide six criteria that you can choose to consider in the overview chart.
Recurring Postings consider business partner row amounts only.
Recurring Transactions
Blanket Agreements
Journal Vouchers consider business partner row amounts only.
Draft Documents
Consider Delays in Payments takes into consideration the value defined in the Average Delay field in Business
Partner Master Data Payment Terms
Certainty Level provides choices of various certainty levels of cash flow. Drag the square icon to change certainty levels. For
higher levels, the cash is more certain to be earned. To customize certainty levels, choose , and in the Certainty Level
Settings window, drag business objects to required certainty levels, and choose the Save button.
The default settings are as follows:
Certainty Level 1:
Cash Accounts display the cash account amounts in payments, manual journal entries, journal vouchers,
and recurring postings.
Incoming Payments display the amount of business partner rows only.
Outgoing Payments display the amount of business partner rows only.
Certainty Level 2: Credit displays the credit account amounts in payments, manual journal entries, journal
vouchers, and recurring postings.
Certainty Level 3:
Checks display the check account amounts in payments, manual journal entries, journal vouchers, and
recurring postings.
Certainty Level 4:
A/P Invoices includes A/P invoice documents and drafts.
A/P Credit Memos includes A/P credit memo documents and drafts.
A/P Correction Invoices includes A/P correction invoice documents and drafts.
A/R Invoices includes A/R invoice documents and drafts.
A/R Credit Memos includes A/R credit memo documents and drafts.
A/P Correction Invoices includes A/R correction invoice documents and drafts.
Manual Journal Entries display the amount of business partner rows only.
Certainty Level 5:
A/P Down Payment includes A/P down payment invoices, A/P down payment requests, and drafts.
A/R Down Payment includes A/R down payment invoices, A/R down payment requests, and drafts.
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:04 AM
Certainty Level 6:
Goods Receipt PO includes goods receipt PO documents and drafts.
Goods Return includes goods return documents and drafts.
Delivery includes delivery documents and drafts.
Returns include return documents and drafts.
Certainty Level 7:
Purchase Orders: Besides purchase order documents and drafts, Purchase Orders also include blanket
agreements and business partner row amounts in journal vouchers and recurring postings.
Sales Orders: Besides sales order documents and drafts, Sales Orders also include blanket agreements and
business partner row amounts in journal vouchers and recurring postings.
Company Overview
The upper area provides a time bar of two years from the current date for you to specify a time range or date.
To make the time range longer or shorter, drag to the required date.
To apply the same length of time range to a different period, drag the shaded time range to the required period.
The lower part is a chart with bars and a line showing the incoming, outgoing, and net cash amount in the required period. The
three kinds of amounts are displayed accumulatively. For example, the incoming cash flow for today is $50, and the incoming cash
flow for tomorrow is $30; therefore, the incoming amount displayed for tomorrow is $80.
 Note
The following documents are split according to their installment settings:
Sales order documents and drafts
Purchase order documents and drafts
A/R down payment request documents, A/R down payment request drafts, and A/R down payment invoice drafts
A/P down payment request documents, A/P down payment request drafts, and A/P down payment invoice drafts
A/R invoice drafts
A/P invoice drafts
A/R correction invoice drafts
A/P correction invoice drafts
For most documents, the forecast date is the delivery date or due date of the document or installment. For the following
documents, the forecast date is calculated according to a set of priorities:
Recurring transactions
Sales order documents and drafts
Purchase order documents and drafts
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:04 AM
Delivery documents and drafts
The calculation priorities are as follows:
1. The installment date setting if the document is listed in the previous note
To set the installment date, on the Accounting tab of the document, choose the link button beside the Installments field.
The Installments window appears, displaying the installment date setting from the selected payment terms. You can
change the installment date if required. The forecast date of each installment will be set to the date you specified in the
Installments window.
If there is no such field named Installments on the Accounting tab, choose the link button beside the Payment Terms
dropdown list, and in the Payment Terms - Setup window, choose the link button beside the No. of Installments field. In the
Installments window, specify numbers in the Month and Days columns for a specific installment.
 Example
The delivery date or due date of the document is 2012.08.15. If there is no such field named Installments on the
Accounting tab, the forecast date will be calculated according to the numbers you specified in the Installments window
by choosing the link button beside the No. of Installments field in the Payment Terms - Setup window. For the first
installment, you entered 1 and 14 in the Month and Days columns. The forecast date of the first installment will be
calculated as 2012.(08+1).(15+14), and thus set to 2012.09.29.
2. The Manually Recalculate Due Date setting of the document
To define the Manually Recalculate Due Date setting, on the Accounting tab of the document, select the options in the
Manually Recalculate Due Date dropdown list, and enter numbers in the Months and Days fields:
Month End: the last day of the current month
Half Month: the 15th of the current month
Month Start: the first day of the next month
<empty>
 Example
The date after the previous round of calculation is 2012.09.29. You select Month End in the Manually Recalculate Due
Date dropdown list, and enter 1 and 2 in the Months and Days fields, respectively. The forecast date will be calculated
as 2012.(09+1).(30+2), and thus set to 2012.11.02.
3. The Payment Date setting of the business partner
To define the Payment Date setting of the business partner, from the SAP Business One, version for SAP HANA Main Menu,
choose Business Partner Master Data Payment Terms Payment Dates , and in the Payment Dates window, enter
numbers between 1 and 31 inclusive.
 Example
You enter the following numbers in the Payment Dates window respectively:10, 5, 25, 20, and 30.
When you open the window again, the dates will be automatically sorted as: 5, 10, 20, 25 and 30.
The date after the previous two rounds of calculation is 2012.11.02. The forecast date will be set to 2012.11.05, because
the number 2 falls between 0 and 5.
4. The Holidays setting of the company or the business partner
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:04 AM
If the document is in the Purchasing - A/P module, the forecast date is calculated according to the Holidays setting
of the company.
To define the Holidays setting of the company, choose Administration System Initialization Company Details
Accounting Data Holidays . If the date after the previous three rounds of calculation falls on a holiday date, the
forecast date will be set to the next working day.
If the document is in the Sales - A/R module, the forecast date is calculated according to the Holidays setting of the
business partner.
To define the Holidays setting of the business partner, on the Payment Terms tab of the business partner, choose
the holidays in the Holidays dropdown list. If the date after the previous three rounds of calculation falls on a holiday
date, the forecast date will be set to the next working day. If you do not select any holiday in the dropdown list, the
forecast date will still be the date after the previous three rounds of calculation.
 Example
The date after the previous three rounds of calculation is 2012.11.05, and the document is in the Purchasing - A/P
module. According to the Holidays setting of the company, 2012.11.05 is a holiday date of year 2012, so the forecast
date will be set to 2012.11.06.
5. The delays in payments if you select the Consider Delays in Payments checkbox in the Configuration area
To define the delays in payments, from the SAP Business One, version for SAP HANA Main Menu, choose Business
Partners Business Partner Master Data Payment Terms , and in the Average Delay field, enter a number.
 Example
The date after the previous four rounds of calculation is 2012.11.06, and the value in the Average Delay field on the
Payment Terms tab of the business partner is 5. The forecast date will be set to 2012.11.11.
Business Object Details
The Consider Business Objects table lists all the business objects that satisfy your selections in the Configuration area.
For detailed information about the scope of each business object, see the Certainty Level part in Configuration Area.
In the table, to see detailed information of a specific business object, choose the link button in the No. of Document column of the
business object. The Document Details window appears, displaying a list of documents with their information. In the Document
Details window, you can choose the link button in the Original Doc. column to see the document, and the Export button to export
the document details to a Microsoft Excel file.
This is custom documentation. For more information, please visit SAP Help Portal. 95