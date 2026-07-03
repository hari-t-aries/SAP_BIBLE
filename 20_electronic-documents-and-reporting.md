6/8/26, 6:13 AM

SAP Business One 10.0

Generated on: 2026-06-08 06:13:15 GMT+0000

SAP Business One | 10.0

Public

Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/68a2e87fb29941b5bf959a184d9c6727?locale=en-

US&state=PRODUCTION&version=10.0

Warning

This document has been generated from SAP Help Portal and is an incomplete version of the oﬃcial SAP product documentation. The

information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be missing important

aspects and/or correlations to other topics. For this reason, it is not for production use.

For more information, please visit https://help.sap.com/docs/disclaimer.

This is custom documentation. For more information, please visit SAP Help Portal.

1

6/8/26, 6:13 AM

Electronic Documents and Reporting

Electronic document and reporting functionality in SAP Business One allows you to manage documents like A/R invoices in an electronic

format, such as XML. Electronic documents can be created by, sent from, and imported to, SAP Business One. Electronic documents can be

processed automatically by organizations and their systems. Increasingly, organizations and oﬃcial authorities around the world require

documents to be submitted in an electronic format to reduce manual processing.

SAP Business One has diﬀerent standards for electronic documents, and ways of sending electronic documents, called protocols. The

requirements for protocols are often determined by international standards organizations, industry bodies, or national authorities. Some

localizations of SAP Business One have customized electronic document functionality based on local legal requirements. Typically, set up is

required in various areas, such as Electronic Document Service, Electronic File Manager, and the integration framework for SAP Business

One, to communicate and report electronic documents. Registration and set up with authorities and third party intermediaries may be

required.

In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more

information.

Please note that image maps are not interactive in PDF outputs.

Working with Electronic Documents and Reports

File Names, Paths and Formats

When generating electronic files from system documents, you can create files with specific name structures. Rather than having default

name structures, options are available for flexibility in file name and path structures. Some authorities and access points have requirements

for specific file name and path structures as part of validation processes. File name and path definitions are diﬀerent for the same document

under diﬀerent protocols.

A column File Name and Path is available in Electronic Documents Export Setup, follow  Document Settings

 Electronic Documents tab

 Documents Mapping Determination

 Electronic Documents Export Setup

 File Name and Path . File Name and Path represents both

the file name and the file path, which are defined as follows:

File name is defined in Query Manager, following the required syntax. The file name is defined by stating the Data Source Table and

Field in brackets, for example [%ODOC.CntctCode] where "ODOC" represents the main table but OINV would represent A/R invoices

or ORIN would represent credit memos. Define parameters by using a user query that relates to a data source; for example: SELECT *

This is custom documentation. For more information, please visit SAP Help Portal.

2

6/8/26, 6:13 AM

FROM OCPR T0 WHERE T0.CntctCode=[%ODOC.CntctCode]. Save your query in Query Manager. The query can then be used in the

file name or path. Data sources can be viewed in Electronic File Manager (EFM).

If Electronic Document Service is used as a processing target, then the file path is defined in the field EDS Export Base Path in

Document Settings, follow  Document Settings

 Electronic Documents tab

 EDS Export Base Path . If Electronic Document

Service is not used as a processing target, then the file path is defined in the field XML Path in General Settings.

File Name and Path contents are defined in the following syntax [%<TableName>.<FieldName>]. Define the structure of the file name by

using a formula; define the path with folders separated by "\" and the file name with an extension. If no path or file name is defined in File

Name and Path then the functionality works by using default values.

Related Information

Exporting Sales Documents to PDFs with XML Attachments

Exporting Sales Documents to PDFs with XML Attachments

Context

When working with a sales document, such as an A/R invoice, you can export it to a custom PDF copy that includes an attachment with the

document data in XML format. This facilitates alignment with various business standards and legislative requirements. Moreover, your

business partners and customers can import the file into their ERP systems for seamless business data exchange. The XML data can also be

used to generate Crystal Reports layouts that meet your specific business requirements.

Let's take an A/R invoice as an example to show you how to export a sales document to a PDF file with an XML attachment.

Procedure

1. Basic setup.

a. Open the add-on Electronic File Manager: Format Definition (EFM). Create a mapping file for the export; or download and

unzip the sample file Mapping_File_for_XML.zip to obtain the Sample.SPP file, and then adjust the sample file in the EFM to

align with your specific business standards and legislative requirements.

b. Open the SAP Business One client. In the window Electronic File Manager - Setup, upload the EFM mapping file to the SAP

Business One client.

c. Go to SAP Business One  Main Menu

 Administration

 System Initialization

 Document Settings

 Electronic

Documents  tab. Go to the section PDF with XML Attachment and configure the settings for XML data embedding in PDFs

as follows:

Enable Protocol: select this checkbox

Encrypt Sensitive Parameters: select this checkbox

Default eDoc Generation Type: Generate

Documents Mapping Determination: Double-click to open

d. Double-click within the Documents Mapping Determination field area to open the window Electronic Documents Export

Setup. In this window, create a new setup and select Sample, the name of the uploaded sample file, from the Export Format

dropdown list. This selection is used to convert business document data into XML format, which can then be attached to

PDFs.

e. Go to the Print Preferences window. Select the following checkboxes on the General tab:

When Adding Marketing Documents, Payments and Deposits, Use Attachments Folder as Default Path to Export

PDF

Attach Exported PDF to Marketing Documents, Payments and Deposits

This is custom documentation. For more information, please visit SAP Help Portal.

3

6/8/26, 6:13 AM

f. (Optional but recommended) Enable automatic creation of PDFs in the backend after addition of sales documents.

In the Print Preferences window, go to the Per Document tab, choose a document type, such as A/R Invoice in this example,

and then select the Export to PDF checkbox for the When Adding Document field below the setting Print Layout Designer

and Crystal Reports Preferences.

g. Go to the Document Numbering - Setup window. Set up a digital numbering series for A/R invoices.

2. Create an A/R invoice. On the Electronic Documents tab, you'll find the following settings configured in the section PDF with XML

Attachment:

eDoc Generation Type: Generate

eDoc Format: Sample

Documents Mapping Determination: Double-click to open

Document Status: New

3. In the A/R invoice, choose Add & View.

Results

If you have performed Step 1.f to enable the automatic creation of PDFs, the PDF file containing the XML-formatted data will be

automatically created in the backend. Please wait for the process to finish.

When the file generation is complete, you can see the file name listed on the Attachment tab. Double-click the file name to open the PDF file

in Adobe Acrobat. In Adobe Acrobat, open the Attachments tab. You can see an attached file named with the .XML extension, which

contains the data exported from the A/R invoice.

Alternatively, you can manually create the PDF after adding the invoice. To do this, use one of the following methods:

Choose  File

 Send

 SAP Business One Mailer

.

Choose  File

 Send

 Outlook E-Mail

.

Choose  File

 Export

 PDF .

If you choose to use SAP Business One Mailer, choose Yes when you're prompted to respond to this message: Do you want to attach

an edited report to the e-mail? The PDF will then appear on the Attachments tab in the Send Message window.

  Note

Please do not choose  File

 Print

 to create such PDFs. Because this is a native operation supported by the Windows OS.

You can monitor the exports of sales documents in the Electronic Document Monitor window. To view the status of all exported documents,

choose PDF with XML Attachment from the Protocol dropdown list.

  Note

This export function is unavailable through the DI API.

Related Information

Electronic File Manager: Format Definition Overview

Setting Up Generic and Special-Purpose Electronic File Formats

Print Preferences: General Tab

Print Preferences: Per Document Tab

Document Numbering - Setup

This is custom documentation. For more information, please visit SAP Help Portal.

4

6/8/26, 6:13 AM

Peppol

Peppol enables trading partners to exchange standards-based electronic documents over the Peppol network.

Peppol Access Points connect users to the Peppol network and exchange electronic documents based on Peppol specifications. Buyers and

vendors are free to choose their preferred single access point provider to connect to all Peppol participants already on the network through

a "connect once, connect to all" principle. SAP oﬀers an access point service for Peppol, for more information see the SAP help portal SAP

Document and Reporting Compliance, Cloud Edition and Integrating the Cloud Edition with SAP Business One.

Electronic invoicing is a legal requirement for public procurement processes in some jurisdictions. Even though Peppol was originally a

European initiative, jurisdictions outside Europe can use and are implementing Peppol standards.

Peppol builds on the standard setup of SAP Business One infrastructure for the processing of electronic documents. Diﬀerent systems and

tools are needed for the Peppol solution:

SAP Business One Client

Electronic Document Service (EDS)

Electronic File Manager (EFM)

Business Technology Platform (BTP)

SAP Document and Reporting Compliance, cloud edition or other Peppol Access Point

Please note that requirements, services and system fields including settings are subject to change. Older feature packs or versions require

diﬀerent systems and settings so check the SAP Notes that are relevant for your installation.

The Peppol protocol is available in a limited set of SAP Business One localizations. The Peppol protocol is not currently available in the

following localizations: Argentina (AR), Brazil (BR), Costa Rica (CR), Guatemala (GT), India (IN), and Mexico (MX).

Some localizations oﬀer local electronic documents and reporting protocols that operate separately to Peppol.

Functionality provides the ability to generate UBL Invoices through EFM and an integration framework package, to connect to the Peppol

Access Point through EDS.

For more information about the initial release of SAP Business One for Peppol, see SAP Note 2915144

.

Setting Up Peppol

Set up is required in various diﬀerent systems and areas to exchange electronic documents through the Peppol network. The following

settings are for using generic Peppol functionality, however the authorities in your localization may have specific legal requirements.

SAP Business One

Document Numbering

Marketing documents relevant for Peppol must have a digital numbering series, follow  Administration
Document Numbering .

  System Initialization

Document Settings

Peppol has a dedicated section and settings on the Electronic Documents tab of Document Settings, follow  Administration

  System

Initialization

  Document Settings

  Electronic Documents tab .

Peppol VAT Structure is specific to a country or region. For example, 0184 is for Denmark, 9930 is for Germany, and 0195 is for

Singapore.

Enter your Participant ID for Peppol. For details of how to create a participant ID with SAP Document and Reporting Compliance,

cloud edition, see the prerequisites of Setting Up SAP Business One for Communication with Peppol Exchange.

This is custom documentation. For more information, please visit SAP Help Portal.

5

6/8/26, 6:13 AM

Choose Documents Mapping Determination to select a format file that you have uploaded to Electronic File Manager.

Choose Processing Target Setup to open Processing Targets for Protocol which gives you several target and connector options on

diﬀerent tabs.

Processing Targets for Protocol

Diﬀerent tabs are available on Processing Targets for Protocol for Peppol, giving you several target and connector options on diﬀerent tabs.

The tab Peppol Connector v1 shows the details and settings for a connector through Electronic Document Service (EDS):

Certificate: choose a certificate to authenticate SAP Business One client for the SAP Document and Reporting Compliance, cloud

edition portal during API calls.

Provider: SAP Access Point represents SAP Document and Reporting Compliance, cloud edition.

Enter your Access Point URL for Peppol. For details of how to create an access point URL with SAP Document and Reporting

Compliance, cloud edition, see the prerequisites of Setting Up SAP Business One for Communication with Peppol Exchange.

Proxy: you can set proxy authentication. For more information, see SAP Note 3523105

.

PEPPOL BIS Code Lists

Specify your business interoperability specification (BIS) code lists in PEPPOL BIS Code Lists - Selection Criteria, follow  Administration

  Setup

  Electronic Documents

  PEPPOL BIS Code Lists . Add at least the three tables and mark one value as default for Invoice Type

Code. The following Business Interoperability Specification Code List Type options are some of those available through PEPPOL BIS Code

Lists - Selection Criteria:

Order Type Code

Delivery Type Code

Invoice Type Code

Credit Memo Type Code

Standard Item Type Identification Code

Item Commodity Classification Code

After choosing a Business Interoperability Specification Code List Type, set up Codes and Descriptions in the PEPPOL BIS Code Lists -

Setup window.

Master and Company Data

Set up is required for data such as:

VAT Structure and Participant ID in the Peppol section on the eDocs tab of relevant business partner master data.

GLN, Ship To and Bill To addresses, Contact Person, and Federal Tax IDs in relevant business partner master data.

Alias Name, GLN, and Federal Tax IDs in Company Details.

Business Partner Catalog Numbers, Standard Item Identification, Item Commodity Classification, and Sales UoM Name for

relevant item master data.

Electronic Document Service

SAP Business One uses Electronic Document Service (EDS) to communicate with other services, for example, SAP Document and Reporting

Compliance, cloud edition. EDS processes electronic documents and reports for SAP Business One. On the web-based dashboard for EDS,

choose the relevant company for the database instance and activate the connectors related to the Peppol protocol. For more information

about EDS, see Electronic Document Service (EDS).

Electronic File Manager, Imports, and Exports

This is custom documentation. For more information, please visit SAP Help Portal.

6

6/8/26, 6:13 AM

Set up is required for Peppol through Electronic File Manager (EFM) mapping files which must be uploaded to SAP Business One.

Separate files are provided for invoice and credit memo document types. The format of files is specific to a UBL version.

EFM mapping files are available on SAP Note 2915144

.

After downloading the EFM mapping files, import the files to SAP Business One through EFM, follow  Administration

 Setup

 General

 Electronic File Manager

. Use the files in Document Settings setup and the Export Mapping Determination windows.

The Electronic Document Import Wizard is an essential part of the Peppol import solution. Information is available in online help Electronic

Document Import Wizard and SAP Note 2915186.

Integration Framework for SAP Business One

Set up was required for the initial release of the Peppol Exchange process in the integration framework for SAP Business One. With the

release of Peppol Connector v1 connecting through EDS, the integration framework is no longer required for Peppol. More information is

available on SAP Note 2915144

.

Peppol Exchange Process Supported by SAP Document and Reporting Compliance, Cloud
Edition

Set up is required to use the Peppol Exchange process supported by SAP Document and Reporting Compliance, cloud edition. For more

information about the process, see the SAP help portal Peppol Exchange Process. To set up the Peppol Exchange process supported by the

cloud edition, you need to use BTP. Cloud Connector is needed for connectivity with BTP, for more information see the SAP help portal SAP

BTP Connectivity. To integrate SAP Business One with the Peppol Exchange process supported by the cloud edition, see the SAP help portal

Integration with SAP Business One.

For more information about Peppol, see SAP Note 2915144

.

Working with Peppol

Peppol builds on the standard setup of SAP Business One infrastructure for the processing of electronic documents. Following the diﬀerent

set up requirements for Peppol, you can process electronic documents through the Peppol Exchange.

Both Sales - A/R and Purchasing - A/P marketing documents are supported by the Peppol Exchange process in SAP Business One; the

following document types are some of those supported:

A/R and A/P Invoices

A/R and A/P Credit Memos

A/R and A/P Debit Memos

A/R and A/P Orders

It is possible to use orders and deliveries as part of the Peppol Exchange process, however these documents are not supported currently by

SAP Document and Reporting Compliance, cloud edition.

Creating A/R Invoices for Peppol Exchange:

Open an A/R invoice and enter the information in the standard way, based on a previous document or as a new stand-alone document.

Check the document and add it to the system.

The system treats the document as an electronic document and displays information about the status of processing on the document. From

the Electronic Documents Monitor, choose  Reports

  Electronic Document Monitor

, you can manage documents for the Peppol

Exchange process. You can also manage follow-up actions for documents directly through Electronic Document Monitor.

Importing Electronic Invoices from Peppol Exchange:

This is custom documentation. For more information, please visit SAP Help Portal.

7

6/8/26, 6:13 AM

The import of electronic invoices is managed by SAP Document and Reporting Compliance, cloud edition and the Electronic Documents

Import Wizard, choose  Purchasing A/P

  Electronic Document Import Wizard . The Electronic Documents Import Wizard loads all

available marketing documents from the integration framework for SAP Business One for processing and matching. For more information,

refer to Electronic Documents Import Wizard.

Importing Peppol Relevant Data with Import from Microsoft Excel:

You can use Import from Excel, follow  Administration

  Data Export/Import

  Data Import

  Import from Excel

, to add Peppol data to

SAP Business One. Import from Excel allows multiple data to be imported at once.

Procedure:

Prepare the required values in a Microsoft Excel file. The numeric code in the first column (A) of the file identifies the type of Peppol code

(Code List), as follows; ensure that your Business Interoperability Specification Code List Type selection matches the code in column A.

Code "1" for Order Type documents

Code "2" for Delivery Type documents

Code "3" for Invoice Type documents

Code "4" for Credit Memo Type documents

Code "5" for Standard Item Type Identification

Code "6" for Item Commodity Classification

Open Import from Excel in SAP Business One.

Choose PEPPOL BIS Codes as the Data Type to Import, and choose the file you created for File to Import.

When the codes and relevant other fields are imported to OUNCL, the values are visible for the relevant code tables.

Select specific fields from the object in the list of fields in the grid of the import form.

Three Import Methods are available for selection:

Add New Records and Update Existing Records

Add New Records Without Updating Existing Records

Update Existing Records Without Adding New Records

Save and use the defined setup as a template for repeat use.

Working with Business Level Responses:

Business Level Responses (BLRs) are a message type that is used in the Peppol Exchange process for electronic documents. You can send

and receive BLRs to communicate business decisions regarding electronic documents in the Peppol Exchange process.

You can send BLRs to accept or reject electronic documents that are imported to SAP Business One as part of the Peppol Exchange

process.

You can receive BLRs to SAP Business One to manage electronic documents as part of the Peppol Exchange process.

BLRs are recorded in statuses of documents that can be seen on the Electronic Documents tab of relevant marketing documents and in the

Electronic Document Monitor. Rejection reasons can only be viewed on Electronic Document Monitor Details.

Document Information Extraction

This is custom documentation. For more information, please visit SAP Help Portal.

8

6/8/26, 6:13 AM

Document Information Extraction is a service from SAP that automatically reads and extracts information from digital document files and

scanned documents. The service is available for use with SAP Business One and SAP Business One, version for SAP HANA, to assist

customers by removing the need to manually process documents such as invoices.

SAP Business One connects to the Document Information Extraction service through Electronic Document Service and an API.

Document Information Extraction service reads A/P invoices from received PDF and JPG files before communicating the structured

information, in .JSON files, to SAP Business One where A/P invoice drafts are created.

The service is activated and controlled through options in Document Settings under the Document Information Extraction protocol.

Document Information Extraction is a service that is available in a Cloud Foundry or Kyma environment. Document Information Extraction

service is available for purchase separately from SAP Business One.

For more information about the service on the help portal, visit Document Information Extraction. For more information about Document

Information Extraction with SAP Business One, see SAP Notes 3021904

 and 3060961

.

Setting Up Document Information Extraction

Set up is required in various diﬀerent systems and areas to use Document Information Extraction service. Some diﬀerences exist between

the fields in diﬀerent versions and localizations.

SAP Business One

Document Settings

The tab Document Information Extraction is available in Document Settings, choose  Administration

  System Initialization

Document Settings

  Electronic Documents tab

  Document Information Extraction section , with information and settings dedicated

to Document Information Extraction service.

Document Information Extraction

Enable Protocol

Service URL

UAA URL. The arrow

 next to UAA URL allows you to upload data from a .txt file to Document Information Extraction settings.

Data for fields such as UAA URL, Service URL, and Client ID can be populated by selecting a .txt file after Windows File Explorer is

opened.

PDF Folder for Extraction: path definition of location on server from where the service collects PDFs and sends them to Document

Information Extraction service. Related PDFs are stored and saved here.

Client Secret: based on SCP account

Client ID: based on SCP account

Mapping Formats

Documents Mapping Determination: format to map JSON responses against fields in SAP Business One.

Server Setup

Outbound Frequency: how often SAP Business One sends PDF files from the storage location where A/P invoices are stored.

Inbound Frequency: how often SAP Business One calls Document Information Extraction service for pending responses.

API URL

A/P Invoice Repository Path

This is custom documentation. For more information, please visit SAP Help Portal.

9

6/8/26, 6:13 AM

General Settings

Set up a path for your attachment folder in General Settings, follow  Administration

  System Initialization

  General Settings

  Paths

.

SAP Business Technology Platform

In your SAP Business Technology Platform (BTP) account, use the related Service Key and copy the relevant information to Document

Settings in SAP Business One.

Electronic Documents Service

Document Information Extraction service uses Electronic Documents Service to connect with SAP Business One.

Working with Document Information Extraction

The SAP Business One integration with Document Information Extraction service works with Electronic Document Import Wizard

functionality in all localizations except for Brazil, Argentina, Costa Rica and Guatemala. The Electronic Document Import Wizard provides

dedicated functionality for importing electronic documents to SAP Business One. For the Document Information Extraction service

integration, there is the Document Information Extraction protocol under which relevant documents are imported.

Default incoming mapping determinations are available. The recommended setup includes the relevant document type A/P invoice and the

identification of business partners through business partner name or Federal Tax ID as preferred options.

Electronic Document Import Wizard Steps

The Electronic Document Import Wizard works through a series of steps.

Step 1 of the Electronic Document Import Wizard shows that the Document Information Extraction protocol is in use and allows you to

upload multiple files at once.

Step 2 of the Electronic Document Import Wizard provides information about the initial determination status of the files that are available

for import. It is possible to see the status, and eventually the reason for any error, in the Message column.

In some cases, for example when there is no business partner found in the database, it is possible to correct the information in the

respective data. For example, you can make a change in Business Partner Master Data and then by using the option You Can Also, you can

re-determine the problematic files that are available for import.

It is possible to use the selection criteria that are available in step 2 of the wizard to choose documents for processing by the wizard.

Step 3 of the Electronic Documents Import Wizard carries out a match of imported data from the Document Information Extraction service

and previews the relevant data before document drafts are created. You can check the original document by selecting the golden arrow icon

next to the Tax ID field to compare the identified business partner, items, prices, quantity, and the identified base documents. You can

remove or replace the identified base document, by right-clicking and using the context menu.

When you choose the Operation "Generate", the system creates a document draft. When selecting "Generate", it is possible to set this

operation for individual rows of a document.

Step 4 of the Electronic Documents Import Wizard informs you of the status of the created drafts.

The created drafts can be viewed in the Document Draft Report and the Electronic Documents Monitor. From both locations, it is possible to

finish the documents from draft.

In the Document Draft Report, there are the columns eDoc Protocol and Source File Path and Name to identify the protocol used for the

import of a particular document, as well as the file name and path of the original document.

This is custom documentation. For more information, please visit SAP Help Portal.

10

6/8/26, 6:13 AM

The following steps describe the original scenario for using Document Information Extraction without using the Electronic Document Import

Wizard. These steps are valid for Brazil, Argentina, Costa Rica and Guatemala localizations:

Copy the respective invoice PDF into the main PDF Folder for Extraction folder.

The system processes the document and stores the result in the database.

Select DOX Import in Document Drafts Report - Selection Criteria to create a draft document from the saved data.

Open the document draft list to check the transferred data.

The processed document is attached to the created invoice draft.

The draft document is created using the following information:

Business Partner Name

Item Description

Vendor Invoice Number

Document Currency

Item Quantity and Price

Document Total

Electronic Document Service (EDS)

Electronic Document Service (EDS) manages, processes, and communicates electronic documents, reports, and related information for SAP

Business One. EDS handles electronic documents and electronic reporting in varying degrees depending on your localization and business

requirements. EDS is required in certain scenarios that use Electronic File Manager (EFM).

EDS runs on Windows or Linux and works in the background.

EDS collects data through System Landscape Directory (SLD) and Service Layer (SL).

EDS sends documents to the authorities and updates statuses in the SAP Business One database through Service Layer.

EDS is registered in SLD on the Services tab.

EDS Dashboard allows you to activate connectors and display information about EDS and connectors, including event logs.

You must install the System Landscape Directory (SLD) and Service Layer (SL) components to use EDS. For more information about SLD

and SL, see the SAP Business One Administrator's Guide. Installation defaults for settings are recommended for SAP Business One

components such as SLD, SL, and EDS. Extremely high throughputs of electronic documents may require changes to component settings.

Use the SAP Business One Setup Wizard or Components Wizard to choose and install the EDS component.

Procedure

1. Install SLD with at least one database server that is registered using the hostname or IP address.

2. Install SL and EDS using the Components Wizard. Ensure that all hostnames or IP addresses are in the same format as the database

server in the SLD registration.

3. In Document Settings in SAP Business One, choose Processing Target Setup for the relevant electronic documents protocol.

Choose an EDS connector as the processing target. For more information about processing targets, see the section on Document

Settings below.

There are fields and settings relevant for EDS in Document Settings in SAP Business One, choose  Administration

  System Initialization

  Document Settings . Depending on your localization in SAP Business One, the sections, labels, and fields vary in Document Settings.

Diﬀerent jurisdictions have diﬀerent legal requirements for electronic documents.

This is custom documentation. For more information, please visit SAP Help Portal.

11

6/8/26, 6:13 AM

  Note

You cannot currently extend EDS or create additional related scenarios for other web services.

Processing Target Setup

For the following protocols you can set basic or complex proxy authentication: AFE for Argentina, CFDI for Mexico. E-Billing for India, E-Books

for Greece, EII, Electronic PDF Signature for Israel, FPA for Italy, DIGIPOORT for Netherlands, Peppol, E-Invoicing, E-Communication, and

Electronic Document Signing for Portugal. HOI for Hungary, KSeF for Poland, and Skat for Denmark.

For specific information about the proxy authentication settings, see SAP Note 3523105

.

Documents Mapping Determination

When generating electronic files from system documents, you can create files with specific name structures. Rather than having default

name structures, options are available for flexibility in file name structures. Some authorities and access points have requirements for

specific file name structures as part of validation processes. File name definitions are diﬀerent for the same document under diﬀerent

protocols.

The column File Name and Path is available in Electronic Documents Export Setup, choose  Document Settings

  Electronic Documents

tab

  Documents Mapping Determination

  Electronic Documents Export Setup

  File Name and Path . File Name and Path represents

both the file name and the file path, which are defined as follows:

File names are defined in Query Manager, following the required syntax. The file name is defined by stating the Data Source Table

and Field in brackets, for example [%ODOC.CntctCode] where "ODOC" represents the main table but OINV would represent A/R

invoices or ORIN would represent credit memos. Define parameters by using a user query that relates to a data source; for example:

SELECT * FROM OCPR T0 WHERE T0.CntctCode=[%ODOC.CntctCode]. Save your query in Query Manager. The query can then be

used in the file name or path. Data sources can be viewed in Electronic File Manager (EFM).

File path is defined in the field EDS Export Base Path in Document Settings.

File Name and Path contains values that are defined in the following syntax [%<TableName>.<FieldName>]. Define the structure of the file

name by using a formula; define the path with folders separated by "\" and the file name with an extension. The defined path follows the EDS

Export Base Path in Document Settings (if EDS is active as a processing target) or the XML Path defined in General Settings. If no path or

file name is defined, then the functionality works by using default values.

  Note

Changes should not be made to appsettings.json files unless there is a problem or a workaround is necessary. In initial releases of

EDS, before the introduction of the dashboard, changes were needed in appsettings.json files but this is no longer necessary.

SAP Notes

For more information about EDS and related topics, see the following knowledge articles, SAP Notes, and other notes that reference the

following notes:

2952067

 – Electronic Document Service

3207052

 – Electronic Documents and Electronic Reports: Standard Behaviors and How-to Scenarios

3139544

 – Optimize Service Layer Performance

2912506

 – Service Layer Controller for SAP Business One

Electronic Document Service Dashboard

The Electronic Document Service (EDS) Dashboard is an interactive application, accessed through the internet, for managing and

monitoring EDS components and connectors to related databases or tenants.

This is custom documentation. For more information, please visit SAP Help Portal.

12

6/8/26, 6:13 AM

The EDS Dashboard allows you to activate protocol connectors and see details and information about connectors, including events. The EDS

Dashboard displays processed event information, like the number of handled events.

You can access the EDS Dashboard through the link in System Landscape Directory (SLD).

When logging in to the EDS Dashboard for on-premises SAP Business One from SLD, the same login details are automatically used as

for the Control Center of SLD. You do not need to re-enter your login details to access the EDS Dashboard in the same browser

session. If you open a diﬀerent browser application, you need to enter the login details to access the EDS Dashboard. You can log out

from the EDS Dashboard and then log in again using diﬀerent login details through the option in the top right corner of the EDS

Dashboard.

To log in to the EDS Dashboard for SAP Business One Cloud, use the details of any operator that is defined in the Cloud Control

Center of SLD.

The EDS Dashboard provides options to choose diﬀerent languages in which to display the dashboard.

The EDS Dashboard displays information in the header, collapsible lists of protocols for tenants, and diﬀerent sections for more information

about connectors.

The section Notifications shows relevant warnings and error messages about EDS. You can expand or collapse the section. You can adjust

the amount of information shown in Notifications by changing the Notifications Level and Notifications Display Count settings.

Notifications Level uses the same logic as for Log Level that is described below.

The section Protocol Connectors shows the diﬀerent connectors for a protocol under a tenant. Each protocol connector has a row with an

option to activate, and information including the name, status, and number of events that have been handled.

Each protocol connector has a Log Level with five options to determine how much, and what kind of, information is stored in the log.

Diﬀerent EDS events are categorized at a log level depending on the importance of the event. Transaction and connection events exist at

diﬀerent log levels, depending on the importance on the event. Choosing a higher log level means that all events at that log level, and lower,

are stored in the log:

Level 5 Debug: All EDS events are logged. Detailed information about many events gives you the background to debug EDS and

identify issues. Use debug to investigate issues, including connection and transaction issues. The size of the log increases rapidly,

therefore debug is not recommended for standard day-to-day operations.

Level 4 Info: All EDS events at this level, and lower, are stored in the log.

Level 3 Warning: All EDS events at this level, and lower, are stored in the log. Repeated warnings can lead to errors.

Level 2 Error: All EDS events at this level are stored in the log. Errors aﬀect the normal running of EDS.

Level 1 None: No EDS events are logged.

The option Logs allows you to download information from the log. The option Details displays Entries from the log, including detailed

information about entry events like GUID. Filter and search options are available for Entries.

SAP Notes

For more information about EDS logs, and related topics, see the following SAP Note, and other notes that reference the following note:

3034774

 – EDS Related Information and Collection of Logs to Help Troubleshoot EDS Related Issues When Handling Electronic

Documents

Electronic Document Import Wizard

The Electronic Document Import Wizard, choose  Purchasing - A/P

 Electronic Document Import Wizard , helps you to process

incoming electronic documents in SAP Business One. Electronic documents can be transformed from formats such as XML to marketing

documents in SAP Business One.

This is custom documentation. For more information, please visit SAP Help Portal.

13

6/8/26, 6:13 AM

The wizard is most frequently used with electronic document protocols such Document Information Extraction service or Peppol, however

you can upload documents manually. A conversion takes place from the incoming document format to a SAP Business One schema format

through Electronic File Manager (EFM) and the wizard. Because EFM runtime is part of Electronic Document Service (EDS), EDS is required

if using the wizard. EFM mapping files define which values are imported and how, using functions and conditions that can be adjusted in the

EFM designer.

The Electronic Document Import Wizard works like other wizards in SAP Business One. The wizard guides you through the diﬀerent options,

in a series of steps, to produce results. The wizard helps you to define what you want to do and which documents you want to work with.

Matching rules are used when the wizard searches for, and tries to connect, related documents:

Using information from imported files, the system searches for related purchase orders. If a purchase order is closed by a goods

receipt purchase order then the system searches and tries to base the incoming document on a goods receipt purchase order. Some

conditions apply for the system to find relevant documents, such as the incoming document file having a relevant purchase order

number and source purchasing documents having a digital numbering series.

When searching for items in the system, the search is based on the import EFM mapping definition and being able to find key data

like item codes, item descriptions, business partner catalog numbers, and EAN codes.

Documents that can be imported include A/P invoices, A/P credit memos, A/P down payment invoices, goods receipt purchase

orders, and A/P purchase orders.

Drafts of documents can be created through the wizard by using data from imported documents. The adding of data into draft documents

follows the standard SAP Business One system of default values, set for specific business partners or items, or through methods like tax

code determination. Through EFM mappings, values such as unit of measure, vendor reference number, document date, delivery date, and

payment terms can be added to document drafts. When preparing document drafts, you can edit data that was not imported as expected,

such as business partner codes, items codes, and prices.

By using the Electronic Document Import Wizard with Document Information Extraction service, you can create sales order document drafts

from received purchase orders using the manual import option. There must be a purchase order file and corresponding JSON file available in

the same folder for Document Information Extraction service.

Steps in the Electronic Document Import Wizard

1 Sources and Selections

Choose the relevant Protocol for your scenario to import files. Only electronic document protocols that are active in Document Settings

show as options in Protocol.

Select Import Setup to open Electronic Documents Import Setup and to enter Xpaths and Namespaces that are relevant for your file

import scenario. Some of the following information is provided as an example:

XPaths Tab

Right-click in a column header to add a row.

Document Type: choose the type of document in the received file that is to be drafted in SAP Business One.

Document Type XPath: specify how to determine the document type in the received file. An example document type XPath is:

/rsm:CrossIndustryInvoice/rsm:ExchangedDocument/ram:TypeCode[text()='380']

Business Partner XPath: specify how to determine the business partner in the received file. An example business partner XPath is:

/rsm:CrossIndustryInvoice/rsm:SupplyChainTradeTransaction/ram:ApplicableHeaderTradeAgreement/ram:BuyerTradeParty/ram:ID

Referenced BP Field: choose which reference in SAP Business One is used to find the business partner in the imported files through

the Business Partner XPath.

Import Format: use a file that is available in Electronic File Manager, choose  Administration

 Setup

 General

  Electronic File

Manager

. You can upload files to Electronic File Manager after making changes in the designer for Electronic File Manager.

Namespaces Tab

This is custom documentation. For more information, please visit SAP Help Portal.

14

6/8/26, 6:13 AM

According to the file that you have used in Import Format on the XPaths tab and the files that you are importing, add prefixes and

namespaces. For example:

a = urn:un:unece:uncefact:data:standard:QualifiedDataType:100

qdt = urn:un:unece:uncefact:data:standard:QualifiedDataType:10

ram = urn:un:unece:uncefact:data:standard:ReusableAggregateBusinessInformationEntity:100

rsm = urn:un:unece:uncefact:data:standard:CrossIndustryInvoice:100

udt = urn:un:unece:uncefact:data:standard:UnqualifiedDataType:100

Select Upload Files to choose the files that you want to import.

Choose Next to process the files according to your setup.

2 Import Files

Use the various options to filter and choose which files you want to process further and import as documents.

To create documents in SAP Business One, a business partner must be identified. Business partner information can be taken from imported

files, but you can choose the business partner for the document row in BP Code.

3 Document Data Matching

The row data of imported electronic documents is shown and can be matched to item master data in SAP Business One. The system tries to

match imported values with master data in SAP Business One, like item codes and item descriptions. Manual changes can be made if

automatic matching is not successful. You can choose to skip row items in the Operation column.

4 Summary Report

You can see the draft documents and their status following the import.

This is custom documentation. For more information, please visit SAP Help Portal.

15

