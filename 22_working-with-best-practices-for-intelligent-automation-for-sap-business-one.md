6/8/26, 6:13 AM

SAP Business One 10.0

Generated on: 2026-06-08 06:13:50 GMT+0000

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

6/8/26, 6:13 AM

Working with Best Practices for Intelligent Automation for SAP
Business One

The best practices for intelligent automation for SAP Business One is a set of best practice templates for business processes

automation solutions and Artificial Intelligence (AI) services that allow users to automate most of their time-consuming, repetitive

tasks. The aim of the intelligent automation oﬀerings is to enable employees to focus more on advanced tasks while more basic or

repetitive tasks can be automatically fulfilled by the respective bots.

Key Benefits

Reduce time-consuming, manual activities by using ready-to-use automation bots and processes that support error-free,

scalable tasks and help users focus on high-value processes.

Bring a new level of operational speed and eﬃciency to respond to customer needs proactively and augment resources to

address more high-value tasks.

Optimize business processes and workflows for maximum eﬃciency and take advantage of intelligent automations to make

more intelligent decisions.

In the interactive graphics below, you can hover over each area for short description and choose the highlighted areas for more

information.

Please note that image maps are not interactive in PDF outputs.

What Is SAP Build Process Automation?

SAP Build Process Automation combines capabilities from SAP Workflow Management and SAP Intelligent Robotic Process

Automation (RPA) with a powerful, yet intuitive no-code development experience. The solution allows business users to adapt,

improve, and innovate business processes using an intuitive graphical interface. SAP Build Process Automation also oﬀers prebuilt

content and features, such as bots, process steps, business rules, and workflow components.

Adapt, Improve, and Innovate Business Processes

Oﬀering an intuitive no-code approach, SAP Build Process Automation empowers users with domain expertise to build process

automations on top of SAP Business One. The solution also allows users to use prebuilt capabilities and predeveloped content,

reuse existing processes and scenarios, and modify processes to meet changing business requirements.

Automate Repetitive Work

SAP Build Process Automation also includes embedded RPA capabilities that help users readily enhance process flows with task

automation using RPA bots. The RPA capabilities automate repetitive manual tasks by mimicking user interactions with the

This is custom documentation. For more information, please visit SAP Help Portal.

2

6/8/26, 6:13 AM

system. These features help users accelerate task processing and reduce error rates.

Support Automation with Workflows

The workflow management capabilities of SAP Build Process Automation help business users digitalize workflows, orchestrate or

extend structured processes tailored to business needs, and use business rules to automate and adapt decision logic.

Simplify Process Automation

With the click of a button, users can combine and reuse a range of capabilities, including bots, workflow components, process

steps, and actions. The process builder and form builder oﬀer drag-and-drop functionality that simplifies the eﬀort needed to

create new automated processes or revise existing processes.

Add the Value of Artificial Intelligence (AI) to Business Process Automation

SAP Build Process Automation also supports document information and extraction using bot automations. Users can classify and

route business documents to the right process, extract data from various sources, and create appropriate records.

For more information, see What is SAP Build Process Automation? in the application help for SAP Build Process Automation on

SAP Help Portal.

How to Set Up the Best Practices for Process Automation for
SAP Business One

Access the full power of intelligent automation with SAP Build Process Automation as part of SAP Business One.

The best practices for process automation for SAP Business One oﬀer the following capabilities:

Create robotic process automation bots or use prebuilt bots to automate repetitive manual processes.

Access artificial intelligence (AI) capabilities for business process automation, such as Intelligent Document Processing

Build or adapt processes with an intuitive graphical interface.

Automate repetitive tasks within existing process flows using robotic process automation.

Create forms to manage and configure workflows using drag-and-drop functionality.

Work eﬃciently from a unified launchpad and task center.

To get you started with setting up the best practices for process automation in SAP Business One, see the following topics:

Setting Up Windows Generic Credentials

Configuring and Orchestrating SAP Build Process Automation

Setting Up and Deploying Best Practices Automation Projects in SAP Build Process Automation

Support Components

Useful Links

  Remember

This is custom documentation. For more information, please visit SAP Help Portal.

3

6/8/26, 6:13 AM

Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template projects to use

the Windows Credential Manager for storing users and passwords for the automations (regardless of whether the automation

is using the front end or back end); however, you can adapt the project to use other similar secure storage systems. Also,

regardless of whether the automation is designed to use the front-end UI or back-end services, we highly recommend that you

create individual technical users (communication arrangement) for each “automation + business user / business scenario”

pair. This enables you to distinguish whether the action was carried out by a physical business user or by an automation, and to

achieve full traceability of automations and human actions individually. As per any other best practices, the user must not

share their credentials with anyone else.

Setting Up Windows Generic Credentials

When running SAP Build Process Automation bots designed for SAP Business One, some bots need user authentication details.

The Windows Credential Manager can be used to keep the secure data at user convenience.

Procedure

1. On your Windows desktop, search for the Credential Manager and open it.

2. In the Manage your credentials window, click Windows Credentials.

3. In the Generic Credentials area, click the Add a generic credential option.

4. In the Internet or network address field, enter a name of your choice to identify this credential (for example,

B1Bot_Credential).

  Note
The name that you enter in Internet or network address field is used as the credentials identifier to access the bot

project template. When setting up the bot in SAP Build Process Automation, you need to enter the name of the

credentials identifier as an input parameter in the B1CredentialEntryName (or B1CredEntryName) field.

5. Enter your user name and password for SAP Business One. The specified credentials are relevant for the system connected

to the bot.

6. Choose OK.

You can check that your credentials are visible in the Generic Credentials list in the Credential Manager.

Watch this video on how to set up Windows credentials for user authentication to SAP Business One when using SAP Build Process

Automation.

This is custom documentation. For more information, please visit SAP Help Portal.

4

6/8/26, 6:13 AM

Open this video in a new window

  Remember

Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template projects to use

the Windows Credential Manager for storing users and passwords for the automations (regardless of whether the automation

is using the front end or back end); however, you can adapt the project to use other similar secure storage systems. Also,

regardless of whether the automation is designed to use the front-end UI or back-end services, we highly recommend that you

create individual technical users (communication arrangement) for each “automation + business user / business scenario”

pair. This enables you to distinguish whether the action was carried out by a physical business user or by an automation, and to

achieve full traceability of automations and human actions individually. As per any other best practices, the user must not

share their credentials with anyone else.

Configuring and Orchestrating SAP Build Process Automation

SAP Build Process Automation oﬀers a low-code and a no-code approach enabling users to design bots, build workflows, and

automate tasks and decisions.

With a no-code approach, users are guided through an intuitive interface with a simple workflow design. The simple-to-use

bot building capabilities oﬀered in SAP Build Process Automation allow expert developers as well as business users to build

and edit cloud projects without writing a line of code.

With a low-code approach, developers and business users can build and run their application bots with their Javascript

hand-coding knowledge.

For more information on subscribing to SAP Build Process Automation, configuring the SAP Launchpad Service, and configuring

the automation capabilities, see Initial Setup in the application help for SAP Build Process Automation on SAP Help Portal (EN

only).

For more information on working with SAP Build Process Automation, such as the Lobby, Store, Monitoring, and Settings, see Use

SAP Build Process Automation in the application help for SAP Build Process Automation on SAP Help Portal (EN only).

Related Information

Authorizations in SAP Build Process Automation

Configuring the SMTP E-Mail Destination

Setting Up a Service Key

Authorizations in SAP Build Process Automation

Authorizations in SAP Build Process Automation are granted by assigning users to role collections. You assign users to role

collections in the SAP BTP Cockpit of the SAP Business Technology Platform (SAP BTP).

This is custom documentation. For more information, please visit SAP Help Portal.

5

6/8/26, 6:13 AM

Automation Type

Role Collection

Description

Automation bots

ProcessParticipant

Performs actions during a user task or a

process implementation.

Process automations

ProcessAutomationParticipant

Is an approver or form step assignee, can

also contribute to runtime.

Permission to view tasks in My Inbox, where

the user assigned to this role is a recipient.

Permission to perform task operations

(claim, release, call the task completion

API).

  Note

You can also run automation bots with the ProcessAutomationParticipant role collection.

For more information, see Authorizations in the application help for SAP Build Process Automation on SAP Help Portal.

Related Information

Assigning Users to a Role Collection

Assigning Users to a Role Collection

Prerequisites

You have administration rights in the subaccount or global account.

The user that you want to assign to a role collection is defined as a user in the subaccount that has a subscription to SAP

Build Process Automation.

Context

This topic describes how to add users to a role collection in the SAP BTP Cockpit of the SAP Business Technology Platform (SAP

BTP).

Procedure

1. In the SAP BTP Cockpit of the SAP Business Technology Platform (SAP BTP), navigate to your subaccount.

2. Choose  Security

  Users .

3. Enter the user ID of the user that you want to assign to a role collection.

4. Select the row for the user.

5. In the Role Collections area on the right side of the screen, select the role collection that you want to assign to the user.

6. Choose the Assign Role Collection button.

Results

The user is assigned to the role collection and has all the authorizations of the role collection.

This is custom documentation. For more information, please visit SAP Help Portal.

6

6/8/26, 6:13 AM

For more information, see Assigning Role Collections to Users or User Groups under Administration in the SAP Business

Technology Platform (SAP BTP) product page on SAP Help Portal.

Watch this video on how to assign users to a role collection in SAP BTP.

Open this video in a new window

Configuring the SMTP E-Mail Destination

To send e-mail notifications on status changes in active business process projects, you need to configure an SAP BTP e-mail server

for e-mail notifications.

Prerequisites

You have the required SAP BTP roles for your subaccount.

Context

This topic describes how to configure an SAP BTP e-mail destination for SAP Build Process Automation.

Procedure

1. In SAP Build Process Automation, choose the Settings tab.

2. In the left panel, choose  Backend Configuration

  Mail Server

.

3. In the Configure mail server screen, choose the Open in BTP Cockpit button.

4. Choose the New Destination button.

5. In the Destination Configuration area, specify the following fields:

a. Name: Enter “sap_process_automation_email”.

b. Type: From the dropdown list, choose MAIL.

c. Description: Enter an optional description.

This is custom documentation. For more information, please visit SAP Help Portal.

7

6/8/26, 6:13 AM

d. Authentication: From the dropdown list, choose BasicAuthentication.

e. User: Enter the user for logging into the e-mail server.

f. Password: Enter the password for logging into the e-mail server.

6. In the Additional Properties area, choose the New Property button and specify the following properties:

Property Key

mail.bpm.send.disabled

mail.smtp.auth

Value

false

true

mail.smtp.from

<your e-mail address>

mail.smtp.host

<SMTP server address of your e-mail client>

mail.smtp.port

<Enter the port on which your e-mail server listens for connections

(typically 587 or 465 in rare cases)>

mail.smtp.ssl.enable

mail.smtp.starttls.enable

mail.smtp.starttls. required

mail.ssl.checkserveridentity

mail.transport.protocol

false

true

true

true

smtp

7. Choose the Save button.

Results

The e-mail destination is displayed on the Configure mail server screen ( Backend Configuration
Process Automation. E-mails can now be successfully received by the recipient.

  Mail Server

) in SAP Build

Watch this video on how to configure the e-mail destination for SAP Build Process Automation.

This is custom documentation. For more information, please visit SAP Help Portal.

8

6/8/26, 6:13 AM

Open this video in a new window

Setting Up a Service Key

To use the API call to trigger an automation, you need a service instance with a service key in your subaccount in SAP Business

Technology Platform (SAP BTP). The service key provides the credentials needed to authenticate to the API and start an instance

of the automation.

Prerequisites

Context

This topic describes how to create a service key for an instance in SAP BTP.

Procedure

1. In your subaccount for the SAP BTP Cockpit, choose  Services

  Instances and Subscriptions .

2. In the Instances area, check if a service instance for SAP Build Process Automation already exists. If a service instance

does not exist, choose the Create button to create a new service instance.

3. On the row for your instance, check the Credentials field to identify if a service key exists. If a service key is not available,

click Details and choose the Create Service Key option.

4. In the New Service Key dialog box, enter a name for your service key and choose the Create button.

5. Locate your newly create service key, click  More actions , and then choose the View option.

6. Copy the following information from the service key:

a. Clientid (client ID)

b. Clientsecret (client secret)

c. uaa URL (token service URL)

d. endpoints API URL

Results

The service key is created and is available to view in your SAP BTP subaccount. Entities outside your deployment can now access
your service with this key.

Watch this video on how to create a service key for an instance in SAP BTP.

This is custom documentation. For more information, please visit SAP Help Portal.

9

6/8/26, 6:13 AM

Open this video in a new window

Setting Up and Deploying Best Practices Automation Projects in
SAP Build Process Automation

Context

The topics in this section guide you through the steps of using SAP Build Process Automation to set up and deploy the best

practices process automation templates for SAP Business One. The setup requirements depend on whether you are working with

automation bots or processes automations; for more information, see the topic for your automation type: Automation Bots or

Business Process Automations.

Related Information

Acquiring a Project Template from the Store

Deploying an Automation Project and Adding a Scheduled Trigger

Adding an API Trigger

Deploying an Automation Project Without a Trigger

Registering and Adding an Agent

Adding Alert Handlers

Acquiring a Project Template from the Store

Prerequisites

You have a subscription to SAP Build Process Automation. For more information, see Subscribe to SAP Build Process

Automation in the application help for SAP Build Process Automation on SAP Help Portal (EN only).

Context

This topic describes how to acquire a best practice project template for SAP Business One from the Store in SAP Build Process

Automation.

Procedure

1. In SAP Build Process Automation, click the Store tab.

2. To limit the projects displayed toSAP Business One, click the Publisher filter in the left panel and select the checkbox for

SAP Business One.

3. On the project tile for the selected project, choose the More information button to view the details of the project. In the

Documents area, you can find and download the technical specification and other documentation available for the project
(for example, configuration files for automation bots).

4. Choose the Add button to retrieve the project.

This is custom documentation. For more information, please visit SAP Help Portal.

10

6/8/26, 6:13 AM

5. The project Overview page is displayed. The status of the project is changed to Released.

Results

The project is successfully released and ready for deployment. After adding a project, the project is displayed in the Lobby. You can
navigate to the Lobby tab to access the project at any time.

Watch this video on how to acquire a best practice project template for SAP Business One from the Store in SAP Build Process

Automation.

Open this video in a new window

Related Information

Deploying an Automation Project and Adding a Scheduled Trigger

Deploying an Automation Project Without a Trigger

Deploying an Automation Project and Adding a Scheduled Trigger

Prerequisites

You have acquired a project template from the Store and released your project.

Context

After adding the project, you are ready to deploy the project and add a scheduled trigger to the automation project. A trigger is a

rule that defines the execution of an automation project by an agent. A scheduled trigger creates jobs based on the schedule you

define in the trigger.

Procedure

1. In the Lobby of SAP Build Process Automation, select the automation project that you want to deploy.

This is custom documentation. For more information, please visit SAP Help Portal.

11

6/8/26, 6:13 AM

2. On the Overview page for the project, choose the Deploy button.

3. The Deploy a project wizard is displayed. In the Variables screen, select the Create a Trigger radio button and choose the

Next button.

4. In the Trigger Type screen, select the type of trigger you want to add (API or scheduled), and choose the Next button.

5. To configure an API or a scheduled trigger, select the relevant automation, and choose the Next button.

6. In the Configuration screen, enter a name for your trigger and define the scheduling of the trigger, including the date range,

time zone, and times when the automation is to run. Choose the Next button.

7. Optional: In the Advanced Settings screen, in the Attributes area, you can add agent attributes that define which agents

the job is distributed to.

8. In the Input parameters area, enter the input parameters required for the automation.

9. Choose the Confirm button.

Results

Your project and scheduled trigger are now deployed.

Watch this video on how to deploy an automation project and add a scheduled trigger.

Open this video in a new window

Related Information

Registering and Adding an Agent

Deploying an Automation Project Without a Trigger

You can deploy a project before adding a trigger. In this case, your project will be ready for use later. For instance, you can deploy a

project without a trigger to test your project before an external API call is available.

Prerequisites

This is custom documentation. For more information, please visit SAP Help Portal.

12

6/8/26, 6:13 AM

You have acquired a project from the Store and released your project.

Context

This topic describes how to deploy a project without adding a trigger to start it.

Procedure

1. In the Lobby of SAP Build Process Automation, select the automation project that you want to deploy.

2. On the Overview page for the project, choose the Deploy button.

3. The Deploy a project wizard is displayed. In the Variables screen, select the No trigger creation radio button and choose

the Next button.

4. If applicable, enter the environmental variables required to run the project.

5. Choose the Confirm button.

6. Choose the Deploy button.

Results

Your project is now listed as deployed in your projects list.

Related Information

Adding an API Trigger

Adding an API Trigger

An API trigger opens a dedicated endpoint that allows an external application to start the automation in a specified deployed

project using an HTTP POST call.

Prerequisites

You have released your project.

You have set up a service key. For more information, see Setting Up a Service Key.

Context

This topic describes how to add an API trigger after a project has been deployed.

Procedure

1. In SAP Build Process Automation, choose the Monitor tab.

2. Choose Manage in the left panel and the choose Automations.

3. Choose the Add Trigger button.

4. In the Create Trigger dialog, select the automation from the list and choose the Next button.

5. Select the API radio button as the trigger type.

6. Choose a name and enter an optional description for your trigger.

This is custom documentation. For more information, please visit SAP Help Portal.

13

6/8/26, 6:13 AM

7. Select the priority for the trigger.

8. Select the expiration time of jobs created by the trigger in minutes, hours, days, or weeks (Jobs expire after), and then

choose Next.

The maximum expiration time is 30 days or 4 weeks. Once the expiration time is passed, the trigger appears in Expired

status.

9. Define the Agent Attributes that will define which agents the job is distributed to.

10. Choose the Confirm button, and then choose the Deploy button.

Results

An external API trigger can now start the implementation of an automation in your project.

Registering and Adding an Agent

Prerequisites

You have deployed the project.

You have installed the Desktop Agent on your local machine. For more information, see Install Desktop Agent and Manage

Updates in the application help for SAP Build Process Automation on SAP Help Portal (EN only).

Context

After deploying a project, you need to register the Desktop Agent and add the agent to SAP Build Process Automation. This

process enables SAP Build Process Automation to distribute projects and jobs to the agent.

Procedure

1. In SAP Build Process Automation, choose the Settings tab.

2. On the top-right side of the Agents screen, choose the Register new agent… button.

3. In the Register new agent pop-up window, choose the Copy and Close button. You will need the link for the Desktop Agent

connection in a later step.

4. In your taskbar, click the Desktop Agent icon.

5. In the Desktop Agent pop-up window, click  More actions, and choose the Tenants button.

6. To add the tenant, choose the Add button.

7. Enter the name of the tenant and paste the URL you copied in Step 3. Choose the Save button.

8. After the tenant validation is complete, choose the Activate button.

9. In the message box, choose the OK button.

10. If you are using SAP ID Service with two-factor authentication, in the Two-Factor Authentication window, provide your user

name and password. Otherwise, enter the e-mail address and password you used for registration.

11. In the left panel, click Agents Management.

12. On the top-right side of the Agents Management screen, choose the + Add Agent button.

13. In the Add agent pop-up window, select your agent in the Agents list and choose the Add Agent button.

Results

This is custom documentation. For more information, please visit SAP Help Portal.

14

6/8/26, 6:13 AM

Your agent is successfully added to SAP Build Process Automation. On the Settings tab, your agent is now registered in the Agents
List.

Watch this video on how to register the Desktop Agent and add the agent to SAP Build Process Automation.

Open this video in a new window

Adding Alert Handlers

Alert handlers enable SAP Build Process Automation to send e-mails for alerts employed in a deployed process.

Prerequisites

You have deployed the project that contains alerts.

You have configured an e-mail server destination. For more information, see Configuring the SMTP E-Mail Destination.

Context

This topic describes how to create an alert handler to use the alerts in your project.

Procedure

1. In SAP Build Process Automation, choose the Settings tab.

2. In the left panel, choose Alert Handlers.

3. Choose the Add Alert Handler button.

4. In the Select Event dialog box, select the alert for which an e-mail is to be sent when raised in the automation.

5. In the Enter Properties dialog box, enter a name for the alert handler in the Name field.

6. In the Description field, enter a description for the alert handler.

7. Choose the Next button.

8. In the Add Details dialog, enter the e-mail address of the recipient in the Recipients field.

This is custom documentation. For more information, please visit SAP Help Portal.

15

6/8/26, 6:13 AM

The Recipients field can have multiple addresses. You can also provide the e-mail addresses using an alert parameter, for

example, ${alert.parameters.recipients}.

9. Enter the subject of the e-mail in the Subject field.

10. Enter the content of the e-mail in the Content field.

In the content body, you can select and insert variables from the alert parameters available in the automation. To do so,

click the respective alert parameter above the content body (for example, context, automation, event, alert) and

choose a variable in the dropdown list.

11. Choose the Add button.

Results

The created alert handler will be triggered whenever the selected event is raised from an automation in the corresponding project.

Watch this video on how to add alert handlers in SAP Build Process Automation.

Open this video in a new window

Support Components

If you need to create a support ticket, you can use the following components:

SBO-INT-PA: for all issues related to using the the standard (non-customized) process automation templates for SAP

Business One.

For issues related to SAP Build Process Automation, including issues during installation or with the functionalities of the

solution, use the support components listed in Troubleshooting and Monitoring in the application help for SAP Build

Process Automation.

Useful Links

This is custom documentation. For more information, please visit SAP Help Portal.

16

6/8/26, 6:13 AM
SAP Build Process Automation

SAP Build Process Automation on SAP Help Portal

Explore the Store

SAP Business Accelerator Hub

 - SAP Build Content Catalog

Composing and automating with SAP Build the No-Code Way

 - SAP Learning Journey

Creating Processes and Automations with SAP Build Process Automation

 - SAP Learning Journey

Intelligent Automation for SAP Business One

Intelligent Automation for SAP Business ByDesign and SAP Business One

 - openSAP course

Creating a Document Template in SAP Build Process Automation for Supplier Invoice Upload in SAP Business One

 -

openSAP Microlearning

Return Request Process Automation for SAP Business One

 - openSAP Microlearning

SAP AI Business Services and Document Information Extraction

SAP AI Services on SAP Help Portal

Use SAP AI Business Services to Kick-Start Your Intelligent Processes

 - openSAP course

Tutorials for Developers:

Use Machine Learning to Process Business Documents

Use Machine Learning to Extract Information from Documents with Swagger UI

AI Business Services (example for Document Information Extraction)

SAP Business Technology Platform

SAP Business Technology Platform (SAP BTP) on SAP Help Portal

How to Work with Best Practices for Process Automation for SAP
Business One

During their daily work, users need to handle many small, monotonous, administrative tasks that are time-consuming. Documents

such as invoices, purchase orders, and proof of delivery notes are sent to the Inbox. The user then needs to open the document,

read it, and manually enter the data into the ERP system.

But what if users don't have to complete all these tasks themselves? The best practices for process automation for SAP Business

One give you access to automation bots and processes that replace manual clicks, interpret text-heavy communications, and

automate other tedious business processes. You can use the automations out of the box or adapt them to your needs.

For more information, see the relevant topic for each automation.

Related Information

Automation Bots

This is custom documentation. For more information, please visit SAP Help Portal.

17

6/8/26, 6:13 AM

Business Process Automations

Automation Bots

SAP Build Process Automation gives you access to software bots that are designed to mimic humans by automating manual,

repetitive tasks such as retrieving data from a spreadsheet or submitting information to a database. The unattended bots for SAP

Business One run automatically without any human intervention.

The following best practices template bots are available for SAP Business One in the SAP Business Accelerator Hub

:

Business Document Extraction from E-Mail

Supplier Invoice Upload for Intelligent Invoice Scanning

Proof of Delivery Note Upload in the Outbound Delivery and the Invoice

Sales Order Creation from a Local Purchase Order

Master Data Enrichment for Business Partner Identification

Activity Creation for Business Partners

To set up template bot projects for SAP Business One, see the following topics:

Acquiring a Project Template from the Store

Deploying an Automation Project and Adding a Scheduled Trigger

Registering and Adding an Agent

Business Document Extraction from E-Mail

This bot automatically scans relevant e-mails in your Outlook Inbox, downloads the attachments in those e-mails, and categorizes

them based on the document type and company code. This automation reduces user eﬀort and sets the stage for further process

automation.

You can find the Business Document Extraction from E-Mail project template in the SAP Business Accelerator Hub

.

Business Case

Problem

Companies receive many business documents through e-mail from vendors and customers, such as local purchase orders, signed

proof of deliveries, and payment advice. Users typically need to scan through their e-mails, download the documents, and

categorize them based on the document type and the company code before creating relevant objects in SAP Business One. This

manual process takes a significant amount of the user's daily time.

Solution

The Business Document Extraction from E-Mail bot automatically scans relevant e-mails, downloads the attachments, and

categorizes them based on the document type and company code. This automation reduces users eﬀort and sets the stage for

further intelligent business process automation.

This is custom documentation. For more information, please visit SAP Help Portal.

18

6/8/26, 6:13 AM

  Note

This bot is designed to be the first automation in the end-to-end automation processes, which works in conjunction with the

following best practices for process automation project templates for SAP Business One:

Sales Order Creation from a Local Purchase Order

Supplier Invoice Upload for Intelligent Invoice Scanning

Proof of Delivery Note Upload in the Outbound Delivery and the Invoice

Business Benefit

Reduces user eﬀort

Reduces the risk of manual errors

Improves work eﬃciency

Technical Specification

Content and Strategic Intent

Downloading various business documents from e-mails and placing them into corresponding folders is a manually intensive, time-

consuming, and error-prone process. By automating this process using the Business Document Extraction from E-mail bot, these

drawbacks are avoided, valuable employee time is freed up, and error rates are reduced.

The Business Document Extraction from E-mail bot can be used as a standalone bot. However, if you are using other best

practices process automation bots for SAP Business One that require business documents to be manually placed in a specific

folder for the bot, we recommend using the Business Document Extraction from E-mail bot as the first part of the end-to-end

automation scenario. This can reduce the manual eﬀort required when using the following bots:

Supplier Invoice Upload for Intelligent Invoice Scanning

Proof of Delivery Note Upload in the Outbound Delivery and the Invoice

Sales Order Creation from a Local Purchase Order

Watch this video about the setup and use of the Business Document Extraction from E-mail bot.

This is custom documentation. For more information, please visit SAP Help Portal.

19

6/8/26, 6:13 AM

Open this video in a new window

Technical Details

Overview

This bot can be set up in unattended mode using SAP Build Process Automation.

Type

Attended

Unattended

Screen Scraping

No

Yes

No

For information on how to set up the bot in SAP Build Process Automation, see Automation Bots.

Input/Output

Before executing the bot, a local root folder must be created that will be used by the bot to create a log folder to store the log files

and a folder structure to store the business documents downloaded from e-mails. If this bot is working with other bots in an end-

to-end automation process, all bots need to use the same local root folder.

You have downloaded the configuration Excel file available in the Documents section of the project template and placed it in the

local root folder. In the configuration file, you have specified the "Business Object" and "Company Code" values. The "Company

Code" can be an arbitrary value (consisting of numbers, letters, or both) to identify the company, or the branch identification

number if you are using branches for the SAP Business One company. For the remaining columns, you have specified the rules on

each row for filtering e-mails in the user’s Outlook Inbox. The bot creates a folder in the root folder for each row you have specified.

The name of the configuration file must be specified in SAP Build Process Automation as the variable “configExcelFilename”.

  Note

If the bot is working with other bots, use the same configuration file for all the bots (except for the bot-specific files for Activity

Creation for Business Partners), with the business object and company codes specified for each bot.

In the user’s Outlook account, you have created a subfolder (for example, “Processed”) in the Inbox to be used by the bot.

The bot automatically creates a root folder structure so that the folder for each business object contains three subfolders for each

company code: “Failed”, “Processed” and “ToBeProcessed”. Downloaded files from e-mails are placed by the bot in the local

“ToBeProcessed” folder. If the files are later used by other bots, the files are moved to the “Processed” folder by the particular bot

if the automation of the file was successful, or to the “Failed” folder if the automation of the files was unsuccessful. Similarly,

Outlook e-mails with successfully downloaded attachment files are moved to the subfolder in the user’s Inbox that you created for

this purpose (for example, “Processed”).

After running the bot, you can find the log files for the bot in the "Logs" folder.

Constraints

The bot can only download .PNG, .JPG, .PDF and .TIFF file formats from e-mails.

This is custom documentation. For more information, please visit SAP Help Portal.

20

6/8/26, 6:13 AM

This bot can only work on the Microsoft Windows operating system.

Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember
Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Supplier Invoice Upload for Intelligent Invoice Scanning

This bot fetches the invoice documents from the specified folder and uploads them to the Document Information Extraction

service (SAP AI Business Services), which scans and extracts the information from the documents. The extracted information is

passed to SAP Business One using the Open Data Protocol to create a record in the SAP Business One database. From this point

on, you can use the Electronic Document Import Wizard functionality in SAP Business One to import the documents and generate

a draft invoice.

You can find the Supplier Invoice Upload for Intelligent Invoice Scanning project template in the SAP Business Accelerator Hub

.

Business Case

Problem

The supplier invoice is a common document received by companies. A user in the procurement department typically needs to

enter or copy and paste the details from the documents to the system. This manual process is not only time-consuming but also

prone to errors such as incorrect or missing information.

Solution

The Supplier Invoice Upload for Intelligent Invoice Scanning bot automates the process of uploading supplier invoices to the

Document Information Extraction service, which scans and extracts the information from the documents. The extracted

This is custom documentation. For more information, please visit SAP Help Portal.

21

6/8/26, 6:13 AM

information is passed by the bot to SAP Business One using the Open Data Protocol to create a record in the SAP Business One

database. From this point on, you can use the Electronic Document Import Wizard functionality in SAP Business One to import the

documents and generate a draft invoice.

  Note

The Document Information Extraction service license is part of the SAP Build Process Automation license. If an SAP Business

One customer already uses intelligent automation for their business, this bot makes it possible to consume the Intelligent

Invoice Scanning functionality available in SAP Business One at no extra costs.

Business Benefit

Reduces user eﬀort

Reduces the risk of manual errors

Improves work eﬃciency and business flexibility

Technical Specification

Content and Strategic Intent

Uploading invoice documents to the SAP Business One is a manually intensive, time-consuming, and error-prone process. It adds

unnecessary manual eﬀort and poses potential risks to the business. By automating this process using the Supplier Invoice

Upload for Intelligent Invoice Scanning bot, these drawbacks are avoided, valuable employee time is freed up, and error rates are

reduced.

Watch this video about the setup and use of the Supplier Invoice Upload for Intelligent Invoice Scanning bot.

Open this video in a new window

Technical Details

This is custom documentation. For more information, please visit SAP Help Portal.

22

6/8/26, 6:13 AM

Overview

This bot can be set up in unattended mode using SAP Build Process Automation.

Type

Attended

Unattended

Screen Scraping

No

Yes

No

For information on how to set up the bot in SAP Build Process Automation, see see Automation Bots.

Input/Output

As a prerequisite for running of this bot, in SAP Business One, in  Administration

  System Initialization

  Document Settings

, on the Electronic Documents tab, you have activated the Document Information Extraction protocol.

Before running the bot, you have created a local root folder that will be used by the bot to create a log folder and to store the

business documents in a categorized folder structure. If this bot is working with other bots in an end-to-end automation process,

all bots need to use the same local root folder.

You have downloaded the configuration Excel file available in the Documents section of the project template and placed it in the

local root folder. In the configuration file, you have specified the "Business Object" ("Invoice") and "Company Code" values. The

"Company Code" can be an arbitrary value (consisting of numbers, letters, or both) to identify the company, or the branch

identification number if you are using branches for the SAP Business One company. If you are using the Business Document

Extraction from E-mail bot, you have specified e-mail filter rules for each row in the remaining columns. The bot creates a folder in

the root folder for each row you have specified. The name of the configuration file must be specified in SAP Build Process

Automation as the variable “configExcelFilename”.

  Note

If the bot is working with other bots, use the same configuration file for all the bots (except for the bot-specific files for Activity

Creation for Business Partners), with the business object and company codes specified for each bot.

If you are using the Supplier Invoice Upload for Intelligent Invoice Scanning bot as a standalone bot, you need to manually create

the required root folder structure. In the "Invoice" folder, each folder you create corresponding to a company code needs to

contain three subfolders: “Failed”, “Processed”, and “ToBeProcessed”. If you are using the Business Document Extraction from E-

mail bot, the bot automatically creates the required folder structure (ensure that you are using the same configuration file for both

of the bots).

Supplier invoices that you want the bot to process need to be placed in the local “ToBeProcessed” folder. If you are using the

Business Document Extraction from E-mail bot, relevant files downloaded from e-mails are automatically placed by the bot in the

“ToBeProcessed” local folder.

The invoice is sent by the bot to SAP Business One using the Open Data Protocol to create a record in the SAP Business One

database. From this point on, you can use the Electronic Document Import Wizard functionality in SAP Business One to import the

documents and generate a draft invoice. Successfully processed invoices are moved by the bot to the “Processed” folder.

After running the bot, you can find the log files for the bot in the "Logs" folder.

Constraints

This bot can only work on the Microsoft Windows operating system.

This is custom documentation. For more information, please visit SAP Help Portal.

23

6/8/26, 6:13 AM
Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember
Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Proof of Delivery Note Upload in the Outbound Delivery and the
Invoice

This bot reads proof of delivery notes from customers, extracts the delivery note number, and uploads the proof of delivery as an

attachment to the outbound delivery and the invoice that corresponds to the relevant delivery note number.

You can find the Proof of Delivery Note Upload in the Outbound Delivery and the Invoice project template in the SAP Business

Accelerator Hub

.

Business Case

Problem

A proof of delivery (POD) note is an acknowledgment from customers that goods or services have been received or completed,

and that the customer can be billed for the goods or services. Typically, an electronic POD is sent to the company as a scan

through e-mail. Business users need to download the PODs and manually upload them to each outbound delivery or invoice in SAP

Business One. This manual process takes a significant amount of time and can be prone to errors.

Solution

The Proof of Delivery Note Upload in the Outbound Delivery and the Invoice bot sends a POD file to the Document Information

Extraction service (SAP AI Business Services) to scan it and identify the delivery note number. Based on this information, the bot

connects to SAP Business One using the Open Data Protocol and uploads the file to the relevant delivery note. If a linked invoice is

also identified, the bot replicates the POD to the invoice as well.

This is custom documentation. For more information, please visit SAP Help Portal.

24

6/8/26, 6:13 AM

  Note

This bot can be used as a stand-alone bot or it can work with the Business Document Extraction from E-mail bot, which

downloads files from e-mails and places them in an automatically created folder structure. In this scenario, the Proof of

Delivery Note Upload in the Outbound Delivery and the Invoice bot works in the second part in the end-to-end automation

process.

Business Benefits

Reduces repetitive tasks

Improves work eﬃciency

Reduces the risk of manual errors

Technical Specification

Content and Strategic Intent

Extracting information from proof of delivery notes from customer e-mails and attaching the documents to delivery notes is a

manually intensive, time-consuming, and error-prone process. The Proof of Delivery Note Upload to the Outbound Delivery and

the Invoice bot uses the Document Information Extraction service (SAP AI Business Services) to extract the delivery note number

and attach the proof of delivery note to the delivery note and the related invoice.

Watch this video about the setup and use of the Proof of Delivery Note Upload to the Outbound Delivery and the Invoice bot.

Open this video in a new window

Technical Details

Overview

This is custom documentation. For more information, please visit SAP Help Portal.

25

6/8/26, 6:13 AM

This bot can be set up in unattended mode using SAP Build Process Automation.

Type

Attended

Unattended

Screen Scraping

No

Yes

No

For information on how to set up the bot in SAP Build Process Automation, see Automation Bots.

Input/Output

Before running the bot, you have created a local root folder that will be used by the bot to create a log folder and to store the

business documents in a categorized folder structure. If this bot is working with other bots in an end-to-end automation process,

all bots need to use same the local root folder.

You have downloaded the configuration Excel file available in the Documents section of the project template and placed it in the

local root folder. In the configuration file, you have specified the "Business Object" ("Proof of Delivery") and "Company Code"

values. The "Company Code" can be an arbitrary value (consisting of numbers, letters, or both) to identify the company, or the

branch identification number if you are using branches for the SAP Business One company. If you are using the Business

Document Extraction from E-mail bot, you have specified e-mail filter rules for each row in the remaining columns. The bot

creates a folder in the root folder for each row you have specified. The name of the configuration file must be specified in SAP Build

Process Automation as the variable “configExcelFilename”.

  Note

If the bot is working with other bots, use the same configuration file for all the bots (except for the bot-specific files for Activity

Creation for Business Partners), with the business object and company codes specified for each bot.

If you are using the Proof of Delivery Note Upload in the Outbound Delivery and the Invoice bot as a standalone bot, you need to

manually create the required root folder structure. In the "Proof of Delivery" folder, each folder you create corresponding to a

company code needs to contain three subfolders: “Failed”, “Processed”, and “ToBeProcessed”. If you are using the Business

Document Extraction from E-mail bot, the bot automatically creates the required folder structure (ensure that you are using the

same configuration file for both of the bots).

Proof of deliveries that you want the bot to process need to be placed in the local “ToBeProcessed” folder. If you are using the

Business Document Extraction from E-mail bot, relevant files downloaded from e-mails are automatically placed by the bot in the

“ToBeProcessed” local folder.

Proof of deliveries received for a company are uploaded to the relevant delivery note and A/R invoice in SAP Business One.

Successfully processed proof of deliveries are moved to the “Processed” folder, and failed proof of deliveries are moved to the

“Failed” folder in the local or shared folder.

After running the bot, you can find the log files for the bot in the “Logs” folder.

Constraints

This bot can only work on the Microsoft Windows operating system.

Security

Protecting User Credentials

This is custom documentation. For more information, please visit SAP Help Portal.

26

6/8/26, 6:13 AM

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember
Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Sales Order Creation from a Local Purchase Order

This bot automates the process of creating a sales order from a local purchase order received from customers.

You can find the Sales Order Creation from a Local Purchase Order project template in the SAP Business Accelerator Hub

.

Business Case

Problem

Companies regularly receive purchase order documents from their customers. These external documents are referred by business

users to create sales orders in SAP Business One. Typically, a user enters or copies the details from the documents to the system.

This manual process is often prone to errors such as incorrect or missing information.

Solution

The Sales Order Creation from a Local Purchase Order bot sends a purchase order to the Document Information Extraction

service (SAP AI Business Services) to scan the information. The extracted details are passed by the bot to SAP Business One using

the Open Data Protocol to create a draft sales order and upload the document to the draft for business user review.

  Note
This bot can be used as a stand-alone bot or work with the Business Document Extraction from E-mail bot, which extracts

customer purchase orders from e-mails and places the files in an automatically created folder structure. To further automate

and improve the accuracy of the sales order creation, users can use the Master Data Enrichment for Business Partner

Identification bot, which helps the bot to identify the business partner code based on the scanned information such as the

business partner name, address, and bank account.

Business Benefits

This is custom documentation. For more information, please visit SAP Help Portal.

27

6/8/26, 6:13 AM

Reduces user eﬀort by automating repetitive tasks

Reduces the risk of manual errors, resulting in higher accuracy

Improves work eﬃciency

Technical Specification

Content and Strategic Intent

Automating the creation of sales orders based on purchase order documents from customers can save valuable employee time

and reduce error rates. The Sales Order Creation from a Local Purchase Order bot sends external purchase order documents to

the Document Information Extraction service (SAP AI Business Services) to scan the information and pass the details to SAP

Business One using the Open Data Protocol to create a draft sales order.

To further automate and improve the accuracy of the sales order creation, users can use the Master Data Enrichment for

Business Partner Identification bot, which helps the bot identify the business partner code based on the scanned information.

Watch this video about the setup and use of the Sales Order Creation from a Local Purchase Order bot.

Open this video in a new window

Technical Details

Overview

This bot can be set up in unattended mode using SAP Build Process Automation.

Attended

Unattended

Screen Scraping

No

Yes

No

For information on how to set up the bot in SAP Build Process Automation, see Automation Bots.

This is custom documentation. For more information, please visit SAP Help Portal.

28

6/8/26, 6:13 AM

Input/Output

Before running the bot, you have created a local root folder that will be used by the bot to create a log folder to store the log files

and a folder structure to store the business documents downloaded from e-mails. If this bot is working with other bots in an end-

to-end automation process, all bots need to use the same local root folder.

You have downloaded the two configuration Excel files available in the Documents section of the project template and placed them

in the local root folder. In the configuration file, you have specified the "Business Object" ("Purchase Order") and "Company Code"

values. The "Company Code" can be an arbitrary value (consisting of numbers, letters, or both) to identify the company, or the

branch identification number if you are using branches for the SAP Business One company. If you are using the Business

Document Extraction from E-mail bot, you have specified e-mail filter rules for each row in the remaining columns. The bot

creates a folder in the root folder for each row you have specified. The name of the configuration file must be specified in SAP Build

Process Automation as the variable “configExcelFilename”.

  Note

If the bot is working with other bots, use the same configuration file for all the bots (except for the bot-specific files for Activity

Creation for Business Partners), with the business object and company codes specified for each bot.

In the second, bot-specific configuration file, you have specified "Yes" or "No" to the three rules and entered a confidence score

(ranging from 0-1.0) as the criteria for the bot to filter out fields above the confidence value.

If you are using the Sales Order Creation from a Local Purchase Order bot as a standalone bot, you need to manually create the

required root folder structure. In the "Purchase Order" folder, each folder you create corresponding to a company code needs to

contain three subfolders: “Failed”, “Processed”, and “ToBeProcessed”. If you are using the Business Document Extraction from E-

mail bot, the bot automatically creates the required folder structure (ensure that you are using the same configuration file for both

of the bots).

Purchase orders that you want the bot to process need to be placed in the local “ToBeProcessed” folder. If you are using the

Business Document Extraction from E-mail bot, relevant files downloaded from e-mails are automatically placed by the bot in the

“ToBeProcessed” local folder.

The bot creates a draft sales order in SAP Business One and uploads the purchase orders received by the specified company to

the sales order. Successfully processed purchase orders are moved to the “Processed” folder, and failed sales orders are moved to

the “Failed” folder in the local or shared folder.

After running the bot, you can find the log files for the bot in the "Logs" folder.

Constraints

This bot only processes PDF files.

This bot can only work with the Microsoft Windows operating system.

Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember

Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

This is custom documentation. For more information, please visit SAP Help Portal.

29

6/8/26, 6:13 AM

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Master Data Enrichment for Business Partner Identification

This bot automates the process of enriching the data fields extracted by the Document Information Extraction service with

business partner master data.

You can find the Master Data Enrichment for Business Partner Identification project template in the SAP Business Accelerator

Hub

.

Business Case

Problem

As master data is subject to change, business users need to perform several manual steps on a regular basis to enrich the master

data extracted by the Document Information Extraction service. Enriching the Document Information Extraction service manually

requires multiple steps: creating a report in SAP Business One with specific columns, extracting the values, uploading them to the

Document Information Extraction service API, and activating the service.

Solution

The Master Data Enrichment for Business Partner Identification bot automates the manual steps required in updating the

Document Information Extraction service API whenever business partner master data is modified. The bot retrieves the business

partner list from SAP Business One, deletes the existing master data in the Document Information Extraction API, creates the

business entity, and activates the business partner master data for use by the Document Information Extraction service.

  Note
The bot is designed to work with the Sales Order Creation from Local Purchase Order bot in an end-to-end automation

process. When using the Sales Order Creation from Local Purchase Order bot, the Master Data Enrichment for Business

Partner Identification bot can further improve the accuracy of the sales order creation by helping to identify the business

partner code based on the business partner name, address, bank account, and other details scanned by the service from the

purchase order document.

Business Benefits

Reduces user eﬀort

This is custom documentation. For more information, please visit SAP Help Portal.

30

6/8/26, 6:13 AM

Reduces the risk of manual errors

Improves work eﬃciency

Technical Specification

Content and Strategic Intent

When extracting information from customer documents, the process of identifying the relevant business partner code depends on

the accuracy of the business partner master data in the Document Information Extraction service API. The Master Data

Enrichment for Business Partner Identification bot automates the process of enriching the data fields extracted by the

Document Information Extraction service with business partner master data.

This bot is designed to work with the Sales Order Creation from a Local Purchase Order bot. The Master Data Enrichment for

Business Partner Identification bot accesses the business partner master data in SAP Business One using the REST API. The bot

then uses the business partner master data to update the data fields extracted by the Document Information Extraction service in

the Sales Order Creation from a Local Purchase Order bot.

Watch this video about the setup and use of the Master Data Enrichment for Business Partner Identification bot.

Open this video in a new window

Technical Details

Overview

This bot can be set up in unattended mode using SAP Build Process Automation.

Attended

Unattended

Screen Scraping

No

Yes

No

This is custom documentation. For more information, please visit SAP Help Portal.

31

6/8/26, 6:13 AM

For information on how to set up the bot in SAP Build Process Automation, see Automation Bots.

Input/Output

Before running the bot, you have created a local root folder that will be used by the bot to create a log folder.

After running the bot, you can find the log files for the bot in the "Logs" folder.

Constraints

This bot can only work with the Microsoft Windows operating system.

Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember
Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Activity Creation for Business Partners

This bot creates activities for new business partner leads and automatically schedules a reminder for the follow-up of new leads in

the user’s Outlook calendar.

  Note

This bot is available to users of SAP Business One, Web client.

You can find the Activity Creation for Business Partners project template in the SAP Business Accelerator Hub

.

Business Case

This is custom documentation. For more information, please visit SAP Help Portal.

32

6/8/26, 6:13 AM
Problem

Company representatives meet new leads at events or during their daily work. Based on their meetings, business users create new

business partner leads in SAP Business One and manually schedule activities to follow up with the leads. This manual process is

time-consuming and is also often prone to error.

Solution

The Activity Creation for Business Partners bot, developed to run in unattended mode, automatically creates activities for new

business partner leads. The bot automatically schedules a reminder for the follow-up with new leads in the user’s Outlook

calendar. Users can schedule this bot to run depending on their specific requirements.

  Note

This bot is available to users of SAP Business One, Web client.

Business Benefits

Reduces user eﬀort

Reduces the risk of manual errors

Improves work eﬃciency

Technical Specification

Content and Strategic Intent

Following up on new business partner leads is a time-consuming activity that is prone to errors when performed manually. The

Activity Creation for Business Partners bot automates this process by creating activities for new business partner leads and

automatically scheduling a reminder for the follow-up of new leads in the user’s Outlook calendar.

  Note

This bot is available for users of SAP Business One, Web client.

Watch this video about the setup and use of the Activity Creation for Business Partners bot.

This is custom documentation. For more information, please visit SAP Help Portal.

33

6/8/26, 6:13 AM

Open this video in a new window

Technical Details

Overview

This bot can be set up in unattended mode using SAP Build Process Automation.

Attended

Unattended

Screen Scraping

No

Yes

Yes

For information on how to set up the bot in SAP Build Process Automation, see see Automation Bots.

Input/Output

As a prerequisite for running this bot, you have performed the following:

In the SAP Business One client, in  Business Partners

 Activity

, you have defined a new activity Subject (for example,

“Created by SPA bot”) (an activity Subject in SAP Business One corresponds to an activity Subcategory in Web client). The

bot requires a unique activity subcategory to avoid duplications in activities. The activity subject codes that are

automatically created by the system for the activity subject correspond to the values entered in the “Activity Subcategory

Code” column in the configuration file.

In SAP Business One, Web client, in  Analytics

  User-Defined Queries , you have created a user-defined query with

Business Partner as the Category and “New Lead” as the Name. Example SQL and SAP HANA queries are provided in the

configuration file on the “DB Query” sheet. To create a tile for the user-defined query on the home page, set the Default Tile

switch to Yes.

Before running the bot, you have created a local root folder that will be used by the bot to create a log folder to store the log files.

You have downloaded the configuration Excel file available in the Documents section of the project template and placed it in the

local root folder. In the configuration file, you have specified the "Business Object" ("BP Activity") and "Company Code" values. The

"Company Code" can be an arbitrary value (consisting of numbers, letters, or both) to identify the company, or the branch

identification number if you are using branches for the SAP Business One company. In the “Activity Subcategory Code” column,

you have entered the activity Subject codes from SAP Business One. The activity subject codes are primary key values that you

can find in the OCLS table.

The remaining columns in the configuration file contain the rules for the activity creation and notifications in the user’s Outlook

account.

The name of the configuration file must be specified in SAP Build Process Automation as the variable “WorkSheetName”.

  Note

If the bot is working with other bots, use the same configuration file for all the bots (except for the bot-specific files for Activity

Creation for Business Partners), with the business object and company codes specified for each bot.

This is custom documentation. For more information, please visit SAP Help Portal.

34

6/8/26, 6:13 AM

After running the bot, you can find the log files for the bot in the "Logs" folder. If the configuration file is set to send a reminder

about the activity in the user’s Outlook account, reminders are created in the specified user’s Outlook calendar.

Constraints

This bot can only work with the Microsoft Windows operating system.

Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember

Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template bots to use the

Windows Credential Manager for storing users and passwords for the bots (regardless of whether the bot is using the front end

or back end); however, you can adapt the bot to use other similar secure storage systems. Also, regardless of whether the bot is

designed to use the front-end UI or back-end services, we highly recommend that you create individual technical users

(communication arrangement) for each “bot + business user / business scenario” pair. This enables you to distinguish whether

the action was carried out by a physical business user or by a robot, and to achieve full traceability of the bots and human

actions individually. As per any other best practices, the user must not share their bot credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

Business Process Automations

SAP Build Process Automation oﬀers you access to workflow capabilities that allow you to build, run, and manage workflows and

automate decision making. From simple approvals to end-to-end processes across organizations and apps, process automations

allow you to speed up and simplify business processes.

With the workflow management capabilities of SAP Build Process Automation, you can visually create business processes using a

combination of artifacts (such as approval forms and decisions) and process controls (such as e-mail notifications and

conditions). The business process is started by a trigger, such as when a request form is submitted, or an API call, in which an

external system starts the process.

The following best practices template process automation is available for SAP Business One in SAP Build Process Automation on

the Store tab:

Return Request

To set up template process automations for SAP Business One, see the following topics:

Setting Up a Service Key

This is custom documentation. For more information, please visit SAP Help Portal.

35

6/8/26, 6:13 AM

Acquiring a Project Template from the Store

Deploying an Automation Project Without a Trigger

Adding an API Trigger

Registering and Adding an Agent

Return Request

This process automates the creation of a return request on the seller’s side after a request is triggered by a customer entering

return request data. After the request is validated by the automation and confirmed by the seller, the customer is automatically

informed about the status.

You can find the Return Request process automation project template in the SAP Business Accelerator Hub

.

Business Case

Problem

A product return request occurs when a customer asks to return previously purchased items to the seller. The return request

information is often sent through e-mail and needs to be manually entered into a return request document in SAP Business One.

After manually verifying the data, the seller needs to confirm the request and then manually notify the customer. This process

costs time on the seller's side and can be prone to errors.

Solution

The Return Request process automation automates the creation of a return request on the seller's side after a return is initiated

by a customer. The automation is triggered by an API call that receives the return request data. The input data is automatically

validated. If no errors are identified, the automation creates the return request, sends an e-mail notification to the user to confirm

or reject the return request, and automatically informs the customer about the return request status.

Business Benefits

Reduces user eﬀort

Improves work eﬃciency

Reduces the risk of manual errors

Technical Specification

Content and Strategic Intent

Manually entering return request information from customers into a return request document in SAP Business One, verifying the

data, and informing customers about the request’s status, is a time-consuming process for sellers. By automating this process

using the Return Request process automation, sellers (“processors”) simply need to confirm or accept an automatically created

return request based on validated customer input data. The automation then sends a predefined, customized e-mail to the

customer (“requester”) about the return request status.

This is custom documentation. For more information, please visit SAP Help Portal.

36

6/8/26, 6:13 AM

Watch this video about the Return Request process automation.

Open this video in a new window

Technical Details

Prerequisites

The processor has full authorization to Return Requests and Document Confirmation in SAP Business One (

Administration

  System Initialization

  Authorizations

  General Authorizations ).

You have assigned the required role collection to the processor. For more information, see Authorizations in SAP Build

Process Automation.

Setup

After completing the setup steps for process automations (for more information, see Business Process Automations, you need to

do the following:

1. Configure the SMTP E-mail Destination

To send e-mail notifications to requesters on status changes in a deployed automation project, you need to configure an

SAP BTP e-mail destination for SAP Build Process Automation. For more information on how to configure the e-mail

destination, see Configuring the SMTP E-Mail Destination.

2. Add Alert Handlers

Alert handlers enable SAP Build Process Automation to send e-mail notifications for the alerts used in a deployed process.

The alert handler allows sellers to customize the e-mail notifications sent to their customers. The following alerts can be

triggered in the Return Request process automation:

Return_Request_Requestor_Confirmation

This alert is triggered if the return request is approved. Adding an alert handler for this alert sends a confirmation e-

mail to the requestor.

Return_Request_Requestor_Rejection

This is custom documentation. For more information, please visit SAP Help Portal.

37

6/8/26, 6:13 AM

This alert is triggered if the return request is rejected. Adding an alert handler for this alert sends a rejection e-mail

to the requestor.

Return_Request_Requestor_WrongData

This alert is triggered if the return request contains incorrect data. Adding an alert handler for this alert sends a

notification e-mail to the requestor, indicating that the return request data did not match the data in the seller’s

system.

For more information on how to add alert handlers, see Adding Alert Handlers.

3. Create a Web Form and Add an API Trigger

The process is started by an API trigger when a request form with the return information is submitted by the customer. The

seller needs to perform the following steps:

a. Create a web form that authenticates the customer and collects the required return request information from the

customer.

b. Add an API trigger in SAP Build Process Automation. For more information, see Adding an API Trigger.

Security

Protecting User Credentials

In certain configuration scenarios, a technical user is required. In such cases, every natural person needs a separate technical user

(for example, a separate communication arrangement). The user must not share their credentials with any other natural person.

  Remember

Some of the best practices for process automation for SAP Business One use OData for the back-end connection to SAP

Business One. These services use basic authentication (user name and password). We designed our template projects to use

the Windows Credential Manager for storing users and passwords for the automations (regardless of whether the automation

is using the front end or back end); however, you can adapt the project to use other similar secure storage systems. Also,

regardless of whether the automation is designed to use the front-end UI or back-end services, we highly recommend that you

create individual technical users (communication arrangement) for each “automation + business user / business scenario”

pair. This enables you to distinguish whether the action was carried out by a physical business user or by an automation, and to

achieve full traceability of automations and human actions individually. As per any other best practices, the user must not

share their credentials with anyone else.

For security-relevant information that applies to SAP Build Process Automation, see Security in the application help for SAP Build

Process Automation (EN only).

Further Information

For more information, see the Technical Specification

 available in the SAP Business Accelerator Hub.

This is custom documentation. For more information, please visit SAP Help Portal.

38

