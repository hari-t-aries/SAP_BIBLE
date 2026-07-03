6/8/26, 6:11 AM

SAP Business One 10.0

Generated on: 2026-06-08 06:11:58 GMT+0000

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

6/8/26, 6:11 AM

Project Management

Use the Project Management module to manage your projects from start to finish, centralizing all project related transactions,

documents, resources, and activities. The feature helps you monitor the progress of tasks, stages, subprojects, analyze budget

costs, and generate reports on various aspects of the project, such as stage analysis, open issues, and resources.

A project comprises stages which contain one or more tasks. For each stage, you can manage open issues, documents,

attachments, work orders, and activities. All this information is maintained in the Project window, where you can also view financial

information for the project.

A project can have only one level, or it can contain lower-level projects called subprojects. Subprojects can contain further

subprojects underneath them, and so on, forming a hierarchical tree of subprojects, with the main project at the top level.

If a project contains a subproject, you can access it from the Project window. The information about the subproject is displayed in

the Subproject window, which is similar in layout to the top-level Project window.

In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more

information.

Please note that image maps are not interactive in PDF outputs.

Initial Settings

Before you start to use the Project Management module, you must first enable it and set the available stages for your projects.

Activities

Enablement

Defining Stages

Enablement

Context

To enable the Project Management module, perform the following:

Procedure

1. From the SAP Business One Main Menu, choose  Administration

 System Initialization

 Company Details .

This is custom documentation. For more information, please visit SAP Help Portal.

2

6/8/26, 6:11 AM

2. On the Basic Initialization tab, select the Enable Project Management checkbox.

3. Choose Update.

Defining Stages

Context

SAP Business One provides five predefined project stages that will apply to the projects you create, unless you change the stages

setup:

1. Conception/Initiation

2. Definition/Planning

3. Launch/Execution

4. Performance and Control

5. Finishing Stage

You can rename a stage, add a new stage, or remove a stage.

Procedure

1. From the SAP Business One Main Menu, choose  Administration

 Setup

 Project Management

 Stages .

2. On the Stages - Setup window, you can do the following:

Rename a stage, by selecting the desired field and entering a new name or description.

Add a new stage, by right-clicking the first column of the row where you want to add a stage and choosing Add Row.

Then specify the name and the description of the stage.

Delete a stage, by right-clicking the first column of the stage you want to delete and choosing Delete Row.

3. Choose Update to save your changes.

Working with Project Management

All information about your projects is centralized in the Project window. From here you can set and access information about your

projects.

To access the Project window, from the SAP Business One Main Menu, choose  Project Management

 Project

.

Project Window: General Area

In the header of the Project window, specify general information about your individual project. Further information is maintained

on the following tabs: Overview, Subprojects (if the project consists of subprojects), Stages, Summary, Remarks, and

Attachments.

Project Type

Select one of the radio buttons:

This is custom documentation. For more information, please visit SAP Help Portal.

3

6/8/26, 6:11 AM

External - the project is created for a business partner

Internal - the project is created for your company

BP Code

  Note
This field is relevant only if the project type is External.

From the choose from list, select the relevant business partner.

Contact Person

  Note

This field is relevant only if the project type is External.

Displays the default contact person, as defined in the business partner master data. You can select a diﬀerent contact person.

BP Territory

From the choose-from list, select the territory. The territories available in the list are those that you define in the Territories -
Setup window ( Administration

 Territories ).

 General

 Setup

Sales Employee

From the choose from list, select the relevant sales employee.

Owner

From the choose from list, select the relevant employee.

Project with Subprojects

Select this checkbox if the project consists of subprojects. As a result, an additional tab Subprojects appears in the Project
window.

Project Name

Specify the name of the project. This field is mandatory.

Project No.

Displays the project number automatically.

Status

Select one of the following to characterize the status of the project:

Started

Paused

Stopped

Finished

  Note

If you select Stopped or Finished, the current date is automatically entered as the closing date.

Start Date

Specify the start date of the project.

This is custom documentation. For more information, please visit SAP Help Portal.

4

6/8/26, 6:11 AM

Due Date

Specify the planned end date of the project.

Closing Date

Once the project is finalized, enter the date of its closure. You can later update this field if needed.

Open Activities

Displays the number of open activities linked to all stages.

Completeness %

Displays the percentage of completeness of the project based on its stages and subprojects.

  Example

A project has one stage and one subproject. The contribution of the stage to the project is 50% and the contribution of the

subproject to the project is also 50% as well.

The stage is finished, hence the completeness of the project is 50%.

The subproject has its stages and subprojects, and is 50% complete. Hence, another 25% is added to the project's

completeness. Once the subproject is 100% complete, the project is 100% complete as well.

Financial Project

Select a financial project. The selected financial project will be used as the default financial project for the documents that are
linked to the current project.

Project Window: Overview Tab

Overview Tab Fields

Risk Level

Select the appropriate risk level for the project:

Low

Medium

High

Industry

From the dropdown list, select an existing industry or define a new one.

To save any changes, choose Update.

In the Overview Tab Fields, if the project does not contain subprojects, the system will list all tasks relevant to the project, their

hierarchy, fulfilment, and status. If the project has subprojects, the table will list subprojects. You can access any task or subproject

by selecting

 in the relevant row.

Project Window: Subprojects Tab

Context

This is custom documentation. For more information, please visit SAP Help Portal.

5

6/8/26, 6:11 AM

The Subprojects tab is visible only if the Project with Subprojects checkbox in the header area is selected. On this tab, you can

assign subprojects to the project, that is, you can create subprojects that are directly below the project on the hierarchy level.

Adding Subprojects:

Procedure

1. On the Subprojects tab, choose the Add New Subproject option to open a Subproject window.

The Subproject window is similar to the Project window. It shows similar information in the header area and contains the

Subprojects, Stages, and Summary tabs, which you define in the same way as the tabs in the main Project window. A

subproject is treated as a lower level project. One project can contain several subprojects, each of which can contain

subprojects as well.

2. Define the information about the subproject and choose Add. The Subproject window closes and the subproject is added

to the Subprojects tab. Basic information from the subproject is copied onto the row.

3. To save the changes, choose Update.

Alternatively, you can add a subproject from a template by expanding the Add New Subproject option. Remove a

subproject by right-clicking the subproject entry and choosing the relevant option.

Project Window: Stages Tab

On this tab, you can specify tasks related to individual project stages to build up your project. More than one task can be related to

a stage. The Stages tab allows you to add open issues, attachments, documents, work orders, and activities.

When you highlight a row in the table, the sections below (Open Issues, Attachments, Documents, Work Orders, and Activities)

contain information related to the stage in the selected row. To view and manage the information in a section, expand it by

selecting

 (Expand).

After expanding a section such as Documents, choose from the relevant fields in the table to add and assign an item like a

document. To add a document, choose a Doc. Type then a Document Number and whether the document is chargeable to the

client. You can also assign documents to a project when prompted by opening a Project window, if documents were created in the

system with the relevant financial project but were not yet assigned to the project.

Stage Tab Field Information

Stage

Select a stage as defined in the Stages - Setup window.

Planned Cost

Enter the planned or expected cost of the task. This amount is used as a reference only.

Invoiced Amount (A/R)

Displays the total amount of all open A/R invoices that are linked to the relevant financial project and stage.

Open Amount (A/R)

Displays the total amount of all open A/R documents except A/R invoices which are connected to the project and stage.

Invoiced Amount (A/P)

Displays the total amount of all open A/P invoices that are linked to the relevant financial project and stage.

Open Amount (A/P)

This is custom documentation. For more information, please visit SAP Help Portal.

6

6/8/26, 6:11 AM

Displays the total amount of all open A/P documents except A/P invoices which are connected to the project and stage.

%

Displays the contribution percentage of the stage to the project. The sum of all stage contribution percentages and any subproject
contribution percentages cannot exceed 100.

Finished

To close the stage, select this checkbox. If there are open activities or issues related to the stage, you cannot close it.

Stage Dependence (1) (2) (3) (4) (5)

Specify if finishing the stage is dependent on finishing one or more other stages. If a stage is dependent on another stage, you
cannot finish the stage until the stage it is dependent on is finished.

  Note

A stage can be dependent on one or more stages within the same subproject or within the upper project level.

Project Window: Summary Tab

The Summary tab gives you an overview of the project you are viewing. The summary is arranged by the following sections.

Budget

  Note

This section is related to the currently selected project (or subproject). It does not take into account the values related to its

subprojects.

Phase Budget

Displays the accumulated planned costs of all stages of the project (or subproject).

Open Amount (A/P)

Displays the accumulated line totals of all open A/P documents linked to the current project or subproject (except A/P invoices), if
the line is related to the project.

Invoiced (A/P)

Displays the accumulated line totals of all A/P invoices linked to the current project or subproject, if the line is related to the
project.

Total (A/P)

Displays the sum of Open Amount (A/P) and Invoiced (A/P).

Total Variance

Displays the monetary value of Total (A/P) minus Phase Budget.

Variance %

Displays the total variance expressed in percentages.

Accumulated Budget

This section displays the same information as the Budget section, but the values from all the lower-level subprojects related to the

current project or subproject are taken into account as well.

This is custom documentation. For more information, please visit SAP Help Portal.

7

6/8/26, 6:11 AM
Direct Profit Values

  Note

This section is related to the current project (or subproject). It does not take into account the values related to its subprojects.

Potential Subproject Amount

Enter the potential profit amount of the current project or subproject.

Open Amount (A/R)

Displays the accumulated line totals of all open A/R documents linked to the current project or subproject (except A/R invoices), if
the line is related to the project.

Invoiced (A/R)

Displays the accumulated line totals of all A/R invoices linked to the current project or subproject, if the line is related to the
project.

Total (A/R)

Displays the sum of Open Amount (A/R) and Invoiced (A/R).

Total Variance

Displays the monetary value of Total (A/R) minus Phase Budget.

Variance %

Displays the total variance expressed in percentages.

Accumulated Profit Values

This section displays the same information as the Direct Profit Values section, but the values from all lower-level subprojects

related to the current project or subproject are taken into account as well.

Work Order Costs

Actual Item Component Cost

Displays the accumulated item component costs of all work orders in all stages of the current project or subproject (the work
orders related to any lower-level subprojects are not taken into account).

Actual Resource Component Cost

Displays the accumulated item resource component costs of all work orders in all stages of the current project or subproject.

Actual Additional Cost

Displays the accumulated additional costs of all work orders in all stages of the current project or subproject.

Actual Product Cost

Displays the accumulated item component cost of all stages of the current project or subproject.

Actual By-Product Cost

Displays the accumulated by-product costs of all work orders in all stages of the current project or subproject.

Total Variance

Displays the accumulated total variance of all work orders in all stages of the current project or subproject.

Dates

This is custom documentation. For more information, please visit SAP Help Portal.

8

6/8/26, 6:11 AM

Due Date

Displays the due date of the current project or subproject.

Actual Closing Date

Displays the closing date of the current project or subproject.

Overdue

Displays the number of overdue days between the due date and the actual closing date.

Project Window: Attachments Tab

Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by

dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.

  Note

To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your

images before uploading them.

  Note

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

This is custom documentation. For more information, please visit SAP Help Portal.

9

6/8/26, 6:11 AM

Project Overview

Once a project has been added, you can view a detailed overview of the project. To do this, from the SAP Business One Main Menu,

choose  Project Management

 Project

, right-click on the project to generate a context menu, then choose Project Overview.

The Project Overview shows all time-dependent details of projects and subprojects with the relevant stages. You can filter for

levels of the project you want to see by choosing from the Select Level field.

Project Overview Fields

Project / Sub-Project

Displays the name of the project or subproject. Select

 (Link Arrow) to open the connected form.

Stage

Shows the stage description from the stage tab.

Task (Stage)

Displays the task description from the stage tab.

Description (Stage)

Displays the description of the stage row from the stage tab.

Work Order

Shows the work order number of the stage row from the stage tab. Select

 (Link Arrow) to open the connected work order.

Resource

Displays the resource connected to the work order of the stage row in the stage. Select
resource.

 (Link Arrow) to open the connected

Activity

Activity Number of the stage row in the stage tab. Select

 (Link Arrow) to open the connected activity.

Start Date

Start date of the project, subproject, stage (row), work order, or activity.

Due Date

The due date of the project, subproject, or work order. The end date of the stage or activity.

Progress

The progress percentage of the project or subproject.

Completed

Indicates if the row is closed or finished.

Billing Documentation Generation Wizard

The wizard collects open documents and billable items connected to your project for invoicing through A/R invoices or A/R

delivery documents. You can choose the sources that the wizard targets for invoicing.

To do this:

From the SAP Business One Main Menu, choose  Project Management

 Billing Document Generation Wizard .

This is custom documentation. For more information, please visit SAP Help Portal.

10

6/8/26, 6:11 AM

Alternatively, open the Billing Document Generation Wizard from a Project window to pre-populate the wizard with the selected

stage information (this will assign the created documents to the same stage). From the SAP Business One Main Menu, choose

Project Management

 Project

, right-click the project to generate a context menu once the stage has been selected, then

choose Billing Document Generation Wizard.

The wizard guides you through the necessary steps to generate marketing documents:

In step 1, specify what type of document you want to generate and what sources to use. To use diﬀerent sources the wizard may

need to be run multiple times. A selection of fields are described below.

Target Document: Choose the document that you want to create from the inputs in the wizard.

Financial Project, Project No., Subproject No., and Stage: Choose some project details to determine from where source

inputs are taken.

Source Types: Limit or expand the sources to control the inputs for the wizard.

In step 2, confirm which documents you want to place on the target document by using the Confirmed checkbox. Items must exist

for a document to be confirmed.

Gantt Chart

You can represent your project in a Gantt chart format to display the diﬀerent project elements and timelines in an easy to

understand layout.

To do this, from the SAP Business One Main Menu, choose  Project Management

 Project

, right-click on the project to

generate a context menu, then choose Gantt Chart.

Working with Project Reports

The following reports are available to analyze your projects:

Stage analysis - Lists stages of a project or subproject according to the selection criteria.

Open issues - Lists open or closed issues recorded in a project or a subproject according to the selection criteria.

Resources - Lists resources that are connected to a project or a subproject within a work order according to the selection

criteria.

Time sheet - Lists the recorded times connected to a project or subproject according to the selection criteria.

Stage Analysis Report

Context

The report summarizes information for the selected stages by project and subproject. To access a detailed view of stages

belonging to the project or subproject, double-click the desired row.

Procedure

1. From the Main Menu, choose  Project Management

 Project Reports

 Stage Analysis .

This is custom documentation. For more information, please visit SAP Help Portal.

11

6/8/26, 6:11 AM

2. Fields for selection include:

Project Stage

If you want to specify which stages you want to include in the report, select this checkbox, click the Browse button and
select one or more stages.

Employee

To include one or more sales employees in the report, select this checkbox, click the Browse button and select one or more
sales employees.

BP Code

To include one or more business partners in the report, select this checkbox, click the Browse button, and select one or
more business partners.

Add Finished Stages

To include finished stages in the report, select this checkbox.

3. To generate the report, choose OK.

Open Issues Report

Context

The system generates the report with open issues according to the selection criteria.

Procedure

1. From the Main Menu, choose  Project Management

 Project Reports

 Open Issues .

2. Fields for selection include:

Closed

Select this checkbox to include open issues that have been marked as Closed.

Priority

To specify one or more priority levels of open issues which you want to include in the report, select this checkbox. Then
click the Browse button and select one or more priority levels.

Area

To specify one or more areas of open issues which you want to include in the report, select this checkbox. Then click the
Browse button and select one or more areas.

3. To generate the report, choose OK.

Resources Report

Procedure

1. From the Main Menu, choose  Project Management

 Project Reports

 Resources .

2. Fields for selection include:

Resource

This is custom documentation. For more information, please visit SAP Help Portal.

12

6/8/26, 6:11 AM

Select this checkbox to specify one or more resources to be included in the report. Then choose the Browse button and
select one or more resources.

3. To generate the report, choose OK.

Time Sheet Report

Procedure

1. From the Main Menu, choose  Project Management

 Project Reports

 Time Sheet

.

2. Complete the required fields.

3. To generate the report, choose OK.

This is custom documentation. For more information, please visit SAP Help Portal.

13

