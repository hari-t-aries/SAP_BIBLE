6/8/26, 5:56 AM

SAP Business One 10.0

Generated on: 2026-06-08 05:56:04 GMT+0000

SAP Business One | 10.0

Public

Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/68a2e87fb29941b5bf959a184d9c6727?locale=en-

US&state=PRODUCTION&version=10.0

Warning

This document has been generated from SAP Help Portal and is an incomplete version of the oﬃcial SAP product documentation.

The information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be

missing important aspects and/or correlations to other topics. For this reason, it is not for production use.

For more information, please visit https://help.sap.com/docs/disclaimer.

This is custom documentation. For more information, please visit SAP Help Portal.

1

6/8/26, 5:56 AM

Opportunities

The Opportunities module lets you track and analyze potential sales and purchasing transactions that your company identifies in

the market. Your company devises strategies to convert these sales and purchasing opportunities into actual deals, which can

involve activities such as meetings and negotiations.

Equipped with comprehensive forecasting methods, SAP Business One enables you to project potential earnings and prioritize

sales and purchasing activities.

The graphics below are interactive. Choose the highlighted areas for more information.

Please note that image maps are not interactive in PDF outputs.

Managing Opportunities

Managing an opportunity entails maintaining data that pertains to the various activities of each stage of the process, until the

opportunity is classified as won or lost, and is closed.

Using the Opportunity window, you can:

Monitor information on potential sales and purchasing volumes.

Update the progress of negotiations.

Analyze each stage of the sales and purchasing processes.

Produce reports.

Close or delete an opportunity.

Reopen a closed opportunity.

The diagram below shows the subject and the relevant tasks covered in this section. Choose each topic for more details.

This is custom documentation. For more information, please visit SAP Help Portal.

2

6/8/26, 5:56 AM

Please note that image maps are not interactive in PDF outputs.

Related Information

Business Partner Master Data Window

Working in Add Mode

Working in Find Mode

Opportunity Window

Use this window to add, update, delete, and close sales and purchasing opportunities.

The general area displays information about opportunities and the business partner.

As an opportunity progresses, you can input and update the information in the various tabs. Once an opportunity is won or lost, it

is closed.

To open this window, from the SAP Business One Main Menu, choose  Opportunities

 Opportunity . The window opens in the

default Add mode.

Related Information

Opportunity: General Area Fields

Managing Opportunities

Activity Window

Opportunity Reports

Opportunity: General Area Fields

Use these fields to enter basic customer/lead or buyer information, and to provide information about a specific sales or

purchasing opportunity.

To open this window, from the SAP Business One Main Menu, choose  Opportunities

 Opportunity .

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

This is custom documentation. For more information, please visit SAP Help Portal.

3

6/8/26, 5:56 AM

General Area Fields

Opportunity Type

There are two types of opportunity: Sales and Purchasing.

A sales opportunity is created for a customer or sales lead, while a purchasing opportunity is create for a vendor.

Business Partner Name

Name of customer corresponding to specified business partner code.

Contact Person

Default contact person for business partner, as defined in business partner master data; editable field.

Total Amount Invoiced

Number of invoices, minus number of credit memos, created for this customer.

Business Partner Territory

Territory to which the business partner has been defined; editable field.

Sales Employee/Buyer

Specify the sales employee or buyer assigned to the selected business partner and responsible for this opportunity.

By default, this field displays the sales employee or buyer defined in the Business Partner Master Data.

If the default sales employee or buyer is not defined, this field displays the sales employee or buyer defined in the Sales

Employees/Buyers - Setup window.

If no sales employee or buyer is defined in these windows, this field displays No Sales Employee.

Owner

Specify the sales employee or buyer who is responsible for this opportunity.

Prerequisite: An employee has been defined in the Employee Master Data window and linked to the business partner.

You can:

Select a diﬀerent owner for each stage.

Limit access to the Opportunity window and its reports to specific employees. For more information, see  Administration

 System Initialization

 Authorization

 Data Ownership Authorizations .

Display in System Currency

All financial fields display values in system currency.

Opportunity Name

Enter a descriptive name.

Opportunity No.

SAP Business One automatically assigns a sequential number.

Status

Status of the opportunity.

Default: Open.

This is custom documentation. For more information, please visit SAP Help Portal.

4

6/8/26, 5:56 AM

For closed opportunities, this field displays Won or Lost, as selected in the Summary tab.

When selecting Won or Lost as the Opportunity Status, the following system message appears: You changed the

opportunity status to won. Do you want to close the related activities? choose Yes or No.

Start Date

Date when the opportunity is created in SAP Business One.

Default: system date

Closing Date

The date when the opportunity is defined in the Summary tab as Won or Lost.

Open Activities

Total number of activities with status Open for the selected business partner.

Closing %

Percentage value entered on the Stages tab for the last stage, indicating the progress of the opportunity.

Related Activities

All activities connected to this opportunity.

Related Documents

All documents linked to this opportunity.

Related Information

Opportunity Window

Opportunity: Potential Tab

Use this tab to estimate the potential profit from an opportunity, and the duration of the pprocess.

To access this tab, choose  Opportunities

 Opportunity

 Potential

.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Potential Tab Fields

Predicted Closing In

Enter time span, in number of days, weeks, or months, until expected close of an opportunity.

Predicted Closing Date

Expected conclusion date, based on value in Predicted Closing In field; editable.

Potential Amount (mandatory)

Specify total amount expected for this opportunity.

This is custom documentation. For more information, please visit SAP Help Portal.

5

6/8/26, 5:56 AM

Weighted Amount

Potential Amount multiplied by Closing % (last stage).

Gross Profit %

Specify expected profit from final sale as a percentage rate.

Gross profit is calculated from the last attached sales document.

Gross Profit Total

Sum of Potential Amount and Gross Profit %.

Level of Interest

Click

 to choose a level of interest from a predefined list, or choose Define New to open the Level of Interest - Setup window and

define custom interest levels.

To define your custom interest levels, in the Description column, specify the degree of customer or vendor interests, such as Very

Interested. The specified values appear as options in the Level of Interest dropdown list.

In the Sort column, specify a positive integer to determine the sort order of the level-of-interest options in the dropdown list. The

smaller the sort number, the higher the option appears in the dropdown list. For example, if you specify the number 1 for the level

Very Interested and the number 2 for Interested, Very Interested appears as the first option in the dropdown list,

followed by Interested.

Interest Range, Description

Click

 to choose an interest range from a predefined list, or choose Define New to open the Interest - Setup window and define

custom interest ranges.

To define your custom interest ranges, in the Description column, specify the scope of customer or vendor interests, such as real

estate or health care. The specified values appear as options in the dropdown list of the Description column.

In the Sort column, specify a positive integer to determine the sort order of the interest range options in the dropdown list. The

smaller the sort number, the higher the option appears in the dropdown list. For example, if you specify the number 1 for interest

range Real Estate and the number 2 for Health Care, Real Estate appears as the first option in the dropdown list,

followed by Health Care.

Interest Range, Primary

Of those listed in the table, indicate most significant interest of business partner.

Related Information

Opportunity Window

Opportunity: General Tab

Use this tab to classify opportunities according to the business partner channel and other factors.

To access this tab, from the SAP Business One Main Menu, choose  Opportunities

 Opportunity

 General

.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

This is custom documentation. For more information, please visit SAP Help Portal.

6

6/8/26, 5:56 AM

General Tab Fields

BP Channel Code

If required, specify the business partner channel.

Channels are business partners with whom your company can provide services in certain transactions.

BP Channel Name

Name of the business partner channel.

BP Channel Contact

Name of the default contact person for the business partner channel; editable.

Remarks

Insert any relevant comments.

BP Project

Specify the project that you want to relate to the specified business partner. If you defined the project for the specified business

partner in the Business Partner Master Data, the field displays the project code by default.

Information Source

In the Description column, specify the catalyst for initial customer or vendor interest. Possible sources include online

advertisements, newspaper articles, exhibitions, and personal contacts. The specified sources appear as options in the

Information Source dropdown list.

In the Sort column, specify a positive integer to determine the sort order of the information source options in the dropdown list.

The smaller the sort number, the higher the option appears in the dropdown list. For example, if you specify the number 1 for

information source Online Advertisements and the number 2 for Newspaper Articles, Online Advertisements

appears as the first option in the dropdown list, followed by Newspaper Articles.

Industry

Specify the industries where the customers or the leads of your sales opportunities are from, or where the vendors of your

purchasing opportunities are from.

Related Information

Opportunity Window

Opportunity: Stages Tab

Use this tab to monitor the various phases of a sales or purchasing activity, and to create a new phase, as necessary.

To access this tab, choose  Opportunities

 Opportunity

 Stages .

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Stages Tab Fields

Start Date

This is custom documentation. For more information, please visit SAP Help Portal.

7

6/8/26, 5:56 AM

Enter the date when the first activity begins, per stage.

The start date of each stage must be equal to or later than:

- the start date specified in the general area

- the closing date of the previous stage

Closing Date

Enter the expected closing date, per stage.

If the closing date for the last stage is later than the predicted closing date specified in the Potential tab, the latter is updated

accordingly.

Stage

Click

 to choose a stage from a predefined list, or define a new one.

You can choose any stage, regardless of the order in which it was defined.

Information from the previous stage is displayed in a newly added row.

  Note

To add a new row, the previous row's stage cannot be designated as Canceled. To change this, choose  Administration

 Setup

 Opportunities

 Opportunity Stages .

%

Displays the closing percentage defined as the default for a stage; editable.

View this figure in graphical format in the Closing % field of the general area.

Potential Amount

Reflects the value in the Potential Amount field on the Potential tab.

Weighted Amount

Sum in Potential Amount multiplied by the percentage (%) of the last stage.

Show BPs Docs

If this checkbox is selected, only documents related to the current business partner can be selected and linked to a specific stage

through the next Document Type and Doc. No. fields; otherwise, all documents of all business partners are available for selection.

Document Type

Specify the type of document to be linked to the current stage.

Doc. No.

To attach a specific document to a stage, enter the document number, or click

 and select it from the List of Documents window.

Choosing a newly created document prompts a confirmation message to update the amount and gross profit. Choose Yes to

update the document amount for the current stage, and Potential Amount and Gross Profit Total in the Potential tab. These

amounts exclude tax.

Activities

To create or update an activity related to a sales stage, click

.

If an activity has already been related to this stage, the Activities Overview window appears when you select the link arrow.

This is custom documentation. For more information, please visit SAP Help Portal.

8

6/8/26, 5:56 AM

Owner

Designate one sales employee or buyer as responsible for all stages, or specify a diﬀerent owner per stage.

Opportunity: Partners Tab

Use this tab to monitor the business partners (vendors and leads) with whom this opportunity is being jointly handled.

To access this tab, choose  Opportunities

 Opportunity

 Partners .

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Partners Tab Fields

Name

Specify the partner name.

Relationship

Specify the relationship between the partner and the company.

Related BP

Specify the partner code.

Remarks

Add relevant comments of up to 50 characters.

Related Information

Opportunity Window

Opportunity: Competitors Tab

Use this tab to monitor any competitors, per opportunity.

To access the tab, choose  Opportunities

 Opportunity

 Competitors .

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Competitors Tab Fields

Name

Specify a competitor by name.

Threat Level

This is custom documentation. For more information, please visit SAP Help Portal.

9

6/8/26, 5:56 AM

Classify the threat from a competitor.

Remarks

Add comments of up to 50 characters.

Won

Indicate a successful competitor, if an opportunity is lost.

Related Information

Opportunity Window

Opportunity: Summary Tab

Use this tab to close an opportunity as either Won or Lost. To update any fields, you need to reopen the opportunity.

To access this tab, choose  Opportunities

 Opportunity

 Summary .

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Summary Tab Fields

Opportunity Status

Select Won or Lost, as appropriate.

In the general area, the default status Open is updated accordingly to Closed.

Document Type

By default, this field automatically displays the classification of the document linked to the last stage of an opportunity.

When the opportunity status is Won, you can choose a diﬀerent document type if the opportunity has been closed by a diﬀerent

type of document.

Document No.

By default, this field automatically displays the number of the document linked to the last stage of an opportunity.

When the opportunity status is Won, you can choose a diﬀerent document number if the opportunity has been closed with a

diﬀerent document. To open the relevant document, click

.

Show Documents Related to the BP

This field is available when you set the opportunity status to Won.

If this checkbox is selected, only documents related to the current business partner can be selected and linked to an opportunity

through the above Document Type and Document No. fields; otherwise, all documents of all business partners are available for

selection.

Reasons

Click

 to choose a reason from a predefined list, or choose Define New to open the Reasons - Setup window and define custom

reasons.

This is custom documentation. For more information, please visit SAP Help Portal.

10

6/8/26, 5:56 AM

To define custom reasons, in the Description column, specify an explanation for the success or failure of the sales or purchasing

activity with up to 30 alphanumeric characters. The reasons that you specify here appear as options in the dropdown list of the

Reason column in the Reasons section in the Summary tab when you create or edit an opportunity and set the opportunity status

to Won or Lost in the Summary tab.

In the Sort column, specify a positive integer to determine the sort order of the reason options in the dropdown list. The smaller

the sort number, the higher the option appears in the dropdown list. For example, if you specify the number 1 for Reason 1 and

the number 2 for Reason 2, Reason 1 appears as the first option in the dropdown list, followed by Reason 2.

Related Information

Opportunity Window

Linked Document

Use this window to see the relevant documents of specific business partners. To access this window, in SAP Business One Main

Menu, choose  Opportunities

 Opportunity

 Summary . Choose the Related Documents button. The Linked Document

window opens.

You can see the following details:

Opportunity No.

Displays the opportunity number.

Document

Displays the document type and the number.

Remarks

Displays the remarks relevant to the document in line.

Total (LC)

Displays the total amount in local currency.

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunity: Attachments Tab

Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by

dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.

  Note

To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your

images before uploading them.

  Note

This is custom documentation. For more information, please visit SAP Help Portal.

11

6/8/26, 5:56 AM

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

Opportunity Window

General Settings: Path Tab

Viewing and Updating Opportunities

Prerequisites

You have defined business partners, either in the Business Partner Master Data or in the Opportunity window.

You have created an opportunity.

Procedure

1. From the SAP Business One Main Menu, choose  Opportunities

 Opportunity .

2. Switch to Find mode in one of the following ways:

Choose  Data

 Find  in the menu bar.

Press  Ctrl  +  F  ..

Choose the

 icon in the toolbar.

3. In the No. field, specify the number of the relevant opportunity, or use the SAP Business One standard search functions.

This is custom documentation. For more information, please visit SAP Help Portal.

12

6/8/26, 5:56 AM

4. Update the required details.

5. Choose Update to save the changes, then OK to close the window.

Adding Opportunities

Prerequisites

You have defined the following:

Business partners (in  Business Partners

 Business Partner Master Data )

Sales employees (in  Human Resources

 Employee Master Data )

Opportunity stages (in  Administration

 Setup

 Opportunities

 Stages )

  Note

You can also define business partners and opportunity stages from within the Opportunity window while creating or updating

the opportunity.

Context

You add opportunities to record your activities with potential business partners such as meetings, phone calls or negotiations.

Procedure

1. Choose  Opportunities

 Opportunity .

The Opportunity window appears in Add mode.

2. Choose an Opportunity Type.

To create a sales opportunity for a customer or lead, choose Sales.

To create a purchasing opportunity for a vendor, choose Purchasing.

3. Choose the Business Partner Code.

In addition to the business partner code and name, the customer's default contact person and sales employee or buyer are

also displayed. Adjust information as required.

4. Assign an Owner for the opportunity.

Optionally, assign a diﬀerent owner for each stage.

5. In the Potential or Stages tab, enter the potential amount for each stage of the opportunity.

6. Enter any optional information, according to your requirements.

7. Choose Add to save the changes and close the window.

Closing and Deleting Opportunities

You close an opportunity in SAP Business One when the purchasing process or the sales process with a lead is finished – whether

the process is successful or not. At this stage, you classify the opportunity as either won or lost, and close it. Closing opportunities

assists you in analyzing your purchasing or sales eﬀectiveness with the reports available in SAP Business One.

This is custom documentation. For more information, please visit SAP Help Portal.

13

6/8/26, 5:56 AM
Procedure

To close an opportunity:

1. Choose  Opportunities

 Opportunity .

The Opportunity window appears.

2. Browse to the relevant opportunity.

3. On the Summary tab, select Won or Lost.

The Last Document Amount displays the amount listed in the last related document, for example, a sales quotation. If no

document has been linked, the Potential Amount is displayed.

4. Choose Update to save the data. All fields are then disabled.

  Note
If required, you can reopen an opportunity by selecting Open.

To delete an opportunity:

1. Choose  Opportunities

 Opportunity .

The Opportunity window appears.

2. Browse to the relevant opportunity.

  Note

Make sure that the opportunity is set to Open on the Summary tab.

3. In the Data menu, choose Remove.

A message warns that this procedure is irreversible.

4. To delete the opportunity, choose Continue.

Related Information

Managing Opportunities

Opportunity Reports

Consistently generated and correctly analyzed reports can provide valuable insight into the reasons for both failures and

successes with the company's sales and purchasing opportunities.

SAP Business One provides windows for creating reports and others for viewing them.

You can base a report on all parameters, or filter it to determine the scope and the focus of the report.

Once you enter a value for an option, SAP Business One selects the checkbox beside the appropriate field. If the checkbox is

deselected, the data is not taken into account during the next selection process, although the fields remain selected with the

chosen criteria.

This is custom documentation. For more information, please visit SAP Help Portal.

14

6/8/26, 5:56 AM

Certain reports can be displayed in graph or table formats. You can choose

 in each of the reports to display or hide selected

columns.

All opportunity reports can be generated from  Opportunities

 Opportunities Reports , or from the Reports module, including

the following:

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

To open the window, choose  Opportunities

 Opportunities Reports

 Opportunities Forecast Report

, or open it from the

Reports module.

After defining the report, you can view it in the Opportunities Forecast Report window.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Forecast Report

Territories

Required territories from those defined in the Business Partner Master Data.

Main Sales Emp./Buyer

Required sales employee or buyer; usually the one that opened an opportunity.

Last Sales Emp. /Buyer

This is custom documentation. For more information, please visit SAP Help Portal.

15

6/8/26, 5:56 AM

Last sales employee or buyer that handled the opportunity.

Stages

Stages to be included in the report.

Dates

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

This aﬀects each defined primary group.

Related Information

Opportunity Reports

Opportunities Report

Opportunities Forecast Report Window

This window displays the Opportunities Forecast report according to the defined selection criteria.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Forecast Report

Oppr. No.

System-generated opportunity number.

This is custom documentation. For more information, please visit SAP Help Portal.

16

6/8/26, 5:56 AM

To display the opportunity, click

.

Oppr. Name

Oopportunity name, if defined.

Contact Person

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

This is custom documentation. For more information, please visit SAP Help Portal.

17

6/8/26, 5:56 AM

Potential amount (SC)

Potential amount, in system currency, for the opportunity.

Predicted Closing Date

Date by which the current stage of the opportunity should be completed.

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

To open the window, choose  Opportunities

 Opportunities Reports

 Opportunities Forecast Over Time Report

.

Alternatively, open it from the Reports module.

After defining the report, you can view it in the Opportunities Forecast Over Time window.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Forecast Over Time - Selection Criteria Fields

This is custom documentation. For more information, please visit SAP Help Portal.

18

6/8/26, 5:56 AM

Territories

Required territories from those defined in the Business Partner Master Data.

Main Sales Emp./Buyer

Required sales employee or buyer; usually the one that opened an opportunity.

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

  Note

This is custom documentation. For more information, please visit SAP Help Portal.

19

6/8/26, 5:56 AM

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Forecast Over Time Report Fields

Month/Quarter/Year

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

Clicking

 in the fields Total, Total Open, Total Won, Total Lost, and Total Completed opens an Opportunity List. In each instance,

the list presents particulars of each component of the total, according to the opportunity number.

Opportunities Statistics Reports - Selection Criteria

Use this window to specify selection criteria for the Opportunities Statistics report.

To open this window, choose  Opportunities

 Opportunities Reports

 Opportunities Statistics Report

. Alternatively, open it

from the Reports module.

After defining the report, you can view it in the Opportunity Statistics window.

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunies Statistics Report - Selection Criteria

This is custom documentation. For more information, please visit SAP Help Portal.

20

6/8/26, 5:56 AM

Territories

Required territories, as defined in the Business Partner Master Data.

Main Sales Emp./Buyer

Required sales employee or buyer; usually the one that opened the opportunity.

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

This aﬀects each defined primary group.

Opportunity Statistics Window

This window displays the Opportunity Statistics report according to the defined selection criteria.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

This is custom documentation. For more information, please visit SAP Help Portal.

21

6/8/26, 5:56 AM

Opportunity Statistics Report Fields

Total

Total number of open and closed opportunities.

Total Open

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

To open this window, choose  Opportunities

 Opportunities Reports

 Opportunities Report

. Alternatively, open it from the

Reports module.

After defining the report, you can view it in the Opportunities Report window.

This is custom documentation. For more information, please visit SAP Help Portal.

22

6/8/26, 5:56 AM

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Report Fields

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

This is custom documentation. For more information, please visit SAP Help Portal.

23

6/8/26, 5:56 AM

This window displays the Opportunities report according to the defined selection criteria.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Report Fields

Oppr. Num

System-generated opportunity number.

To display the opportunity, click

.

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

To open this window, choose  Opportunities

 Opportunities Reports

 Stage Analysis . Alternatively, open it from the Reports

module.

After defining the report, you can view it in the Stage Analysis window.

  Note

This is custom documentation. For more information, please visit SAP Help Portal.

24

6/8/26, 5:56 AM

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Stage Analysis - Selection Criteria Fields

Start Date From...To ...

Range of start dates to view a limited time period.

Predicted Closing Date From...To...

Range of closing dates to view a limited time period.

Opportunity Stage

Required stages.

Add Opportunities with Expired Closing Date

Displays also opportunities of which the closing date has passed.

Stage Analysis Window

This window displays the Stage Analysis report according to the defined selection criteria.

Access the details of a specific stage by double-clicking a stage row.

To filter the display to a specific stage or sales employee or buyer, click

, choose the required options, and Refresh.

The lower part of the screen displays the value for each stage, subdivided per sales employee or buyer in a printable graph form.

To display opportunities with an expired closing date, select the corresponding checkbox, and Refresh.

  Note

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

This is custom documentation. For more information, please visit SAP Help Portal.

25

6/8/26, 5:56 AM

Number of times each stage appears in all the closed opportunities. This figure is also displayed per sales employee or buyer, in

addition to the total.

Information Source Distribution Over Time

This report presents sales and purchasing opportunities according to their sources. The data can be grouped to display in specific

time periods, either days, weeks, or months.

Related Information

Opportunity Reports

Information Source Distribution Over Time - Selection Criteria

Use this window to specify selection criteria for the Information Source Distribution Over Time report.

To open this window, choose  Opportunities

 Opportunities Reports

 Information Source Distribution Over Time Report

.

Alternatively, open it from the Reports module.

After defining the report, you can view it in the Information Source Distribution Over Time window.

  Note

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

This is custom documentation. For more information, please visit SAP Help Portal.

26

6/8/26, 5:56 AM

Required range of closing percentage (%).

Sources

Required sources.

Partners

Required partners.

Competitors

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

Diﬀerent time range than the one specified

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Information Source Distribution Over Time Report Fields

Days, Weeks, Months

Opportunities grouped by days, weeks or months, according to the Predicted Closing Date.

Type of Information Source column

Number of opportunities in each column according to the type of the source.

Total

Total number of opportunities for each time period.

This is custom documentation. For more information, please visit SAP Help Portal.

27

6/8/26, 5:56 AM

Won Opportunities

This report details information about successful opportunities. It displays:

Days remaining until closing

Number of won opportunities

Total receivables

Total income and number of opportunities within a specific time range (graph form).

You can filter the report to include specific dates, sales employees or buyers, and business partners.

Won Opportunities - Selection Criteria

Use this window to specify selection criteria for the Won Opportunities report.

To open the window, choose  Opportunities

 Opportunities Reports

 Won Opportunities Report

. Alternatively, open it from

the Reports module.

After defining the report, you can view it in the Won Opportunities window.

  Note

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

This is custom documentation. For more information, please visit SAP Help Portal.

28

6/8/26, 5:56 AM

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Won Opportunities Report Fields

Days Until Closing

Number of days required to win an opportunity.

This value comes from the Predicted Closing In field of the Opportunity window.

No. of Opportunities

Number of successful opportunities, per time period.

Total Amount

Total of all potential amounts per time period.

Lost Opportunities

Use this report to analyze unsuccessful sales and purchasing opportunities. Filter the report according to various relevant criteria

such as business partner and territory.

Lost Opportunities - Selection Criteria

Use this window to specify selection criteria for the Lost Opportunities report.

To open this window, choose  Opportunities

 Opportunities Reports

 Lost Opportunities Report

. Alternatively, open it from

the Reports module.

After defining the report, you can view it in the Lost Opportunities window.

  Note

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

This is custom documentation. For more information, please visit SAP Help Portal.

29

6/8/26, 5:56 AM

Industry

Required industries.

Documents

Required document types related to the opportunity.

Percentage Rate

Required range of closing percentage (%).

Sources

Required sources.

Partners

Required partners.

Competitors

Required competitors.

Group By:

Required option to define a group display of specific parameters.

Group By (2):

Required option to define a secondary group display under the primary one defined in Group By.

This aﬀects each defined primary group.

Related Information

Opportunity Reports

Lost Opportunities Window

This window displays the Lost Opportunities report according to the defined selection criteria.

Lost Opportunities Report

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Oppr. No.

System-generated opportunity number.

To display the opportunity, click

.

Oppr. Name

Opportunity name, if defined.

Territory

This is custom documentation. For more information, please visit SAP Help Portal.

30

6/8/26, 5:56 AM

Territories to which business partner is assigned.

Industry

Industries related to a business partner.

Closing %

Percentage entered in the Closing % field in the Opportunity window.

Potential Amount (LC)

Local currency value of Potential Amount for the last stage achieved.

Weighted Amount (LC)

Local currency value of Weighted Amount entered in the last stage.

Related Information

Opportunity Reports

My Open Opportunities

This report displays all open sales and purchasing opportunities, per sales employee or buyer, and requires no selection criteria.

The report is restricted to the sales employee or buyer concerned, and users who are linked to this sales employee or buyer. The

link is created either in the Employee Master Data window, or in the User Defaults window.

To generate this report choose  Opportunities

 Opportunities Reports

 My Open Opportunities . Alternatively, generate it

from the Reports module.

  Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

My Open Opportunities Fields

Oppr. Num

System-generated opportunity number.

To display the opportunity, click

.

Oppr. Name

Opportunity name, if defined.

Last Sales Employee

Person who worked on the opportunity in the last stage.

Last Stage

Most recent stage achieved in the opportunity.

Status

Status chosen in the Summary tab of the Opportunity window.

This is custom documentation. For more information, please visit SAP Help Portal.

31

6/8/26, 5:56 AM

Closing %

Percentage entered in the Closing % field in the last stage.

Potential Amount

Potential amount, in local or system currency, for the last stage achieved.

Related Information

My Closed Opportunities

My Closed Opportunities

This report displays all closed sales and purchasing opportunities, per sales employee or buyer, and requires no selection criteria.

The report is restricted to the selected sales employee or buyer, and users who are linked to this sales employee or buyer. The link

is created either in the Employee Master Data window, or in the User Defaults window.

To generate this report, choose  Opportunities

 Opportunities Reports

 My Closed Opportunities . Alternatively, generate it

from the Reports module.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

My Closed Opportunities Fields

Oppr. Num

System-generated opportunity number.

To display the opportunity, click

.

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

This is custom documentation. For more information, please visit SAP Help Portal.

32

6/8/26, 5:56 AM

Opportunity Window

Opportunities Pipeline

This report lets you analyze open opportunities in the sales and purchasing pipelines and to identify the most potentially

successful ones.

Opportunities Pipeline - Selection Criteria

Use this section of the Opportunities Pipeline window to specify selection criteria for the Opportunities Pipeline report.

To open this window, choose  Opportunities

 Opportunities Reports

 Opportunities Pipeline . Alternatively, open it from the

Reports module.

  Note

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

Choose Clear Conditions and Refresh to display the table and graph with diﬀerent selection criteria.

To print the graphic shown in the window, choose Print Graph.

This is custom documentation. For more information, please visit SAP Help Portal.

33

6/8/26, 5:56 AM

To view the open opportunities in dynamic mode, see the topic Dynamic Opportunity Analysis.

To open this window, choose  Opportunities

  Opportunities Reports

 Opportunities Pipeline . Alternatively, open it from the

Reports module.

  Note

This topic documents fields and other elements in this window that either are not self-explanatory or require additional

information.

Opportunities Pipeline Selection Criteria

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

This is custom documentation. For more information, please visit SAP Help Portal.

34

6/8/26, 5:56 AM

Opportunity Reports

Dynamic Opportunity Analysis

Dynamic Opportunity Analysis

This window is part of the Opportunities Pipeline report.

Each sales or purchasing opportunity is represented by a balloon, whose size corresponds to the size of the planned opportunity.

Each vertical division represents a stage in the sales or purchasing process.

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

Random: every opportunity is in a diﬀerent color.

By Employee: All opportunities, per employee, are the same color.

By BP: All opportunities, per business partner, are the same color.

By BP Groups: All opportunities, per business partner group, are the same color.

Step Size (Days)

Display the progress of each step in the report according to the number of days.

Step Delay (Seconds)

Display the delay between steps in increments of seconds.

This is custom documentation. For more information, please visit SAP Help Portal.

35

6/8/26, 5:56 AM

Displaying the Dynamic Opportunity Analysis Report

Procedure

1. From Opportunities Reports, display the Opportunities Pipeline window.

2. In the menu bar, choose  Go To

 Dynamic Opportunity Analysis . The Dynamic Opportunity Analysis window appears,

with each opportunity represented by a balloon.

3. To start, accelerate, interrupt, forward or reverse the dynamic display, click the control arrows at the bottom left of the

screen. The slider moves accordingly.

4. To choose a specific date, move the slider. The date is displayed at the bottom of the screen in the center.

Related Information

Opportunity Reports

This is custom documentation. For more information, please visit SAP Help Portal.

36

