**==> picture [596 x 420] intentionally omitted <==**

User Guide | PUBLIC Document Version: 1.2 – 2024-05-10 

## **How to Schedule Report Execution and Mailing in SAP Business One** 

**==> picture [58 x 30] intentionally omitted <==**

## **Content** 

|**1**|**Document History. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3**|
|---|---|
|**2**|**Introduction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4**|
|**3**|**Scheduling Report Execution. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5**|
|3.1|Report Execution Scheduler Window. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8|
|**4**|**Viewing Scheduled Reports in SAP Business One. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11**|
|**5**|**Confguring Job Service for Report Scheduling and Mailing. . . . . . . . . . . . . . . . . . . . . . . . . . . 13**|
|5.1|Establishing User Credentials for SAP Business One Messaging Service on Microsoft Windows|
||. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .15|
|**6**|**Authorizations. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16**|



How to Schedule Report Execution and Mailing in SAP Business One **Content** 

PUBLIC 

**2** 

## **1 Document History** 

|Version|Date|Change|
|---|---|---|
|1.0|2012-09-02|First version|
|1.1|2020-12-10|Minor updates|
|1.2|2024-05-10|Guide converted from PDF to HTML format for viewing on the SAP Help Portal.|
|1.3|2025-08-04|Updated the procedure of confguring Job Service - Report Scheduling & Fax.|
|1.4|2025-09-25|Updated the description for_User Code_and_User Password_on the_Report Execution_|
|||_Scheduler_window.|



How to Schedule Report Execution and Mailing in SAP Business One **Document History** 

PUBLIC 

**3** 

## **2 Introduction** 

This how-to guide introduces the report scheduling function of SAP Business One. You schedule report executions by running queries and specify recipients of the generated reports. The recipient either obtains the reports via email or views them directly in SAP Business One as a user. 

Formats of generated reports include PDF, HTML, and XML. Via email, these reports are sent as attachments; reports in HTML format can also be sent as the email message body. 

The following situations are the main triggers for setting up report execution schedules: 

- You cannot or do not want to wait a long time for a report to be executed. 

- You need to obtain data of certain reports on a regular basis. 

- You have no immediate access to SAP Business One, either frequently or for a long time. 

- You want to compare the different results of one report executed at regular intervals. 

##  Note 

This function is not supported in SAP Business One, version for SAP HANA. 

## **Prerequisites** 

- You have full authorization for the report scheduling functionality. For more information about authorizations, see the SAP Business One online help. 

- You have enabled SBO Mailer in SAP Business One client. For more information, see SAP Business One online help. 

- You have configured Job Service - Report Scheduling & Fax. For more information, see Configuring Job Service for Report Scheduling and Mailing [page 13]. 

How to Schedule Report Execution and Mailing in SAP Business One 

**Introduction** 

**4** PUBLIC 

## **3 Scheduling Report Execution** 

## **Prerequisites** 

- You have assigned at least one layout to the query you want to run. For more information, see the SAP Business One online help. 

- You have configured _SBO Mailer_ . 

## **Context** 

##  Note 

You can schedule executions of reports only by running queries without parameters. 

## **Procedure** 

1. From the SAP Business One menu bar, choose _Tools Queries Query Manager_ . 2. In the _Query Manager_ window, select a query and choose the _Schedule_ button. 

How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

PUBLIC **5** 

**==> picture [340 x 303] intentionally omitted <==**

3. In the _Report Execution Scheduler_ window, in the general area, specify the required details. 

How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

PUBLIC 

**6** 

**==> picture [403 x 492] intentionally omitted <==**

4. In the _Recipients_ area, specify information about recipients of the generated reports. 

To add recipients, choose the _Add Recipients_ button. 

In the _Add Recipients_ window, select required SAP Business One users and distribution lists and choose the _OK_ button. 

To save specified recipients as members of a new distribution list, choose the _Save as Distribution List_ button. 

5. To enable viewing the report execution results in SAP Business One, select the _Access to Overview_ checkbox. 

How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

PUBLIC 

**7** 

##  Note 

This function is available only for SAP Business One users. 

6. To enable sending emails with generated reports to a recipient, select the _Email_ checkbox and specify an email address. 

7. Specify in which formats you want the generated reports to be sent via email as attachments. 

8. Choose the _Add_ button. 

## **Results** 

The scheduled report will be executed and sent to the specified recipients via email at specified times. 

##  Note 

To modify a specific report execution schedule, you can access the _Report Execution Scheduler_ window to find it or access it directly from the _Scheduled Report Overview_ window. For more information, see Viewing Scheduled Reports in SAP Business One [page 11]. 

## **3.1 Report Execution Scheduler Window** 

To open the _Report Execution Scheduler_ window, from the SAP Business One menu bar, choose _Tools Queries Query Manager_ . 

## **General Area** 

|UI Element|Description|
|---|---|
|_Active_checkbox|Select this checkbox to specify whether the report is to be executed as sched-|
||uled.|
|Query type and name|Displays the query category:`System Query`or`User Query`or displays|
||the query name:`Query - <Query Name>`.|
||Not editable|
|_Report Title_|Name of the scheduled report. Displays by default the name of the query to run|
||to generate the report.|
|_Print Layout_dropdown list|List of print layouts for generated reports in PDF format.|



How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

**8** 

PUBLIC 

|UI Element|Description|
|---|---|
|_User Code_|Displays the code of the user who makes this particular report execution sched-|
|ule.||
|Not editable||
||Note|
||The feld is hidden when an identity provider is activated in the SLD control|
||center.|
|_User Password_|Password of the current user who is making the schedule.|
||Note|
||The feld is hidden when an identity provider is activated in the SLD control|
||center.|
|_Report Execution Timeout_dropdown list<br>Time limit for an unsuccessful report execution.||
|_Action on Error_dropdown list|Action to be taken if there is any error during report execution. Available op-|
||tions are:|
||•<br>_Deactivate Immediately_|
||•<br>_Continue_|
||•<br>_Deactivate On Second Failure_|
||•<br>_Deactivate On Third Failure_|
||•<br>_Deactivate On Fourth Failure_|
||Note|
||The second option (_Continue_) deactivates the schedule.|
|_Start Time_|Date and time for the report execution or the frst recurring report execution.|
|_Recurrence_dropdown list|The basis on which the report execution should recur. Available options are:|
||•<br>_None_|
||•<br>_Daily_|
||•<br>_Weekly_|
||•<br>_Monthly_|
||•<br>_Annually_|
|_Repeat Every_|The frequency at which the report execution should recur. Available for daily,|
||weekly, monthly, and annual recurrences.|
|_Repeat on_|Days on which the report execution recurs. Available for weekly, monthly, and|
||annual recurrences.|
|_Range Start_|Date of the_Start Time_feld. Available only for recurring executions and not|
||editable.|
|_Range End_|Ending date or condition of the report execution. Available only for recurring|
||executions.|



How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

PUBLIC 

**9** 

|UI Element|Description|
|---|---|
|_Next Execution_|Due time of the next report execution. Available only for recurring executions.|
|_Number of Executions_|Number of completed executions of the scheduled report, including both suc-|
||cessful and failed executions. Not editable.|
|_Reset Counter_button|Resets the value of the_Number of Executions_feld to 0. Available only if the|
||value of the_Number of Executions_feld is greater than zero.|
|_Remarks_|Notes to the scheduled report; shown in the_Scheduled Report Overview_win-|
||dow. Optional.|
|_Email Subject_|Email subject to be displayed after the prefx defned in the_SBO Mailer_settings.|
||For more information, seeConfguring Job Service for Report Scheduling and|
||Mailing [page 13].|
|_HTML Output as Message Body_radio but-|Select this radio button to use the HTML format of the generated report as the|
|ton|email message body.|
|_Message Body_radio button|Select this radio button to enter words as the email message body. You can use|
||any HTML tags for formatting the text, except for`<HTML>`and`<BODY>`.|



## **Recipients Table** 

This table lists all recipients of the generated reports and other relevant information. 

|UI Element|Description|
|---|---|
|_Recipient_|Name of the recipient.|
|_Access to Overview_checkbox|Select this checkbox to grant access to viewing the execution outputs of the|
||scheduled report in SAP Business One. Available only for SAP Business One|
||users.|
|_Send Email_checkbox|Select this checkbox to enable sending emails with generated reports to the|
||recipient.|
|_Email Address_|Email address of the recipient.|
|_PDF_,_HTML_,_XML_checkboxes|Formats of the generated reports to be sent via email as attachments.|



How to Schedule Report Execution and Mailing in SAP Business One **Scheduling Report Execution** 

**10** 

PUBLIC 

## **4 Viewing Scheduled Reports in SAP Business One** 

## **Prerequisites** 

In the _Report Execution Scheduler_ window, you have been granted access to the _Scheduled Report Overview_ window. 

## **Context** 

In the _Scheduled Report Overview_ window, you can view the details of scheduled report executions and the generated reports. The scheduled reports include reports that have not yet been executed or whose schedules have been deactivated. 

## **Procedure** 

1. From the SAP Business One menu bar, choose _Tools Scheduled Report Overview._ 

**==> picture [7 x 11] intentionally omitted <==**

2. In the _Scheduled Report Overview_ window, to view the details of executions of a schedules report, click the arrow next to the report title. 

To view the details of executions of all scheduled reports, choose the _Expand_ button. 

How to Schedule Report Execution and Mailing in SAP Business One **Viewing Scheduled Reports in SAP Business One** 

PUBLIC **11** 

**==> picture [409 x 271] intentionally omitted <==**

3. To view a generated report of one execution, double-click the row. 

To view a particular format of a generated report, click the corresponding icon. 

To view the execution schedule of a report, double-click the scheduled report row (first level). If you are the creator of the report schedule, in the _Report Execution Scheduler_ window that opens, you can modify and update the scheduling settings. 

If you are the creator of a report schedule, to remove the report execution details and results, do one of the following: 

- To remove all execution details and generated reports, right-click the scheduled report row (first level) and choose _Remove_ . 

- To remove details and generated reports of one execution, right-click the corresponding row (second level) and choose _Remove_ . 

How to Schedule Report Execution and Mailing in SAP Business One **Viewing Scheduled Reports in SAP Business One** 

**12** PUBLIC 

## **5 Configuring Job Service for Report Scheduling and Mailing** 

## **Context** 

To schedule report execution and send generated reports via email, you must first define the mail settings. For more information, see the _SAP Business One Administrator’s Guide_ on the SAP Help Portal. 

## **Procedure** 

1. In the Windows system tray, double-click ( _SAP Business One Service Manager_ ). 

   - Alternatively, choose _Start Programs SAP Business One Server Tools Service Manager_ . 

2. In the _SAP Business One Service Manager_ window, in the _Service_ drop-down list, select _Job Service - Report Scheduling & Fax_ and choose _Schedule_ . 

3. In the _Scheduler - Job Service - Report Scheduling & Fax_ window, select one of the following options: 

   - _By Intervals_ - Sets report processing to regularly start every x hours and y minutes. 

   - _On Specific Date_ - Sets report processing for a specific date and time. 

   - _Daily_ - Sets report processing for a fixed hour of each day. 

   - _Weekly_ - Sets report processing for a fixed hour on a fixed day of each week. 

   - _Monthly_ - Sets report processing for a fixed hour on a fixed day of each month. 

   - Choose _OK_ to return to the _SAP Business One Service Manager_ window. 

4. In the _SAP Business One Service Manager_ window, in the _Service_ drop-down list, select _Job Service - Report Scheduling & Fax_ and choose _Settings_ . 

5. In the _General Settings_ window, define the mail settings according to your company settings. 

How to Schedule Report Execution and Mailing in SAP Business One **Configuring Job Service for Report Scheduling and Mailing** 

PUBLIC **13** 

**==> picture [338 x 436] intentionally omitted <==**

   1. In the _SAP Business One Client Executable_ area, specify the file path of the SAP Business One client. 

   2. Optionally, enter an email subject prefix which precedes the subject of each scheduled email with the generated report. 

   3. Enter a name as the email sender. 

   4. Enter the sender email address. 

   5. Specify the timeout period for unsuccessful report execution. 

   6. Specify the logging level. 

   7. Choose the _OK_ button. 

6. In the _SAP Business One Service Manager_ window, in the _Service_ drop-down list, select _Job Service - Report Scheduling & Fax_ and choose _Connection_ . In the _Connection Settings_ window, you can view the database information and SLD address. 

7. In the _SAP Business One Service Manager_ window, in the _Service_ drop-down list, select _Job Service - Report Scheduling & Fax_ , choose ( _Play_ ), and select the checkbox _Start when operating system starts_ . 

How to Schedule Report Execution and Mailing in SAP Business One **Configuring Job Service for Report Scheduling and Mailing** 

**14** PUBLIC 

## **5.1 Establishing User Credentials for SAP Business One Messaging Service on Microsoft Windows** 

## **Context** 

When the SBO Mailer service is first started, the default Microsoft credentials for the SAP Business One messaging service are local system credentials. To fully deliver this service, you need to change the credentials to user credentials. 

The authenticated user should meet the following two requirements: 

- Has a user account in SAP Business One with full authorization for the report scheduling function 

- Has a physical printer (not virtual) available 

## **Procedure** 

1. In the taskbar of Microsoft Windows, choose the _Start_ button or ( _Start_ ). 

2. In the start menu, choose _Run_ , enter **`services.msc`** , and choose _OK_ . 

3. In the _Services_ window, configure _SAP Business One Messaging Service_ as required. 

**==> picture [422 x 268] intentionally omitted <==**

For more information about configuring services, refer to the Microsoft online help. 

How to Schedule Report Execution and Mailing in SAP Business One **Configuring Job Service for Report Scheduling and Mailing** 

PUBLIC 

**15** 

## **6 Authorizations** 

For information about the authorizations required for report scheduling, see the online help as well as the document _How to Define Authorizations_ , which you can download from the Help Portal. 

How to Schedule Report Execution and Mailing in SAP Business One **Authorizations** 

**16** PUBLIC 

## **Important Disclaimers and Legal Information** 

## **Hyperlinks** 

Some links are classified by an icon and/or a mouseover text. These links provide additional information. About the icons: 

- Links with the icon : You are entering a Web site that is not hosted by SAP. By using such links, you agree (unless expressly stated otherwise in your agreements with SAP) to this: 

   - The content of the linked-to site is not SAP documentation. You may not infer any product claims against SAP based on this information. 

   - SAP does not agree or disagree with the content on the linked-to site, nor does SAP warrant the availability and correctness. SAP shall not be liable for any damages caused by the use of such content unless damages have been caused by SAP's gross negligence or willful misconduct. 

- Links with the icon : You are leaving the documentation for that particular SAP product or service and are entering an SAP-hosted Web site. By using such links, you agree that (unless expressly stated otherwise in your agreements with SAP) you may not infer any product claims against SAP based on this information. 

## **Videos Hosted on External Platforms** 

Some videos may point to third-party video hosting platforms. SAP cannot guarantee the future availability of videos stored on these platforms. Furthermore, any advertisements or other content hosted on these platforms (for example, suggested videos or by navigating to other videos hosted on the same site), are not within the control or responsibility of SAP. 

## **Beta and Other Experimental Features** 

Experimental features are not part of the officially delivered scope that SAP guarantees for future releases. This means that experimental features may be changed by SAP at any time for any reason without notice. Experimental features are not for productive use. You may not demonstrate, test, examine, evaluate or otherwise use the experimental features in a live operating environment or with data that has not been sufficiently backed up. 

The purpose of experimental features is to get feedback early on, allowing customers and partners to influence the future product accordingly. By providing your feedback (e.g. in the SAP Community), you accept that intellectual property rights of the contributions or derivative works shall remain the exclusive property of SAP. 

## **Example Code** 

Any software coding and/or code snippets are examples. They are not for productive use. The example code is only intended to better explain and visualize the syntax and phrasing rules. SAP does not warrant the correctness and completeness of the example code. SAP shall not be liable for errors or damages caused by the use of example code unless damages have been caused by SAP's gross negligence or willful misconduct. 

## **Bias-Free Language** 

SAP supports a culture of diversity and inclusion. Whenever possible, we use unbiased language in our documentation to refer to people of all cultures, ethnicities, genders, and abilities. 

How to Schedule Report Execution and Mailing in SAP Business One **Important Disclaimers and Legal Information** 

PUBLIC **17** 

www.sap.com/contactsap 

© 2026 SAP SE or an SAP affiliate company. All rights reserved. 

No part of this publication may be reproduced or transmitted in any form or for any purpose without the express permission of SAP SE or an SAP affiliate company. The information contained herein may be changed without prior notice. 

Some software products marketed by SAP SE and its distributors contain proprietary software components of other software vendors. National product specifications may vary. 

These materials are provided by SAP SE or an SAP affiliate company for informational purposes only, without representation or warranty of any kind, and SAP or its affiliated companies shall not be liable for errors or omissions with respect to the materials. The only warranties for SAP or SAP affiliate company products and services are those that are set forth in the express warranty statements accompanying such products and services, if any. Nothing herein should be construed as constituting an additional warranty. 

SAP and other SAP products and services mentioned herein as well as their respective logos are trademarks or registered trademarks of SAP SE (or an SAP affiliate company) in Germany and other countries. All other product and service names mentioned are the trademarks of their respective companies. 

Please see https://www.sap.com/about/legal/trademark.html for additional trademark information and notices. 

**==> picture [58 x 30] intentionally omitted <==**

