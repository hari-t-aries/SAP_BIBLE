6/8/26, 6:11 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:11:22 GMT+0000
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

6/8/26, 6:11 AM
Service
If your company provides support services to its customers, or receives support services from your vendors, you can manage all
activities related to those services using the Service component.
For example, you can:
Manage the interaction between service representatives and business partners.
Maintain information on service contracts, items, and serial numbers as well as customer complaints and inquiries.
Monitor and manage the activities of your service department by using standard and custom reports that assist managers
and support staff with their daily work.
Optimize the potential of your sales and service departments and generate additional revenue by supporting business
functions such as:
Service operations
Service contract management
Service planning
Tracking of customer interaction activities
Customer support
Management of opportunities
Create a knowledge base of solutions for issues raised by your customers. You can manage this knowledge base according
to your items; therefore, when a certain problem reoccurs, you can reduce the time required to solve it by searching for
solutions by item.
To support your services operations, you work with the following service tools in SAP Business One.
Please note that image maps are not interactive in PDF outputs.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:11 AM
The graphics above are interactive. Hover over each area for a short description. Choose the highlighted areas for more
information.
Working with Service Calls
You use service calls to manage service and support activities that you provide to your customers. Also, you can track services that
your company receives. For example, you can track customers’ complaints and problems, provide solutions to these problems, and
view the activities and expenses related to these problems. These services may be covered by a service contract or warranty, or a
customer can pay for the service call. You can open a service call for an item even if a corresponding equipment card or a service
contract has not been defined.
The following image is interactive. Hover over each area for a description. Choose the highlighted areas for more information.
Please note that image maps are not interactive in PDF outputs.
Service Call Window
Use this window to open or update a service call for an item group, a business partner, or a serial number.
To access the general area, from the SAP Business One Main Menu, choose Service Service Call .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area Fields
Service Call Type
Specify the service call type.
Sales type indicates that the service is provided to your customer.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:11 AM
Purchasing type indicates that the service is provided by your vendor.
Business Partner Code, Business Partner Name
Specify the code and the name of the business partner that opened the service call. If a business partner deviates from credit or
commitment limits, a warning message is displayed.
If you specify the Serial Number or Mfr Serial No. before the Business Partner Code and the number is linked to a business
partner through an equipment card, the Business Partner Code will be filled in automatically.
If there is more than one business partner in the equipment card, you need to select one from a list of linked business partners. To
view or select from other business partners, clear the Serial Number or Mfr Serial No. field.
For more information about enabling adding multiple business partners to an equipment card, see Document Settings: Per
Document Tab.
 Note
If you choose an item first, and the business partner does not have a valid contract for this item, SAP Business One displays a
warning message before you add the item to the service call.
Contact Person
Specify the name of the person who made the service call.
Telephone No.
If a telephone number is defined for the specified contact person, it is displayed automatically. Otherwise, the telephone number
defined for the business partner in the Business Partner Master Data window is displayed.
No.
Field on the left: name of the numbering series. Specify a series.
Field on the right: the number of the service call.
Call Status
There are three default service call statuses:
Open: The initial status of a service call after it is created. It awaits service engineers to work on it.
Pending: The issue is acknowledged but the call has not yet been resolved or closed. This could be due to needing approval,
needing further information, waiting for parts, or any other reason that might delay the completion of the service call.
Closed: The service call is resolved.
Select one of the default statuses for the service call or define a new status.
The call status influences the relevant service reports.
To define a custom status, choose Define New. The Service Call Statuses - Setup window opens. To hide a user-defined status,
deselect the Active checkbox.
 Note
You cannot add a service call with such hidden options or update such hidden options of an existing service call through the
Data Interface.
You cannot set a service call to Closed if you have not attached a solution or entered a resolution.
Call ID
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:11 AM
Automatically defined sequential number that identifies the service call
Business Partner Ref. No.
Displays the business partner reference number, if it exists.
Mfr Serial No.
Specify the manufacturer's serial number. If you have entered the Serial Number, the manufacturer's serial number is displayed
automatically.
Serial Number
Specify the serial number related to the service call, if required.
 Note
You can select only serial numbers recorded in equipment cards having Active or Loaned statuses and which are related to the
selected business partner.
Created On, Closed On
Date and time when the service call was created or closed. If you reopen a closed service call, the closed date and time will be
deleted.
 Note
You can manually edit the Created On and Closed On fields if you have full authorization. To set authorizations, choose
Administration System Initialization Authorizations . In the General Authorizations area, expand Service Special
Service Call Authorization Edit Created On/Closed On .
The date and time in the Created On filed must be earlier than Closed On.
All manual changes are recorded at the History tab of the Service Call window.
Contract No.
Number of the service contract linked to the selected serial number. When there is no contract for the item, the field contains a
value of No Contract.
If you create equipment cards manually, and you created a service contract after you created a service call for the same business
partner and the same item, then when you go back to the service call you get a message asking if you want to connect the service
call to the newly created service contract.
 Note
After you have responded to a service call, you can no longer change the contract number.
End Date
Expiration date of the service contract
Related Information
Working with Service Calls
Creating and Updating Service Calls
Service Call: General Tab
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:11 AM
Use this tab to enter or update general information about a service call, including the type of problem and the technician assigned
to the service call.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the General tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab Fields
Origin
Specify how an assistance and support request is received from customers or sent to vendors.
There are three default service call origins:
Email: Service requests are received or sent by emails.
Telephone No.: Service requests are received or sent by phone calls.
Web: Service requests are received or sent online from webpages.
You can define custom origins, but you cannot delete the default origins. To define a custom origin, choose Define New. The Define
Service Call Origins - Setup window opens. To hide a user-defined origin, deselect the Active checkbox.
 Note
You cannot add a service call with such hidden options or update such hidden options of an existing service call through the
Data Interface.
Problem Type
Specify the type of the reported problem.
To define a custom problem type, choose Define New. The Define Service Call Problem Types - Setup window opens. To hide a
user-defined problem type, deselect the Active checkbox.
 Note
You cannot add a service call with such hidden options or update such hidden options of an existing service call through the
Data Interface.
Problem Subtype
Specify the subtype of the reported problem.
To define a custom problem subtype, choose Define New. The Define Service Call Problem Subtypes - Setup window opens. To
hide a user-defined problem subtype, deselect the Active checkbox.
 Note
You cannot add a service call with such hidden options or update such hidden options of an existing service call through the
Data Interface.
Call Type
Specify the type of the service call.
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:11 AM
Use this field to classify your service calls, for example, First Level, Technician, Field Repair.
To define a custom type, choose Define New. The Define Service Call Types - Setup window opens. To hide a user-defined type,
deselect the Active checkbox.
 Note
You cannot add a service call with such hidden options or update such hidden options of an existing service call through the
Data Interface.
Technician
If the service call requires a technician, specify the code of the assigned technician.
You can select any company employee defined as technician from the Roles table of the Membership tab in Human Resources
Employee Master Data .
Handled by
Specify a user responsible for handling the service call. When a service call is created, this option is selected by default and it is the
user who creates the service call.
You can select a different user, for example, if you need to forward the service call for advanced handling. The new assignee
receives an alert regarding the forwarded service call via the internal messaging system.
 Note
When you create a new service call, you select either an assignee or a queue. When you update a service call, you must allocate
it to a specific assignee.
Queue
Select this option if you use queue to manage service calls.
You can define queues under Administration Setup Service Queues .
 Note
When you create a new service call, you select either an assignee or a queue. If a service call is assigned to a queue, it must be
assigned to an assignee to allow updates and further handling.
Response
By
The last date and hour you are committed to respond to the service call. This date is calculated according to the Response
Time field and coverage of the service contract (from the Coverage tab in Service Service Contract ).
On
The date and time of the first response to the service call. SAP Business One considers any of the following a response:
Creating and closing a telephone call or meeting activity
Adding a resolution or solution to the service call
Resolution
Time and date by which you must resolve the problem. This date is calculated according to the resolution time and coverage of the
service contract.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:11 AM
By
The last date and hour you are committed to provide a resolution for the service call. This date is calculated according to
the Resolution Time field and coverage of the service contract (from the Coverage tab in Service Service Contract ).
On
The date and time of the resolution provided for the service call. SAP Business One considers it a resolution when you add a
resolution or a solution to the service call.
 Note
Deleting solutions from the Solution tab or the text from the Resolution tab clears the Resolution On field. However, the
Response On field is not cleared since you have responded to the service call but have not yet resolved it.
More Information
Working with Service Calls
Service Contract: General Tab
Service Call Origins - Setup Window
Use this window to define different origins of the service call.
To open this window, from the SAP Business One Main Menu, choose Service Service Call . On the General tab, from the
drop-down box of the Origin field, choose Define New.
More Information
Service Call: General Tab
Service Call Problem Types - Setup Window
Use this window to define different types of problem that was reported.
To open this window, from the SAP Business One Main Menu, choose Service Service Call . On the General tab, from the
drop-down box of the Problem Type field, choose Define New.
More Information
Service Call: General Tab
Service Call Types - Setup Window
Use this window to define different types of service calls.
To open this window, from the SAP Business One Main Menu, choose Service Service Call . On the General tab, from the
drop-down box of the Call Type field, choose Define New.
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:11 AM
More Information
Service Call: General Tab
Service Call Statuses - Setup Window
Use this window to define statuses for the service call.
To open this window, from the SAP Business One Main Menu, choose Service Service Call . From the drop-down box of the
Call Status field, choose Define New.
More Information
Service Call Window
Service Call: Business Partner Tab
Use this tab to view all necessary details of the business partner for handling the service call.
You can edit the fields of this tab, but the changes do not automatically update the fields in business partner master data.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Business Partner tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Business Partner Tab Fields
Ship To, Bill To
Displays the ship-to address, bill-to address, and additional description as defined in the business partner master data. If required,
you can change the address and the description.
 Note
You can use the ellipsis (...) button to edit addresses.
Territory
Displays the territory to which this business partner belongs. If required, you can change it.
Contact Person, Tel 1, Tel 2, Mobile Phone, Fax, E-mail
Displays the communication details of the business partner.
BP Project
The project associated with the business partner.
Distribution Rule
The distribution rule according to which the service call will be allocated to cost centers.
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:11 AM
More Information
Working with Service Calls
Business Partner Master Data Window
Service Call: Remarks Tab
Use this tab to specify a detailed description and any other remarks related to the service call. You can record more details about
the service call here than in the Subject field.
To access the tab, from the SAP Business One Main menu, choose Service Service Call and select the Remarks tab.
More Information
Working with Service Calls
Service Call: Activities Tab
Use this tab to specify new activities and to display existing activities, such as tasks and meetings, related to the service call.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Activities tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Activities Tab Fields
Date
Date on which the activity was created
Time
Time at which the activity was created
Handled by
User or employee assigned to the activity
New Activity
Date on which the activity took place or is to take place
Content
The text inserted in the Content tab of the activity.
[Attachment]
Displays whether there is an attachment related to the activity. To open an attachment, click the icon in the relevant row.
[Document]
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:11 AM
Displays whether there is a document linked to the activity. To open a linked document, click the icon in the relevant row.
Activity
Opens a window in which you can record a new activity related to this service call.
You can also right-click the activities table and choose Add Row.
More Information
Working with Service Calls
Service Call: Solutions Tab
Use this tab to add new solutions for the problem or to link to existing ones. All the solutions are recorded in the Knowledge Base
Solution window. Therefore, the next time the problem comes up, technicians are aware of possible solutions. As a result, the time
required to solve the problem might be reduced. A service call can have more than one solution.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Solutions tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Solutions Tab Fields
Solution
Description of the solution to the problem
Created on
The date on which the solution was added to the Solutions Knowledge Base.
Owner
Code of the employee who created the solution
Status
There are three default solution statuses:
Internal: A solution is in the internal processing stage inside a department or organization.
Publish: A solution has been made publicly available and is accessible to all users within a company.
Review: A solution is going through a review process to ensure quality and correctness before it is published.
Select one of the default statuses for the solution or define a new status.
To define new statuses, from the dropdown list, choose Define New. The Solution Statuses – Setup window opens. You specify the
name and description of the new status and update the status information.
To hide a user-defined status, deselect the Active checkbox.
Handled by
Employee responsible for the service call
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:11 AM
Recommend
Opens the Recommended Solutions window, in which you can view a list of solutions used in similar service calls.
New
Opens the Solutions Knowledge Base window, in which you can create a new solution for the problem.
More Information
Working with Service Calls
Solutions Knowledge Base Window
Recommended Solutions Window
Recommended Solutions Window
Use this window to display a list of recommended solutions to the service call problem and to select relevant solutions. The
selected solutions appear in the Service Call window on the Solutions tab.
To open the window, from the SAP Business One Main Menu, choose Service Service Call , select the Solutions tab, and
choose the Recommend button.
To link a solution to the service call, select a row or a number of rows and choose the Choose button.
 Note
You can remove a solution from a service call using one of the following methods:
Right-click a solution row and choose Delete Row.
Select a row and from the menu bar choose Data Delete Row .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Recommended Solutions Window Fields
Created on
The date on which the solution was added to the Solutions Knowledge Base.
Owner
Employee who created the solution
Solution
Description of the solution to the problem
Status
There are three default solution statuses:
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:11 AM
Internal: A solution is in the internal processing stage inside a department or organization.
Publish: A solution has been made publicly available and is accessible to all users within a company.
Review: A solution is going through a review process to ensure quality and correctness before it is published.
Select one of the default statuses for the solution or define a new status.
To define new statuses, from the dropdown list, choose Define New. The Solution Statuses – Setup window opens. You specify the
name and description of the new status and update the status information.
To hide a user-defined status, deselect the Active checkbox.
Find
Opens the Solutions Knowledge Base window, in which you can look for additional solutions other than the recommended ones.
Choose
Includes the solution you selected in the service call.
More Information
Working with Service Calls
Service Call: Solutions Tab
Solutions Knowledge Base Window
Service Call: Related Documents Tab
Use this tab to view documents related to the service call, such as invoices for parts (items), working hours (labor), and travel
hours.
You can specify the following item types:
Items used for repairing broken parts
Items that are returned by the business partner
Items that are transferred to the technician to solve the problem
Items that the technician returned to the warehouse
You can specify working hours for the time the technician worked at the business partner site and the travel hours required
for the technician to travel to the business partner site and back to the office.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Related Documents
tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Related Documents Tab Fields
Date
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:11 AM
Date on which the document was created
SN
Serial number of the item provided to the business partner and a link to the Serial Number Transaction Report window
Quantity
The number of items that appear in the document
From Whse
Warehouse from which the item was received
To Whse
Warehouse to which the item was delivered
Display All Documents
If a service call is of sales type, the Related Documents tab displays only sales documents by default. Only when you choose
Details New Document and add new A/P documents or inventory transfer documents, and you select Display All Documents,
will all documents be displayed.
The same applies to purchasing type service calls.
Details
Opens the Service Call Related Documents window and displays the detailed expenses for the service call.
Related Information
Working with Service Calls
Service Call: Related Documents Window
Adding a Related Document
Service Call: Related Documents Window
Use this window to add and display the detailed expenses associated with the service call, that is, the expenses related to the
items, and to labor and travel.
To open the window, from the SAP Business One Main Menu, choose Service Service Call . On the Related Documents tab,
choose Details.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Inventory Items Fields
Transfer to Tech.
Number of items the technician received from the warehouse to complete the service call
Delivered
Number of items delivered to the customer
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:11 AM
Returned from Tech.
Number of items the technician returned to the warehouse after completing the service call
Returned
Number of items that were returned by the business partner (using returns or credit memo documents)
Bill
Defines whether to charge the customer for the item parts.
Non-Inventory Items, Labor and Travel Fields
Bill
Defines whether to charge the customer for non-Inventory items, labor and travel.
Related Information
Service Call: Related Documents Tab
Adding a Related Document
Adding a Related Document
Use this window to add one of the documents described below and to specify inventory transfer and expense details for the service
call.
To open this window, from the SAP Business One Main Menu, choose Service Service Call . On the Related Documents tab,
choose Details and then choose New Document.
Document Types
Transferred to Technician
To create an inventory transfer from the warehouse to the technician, select this document type.
 Note
If you defined a warehouse for each technician and you want to document the items that you delivered to the technician for the
service call, in the field To Warehouse, choose the warehouse of the technician.
Returned from Technician
To create an inventory transfer from the technician to the warehouse, select this document type.
 Note
If you defined a warehouse for each technician and you want to document the items that the technician returned, in the field
From Warehouse, choose the warehouse of the technician.
Sales Quotation
To create a sales quotation document, select this document type.
Sales Order
To create a sales order, select this document type.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:11 AM
Delivery
To create a delivery document, select this document type.
Return Request
To create a return request document, select this document type.
Returns
To create a return document, select this document type.
 Note
If you record a return document with a serial number that is defined as Active on the Equipment Card, the status of the
Equipment Card changes to Returned.
A/R Invoice
To create an A/R invoice, select this document type.
A/R Credit Memo
To create an A/R credit memo, select this document type.
You can also add the following type of A/P documents:
Purchase Quotation
Purchase Order
Goods Receipt PO
Goods Return Request
Goods Return
A/P Invoice
A/R Credit Memo
Related Information
Service Call: Related Documents Window
Service Call: Resolution Tab
Use this tab to specify information about the resolution of the problem. You can enter any additional information about the
resolution on the Solutions tab.
To access the tab, from the SAP Business One Main menu, choose Service Service Call and select the Resolution tab.
More Information
Working with Service Calls
Service Call: History Tab
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:11 AM
Use this tab to display all actions related to the service call. All updates and changes appear under the corresponding date and
time.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the History tab.
The number of updates displayed in the History tab is determined by the setting of the History / Log field on the Services tab, in
Administration System Initialization General Settings . For more information, see General Settings: Services Tab.
The History tab displays the following updates:
Service call created
Response due by
Response added
Resolution due by
Resolution added
Reassigning
Status changed
Priority changed
Solution added
Solution removed
Activity added
Service call closed
Expenses document added
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
History Fields
Date of Update, Update Time
The date and time on which the service call record was updated.
Description
Description of the update, for example, service call created, activity added, and so on
Previous Value
Previous value, if any, of an updated field
New Value
New value of the updated field
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:11 AM
Working with Service Calls
Service Call: Scheduling Tab
Use this tab to schedule service calls.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Scheduling tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Scheduling Tab Fields
Start Time
Specify the date and time for the start of the activity. By default, the system date and time are displayed.
End Time
Specify the time for the conclusion of the activity. By default, the end time is set to fifteen minutes past the start time.
 Note
You cannot set the end time to a time earlier than the start time.
Duration
Specify the length of time you expect the activity to take. By default, the duration is set to fifteen minutes. If you change it, the end
time is updated accordingly.
 Note
To specify hours, type the number of hours followed by the letter H.
Address
Specify the address details of the meeting location.
 Note
To automatically specify the business partner’s default Ship to address, select Business Partner Address in the Meeting
Location field.
Reminder
Select to display a reminder in the Messages/Alert Overview window prior to the time set for the meeting.
Specify the reminder in minutes or hours. To specify hours, type the number of hours followed by the letter H.
After you select the checkbox, an alert will pop up to notify the Service Call Handled By user and the service call technician that
the service call is scheduled.
Display in Calendar
Select the checkbox to display the service call in the Calendar window. To open the calendar, choose .
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:11 AM
The scheduled service calls is displayed in the Calendar for the relevant service call technician and to the service call handled by
user.
More Information
Working with Service Calls
Service Call Window
Calendar Window
Service Call: Attachments Tab
Use this tab to attach relevant files, using the standard Browse, Display, and Delete functions. You can also add attachments by
dragging and dropping files directly onto the tab. Acceptable file types include Microsoft Excel files, images, Web links, and so on.
 Note
To protect your privacy, it is recommended that you remove any Exchangeable Image File Format (EXIF) information from your
images before uploading them.
To access the tab, from the SAP Business One Main Menu, choose Service Service Call and select the Attachments tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Attachments Tab Fields
Target Path
The destination folder in which the attachment is stored.
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
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
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:11 AM
Related Information
Working with Service Calls
General Settings: Path Tab
Creating and Updating Service Calls
Context
You can create an initial service call or update a service call to record tasks, meetings, notes, or expenses related to the call, or to
enter a solution to the service problem.
 Note
You can also use the Business Partner Master Data window to display the service calls recorded for a business partner. Find
the relevant business partner and choose Related Service Calls.
Typically a customer who contacts you for service already has a service contract with your company for an item or group of items,
or the item is covered by a warranty. Additionally, you have created customer equipment cards for the items for which the
customer is requesting service. However, you can create a service call without a contract or warranty, although you will get a
warning message when you save the service call.
You can create a service call only for serial number items with an Active or Loaned status. You get an error message for serial
number items with one of the following statuses:
Returned
Terminated
In repair lab
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
The Service Call window opens.
2. In the general area, specify the business partner code, the item number, and (if necessary) the serial number of the item. In
the Subject field, enter a short problem description.
You can also set the status of the service call. For example, after you have entered a solution or a resolution, you can set the
status to Closed.
If you specify the Serial Number or Mfr Serial No. before the Business Partner Code and the equipment card is linked to a
business partner, the Business Partner Code will be filled in automatically.
If the equipment card is linked to multiple business partners, you need to select one from a list of linked business partners.
To view or select from other business partners, clear the Serial Number or Mfr Serial No. field.
For more information about enable adding multiple business partners to an equipment card, see Document Settings: Per
Document Tab.
3. On the General tab, specify details about the origin of the problem, its type, and the employee and technicians who are
responsible for the service call.
4. On the Business Partner tab, view the necessary details for handling the service call.
5. On the Remarks tab, specify any important additional information regarding the service call.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:11 AM
6. On the Activities tab, specify a new activity for the service call.
7. On the Solutions tab, search for the recommended solution for the problem or specify a new solution.
8. On the Related Documents tab, specify, for example, the expenses of the service call.
9. On the Resolution tab, specify a description of the resolution to the service call problem.
10. On the History tab, view the updates and the changes made in the service call.
11. To save the service call, choose Update and OK.
Related Information
Working with Service Calls
Service Call Window
Managing Activities Related to Service Calls
Context
You can create a new activity or view existing activities related to a service call for a business partner.
 Note
An activity can be attached to only one service call.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
The Service Call window opens.
2. In the general area, search for a specific service call by specifying the business partner code, the item number, or the serial
number of the item.
3. Select the Activities tab.
4. To record a new activity for the business partner, choose the Activity button.
The Activity window opens. For information, refer to Activity Window.
Related Information
Service Call: Activities Tab
Creating and Updating Service Calls
Searching for and Creating Solutions
Context
You can view existing solutions or create a solution related to a service call for a business partner.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:11 AM
The Service Call window opens.
2. In the general area, search for a specific service call by specifying the business partner code, the item number, or the serial
number of the item.
3. Select the Solutions tab.
4. On the Solutions tab you can:
Record a new solution that relates to the service call. Choose the New button to open the Solutions Knowledge
Base window.
For information, see Solutions Knowledge Base Window.
Display all the prior solutions of previous service calls that relate to the same item or item group or which have the
same Problem type. Choose the Recommend button. You can attach those solutions to the current service call.
For information, see Recommended Solutions Window.
Related Information
Service Call: Solutions Tab
Creating and Updating Service Calls
Entering Expenses for Service Calls
Context
If the business partner does not have a service contract with your company, or if replacement parts, travel, or other costs are not
covered by a warranty or service contract, you need to record the expenses for a service call. These expenses are used to create an
invoice.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
The Service Call window opens.
2. In the general area, search for a specific service call by specifying the business partner code, the item number, or the serial
number of the item.
3. Select the Related Documents tab.
4. To add new expenses or to view additional details regarding the expenses related to the service call, choose Details.
The Service Call Related Documents Details window opens.
5. You can view the two types of items that have been defined for expenses.
In the Inventory Items table, you can view all the items defined as Item type in the documents related to the service
call ( Inventory Item Master Data , the Type field).
In the Non-Inventory Items, Labor and Travel table, you can view all the non-inventory items and those defined as
Labor or Travel in the documents related to the service call ( Inventory Item Master Data window , the Type
field).
6. To record additional expenses related to the service call, choose New Document.
The Document Type window opens.
Choose the type of document you want to add to the Related Documents tab in the service call, and choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:11 AM
After you add the corresponding document, a new row including the document details is added to the Service Call Related
Documents Details window.
7. To save the changes, choose Update.
Related Information
Adding a Related Document
Service Call: Related Documents Window
Service Call: Related Documents Tab
Creating and Updating Service Calls
Viewing the History of Service Calls
Context
You can see all activities taken by your service representatives for a specific service call.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
The Service Call window opens.
2. In the general area, search for a specific service call by specifying the business partner code, the item number, or the serial
number of the item.
3. From the Tools menu, choose Change Log.
The Change Log window opens.
4. To review detailed information about the changes that were made to the service call, do one of the following:
To view all changes since a specific change was made, click a row and choose Show Differences.
To view changes between two specific changes, click the two rows and choose Show Differences.
 Note
An information change that is automatically created by SAP Business One and does not affect any field is displayed in
green.
The number of updates displayed in the Change Log window is determined by the setting in the History / Log field, in
Administration System Initialization General Settings , Services tab.
Related Information
Creating and Updating Service Contracts
Service Call: History Tab
Printing Service Calls for Technicians
Context
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:11 AM
You can print service calls and technician forms using default print layouts. While at the business partner site, the technician can
used the printed form to view the details of a service call. The technician can write up the solution, the items that were replaced
while at the business partner site, and the travel and labor hours at the business partner site. In addition, the technician can use
the form to sign up the business partner as a reference for the visit.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Call .
The Service Call window opens.
2. In the general area, search for a specific service call by specifying the business partner code, the item number, or the serial
number of the item.
3. From the Tools menu, choose Layout Designer... or click in the toolbar.
4. Choose the preferred printing layout.
5. From the File menu, choose Print or click in the toolbar.
6. Select which document to print Technician Form or Service Call, and choose OK.
Related Information
Printing in SAP Business One
Working with Equipment Cards
Equipment cards form the database that contains all serial number items that you sold or purchased and for which service can be
provided. You can track the history of a specific serial number from the day you sold or purchased the item and throughout its
entire service period.
The equipment card contains information such as:
Location of the item at which you provide or receive service
Service calls related to the item
Service contracts that cover the item
Sales information
Inventory transaction data
You have the following options for creating equipment cards:
Enable equipment cards to be created automatically for every sold or purchased item that is managed by serial numbers.
Specify the item data (serial number data) manually in the Equipment Card window.
 Note
If your customer purchased an item, such as equipment, from another source and needs only support or service from your
company for this item, no sales transaction takes place in SAP Business One. For this item, you create the equipment card
manually in the Equipment Card window. You view such items only in the Service module and not in the Inventory module.
To open the Equipment Card window, choose Service Equipment Card .
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:11 AM
The following image is interactive. Choose the highlighted areas for more information on the Equipment Card Window and its
functions.
Please note that image maps are not interactive in PDF outputs.
Equipment Card Window
Use this window to view information about serial numbers that were automatically assigned from the delivery document or to add
serial numbers manually. You can also update the details of serial numbers.
To access the general area, from the SAP Business One Main Menu, choose Service Equipment Card .
 Note
You have to specify a number in at least one of the serial number fields.
The Mfr. Serial No. and the Serial Number fields are unique numbers. If equipment cards are created automatically when a
delivery or an A/R invoice is created, the serial numbers are considered unique as well. To ensure that the serial numbers are
indeed unique, choose Administration System Initialization General Settings , select the Items subtab of the
Inventory tab. In the Unique Serial Numbers by dropdown list, select the unique serial number option.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area Fields
Equipment Card Type
Specify the equipment card type.
The Sales type indicates that the service is provided to your customer.
The Purchasing type indicates that the service is provided by your vendor.
The Sales & Purchasing type indicates that you provide the service to your customers and your vendors provide the service
to you for the same item. You can choose this type if you are a third party to your customers and vendors.
To enable the Sales & Purchasing type, while at the same time enabling the addition of more than one business partner to
the same equipment card of type Sales and of type Purchasing, select Add Multiple Business Partners to an Equipment
Card for equipment cards in the Document Settings Per Document tab.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:11 AM
For more information, see Document Settings: Per Document Tab.
Mfr. Serial No.
Specify the unique manufacturer ID of the sold or purchased item.
This field is required when Mfr. Serial No. is selected for the Unique Serial Numbers By field in the General Settings Inventory
tab.
Serial Number
Specify the unique ID number of the sold or purchased item.
This field is required when Serial Number is selected for the Unique Serial Numbers By field in the General Settings Inventory
tab.
Status
Specify the current status of the item:
Active
The item was shipped.
Returned
The item was returned to the warehouse.
Terminated
The item is not in use and therefore is not eligible for service. An equipment card defined as Terminated cannot be added to
a service contract or service call.
Loaned
The item is loaned to the business partner. You might use this status if you need to repair an item for the business partner,
and you loan the business partner a similar item until the original item is fixed. Specify the serial number of a loaned item in
the Previous SN field.
In Repair Lab
The item was returned for repair. If the business partner received a temporary replacement, this is displayed in the New SN
field. The item cannot be shipped to another business partner.
Previous SN
If an item is loaned as a replacement for an item that is currently being repaired, specify the serial number of the item being
repaired in the equipment card of the loaned item.
New SN
If an item is loaned as a replacement for an item that is currently being repaired, specify the serial number of the loaned item in the
equipment card of the item being repaired.
Business Partner Code
Specify the business partner code.
If you select Add Multiple Business Partners to an Equipment Card on the Per Document tab in the Document Settings window,
you can choose to select additional business partners:
If the equipment card type is Sales, you can select customers only.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:11 AM
If the equipment card type is Purchasing, you can select vendors only.
If the equipment card type is Sales & Purchasing, you can select both customers and vendors.
The first selected business partner automatically becomes the default business partner. The default business partner will be
displayed in the equipment card report and will become the default business partner when you choose You Can Also to create a
service call on the Transactions tab of the equipment card.
You can change the default business partner if you want to.
If the default business partner is inactive, you cannot save the equipment card successfully. If the default business partner is active
but one or more non-default business partners are inactive, you receive a confirmation message for each inactive business partner,
prompting you to decide whether to continue with the process.
Technician
Specify the technician responsible for the item.
 Note
Displays as default the technician specified in the business partner master data record ( Business Partners Business
Partner Master Data , General tab).
Territory
Choose a territory related to the business partner.
 Note
Default: the territory specified in the business partner master data record ( Business Partners Business Partner Master
Data , General tab).
Contact Person, Telephone No.
Select a contact person. The telephone number automatically appears if it is defined for the selected contact person. If there is no
telephone number for the contact person, the telephone number defined in the business partner master data record appears.
Related Information
Document Settings: Per Document Tab
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Address Tab
Equipment Card: Service Calls Tab
Equipment Card: Service Contracts Tab
Equipment Card: Sales Data/Purchasing Data Tab
Equipment Card: Transactions Tab
Equipment Card: Attachments Tab
Equipment Card: Address Tab
Use the Address tab to specify the location of the item for which you are providing service.
To access the tab, from the SAP Business One Main Menu, choose Service Equipment Card and select the Address tab.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:11 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Address Tab Fields
Location
Specify the location of the item with this serial number. Specifying the exact location can help technicians find the item within a
building.
More Information
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Service Calls Tab
Use this tab to view all service calls associated with the serial number.
To access the tab, from the SAP Business One Main Menu, choose Service Equipment Card and select the Service Calls tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Calls Tab Fields
Creation Date
The date in which the service call was created.
Subject
The subject specified in the service call.
Item No.
Number of the item for which the service call was created
SN
Serial number of the item for which the service call was created
Status
The current status of the service call.
You Can Also
Select whether to:
View Related Service Calls - you can view all service calls associated with the related business partner(s).
Create Service Call - you can create a new service call with the default business partner details.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:11 AM
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Service Contracts Tab
Use this tab to view the service contracts recorded for this business partner involving the item with the serial number.
To access the tab, from the SAP Business One Main Menu, choose Service Equipment Card and select the Service
Contracts tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Contracts Tab Fields
Contract
Unique contract identification number.
Start Date
Date on which the service contract became valid
End Date
Date on which the service contract expired
Service Type
Displays whether the contract is a warranty or a regular contract.
More Information
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Sales Data/Purchasing Data Tab
Use this tab to view sales or purchasing information related to the item.
To access the tab, from the SAP Business One Main Menu, choose Service Equipment Card . For sales service call type,
select the Sales Data tab. For purchasing service call type, select the Purchasing Data tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Sales Data/Purchasing Data Tab Fields
Buyer Code/Name
Specify the code and the name of the customer who bought the item.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:11 AM
The difference between the Customer Code in the general area of this window and the Buyer Code here is as follows:
The Customer Code refers to the company's direct customer, for example, a distributor.
The Buyer Code refers to the actual end customer.
In a typical service operation, the following scenarios occur:
1. A manufacturer (our company) conducts a bulk sale of items to its distributor (the Customer Code field)
2. The distributor sells the item to an end customer (the Buyer Code field)
3. The end customer (buyer) registers the item with the manufacturer (our company) to avail of free services during the
warranty period.
The manufacturer (our company) issues A/R invoices to the distributor (in the Customer Code field). The distributor in turn
issues A/R invoices to the end customer (buyer). Although the manufacturer does not contact the end customer directly during
the sales process, the manufacturer still needs to maintain the information about the end customer in order to be able to link
the end customer with the distributor. This enables the manufacturer to determine whether the item is from an authorized
distributor and, therefore, whether service can be rendered for it.
Delivery
Number of the delivery document with which the item was shipped to the customer, with a link to the delivery document
Invoice
Number of the A/R invoice document by which the customer was invoiced for the purchase item, with a link to the A/R invoice
document
More Information
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Transactions Tab
Use this tab to view all inventory transactions associated with the serial number.
To access the tab, from the SAP Business One Main Menu, choose Service Equipment Card and select the Transactions
tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Transaction Tab Fields
Trans. No.
Number of the inventory transaction
Source
Type of inventory transaction, for example, IN (A/R invoice) or Out (delivery)
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:11 AM
Document No.
Number of the document associated with the transaction
Row No.
Row of the transaction in the sales or purchasing document
G/L Acct/BP Code
Code of the G/L account or business partner associated with the transaction
G/L Acct/BP Name
Name of the G/L account or business partner associated with the transaction
Direction
Displays either the incoming (In) or outgoing (Out) transaction.
More Information
Creating, Updating, and Deleting Equipment Cards
Equipment Card: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:11 AM
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
Creating, Updating, and Deleting Equipment Cards
General Settings: Path Tab
Automatically Created Equipment Cards
Equipment cards can be created automatically when A/R invoices or deliveries are created. Use the automatic creation method
when the customer purchases both equipment and service for the item from your company.
When using this method, if you create an A/R invoice or delivery for an item with serial number management, SAP Business One
creates a corresponding equipment card automatically. The Mfr Serial No. and the Serial Number values for this equipment card
are taken from the serial number recorded in the inventory transaction.

 Note
To enable the automatic creation of equipment cards, from the SAP Business One Main Menu, choose  Administration
 System Initialization    General Settings , select the Inventory tab, and choose the option Auto. Create Equipment Card.
For more information, see Enabling the Automatic Creation of Equipment Cards.
Scenarios
The following table describes various scenarios that can result from an attempt to automatically create an equipment card from a
document, either a delivery or an A/R invoice, if an equipment card with the same serial number already exists in SAP Business
One.
Additional Information to the Status of Existing Equipment New Equipment Card Created? Additional Information
| Scenario | Card   |     |      |
| -------- | ------ | --- | ---- |
| None     | Active | No  | None |
The document is recorded for a Returned No The status of the existing
| customer that is linked to an |     |     | equipment card is changed to |
| ----------------------------- | --- | --- | ---------------------------- |
| existing equipment card.      |     |     | Active.                      |
The document is recorded for a Returned Yes, for the new customer The status of the former
| different customer than the one  |     |     | equipment card is changed to |
| -------------------------------- | --- | --- | ---------------------------- |
| linked to the existing equipment |     |     | Terminated.                  |
card.
The document is recorded for Terminated No You can change the status of
| the same customer that is        |     |     | the equipment card manually to |
| -------------------------------- | --- | --- | ------------------------------ |
| linked to the existing equipment |     |     | Active.                        |
card.
The document is recorded for a Terminated Yes, for the new customer None
different customer than the one
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:11 AM
Additional Information to the Status of Existing Equipment New Equipment Card Created? Additional Information
Scenario Card
linked to the existing equipment
card.
None Loaned No None
The document is recorded for In Repair Lab No The status of the existing
the same customer that is equipment card is changed to
linked to the existing equipment Active.
card.
The document is recorded for a In Repair Lab No None
different customer than the one
linked to the existing equipment
card.
Related Information
Working with Equipment Cards
Creating, Updating, and Deleting Equipment Cards
Document Settings: Per Document Tab
Creating, Updating, and Deleting Equipment Cards
 Note
This topic contains an SAP Note that explains additional information.
You create, update, and delete equipment cards. For example, you can update an equipment card by adding attachments, changing
the status, or assigning the related item to a different business partner. You can delete an equipment card that is not linked to an
A/R invoice or delivery and for which there has been no activity.
Procedure
Manually Creating an Equipment Card
1. From the SAP Business One Main Menu, choose Service Equipment Card .
The Equipment Card window opens.
2. Switch to Add mode. For more information, see Working in Add Mode.
3. In the general area, specify the business partner information and the serial number. Choose the status of the equipment
card and enter details for the technician and territory. For more information, see Equipment Card Window.
4. On the Address tab, specify the address details for the business partner who obtained the item with this serial number. For
more information, see Equipment Card: Address Tab.
5.
On the Sales Data tab, specify the buyer code, delivery, and sales invoice details, if available in SAP Business One.
For more information, see Equipment Card: Sales Data Tab.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:11 AM
On the Transactions tab, specify the purchasing transactions. For more information, see Equipment Card:
Transactions Tab.
 Note
You can browse to existing equipment cards and link relevant documents after you create them.
6. On the Attachments tab, add an attachment, if necessary.
For more information, see Equipment Card: Attachments Tab
7. To save the equipment card, choose Add.
Viewing and Updating an Existing Equipment Card
1. From the SAP Business One Main Menu, choose Service Equipment Card .
The Equipment Card window opens.
2. Switch to Find mode. For more information, see Working in Find Mode.
3. In the general area, in the Mfr. Serial No. or Serial Number field, specify the complete or partial serial number and choose
Find.
The equipment card you want to view or update is displayed.
4. View or make the necessary changes to the equipment card.
You can switch the Equipment Type from Sales or Purchasing to Sales & Purchasing. If you want to switch from Sales &
Purchasing to Sales or Purchasing, make sure all additional vendors or customers are removed from the equipment card,
respectively.
 Note
You can delete the serial number from the Edit menu. You can only delete serial numbers with no history information.
 Note
For more information to change customer code, see SAP Note 1957052 .
5. To save the changes, choose the Update button.
Deleting an Equipment Card
 Note
You can delete an equipment card that contains a serial number if the following conditions are met:
The customer equipment card is not linked to an A/R invoice or delivery.
The equipment card does not have a history of service calls or valid service contracts.
1. From the SAP Business One Main Menu, choose Service Equipment Card .
The Equipment Card window opens.
2. Switch to Find mode.
For more information, see Working in Find Mode.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:11 AM
3. In general area, in the Mfr. Serial No. or Serial Number field, specify the complete or partial serial number and choose Find.
The equipment card you want to delete is displayed.
4. Choose one of the following alternatives:
From the Data menu, choose Remove.
Right-click the Equipment Card window and choose Remove.
Tracking Changes and Reviewing the History of an Equipment Card
1. From the SAP Business One Main Menu, choose Service Equipment Card .
The Equipment Card window opens.
2. Switch to Find mode.
3. In general area, in the Mfr. Serial No. or Serial Number field, specify the complete or partial serial number and choose Find.
The equipment card is displayed.
4. From the Tools menu, choose Change Log.
The Change Log window opens.
5. To review detailed information of the changes that were made in specific instances, choose one of the following:
To view all changes since a specific instance was created, click the instance row and choose Show Differences.
To view changes between two specific instances, click the two instance rows and choose Show Differences.
 Note
An information change that is automatically created by SAP Business One and does not affect any field is
displayed in green.
The number of updates displayed in the Change Log window is determined by the setting in the History / Log
field, on the Services tab in Administration System Initialization General Settings .
Related Information
Working with Equipment Cards
Automatically Created Equipment Cards
Assigning an Item to a Different Business Partner
In some cases, items managed by serial numbers are transferred to a different business partner. If the original business partner
has a equipment card, you need to replace the current business partner with another business partner .
Procedure
If the equipment card has no service calls connected to it, proceed as follows:
1. From the SAP Business One Main Menu, choose Service Equipment Card .
2. Open the existing equipment card and change the Business Partner Code field.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:11 AM
3. To save the changes, choose the Update button.
If the equipment card has service calls connected to it, proceed as follows:
1. To close all the service calls connected to the existing equipment card, from the SAP Business One Main Menu, choose
Service Service Call .
2. To assign the item to a different business partner, from the SAP Business One Main Menu, choose Service Equipment
Card .
3. Open the existing equipment card and change the Status field to Terminated.
4. To save your changes, choose the Update button.
5. Using the same serial number, create a new equipment card for the new business partner.
More Information
Creating, Updating, and Deleting Equipment Cards
Working with Service Contracts
A service contract between a business partner and your company enables your company to provide maintenance and repair for an
item beyond the manufacturer’s warranty coverage. You define the type of service for which the business partner is eligible.
SAP Business One supports the following service contract types:
Contract Type Coverage
Customer Service for all items purchased by the customer, regardless of the
item group or serial number
Item Group Service for items that belong to a specific item group
 Example
The contract with a customer named Microchips covers the
service for items in the Printers group. This means the
customer receives service for all items that belong to this group
regardless of their serial numbers.
Serial Number Service for items with specific serial numbers
You can enter a service contract manually or base one on a predefined contract template.
In addition, service contracts can be created automatically when a serial number item is delivered to the customer, either in a
delivery or an A/R invoice document. When several items with different warranty templates are sold in the same document, a
corresponding number of service contracts are created automatically.
For this to occur, both of the following conditions must be fulfilled:
You have created a contract template of the type Warranty, which will automatically copy its data into a service contract
upon creation.
You have defined that equipment cards are created automatically for serial number items (on the Items subtab of the
Inventory tab, in Administration System Initialization General Settings )
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:11 AM
 Example
Here’s an example of how the process works:
1. When a customer orders a serial number item, you create either a delivery note or an A/R invoice to deliver the item to
the customer.
2. A equipment card is created automatically for serial number items. The equipment card provides you with the complete
overview of all service-related information for the serial number.
3. At the same time, a service contract for the serial number items is created automatically, since the warranty covers
these items.
As a result, you can now open service calls for the serial number items.
You can create a equipment card manually. This may be necessary for customers that buy the serial number item from another
vendor but want to buy the maintenance contract for the equipment from you. In this case, you also must create the service
contract manually.
The diagram below shows the topics covered in this section. Choose each topic for more information.
Please note that image maps are not interactive in PDF outputs.
Related Information
Adding, Updating, and Duplicating Contract Templates
Working with Equipment Cards
Service Contract Window
Use this window to specify, view, and modify the details of the service contract for a specific business partner. The service contract
determines the type of service for which the business partner is eligible.
To access the general area, from the SAP Business One Main Menu, choose Service Service Contract .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area Fields
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:11 AM
Service Contract Type
Specify the service contract type.
Sales type indicates that the service is provided to your customer.
Purchasing type indicates that the service is provided by your vendor.
Contact Person
Specify one of the contact persons defined in the business partner master data.
Telephone No.
Displays automatically if a telephone number is defined for the selected contact person. If there is no telephone number for the
contact person, displays the telephone number defined in the business partner master data record.
Description
Specify a description for the contract.
Contract No.
Unique, automatically assigned, sequential number that identifies the service contract
Start Date
Specify the date on which the contract becomes valid.
End Date
Specify the date on which the contract expires.
Termination Date
If a contract is terminated during its validity period (the period between the start date and end date), specify the termination date.
SAP Business One changes the status of the contract to Terminated. As a result, all the fields are display only and blocked for data
entry. In addition, the Renewal option on the General tab is no longer available.
More Information
Creating and Updating Service Contracts
Service Contract: General Tab
Service Contract: Items Tab
Service Contract: Coverage Tab
Service Contract: Attachments Tab
Service Contract: Service Calls Tab
Managing Recurring Transactions from Service Contracts
Service Contract: General Tab
Use this tab to specify, view, and modify general information about the contract.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:11 AM
To access the tab, from the SAP Business One Main Menu, choose Service Service Contract and select the General tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Tab Fields
Service Type
Select either Regular or Warranty.
A warranty contract can be created automatically when an A/R invoice or a delivery is added for an item with serial number
management.
A regular contract can only be created manually.
Contract Type
Choose one of the following types of scope:
Serial Number
For items with a specific serial number (specify serial number on the Items tab)
Business Partner
For all the items you sell to or buy from the business partner
Item Group
For items in a specific item group (specify item group on the Items tab)
Template
Choose an existing contract template instead of specifying all the fields in the contract manually. A contract template that has a
status of Expired is not available for selection.
Response Time
Specify the maximum amount of time allowed to respond to a service call.
Resolution Time
Specify the maximum amount of time allowed to resolve a service call.
Status
Select the status of the service contract.
Approved
The customer is entitled to receive service according to the contract.
On Hold
Contract is set to inactive, and the customer is not entitled to receive service.
Draft
The contract is not approved, and the customer is not entitled to receive service. This is the default status for all new
service contracts.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:11 AM
Terminated
The contract is terminated, and the customer is not entitled to receive service.
To end the service contract, you specify the termination date in the Termination Date field. SAP Business One sets the
status to Terminated.
 Note
You can change the status from Terminated at any time. If you change the status to another status, the Termination
Date field is cleared automatically.
Handled By
Specify the name of the user who is responsible for the service contract.
Renewal
Enables you to renew an expired service contract.
Reminder
Specify the number of days, weeks, or months for the alert to appear prior to the termination of the service contract. You can
specify a value in this field only after you select Renewal.
Active Items
For a serial number contract only: the number of items that are related to the service contract and are defined as Active. An active
item is an item that does not have a Termination Date and whose End Date has not arrived yet, as specified on the Items tab.
More Information
Creating and Updating Service Contracts
Setting Up and Working with Contract Templates
Service Contract: Items Tab
Use this tab to specify or view the item details for the contract. The fields and structure of this tab change according to the
selected Contract Type.
To access the tab, from the SAP Business One Main Menu, choose Service Service Contract and select the Items tab.
 Note
For a customer contract type, the Items tab is inactive. The customer contract covers all the items purchased by the customer
from your company; therefore you do not need to define items manually.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Serial Number Contract Type
Mfr Serial No.
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:11 AM
Specify the manufacturer’s serial number. When you enter a serial number, the manufacturer's serial number appears
automatically.
Serial Number
Specify the serial number. When you specify a manufacturer's serial number, the serial number appears automatically.
Start Date
Specify the date on which the service contract becomes valid.
End Date
Specify the date on which the service contract expires.
Termination Date
If required, specify a date on which the service contract terminates for every item.
Item Group Contract Type
Start Date
Specify the date on which the service contract becomes valid.
End Date
Specify the date on which the service contract expires.
Termination Date
If required, specify a date on which the service contract terminates for the item group.
More Information
Creating and Updating Service Contracts
Service Contract: Coverage Tab
Use this tab to define the hours during which the business partner is entitled to receive service. If you use a contract template for
the service contract, this tab is filled in automatically.
To access the tab, from the SAP Business One Main Menu, choose Service Service Contract and select the Coverage tab.
Coverage Tab Fields
Days
Select the days on which service is provided or received.
Start Time
Specify the time as of when service is provided or received.
End Time
Specify the time until when service is provided or received.
Include
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:11 AM
Select one or more of the following to be included in the service coverage:
Parts
Items used by a technician to fix the problem at the business partner site.
Labor
Amount of time it takes a technician to fix the problem at the business partner site.
Travel
Amount of time it takes a technician to travel to and from the business partner site.
Including Holidays
Select the checkbox to indicate whether to receive service during holidays.
 Note
To define holidays, choose Administration System Initialization Company Details and select the Accounting Data tab.
More Information
Creating and Updating Service Contracts
Service Contract: Attachments Tab
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
When you upload an attachment, it is saved to the default target path folder which is set by your system administrators. However, if
it is needed, you can still change the target path manually. To do this, proceed as follows:
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:11 AM
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
Creating and Updating Service Contracts
General Settings: Path Tab
Service Contract: Service Calls Tab
Use this tab to view all the service calls related to the items in the service contract.
To access the tab, from the SAP Business One Main Menu, choose Service Service Contract and select the Service Calls
tab.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Service Calls Tab Fields
Creation Date
The date in which the service call was created.
Subject
The subject specified in the service call.
Item No.
Item number for which the service call was created
SN
Serial number of the item for which the service call was created. This is relevant only for contracts of the serial number type.
Status
The current status of the service call.
More Information
Creating and Updating Service Contracts
Service Contract: Recurring Transactions Tab
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:11 AM
Use this tab to view recurring transactions related to the service contract.
To access the tab, from the SAP Business One Main Menu, choose Service Service Contract and select the Recurring
Transactions tab.
Recurring Templates
Sales and purchasing BP type can use this list to view all marketing documents (A/P and A/R). For example, purchase orders are
visible to customers.
Creating and Updating Service Contracts
Procedure
 Note
You cannot delete a contract but you can make a contract inactive by entering a Termination Date. SAP Business One sets the
status of the contract to Terminated.
Creating a New Service Contract
1. From the SAP Business One Main Menu, choose Service Service Contract .
The Service Contract window opens.
2. Switch to Add mode. For more information, see Working in Add Mode.
3. In the general area, specify information about the customer and the time period of the service contract.
4. On the General tab, specify general details about the service contract.
5. On the Items tab, specify item details according to the service contract type (serial number or item group).
6. On the Coverage tab, specify details for service coverage and availability.
7. On the Attachments tab, add any attachments that may be relevant for the service contract.
8. On the Service Calls tab, view the service calls related to the items in the service contract.
9. To save your changes, choose Add.
Updating an Existing Service Contract
1. From the SAP Business One Main Menu, choose Service Service Contract .
The Service Contract window opens.
2. Switch to Find mode. For more information, see Working in the Find Mode.
3. Enter the complete or partial business partner code and choose Find.
Existing service contracts of the selected business partner are displayed.
4. Make the changes and choose Update.
5. To close the window, choose OK.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:11 AM
Working with Service Contracts
Service Contract Window
Printing Service Contracts
Context
You can print service contracts for your business partners using default printing layouts. Using printing layouts lets you design the
printed version of the service contracts you give your business partners.
 Note
You can edit the default layouts or create new ones by using Print Layout Designer (PLD). For more information about PLD, see
How to Customize Printing Layouts with the Print Layout Designer at SAP Help Portal.
Procedure
1. From the SAP Business One Main Menu, choose Service Service Contract .
The Service Contract window opens.
2. View the relevant contract.
3. From the Tools menu, choose Layout Designer... or click in the toolbar.
4. Choose the preferred printing layout.
5. From the File menu, choose Print or click in the toolbar.
Related Information
Printing in SAP Business One
Working with Service Contracts
Managing Recurring Transactions from Service Contracts
You can relate recurring transactions and service contracts. This may be valuable, for example, if you agreed to provide your
business partner with a certain service on a monthly basis and want to invoice the business partner regularly.
Procedure
Linking Recurring Templates to Service Contracts
1. From the SAP Business One Main Menu, choose Service Service Contract and open the relevant service contract.
2. Select the Sales Data or the Purchasing Data tab.
3. Under Recurring Templates in the Template column, choose a recurring template that has been defined for the business
partner or create a new one.
4. In the Service Contract window, choose Update and OK.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:11 AM
Executing Recurring Transactions from Service Contracts
Prerequisite: A recurring template has been linked to the service contract, as described above.
1. From the SAP Business One Main Menu, choose Service Service Contract and open the relevant service contract.
2. Select the Sales Data tab or the Purchasing Data tab.
3. To display the recurring transaction instances related to the template that is linked to the service contract, set the check
mark to the left of the template.
Under Recurring Transactions, all instances of the recurring transaction are displayed along with the status, execution
date, and document total.
4. To execute a recurring transaction, click the yellow arrow related to a transaction.
The relevant document draft appears.
5. If necessary, change the draft, and choose Add.
More Information
Recurring Transactions
Creating Solutions and Using the Solutions Knowledge Base
Context
You can:
Create and update common solutions to customer’s problems and questions.
Display all the solutions that were ever recorded in SAP Business One.
Link an existing solution to a service call or record a new solution from a service call.
Procedure
1. From the SAP Business One Main Menu, choose Service Solutions Knowledge Base .
The Solutions Knowledge Base window opens.
2. Specify the information in the general area.
3. On the Description tab, specify the cause and the details of the solution.
4. On the Attachments tab, attach a file to the solution, as needed.
5. To add the solution to the knowledge base, choose Add.
Related Information
Solutions Knowledge Base Window
Solutions Knowledge Base Window
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:11 AM
Use this window to create a solution or to choose an existing solution to solve service call problems. Existing solutions provide you
with information about problems reported in past service calls.
To access the window, from the SAP Business One Main Menu, choose Service Solutions Knowledge Base .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Solutions Knowledge Base Window Fields
Item
Specify the item number that is the subject of the solution.
A link arrow to the Item Master Data window is displayed.
Updated by, Updated on
Date on which the solution was last updated and the code of the user who updated the solution; for an existing solution only.
These fields are not displayed in Add mode.
Status
There are three default solution statuses:
Internal: A solution is in the internal processing stage inside a department or organization.
Publish: A solution has been made publicly available and is accessible to all users within a company.
Review: A solution is going through a review process to ensure quality and correctness before it is published.
Select one of the default statuses for the solution or define a new status.
To define new statuses, from the dropdown list, choose Define New. The Solution Statuses – Setup window opens. You specify the
name and description of the new status and update the status information.
To hide a user-defined status, deselect the Active checkbox.
No.
Unique number of the solution
Owner
User who created the solution
Solution
Description of the solution to the problem
Symptom
Factors or circumstances indicating the existence of the problem
More Information
Creating Solutions and Using the Solutions Knowledge Base
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:11 AM
Printing Service Solutions
Context
You can print service solutions by using default print layouts. The printed solutions can assist your service representatives in their
routine work.
Procedure
1. From the SAP Business One Main Menu, choose Service Solutions Knowledge Base .
2. Find the relevant solution or solutions.
3. From the Tools menu, choose Layout Designer... or click in the toolbar.
4. Choose the preferred printing layout.
5. From the File menu, choose Print, or click in the toolbar.
Related Information
Printing in SAP Business One
Document Printing
Context
Use this function to print batches of documents according to your required selection criteria. You can choose whether to print the
whole list or specific documents.
Procedure
1. From the SAP Business One Main Menu, choose one of the following:
Financials Document Printing
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
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:11 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:11 AM
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
Internal Number From ... To
Specify the range of document numbers from which to draw documents for printing.
For service calls, the Internal Number here refers to the Call No.
For service contracts, the Internal Number here refers to the Contract No.
No. of Copies
Specify the number of copies you want to print for each document.
Print Documents Window
This window displays all the documents that meet the criteria you specified in the Document Printing – Selection Criteria window.
To print the documents, select the desired rows and choose the Print button.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:11 AM
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
Production order
Service call
Service contract
Bill of exchange – receivables, bill of exchange – payables, and bill of exchange – transactions
Printing Documents Automatically
Context
You can set SAP Business One in such a way that certain document types, such as orders, are printed automatically when they are
created.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:11 AM
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
Service Reports
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
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:11 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:11 AM
Selection Criteria
To define the selection criteria, you specify ranges and set filters. To set a filter, click and select the relevant options.
Sort
Displays the sort criteria you can define.
Sort Field
Specify the field(s) to be used as sort criteria. This column appears only when you select Sort.
Order
Specify the order in which the fields in the report should be sorted. This column appears only when you select Sort.
Service Calls by Queue Report Window
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
This report lets you analyze the response time of employees that are assigned to specific service calls. If a service call is in a queue,
you get information about the amount of time the service call was in the queue before an assignee responded to it.
Use this window to specify selection criteria for the Response Time by Assigned to Report.
 Recommendation
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:11 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:11 AM
This report provides details about the average amount of time required to close service calls. Use this report to check the efficiency
of the service department.
You can display service calls with the same closure date. You can also select service calls completed by a specific employee.
To access the window, choose Service Service Reports Average Closure Time . Alternatively, open it from the Reports
module.
After defining the report, you can view it in the Average Closure Time Report window.
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
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:11 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:11 AM
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
Service Monitor
Use this report to analyze the efficiency and performance of your service department. You can view either your own service calls or
all open service calls.
The report presents two dynamic views of service calls:
Open Service Calls
The graph displays the rate of open service calls in SAP Business One; that is, the number of service calls that were opened
per minute during the last hour.
Overdue Service Calls
The graph displays the rate of overdue service calls in SAP Business One; that is, the number of service calls that were
overdue per minute during the last hour.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:11 AM
To view the details of either open or overdue service calls, choose Details.
To open the window, choose Service Service Reports Service Monitor . Alternatively, open it from the Reports module.
Service Monitor Fields
Assignee
To specify an employee responsible for the service call, select the checkbox and specify the assignee.
Queue
To specify the queue to which the service call is assigned, select the checkbox and specify the queue.
Priority
To include service calls with a specific priority, select this checkbox and specify the priority by clicking .
Open Calls Limit
To get an alarm when the number of open service calls exceeds a defined limit, select this checkbox and specify a number.
Overdue Calls Limit
To get an alarm when the number of overdue service calls exceeds a defined limit, select this checkbox and specify a number.
Sound Alarm
To activate a sound alarm when the number of open or overdue service calls exceeds the defined limit, select this checkbox.
Refresh
Specify the amount of time and select the time unit for refreshing the display.
More Information
Service Monitor: Open and Overdue Service Calls
Service Monitor: Open and Overdue Service Calls
Use these reports to view and analyze your open or overdue service calls in detail.
To open the window, choose Service Service Reports Service Monitor and then choose Details for either Open Service
Calls or Overdue Service Calls.
My Service Calls
Use this report to view and analyze the service calls assigned to you. The report displays open, closed, and overdue service calls.
You can evaluate the priority of service calls and take any necessary action. You can also analyze your efficiency and performance.
To open the report window, choose Service Service Reports My Service Calls . Alternatively, open it from the Reports
module.
To display or remove additional fields in the report, choose in the toolbar.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:11 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 60