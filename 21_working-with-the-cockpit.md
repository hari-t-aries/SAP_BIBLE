6/8/26, 6:13 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:13:33 GMT+0000
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

6/8/26, 6:13 AM
Working with the Cockpit
The cockpit is a personalized work center where you can view, search, organize, and perform your regular work and related
activities in SAP Business One.
This topic describes how to work with the cockpit from the perspectives of both system administrators and regular company
users. The cockpit enables you to:
Group your most frequently used functionalities in one place
Focus on your responsibilities with the necessary information and data presented to you
This topic provides information on how to perform the following tasks:
Enabling and disabling the cockpit
Working with SAP predefined cockpits or self-created cockpits
Working with cockpit widgets (small applications in the cockpit that help you to perform specific tasks)
Working with the map services
Managing authorizations for the cockpit
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
Please note that image maps are not interactive in PDF outputs.
For more information about working with the Fiori-style cockpit, see the How to Work with the Fiori-Style Cockpit guide at SAP
Help Portal.
Enabling and Disabling the Cockpit
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:13 AM
When you start to use the cockpit, the user interface of the traditional SAP Business One application window changes. In case
some customers or users might want to work with the traditional SAP Business One user interface, SAP provides a two-level
setting method for enabling and disabling the cockpit:
1. Company level
An authorized user, such as a system administrator, decides for the company whether to use the cockpit or not.
 Note
To enable the cockpit at company level, you require the correct user authorization.
2. User level
After the cockpit is enabled at company level, company users can decide individually whether to work with the cockpit or
not.
 Recommendation
Use the following settings to better view your cockpit:
Minimal screen size: 800 x 600 pixels
Screen resolution: 1280 x 1024 pixels
Font size: 10
Enabling the Cockpit Function and the Dashboard Widget
Prerequisites
To enable the cockpit at company level, you have obtained the correct user authorization.
Procedure
Enabling the Cockpit at Company Level
1. From the SAP Business One Main Menu, choose Administration System Initialization General Settings and choose
the Cockpit tab.
2. On the Cockpit tab, select the Cockpit radio button.
 Note
To enable the dashboard widget, make sure that you have installed the integration component correctly.
3. To save these settings, choose the Update button.
You receive a message that the settings take effect the next time you log on to SAP Business One.
4. For your settings to take effect, log off and then log on again to the same company.
 Note
After you enable the cockpit successfully for the entire company, users in your company need to individually enable the cockpit
to actually view and use it.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:13 AM
Enabling the Cockpit at User Level
After the system administrator enables the cockpit successfully for the whole company, you need to individually enable the
cockpit to access it in SAP Business One. If you prefer to use the traditional SAP Business One user interface, you can choose not
to enable the cockpit.
1. To enable your own cockpit, from the SAP Business One menu bar, choose Tools Cockpit .
2. Choose Enable My Cockpit.
3. For your settings to take effect, log off and then log on again to the same company.
More Information
Enabling and Disabling the Cockpit
Disabling the Cockpit
Disabling the Cockpit
If you want to use the traditional SAP Business One user interface, you can disable the cockpit. There are two levels at which you
can do so:
Disabling the cockpit at company level
An authorized user, such as a system administrator can disable the cockpit for the whole company. This prevents all the
users in the company from viewing or accessing the cockpit, even if they have enabled the cockpit for themselves.
 Note
After you disable the cockpit at company level, other users can still work with the cockpit until their next logon.
Disabling the cockpit at user level
After the cockpit is enabled for the entire company, users can decide for themselves whether to use the cockpit or not.
Disabling your own cockpit does not prevent other users from working with the cockpit.
Prerequisites
To disable the cockpit at company level, you have obtained the correct user authorization.
Procedure
Disabling the Cockpit at Company Level
1. From the SAP Business One navigation panel on the left side of the window, select the Modules tab.
2. Choose Administration System Initialization General Settings .
3. On the Cockpit tab, select the Fiori-Style Cockpit or None radio button.
For more information about working with the Fiori-style cockpit, see the How to Work with the Fiofi-Style Cockpit guide at
SAP Help Portal.
4. For your settings to take effect, log off and then log on again to the same company.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:13 AM
Disabling the Cockpit at User Level
1. To disable your own cockpit, from the SAP Business One menu bar, choose Tools Cockpit .
2. Deselect the Enable My Cockpit checkbox.
3. For your settings to take effect, log off and then log on again to the same company.
More Information
Enabling the Cockpit
Enabling and Disabling the Cockpit
Working with Cockpits
To work with the cockpit, you can work with SAP predefined cockpits or create your own cockpits.
SAP provides the following predefined cockpits: Home, Sales, Service, Finance, and Purchasing.
An authorized user, such as a system administrator in your company can create new cockpit templates according to the
business needs of the company and publish them to all the company users. For more information, see Creating a New
Cockpit Template.
This topic documents the following tasks you can perform with the cockpits:
Selecting a Predefined Cockpit
Customizing a Cockpit
Applying the Original Cockpit Template
Creating a New Cockpit Template
Publishing a Cockpit Template
Removing a Cockpit
Selecting a Predefined Cockpit
After you enable the cockpit, the Home cockpit is the default cockpit you see the first time you log on to SAP Business One. You
can then choose from among the other predefined cockpits according to your work area and job responsibilities, and modify the
cockpit settings and layouts according to your needs.
For each of the SAP predefined cockpits, SAP defines the cockpit widgets and widget settings according to the job role each
cockpit addresses.
Procedure
To start working with an SAP predefined cockpit, from the SAP Business One navigation panel on the left side of the window, under
My Cockpit, select the cockpit you want to use.
You can observe the word Current beside the cockpit you select, and the predefined widgets appear in the canvas area.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:13 AM
More Information
Working with Cockpits
Customizing a Cockpit
Procedure
To customize a cockpit, do the following, as needed:
1. Arrange the necessary widgets.
Select the widgets you want to work with and define the widgets according to your needs. For more information, see Adding
and Setting Up Your Widgets.
2. Adjust the navigation panel on the left side of the window.
To adjust the width of the navigation panel, drag the border line of the navigation panel horizontally.
To collapse the navigation panel on the left of the application window, click any of the names of the three tabs or the
icon in the right upper corner of the panel.
To expand the navigation panel after you collapse it, click any of the names of the three tabs.
The navigation panel appears and displays the tab you chose.
More Information
Working with Cockpits
Applying the Original Cockpit Template
Context
SAP Business One automatically saves the user-defined settings each time you make changes. To restore your cockpit to default
settings and layouts, you can use the Applying Original Cockpit Template menu.
Procedure
1. To restore the default settings, do one of the following:
From the SAP Business One menu bar, choose Tools Cockpit and choose Apply Original Cockpit Template.
From the SAP Business One toolbar, choose .
A message warns you that all user-defined settings for this cockpit will be lost if you apply the original template.
2. Do one of the following:
To confirm your choice, choose the Yes button.
To cancel your choice, choose the No button.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:13 AM
Working with Cockpits
Creating a New Cockpit Template
Prerequisites
To create a new cockpit template, you have obtained the correct user authorization.
Context
For the purpose of reinforcing standard procedures in your company or for other reasons, you may want to establish a new cockpit
and share it with other employees in your company. SAP Business One lets you create cockpit templates at runtime.
After you create a cockpit template, you can choose to do one of the following:
Publish the cockpit template to the company. For more information, see Publishing a Cockpit Template.
Not publish the cockpit template and keep it for your own use.
Procedure
1. To create a new cockpit template tailored to your business needs, do one of the following:
From the SAP Business One menu bar, choose Tools Cockpit Cockpit Management .
From the SAP Business One toolbar, choose .
The Cockpit Management – Setup window appears.
2. In the Cockpit Management – Setup window, specify the following fields for the new cockpit:
Name
Description
Provider
3. To confirm the information you enter, choose the OK button.
The new cockpit appears in the SAP Business One navigation panel on the left side of the window, under My Cockpit, at the
bottom of the cockpit list.
4. To modify the information of a user-created cockpit, specify the fields you need to update, and choose the OK button. You
can update the following fields:
Name
Description
Provider
 Note
You cannot modify the information for SAP predefined cockpits.
5. To define the cockpit you have just created, see Customizing a Cockpit.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:13 AM
You need to publish a new cockpit as a template if you want the users in your company to see and use it. For more
information, see Publishing a Cockpit Template.
Related Information
Working with Cockpits
Publishing a Cockpit Template
Prerequisites
You have been assigned with the correct user authorization for creating and maintaining cockpits.
Context
After you create a cockpit, you can publish it as a template to make it available for general company use.
Procedure
1. To publish a user-created cockpit, do one of the following:
From the SAP Business One menu bar, choose Tools Cockpit Cockpit Management .
From the SAP Business One toolbar, choose .
The Cockpit Management – Setup window appears.
2. In the Cockpit Management – Setup window, select the cockpit you want to publish and choose the Publish button.
The system automatically specifies the following fields for your cockpit:
Publication Date
Publication Time
Published By
Related Information
Working with Cockpits
Removing a Cockpit
Prerequisites
You have been assigned with the correct user authorization for creating and maintaining cockpits.
Context
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:13 AM
You cannot delete an SAP predefined cockpit.
At runtime, you can delete published and unpublished user-defined cockpits in SAP Business One. After you complete the deletion,
the following occurs:
For a published cockpit:
The cockpit template is deleted from the Cockpit Management – Setup window (via Tools Cockpit Cockpit
Management ), but you can still view and access the cockpit from the navigation panel on the left side of the
window.
When you apply the original cockpit template to this cockpit, a message informs you that the original template does
not exist; applying the template deletes the current cockpit.
For an unpublished cockpit:
The cockpit is deleted from the My Cockpit menu. You can no longer access the cockpit.
Procedure
1. To remove a user-defined cockpit, in the Cockpit Management – Setup window, select the cockpit you want to delete.
2. Right-click and choose Remove.
A confirmation message appears.
3. Do one of the following:
To confirm the deletion, choose the Yes button.
To cancel the deletion and return to the Cockpit Management – Setup window, choose the No button.
Related Information
Working with Cockpits
Cockpit Management Window
Use this window to perform the following tasks:
Creating a New Cockpit Template
Publishing a Cockpit Template
Removing a Cockpit
More Information
Working with the Cockpit
Working with Cockpit Widgets
After you successfully enable the cockpit and choose the cockpit you want to work with, your cockpit appears and displays within
the canvas area the widgets you add to the current cockpit. SAP delivers the following widgets to help users to build up and
maintain their personalized work spaces:
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:13 AM
Common Functions
Open Documents
Messages and Alerts
Browser
Dashboards
For more information about how to work with dashboards in the integration component, and how to create dashboards, you
can download the relevant guides at SAP Help Portal.
More Information
Adding and Setting Up Your Widgets
Adding and Setting Up Your Widgets
Prerequisites
You have successfully enabled the cockpit for your account.
You have been assigned with the correct user authorization.
Procedure
Adding a Widget by Using Drag & Drop
1. In the SAP Business One navigation panel on the left side of the window, on the My Cockpit tab, under General Widgets,
click the widget you want to add to your cockpit.
2. Drag the widget into the canvas area and drop it at the position you want it to appear.
Placing and Sizing
1. To relocate a widget within the canvas area, use the drag-and-drop function.
 Note
You cannot place a widget in a location that already contains another widget.
2. To adjust the size of a widget, drag the border lines vertically or horizontally to expand or shrink the widget.
 Note
The application does not support dragging the widget diagonally at the widget corner.
3. To automatically arrange the widgets in your cockpit canvas area, choose Window Auto Arrange All Widgets . Each
time you choose this menu option, the widgets in the current canvas area are arranged automatically.
Working with the Dropdown Menu List
In the widget window bar, click to display a dropdown menu list.
The following table lists and explains the tasks you can perform with the dropdown menu:
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:13 AM
User Task User Action
Maintaining the settings for a widget Choose Settings. The widget settings window opens.
The setting options vary for different widgets. For more information, see Working with
Cockpit Widgets.
Restoring a widget to default settings
1. Choose Settings.
2. In the widget settings window, choose the Restore Default Settings button.
The widget reverts to default settings and any user-defined settings for the
content and the size of the widget are lost.
Refreshing the data of a widget Choose Refresh.
Removing the widget from the current cockpit Choose Close.
Once you remove the widget, you lose your settings for this widget.
Minimizing a widget Choose Minimize.
Only the window bar is displayed for the widget.
Expanding a widget Choose Expand.
This menu option is available only when the widget is minimized.
Viewing information about the widget: name, Choose About.
version, and copyright
More Information
Working with Cockpit Widgets
Common Functions
The Common Functions widget enables you to organize and access your most frequently used functionalities. For faster access to
your documents, reports, and queries, you can add any SAP Business One menu options and SSP developed menu options to this
widget as shortcuts.
To add or remove a menu option for this widget, perform the following procedures:
Procedure
1. To add a menu option for this widget, drag a menu option and drop it in the widget.
2. To remove a menu option from this widget, drag the menu option out of the widget widow, and then drop it.
SAP Predefined Cockpit Content of the Common Functions Widget
Sales
Opportunity
Sales Quotation
Sales Order
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:13 AM
SAP Predefined Cockpit Content of the Common Functions Widget
Delivery
A/R Invoice
Dunning Wizard
Items Master Data
Price Lists
Business Partners Master Data
Service
Service Call
Customer Equipment Card
Service Contract
Solution Knowledge Base
Finance
Journal Entry
Journal Voucher
Incoming Payment
Outgoing Payment
Reconciliation
Checks for Payments
A/P and A/R Invoices
A/P and A/R Credit Memos
Purchasing
Purchase Quotation
Purchase Order
Goods Receipt PO
Goods Return
A/P Invoice
Purchase Analysis
Items Master Data
Business Partners Master Data
Inventory in Warehouse Report
More Information
Working with Cockpit Widgets
Open Documents
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:13 AM
The Open Documents widget provides quick access to open documents and enables you to monitor them.
Procedure
Selecting Document Types for Display in the Widget
1. In the widget window bar, click the icon.
2. From the dropdown menu, choose Settings.
3. In the Open Documents – Widgets Settings window, select the document types you want to display in the widget.
4. Do one of the following:
To confirm your selections, choose the OK button.
To cancel your changes, choose the Cancel button.
Monitoring and Checking Open Documents
The widget displays the number of currently open documents for each document type, and lets you view and monitor the overall
status for each document type.
 Note
Refresh the widget before viewing the number of open documents to make sure you receive the most up-to-date statistics. For
more information about how to refresh the widget, see Adding and Setting Up Your Widgets.
To access the open documents, proceed as follows:
1. Inside the widget, choose the document type with which you want to work.
A window appears, displaying all the open documents for this document type.
2. In the Open Items List window, choose the document you want to open.
The following table shows the open document types defined for each SAP predefined cockpit:
SAP Predefined Cockpit Document Types Displayed in the Open Documents Widget
Sales
Sales Quotations
Sales Orders
Deliveries
Returns
A/R Down Payments – Unpaid
A/R Down Payments – Not Yet Fully Applied
A/R Invoices
A/R Credit Memos
A/R Reserve Invoices – Unpaid
A/R Reserve Invoices – Not Yet Delivered
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:13 AM
SAP Predefined Cockpit Document Types Displayed in the Open Documents Widget
Service
A/R Down Payments – Unpaid
A/R Down Payments – Not Yet Fully Applied
A/R Invoices
A/R Credit Memos
A/R Reserve Invoices – Unpaid
A/R Reserve Invoices – Not Yet Delivered
Finance
A/R Invoices
Open Service Calls
Purchasing
Purchase Orders
Goods Receipt POs
Goods Return
A/P Reserve Invoices
More Information
Working with Cockpit Widgets
Messages and Alerts
Context
The Messages and Alerts widget displays messages in a clearer and easier-to-read way.
 Example
The following table shows examples of the new messages:
Original Alert Messages New Alert Messages
Deviation from Credit Limit BP V70000 exceeds defined credit limit deviation.
Deviation from Commitment Limit BP V70000 exceeds defined commitment limit deviation.
Deviation from % of Gross Profit Sales Order 82: profit margin less than defined value.
Deviation from Discount (in%) Sales Order 82 exceeds defined discount deviation.
Deviation from Budget Accounts exceed defined budget deviation: Office and Building
Rent, Office Maintenance,…
Minimum Inventory Deviation Items below min. inventory level: P10004, S10000,…
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:13 AM
To work with this widget, proceed as follows:
Procedure
1. To view the messages in the Messages and Alerts widget, add the widget to your cockpit.
2. To view the details of one message, in the widget, double-click the message.
The Messages/Alerts Overview window appears and displays the detailed information of this message.
In the Messages/Alerts Overview window, you can forward, reply to, and delete messages.
 Note
After you delete a message in the Messages/Alerts Overview window, the message is automatically removed from the
Messages and Alerts widget.
Related Information
Working with Cockpit Widgets
Alerts Management Window
Browser
Context
The Browser widget enables you to embed Web documents by setting up URLs or HTML/DHTML snippets.
 Note
You can add more than one Browser widget to your cockpit.
To work with this widget, proceed as follows:
Procedure
1. In the widget window bar, click .
2. From the dropdown menu, choose Settings.
3. In the Browser – Widgets Settings window, in the URL field, specify the URL or the HTML/DHTML snippet.
 Note
To make your browser widgets available, since 10.0 FP 2305, you need to add the URL domains in the CSP setting first
under Administration System Initialization General Settings Cockpit tab in the SAP Business One client. For
more information, see General Settings: Cockpit Tab.
4. In the Title field, enter the title to be displayed for the current browser widget.
The default title for the widget is Browser. You can use different titles if you have added multiple browser widgets to your
cockpit.
5. Do one of the following:
To confirm your change, choose the OK button.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:13 AM
To cancel your change, choose the Cancel button.
6. To restore the URL settings to the SAP default, choose the Restore button.
The system restores the URL to https://www.sap.com/go-business-one .
Related Information
Working with Cockpit Widgets
Working with Map Services
Context
Map services enable you to locate business partners and warehouses on maps using external Web browsers. Currently SAP
predefines two map services for users:
Google Map
Microsoft Bing Map
This topic documents how to perform the following tasks with the map services in SAP Business One:
Choosing a Map Service
Defining a New Map Service
Viewing Locations in a Web Browser
Choosing a Map Service
Prerequisites
You have obtained the correct user authorization. For more information, see Authorizations for the Cockpit.
Procedure
1. To specify a Web map you want to use, from the SAP Business One Main Menu, choose Administration System
Initialization General Settings.
2. Select the Service tab.
3. From the Map Service dropdown menu list, select the map service you want to use.
This setting is per Company, your choice here affects all other users' settings. If you want to define other map services, see
Defining a New Map Service.
Related Information
Working with Map Services
Defining a New Map Service
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:13 AM
Prerequisites
You have obtained the correct user authorization. For more information, see Authorizations for the Cockpit.
Procedure
 Note
After you define a new map service, the name of the service appears in the Map Service dropdown menu list. The new service is
visible and accessible for all users in your company.
1. To define other map services, from the Map Service dropdown menu list, select Define New.
The Map Services – Setup window appears.
2. In the Map Services – Setup window, specify the name of the map service.
3. In the Map Services – Setup window, specify a value in the Query URL field.
A query URL is a URL structure to specify a location search in Web map services. A query URL uses necessary parameters
to extract address data from the SAP Business One database and displays the search results in a Web browser.
To build a query URL, proceed as follows:
a. Obtain the base URL structure and the method for adding parameters to the URL.
Most Web map services providers display the information on their Web sites.
b. Add parameters to the URL.
To specify your search, you can add parameters to the URL. For example, for the Microsoft Bing Map, the SAP
predefined query URL is as follows:
http://bing.com/maps/default.aspx?v=[Name][AddressName][Street][Block][City]
[County][State][CountryORRegion]
The following table shows the parameters you can add to the query URL and the field values each parameter stands
for:
Parameter Corresponding Field
[Name] Name (as in the Business Partner Master Data window)
Location (as in the Warehouses – Setup window)
[AddressName] Address Name
[Street] Street/PO Box
[Block] Block
[City] City
[County] County
[State] State
[CountryORRegion] Country or Region
[Zip] Zip Code
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:13 AM
More Information
Working with Map Services
Viewing Locations in a Web Browser
Currently map services enable you to locate business partners and warehouses in maps using external Web browsers.
Prerequisites
You have specified the address information for the business partner or warehouse you want to locate.
You have connection to the Internet and have installed a Web browser in your computer.
Procedure
Locating a Business Partner
1. In the Business Partners Master Data window, locate the business partner you want to find, and select the Addresses tab.
2. Click the Show Location in Web Browser link.
A Web browser appears with the location of the business partner displayed in a Web map.
Locating a Warehouse
1. In the Warehouses – Setup window, locate the warehouse you want to find.
2. Click the Show Location in Web Browser link.
A Web browser appears with the location of the warehouse displayed in a Web map.
More Information
Working with Map Services
Authorizations for the Cockpit
The following table explains the authorizations required for user tasks in the cockpit. For more information, see the General
Settings Window and the Authorizations Window.
User Task User Authorization
Enabling and disabling the cockpit at company level You are permitted to view the General Settings window.
Creating and maintaining the cockpits, including: You require full authorization for the Cockpit Management.
Creating a new cockpit template To assign users with the authorization for the Cockpit
Management, from the Authorizations window, choose
Publishing a cockpit template
Administration System Initialization General Settings
Removing a cockpit template Cockpit & Widget Cockpit Management .
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:13 AM
User Task User Authorization
Adding and removing a cockpit widget You require full authorization for the widget.
To assign users with the authorization for the cockpit widgets, from
| the Authorizations window, choose  |                                         | Administration     |  System  |
| ---------------------------------- | --------------------------------------- | ------------------ | -------- |
| Initialization                     |  General Settings                       |  Cockpit & Widget  |  General |
| Widgets                            | , and then choose the required widgets. |                    |          |
Viewing the content of a cockpit widget You require the correct authorization for the content.
For example, to view Open A/R Invoice in the Open Documents
widget, you require the authorization for the related finance
content.
Specifying a map service You are permitted to view the General Settings window.
Defining a new map service You require full authorization for the Map Service.
To assign users with the authorization for the Map Service, from
| the Authorizations window, choose  |                    | Administration  |  System |
| ---------------------------------- | ------------------ | --------------- | ------- |
| Initialization                     |  General Settings  |  Map Service    | .       |
This is custom documentation. For more information, please visit SAP Help Portal. 19