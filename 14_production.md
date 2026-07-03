6/8/26, 6:10 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:10:31 GMT+0000
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
Production
The Production module, along with the Resources module, provides a base platform for managing light manufacturing processes
in SAP Business One. This module helps businesses streamline the production process, enabling better control and visibility into
the entire production cycle.
The key features of the Production module include the following:
Create and maintain bills of materials (BOMs), which define the components and quantities required to produce a finished
product. BOMs allow you to define a hierarchical arrangement of components, including the items, resources, and route
stages that are required to assemble and produce the finished product.
Use existing BOMs to create production orders and initiate the production process. Production orders can be created
manually or generated automatically based on sales orders using the Procurement Confirmation Wizard or from an MRP
order recommendation. The production order enables you to monitor the entire production process, such as tracking
actual consumption of raw materials and additional costs such as labor overhead.
Issue components to the production order and receive the finished goods once the production is completed.
Define and manage production standard costs for components based on changes in market conditions, prices of raw
materials, and labor rates.
Recalculate the production costs for production orders based on the actual consumption of materials and resources during
the production process.
Update parent item prices globally to ensure that the selling prices of parent items accurately reflect changes in
component costs.
A finished product can be the result of an entire production process, or a collection of items that are sold as a unit but are not the
output of a production or assembly process.
In the interactive graphics below, hover over each graphic for a short description. Choose each graphic for more information.
Documents Used in Production Process
Please note that image maps are not interactive in PDF outputs.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:10 AM
Production Cost and Item Pricing Management Tools
Please note that image maps are not interactive in PDF outputs.
Production Reports
Please note that image maps are not interactive in PDF outputs.
Bill of Materials Management
Use this functionality to replace, add or delete components of all types from BOMs in a batch. Additionally, you can change the
header fields of several BOMs at once or delete batches of BOMs.
More Information
Bill of Materials - Component Management - Selection Criteria
Bill of Materials Management - Selection Criteria
Use this window to replace, add, or delete components for all types of bill of materials (BOMs) in a batch. Additionally, you can
change the header fields of several BOMs at once or delete batches of BOMs.
To access this window, choose Main Menu Production Bill of Materials Management .
 Note
This topic documents fields and other elements in this window that are either not self-explanatory or require additional
information.
Bill of Materials Management - Selection Criteria Fields
Management Task
Select one of the following options:
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:10 AM
Change BOM Lines - To update information about an existing component, for example, quantity, or to replace a
component.
Add BOM Lines - To add a component.
Delete BOM Lines - To delete a component.
Change BOM Header - To update the header fields of several BOMs at once.
Delete BOM Header - To delete several BOMs at once.
Select BOMs
Define the range of BOMs to which you want to apply the selected management task.
Routed
Select Yes if you want to change components for BOMs that contain at least one route stage.
If you are using routed BOMs, you must specify at least one of the following fields:
Route Sequence - Enter a positive integer in the From and To fields to specify the route sequence range.
Route Stage - From the choose from list in the From and To fields, specify the route stage code range.
Select No if you want to change components for BOMs that do not contain a route stage.
Select BOM Lines
From the drop down list, select one of the options:
Resource - To replace one or more resource components, then in the From and To fields, define the range of the resource
components you want to replace.
Item - To replace one or more item components, then in the From and To fields, define the range of the item components
you want to replace.
Text - To replace line text, search for the text that you want to replace in the Contains the Text (Max. 254 Characters) field.
Any text that is entered into this field (including a word or phrase) will be partially matched with existing BOM text lines,
and the entire text line will be replaced with the new text entered in the Replacement Text field. For example, if you enter
the search text “storage”, all existing BOM lines that contain the word “storage” and that match the other filter selections
will be replaced with the new text. The text in the Replacement Text field can be up to 256,000 characters. .
Route Stage - This option is displayed if you indicated you are using routed BOMs. Choose this option to update existing
route stage lines in the selected BOMs.
Specify Properties for BOM Lines to Be Changed
 Note
These fields only appear if you have chosen Change BOM Lines in the Management Task field.
Replacement BOM Component - Select this checkbox if you want to replace the specified components. From the choose
from list, select the replacement component.
Change Additional Quantity - Select this checkbox if you want to change the additional quantity of the selected
components and enter the new additional quantity.
Change Warehouse - Select this checkbox to change the warehouse of the selected components in the BOM, then specify
the new warehouse.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:10 AM
Change Issue Method - Select this checkbox to change the issue method of the selected components in the BOM, then
select the desired issue method.
Change WIP Account - Select this checkbox if you want to change the WIP account of the selected components in the
BOM, and from the choose from list select the new WIP account.
Change Route Sequence - Select this checkbox if you want to change the route sequence of the selected components in
the BOM and then enter the new route sequence value.
Change Route Stage - Select this checkbox if you want to change the route sequence of the selected components in the
BOM and then select the new route stage code from the choose from list.
 Note
The following field only appears if you have chosen Route Stage in the Select BOM Lines area.
Change Waiting Days - To change the waiting days for the route stage, select this checkbox and enter a value for the
number of days.
Select BOM Lines to Add
 Note
This field appears only if you have chosen Add BOM Lines in the Management Task field.
Select one of the options:
Item - To add an item component. In the From and To fields, specify the range of items you want to add.
Resource - To add a resource component. In the From and To fields, specify the range of resources you want to add.
Text - To add line text, in the Text to Be Added field, enter the new text to be added. The text can be up to 256,000
characters.
BOM Line Details to Be Added
 Note
This field appears only if you have chosen Add BOM Lines in the Management Task field.
Quantity - Enter the quantity of the specified components to be added into the BOM.
Additional Quantity - Enter the additional quantity of the specified components to be added into the BOM.
Warehouse - Specify the warehouse of the selected components to be added to the BOM.
Issue Method - Enter the issue method of the specified components to be added into the BOM.
WIP Account - Enter the WIP account of the specified components to be added into the BOM.
Select BOM Lines to Be Deleted
 Note
This field appears only if you have chosen Delete BOM Lines in the Management Task field.
Select one of the options:
Item - To delete an item component. In the From and To fields, specify the range of items you want to delete.
Resource - To delete a resource component. In the From and To fields, specify the range of resources you want to delete.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:10 AM
Text -To delete a text line, search for the text to be deleted in the Contains the Text (Max. 254 Characters) field. Any text
that is entered into this field (including a word or phrase) will be partially matched with existing BOM text lines, and the
entire text line will be deleted. For example, if you enter the search text “storage”, all existing BOM lines that contain the
word “storage” and that match the other filter selections will be deleted.
Route Stage - To delete all lines associated with the route stage.
Update Rows
 Note
This field only appears if you have chosen Change BOM Header in the Management Task field.
Select this checkbox to apply any newly defined values in the Change Price List, Change Distr. Rule, and Change Project fields to
all rows in the selected BOMs.
Bill of Materials
Use the Define Bill of Materials function to create a multilevel BOM, one level at a time.
The BOM has a hierarchical arrangement of components. Enter all the child items and raw materials required to assemble and
produce the finished product.
To open the Bill of Materials window, choose Production Bill of Materials .
More Information
Bill of Materials Types
Bill of Materials Window
Defining Bill of Materials (BOMs)
Defining Bill of Materials (BOMs)
Procedure
1. From the SAP Business One Main Menu, choose Production Bill of Materials .
2. In the Product No. field, press TAB to display a list of item master records, and choose the item that you want to define as
a parent.
 Note
If the parent already has a BOM, its components are displayed. However, you can still create a new BOM for that parent
item.
3. Specify the BOM type, as described in Bill of Materials Types.
 Note
Choose the Production type to be able to include the product in the MRP run and to process standard production
orders.
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:10 AM
4. Enter data for the finished product and its components. For details, see Bill of Materials Window.
 Note
If the BOM contains more than one component with the same serial or batch items, combine the items in a single
component and increase the quantity appropriately to prevent possible errors in the batch or serial quantities.
5. Choose Add to save the Bill of Materials, and OK to close the window.
 Note
Sometimes production gives rise to waste, for example, manufacturing a table produces sawdust.
You can add the sawdust as an additional component (by-product), and enter a negative value in its Quantity field.
When you complete and confirm the production of the table, this component is put into inventory. The other components are
removed from inventory when you complete and confirm production.
More Information
Bill of Materials
Bill of Materials Types
Production
The Production Bill of Materials (BOM) represents a finished product (parent) comprising different inventory components (child
components). During the production process, you turn the components into the finished product. Select the Production BOM to
include the product in the MRP run and to process standard production orders.
Components in the Production BOM are physical items, for example, a screw, a wooden board, a measured quantity of lubricant or
paint, or virtual entities, such as one work hour.
Sales and Assembly
The Sales BOM and the Assembly BOM represent a finished product assembled at the sales stage, that is, the finished product is
composed of its component items only when the parent product is actually sold. The component items are stored and tracked
individually in the warehouse.
For both the Sales BOM and the Assembly BOM, you do not manage the parent product as an inventory item, but rather as a sales
item. The components can also be sales and inventory items in their own right. When you create the delivery to dispatch the
customer order, the components are backflush issued from inventory.
 Note
The components for Sales BOMs and Assembly BOMs must be sales items.
Use a Sales BOM where there is a fixed combination of components and the customer needs confirmation of each item.
The component items cannot be altered or removed from a sales order. Other items cannot be inserted between the parent
and component items in the sales order. However, the quantities of the component items can be modified.
Use the Assembly BOM when you would not expect the customer to check each component in the order, such as a gasket
set.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:10 AM
 Example
Sharon's Garden Furniture (SGF) sells outdoor furniture for gardens. One of SGF's best sellers is the "Metal Table Set".
The set is composed of one metal table, six metal chairs, and one umbrella. The Metal Table Set is probably best suited
as a Sales BOM.
If SGF chooses to represent the Metal Table Set as a Sales BOM, then the table, six chairs and one umbrella, and Metal
Table Set all appear on sales orders. Because quantities of components in a Sales BOM can be changed, SGF can sell the
Metal Table Set with only four chairs. However, because new items cannot be inserted into a Sales BOM at this stage, a
footstool cannot be included as part of the Metal Table Set in the sales order.
If SGF chooses to represent the Metal Table Set as an Assembly BOM, then only the Metal Table Set (the parent
product) is listed in the sales order. The quantities of the components of the Metal Table Set cannot be changed.
In both cases, each of the component items is tracked individually in inventory. When you create the delivery to dispatch
the customer order, the components are automatically issued from the warehouse.
Template
The Template BOM is a bundle of items, where the parent product is the first item on the list. It does not act as a BOM once it is
added to the sales document, but rather as a list of items brought together at the same time. You can update the quantity of those
items, swap items, or delete them in the BOM or the sales order. The components appear below the parent as a list of items in a
sales document. Use the Template BOM when you require flexibility in selecting components for a product.
 Example
Computers can be sold as a standard unit, in which case the Production or Sales BOM is appropriate. However, to customize a
sales order, use the Template BOM to allow for DVD burners, speakers, ergonomic keyboards, and so on.
More Information
Bill of Materials
Multilevel BOMs in Production Orders
A multilevel BOM contains one or more child items that are themselves BOMs containing their own child items. When a child BOM
item is included in a production order, the BOM type determines whether it is treated as an inventory or non-inventory item:
When a component of a production BOM is a production type BOM, the BOM is overlooked in the production order, since it
is an inventory item, which has real inventory and value. If required, you must issue a production order for the parent item
of each BOM.
When a component of a production BOM is an assembly type BOM, the BOM is overlooked in the production order, since it
is a non-inventory item and is treated as such. It does not create an inventory posting, and its cost is debited from an
expense account.
If the assembly BOM is also defined as a phantom item, it is replaced with its components when added to the production
order. The components are handled in the production order according to their type.
More Information
Bill of Materials Types
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:10 AM
Updating Bill of Materials (BOMs)
Context
When updating the Bill of Materials, you can:
Update the quantity, warehouse, BOM type, and price list
Change the components
Update the quantity, warehouse, issue method, price list, and comments of components
Add or update the Parent Product Price
Change the checkbox selection of Purchase Item for:
an item which is a child of a BOM.
a parent item in a Production BOM or Template BOM.
Change the checkbox selection of Sales Item for an item which is a component of a Production BOM or Template BOM, if
the item is not a component of another Sales BOM or Assembly BOM.
Procedure
1. Choose Production Bill of Materials .
2. Enter the product number and choose Find to display the Bill of Materials.
 Note
In an Assembly BOM, if you add or remove items, or update quantities for existing items, SAP Business One
automatically updates open sales orders and reserve invoices. The committed quantity for items that you remove/add is
reduced/is increased accordingly. These changes are also reflected in open purchase orders, for example, if purchase
orders were created for the components in the Assembly BOM; or in MRP recommendations for the Assembly BOM.
3. Choose Update to save the changes.
 Note
To duplicate the Bill of Materials, choose Data Duplicate .
Related Information
Bill of Materials Window
Bill of Materials
Deleting Bill of Materials (BOMs)
Procedure
From the menu bar choose Data Remove .
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:10 AM
You cannot restore a deleted Bill of Materials.
More Information
Bill of Materials
Bill of Materials Window
In this window you can view, add, and modify a multilevel bill of materials.
To open the window, from the SAP Business One Main Menu, choose Production Bill of Materials .
General Area Fields
Product No.
Specify the number of the finished product (parent item) or sub-assembly.
Product Description
The product description as specified in Item Master Data window.
BOM Type
Choose a type for the bill of materials. The values are:
Assembly
Sales
Production (default)
Template
For more information, see Bill of Materials Types.
Planned Average Production Size
Specify the number of parent items that you usually process in one run. This field is related to the Additional Quantity field.
Additional quantity affects the total production standard cost, based on the planned average production size.
 Example
If you plan to produce 10 parent items in one run (the Planned Average Production Size is 10), the production standard cost of
the parent item is increased by 1/10 value of the additional quantities. If you plan to produce 7 parent items in one run, the
production standard cost of the parent item is increased by 1/7 value of the additional quantities.
Production Std Cost
Displays the production standard cost of the parent item as defined on the Production Data tab of its item master data record.
Quantity
Specify the quantity or amount of the parent item that you create from the bill of materials components. For production bill of
materials, the default value is 1, but if you have a formulation that results in a predefined quantity of product, that quantity must be
entered here.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:10 AM
Warehouse
Specify the warehouse code, to which the finished product is taken. This will be the default in the production order, but it can be
changed if required.
If you have selected the Template option in the BOM Type dropdown list, you can additionally specify a dropship warehouse code
in this field.
Price List
Specify the price list for the parent and child items.
 Note
When working with a perpetual inventory system, the price list of a production bill of materials is relevant only for sales
documents. In sales documents, the item price of the Sales and Assembly BOM is determined by the customer price list and
not by the BOM definition.
Distr. Rule
Specify the distribution rule that you want to link to the bill of materials.
Project
Specify the project that you want to relate to the bill of materials.
Table Fields
Type
From the dropdown menu, select one of the following options:
Item - To add an item component.
Resource - To add a resource component.
Text - To add text.
Route Stage - To add a route stage line. With a Route Stage type line, a route stage code would be entered in the No. field of
this line.
No.
Specify the components for the bill of materials.
 Note
If the BOM contains more than one component with the same serial or batch items, combine the items into a single component
with the appropriate increased quantity. This will prevent possible errors in the batch or serial quantities.
Route Sequence
Displays the sequence number that is assigned to each routing stage. The sequence indicates the precise order in which the
routing stages must be performed during the production process.
This field will not be visible by default. The value of this field is automatically populated by the system on creating lines with a line
Type set to Route Stage .
The pull down list will contain a list of all the other route sequence numbers that currently exist in this Bill of Materials grid. No
other numbers can be entered. A selection of another route sequence number in this field will switch all the lines associated with
the current route sequence with all the lines associated with the selected route sequence.
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:10 AM
Quantity
Specify the quantity of the child items required to make the quantity of the parent. The quantity will be one of the following:
Integer quantity for discrete components like fasteners or piece-parts.
Decimal quantity for materials in continuous measure, such as meters of cable, or liters of lubricant
Additional Qty
Enter additional quantity for an item or resource component. This value is copied into the relevant field in the production order
document. Additional quantity is added to the total planned quantity of items and resources in the production order, regardless of
the produced quantity of the parent item .
 Note
Items and resources with the Manual issue method can have zero Base Qty and the Additional Qty larger than zero.
For items and resources with the Backflush issue method, the entire Additional Qty is consumed upon the completion
of the first parent item.
Additional Qty for by-product lines is always zero.
UoM
Displays the unit of measure for each component, for example, box, meter, kg. The value is defined in the item master data.
Warehouse
The warehouse from which the child item is issued. When adding an item to the table, the default warehouse that is defined in the
Item Master Data window is displayed. If required, you can specify a different warehouse.
l
 Note
If no default is defined in the item master data for the child items, the child items are issued from the default warehouse that is
defined in the General Settings window, on the Inventory tab, on the Items subtab.
For more information, see Item Master Data: Inventory Data Tab and General Settings: Inventory Tab.
Issue Method
Choose one of the following issue methods:
Backflush - child items are automatically issued to the production order, once you report the completion of the parent item.
Manual - child items are manually issued to the production order
 Note
The default is derived from the value in the Item Master Data, but can be overridden for any particular bill of materials. An
exception to this is for serial and batch controlled Items, which must be issued manually.
This field is relevant only for a production bill of materials.
Production Std Cost
For items, the field displays the production standard cost as defined on the Production Data tab of the relevant item master data
record.
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:10 AM
For resources, the field displays the total of all underlying resource standard costs as defined on the General tab of the relevant
resource master data record.
Total Production Std Cost
Displays the total production standard cost for each item and resource component according to the following formula: Total
Production Std Cost = Production Std Cost * Basic Quantity (on the row) / Quantity (on the header) + Production Standard Cost *
(Additional Quantity (on the row) / Planned Average Production Size).
At the bottom of the column, the sum of total production std costs of all components is displayed.
Price List
Specify the relevant price list for each child item. If the item has a price in the list, it appears in the unit price column.
Unit Price
To override the child item price in the price list, specify a new price. This price is valid only for the bill of materials. It does not
update the price specified originally in the price list.
 Note
In a production bill of materials, the prices are for nonperpetual inventory only. If you are working with perpetual inventory, the
price is taken from the inventory cost.
 Caution
When you update the unit price in a production bill of materials, make sure that no one else is working on the BOM at the same
time. This can lead to errors in the cost calculations.
Total
The total price for the child items, calculated according to the price lists. This can be used to determine the price of the parent
item.
Comments
Enter additional information about each of the components.
Product Price
Updates the price list field in the general area and, as a result, the price list itself. The value of the field is the total price of the
components for the parent quantity in the bill of materials header. While defining a new bill of materials, you can determine that
the parent item price will be calculated according to the total price of its child items. Choose to copy the total price of the child
items to the parent item price list. You can also change the parent item price manually.
 Note
You can use the Update Parent Item Prices Globally window to update this price in existing bills of material.
Project
Specify the project that you want to relate to each item.
Phantom Items
A phantom item is a sublevel in the BOM that does not actually exist in inventory. It is used to simplify the BOM. Although the
phantom item appears in the BOM, the components that comprise it appear in the Production Order.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:10 AM
An item can be defined as a phantom item in the Item Master Data.
 Note
Only a Production BOM can have a phantom item.
 Note
To define an item as a phantom item, the following conditions must be met:
The item is not used in any previous documents or postings (for example, sales orders, purchase orders, invoices,
deliveries, or production orders).
The item's In Stock, Committed, and Ordered quantities are 0.
The item is not part of a bill of materials (BOMs).
If the item you want to define as a phantom item is a component or parent item of a BOM, you need to identify the BOM which
contains the item and remove the item from the BOM. For more information, see SAP Note 1325861 .
Example 1
The following BOM diagram shows two phantom items.
MRP
The MRP explodes the phantom item and creates recommendations for its components. The phantom item is displayed in the
MRP result window without recommendations, for information only.
Production Order
The Production Order explodes the phantom BOM and displays its components in the required order. In the example below, in the
production order, Components 1 to 6 will appear, but not Phantom 1 and 2.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:10 AM
Production Order
Different departments in the same company can have different BOM requirements. The engineering department could create a
multi level BOM to define an engine. The manufacturing department could then include this BOM as a single phantom item.
Example 2
In MRP Results the due date of a child item is determined by the Lead Time value selected in the Planning Data tab of the parent
item.
1. An item called "Parent" is created. On the Planning Data tab of the Item Master Data for Parent, Planning Method "MRP"
and Lead Time "2" are selected.
2. For Parent, two child items are created: "Child_Phantom" and "Child_Level1".
Child_Phantom is a phantom item (the checkbox Phantom Item is selected on the Production Data in Item Master
Data) and neither Inventory Item nor Purchased Item are selected in Item Master Data. On the Planning Data tab
of Item Master Data, choose Planning Method "MRP" and Lead Time "5".
Child_Phantom is created as a parent of another child called "ABC". ABC has a Lead Time of "7".
Child_Level1 is an item with a Lead Time of "10 days".
Child_Level1 is created as a parent of another child called "XYZ" which has no Lead Time.
3. When the MRP is run, Child_Phantom's lead time is disregarded because it is a phantom Item. The lead time of ABC is
defined for the (grandparent) item, Parent. Child_Level1 is an inventory item and the Lead Time is taken into consideration
to identify when its child, XYZ, is bought.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:10 AM
There is a Production Order for Parent due on July 30. (Parent has a lead time of 2 days).
Consequently, in the MRP results, Child_Phantom and Child_Level1 are due on July 28.
Child_Phantom appears in the MRP results but not in the Order Recommendation report. However, the lead time is not taken into
consideration to define when the child, ABC, is due. For the child, ABC, the lead time of the item Parent (2 days) is taken into
consideration. The child ABC is therefore due on July 28.
The child item of Child_Level1, XYZ, is due on July 18. Because Child_Level1 is an inventory item, its lead time (of 10 days) is
considered for its child, XYZ.
Production Orders
Use different methods to issue different kinds of production orders.
Prerequisites
You have defined the parent and child items in the Item Master Data window.
You have defined the Bill of Materials for the parent and child items in the Bill of Materials window.
If you are working with perpetual inventory, you have determined the Work in Progress (WIP) Material Account and the
WIP Variance Account in the G/L Account Determination: Inventory Tab.
Process
The following example shows the production of one pair of in-line skates.
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:10 AM
Production Order Process
1. Issue a production order.
By default the order opens with Planned status.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:10 AM
2. Create production orders either automatically from MRP Recommendations, make-to-order using the Procurement
Confirmation Wizard, or manually according to sales orders.
For more information, see Creating Production Orders Directly from Sales Orders and Consolidating Multiple Sales Orders
for Production.
3. An authorized staff member changes the status of the production order to Release.
Once released, the production order is available to shop floor staff.
4. Release the child items (with a manual issue method) from inventory using the Issue for Production method.
Child items with a backflush issue method are issued automatically for the production order.
5. Report the completion of the parent item in the Receipt from Production Window.
6. Change the production order status to Closed.
You can do this at any time after the production order is set to Release, even if the planned quantity of the parent item has
not been produced.
Result
The finished product (parent item) is created. The inventory is updated for the finished product and for the child items.
The Production Order details are summarized in the Production Order Window: Summary Tab.
More Information
Production Order Overview
Production Order Window
In this window, choose a product with an existing production Bill of Materials (BOM) for a Standard or Disassembly production
order. For a Special production order, define the components and quantities required to make the product as you create the
production order.
You can amend the component allocations for the production order, if it has planned or released status. You can not add a new
backflush issue component if there have been transactions on the production order.
The Production Order window enables you to track the quantity and cost of materials, and the product status in the
manufacturing process.
 Note
The components that make up a phantom item are included in the production order, but not the phantom item itself.
To access this window, choose Production Production Order .
More Information
Production Order Window: General Area
Production Order Window: Components Tab
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:10 AM
Production Order Window: Summary Tab
Production Order Window: General Area
Use this window to specify general information for a new production order, or update the fields for a production order created
automatically from MRP.
To access the Production Order window, choose Production Production Order .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area Fields
Type
Choose one of the following production order types:
Standard – Based on the bill of materials and used to produce a regular production item.
You manage material transactions of the regular production process.
You can change components at the production stage.
When you open a new standard production order, all the components are filled in automatically.
Special – Used to produce and repair items that could be any inventory items or to perform activities that are not
necessarily bill of materials items, for example, repair orders for customer equipment cards or rejected assemblies.
You create special production order components manually.
Disassembly – Used to dismantle a parent item of the regular product into its child items. The separate parts can then be
put into inventory and sold. For example, you can purchase a used car, take it apart, and sell the individual components.
Status
A production order can be in one of the following statuses:
Planned – SAP Business One initiates production orders with Planned status.
Since the production order is not released to the shop floor for manufacturing:
You cannot yet issue items or report completion of the production order.
You can update the production order.
Released – You change the production order to this status when you release it to the shop floor for production. At this
stage:
You can report transactions for the production order and the issue of the components.
You can update the component items as long as there are no transactions for the selected component.
You can add a new component.
Closed – The production order is Closed when you cannot add any new transactions to it. You close the production order
when production is completed.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:10 AM
Canceled - The production order is removed from the list before the production process starts.
 Note
You can manually cancel a production order that is in status Planned or Released only. The canceled production order is
removed from the list.
Once a receipt from production is added, the production order cannot be canceled. If you have already issued some
components, you can only cancel the production order after returning all of the issued quantities of components.
Product No.
Enter the parent item for the Standard and Disassembly production orders.
Choose Tab to display the parent list of the Bill of Materials.
Choose New to define a new Bill of Materials.
For the Special production order type, select the item from the items list.
Planned Quantity
For manual production orders, enter the planned quantity of the finished product. The default value is 1.
When the production order is the output of the MRP run, the planned quantity is already displayed in the field. However, you can
update quantities for planned and released production orders.
UoM Code, UoM Name
Displays the inventory Unit of Measurement (UoM ) for the product.
Warehouse
Displays the warehouse that receives the finished product.
Priority
Displays the degree of importance of a production order, indicated by integer numbers.
The default value is 100. You can manually change the number here. The smaller the number, the more important the production
order.
Routing Date Calculation
This field determines how the automatic allocation of resources will occur. It contains a list of the following options:
Start Date
End Date
Start Date Forwards
End Date Backwards
Procure Items
Select this checkbox to allow procurement documents to be created from the production order and all existing item type
component rows in the production order.
Procurement Doc.
 Note
This field is only relevant to item type components and is non-editable.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:10 AM
Displays the document number of a procurement document generated from this line using the Procurement Confirmation
Wizard.
Allow Procurmt. Doc.
 Note
This field is only relevant to item type components and is editable.
If the checkbox in this field is selected, the item type component is available for selection in the Procurement Confirmation Wizard.
After you update or add a production order with this checkbox selected for one or more item type components, the Procurement
Confirmation Wizard automatically opens and displays the Product No. and Product Description from the production order.
Pick and Pack Remarks
Enter relevant comments for the pick and pack procedure.
No., Series
Choose the system object that represents sequentially numbered Production Orders.
The production number is an automatically assigned, sequential system number.
Order Date
Date on which the Production Order is created. The current date is displayed by default.
Start Date
Displays the start date of the production. By default, this date is the same as the one in Order Date. You can change it manually,
which may affect the Due Date.
Due Date
By default, displays the date of planned completion. The date is calculated based on the start date and parent item's lead time. You
can update this field manually until you close the Production Order.
User
Specify the employee responsible for the production order.
The employee must be defined as an existing user in the application.
Origin
Indicates how the Production Order was created:
MRP – a result of the MRP report recommendation
Manual – entered by an authorized user
Sales Order – created automatically based on a sales order
Linked To
From the dropdown list, specify if the production order is linked to a sales order or production order. The Sales Order option is
displayed by default.
If a production order procurement document was created using the Procurement Confirmation Wizard, this field displays the base
document type (Sales Order or Production Order).
Linked Order
Choose the relevant sales or production order linked to this production order.
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:10 AM
If a production order procurement document was created using the Procurement Confirmation Wizard, this field displays a link
arrow to the base document.
Customer
Choose the customer code to which the Production Order is linked. When you enter the Sales Order number, the customer
number is entered automatically.
Project
Specify the project that you want to relate to the production order. By default, the field displays the project defined in the
corresponding Bill of Materials window.
More Information
Production Order Window
Production Order Window: Components Tab
This tab displays the product components for the Standard and Disassembly production orders. For the Special production order,
choose the relevant product components.
To access the window, choose Production Production Order Components .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Components Tab Fields
Type
Select one of the following options:
Item - This is the default option. The remaining fields for the Item option are populated by default from the BOM associated
with the parent item, or from the Item Master Data window.
Resource - You can select a desired resource from the choose from list in the No. field. The remaining fields are populated
by default from the BOM associated with the parent item or from the Resource Master Data window.
Text - Select this option to add text in the line; the remaining fields merge into one. The text is added automatically from the
corresponding line in the Bill of Materials window associated with the parent item, or you can define it manually.
Route Stage - You can select this option for a routed production order. The remaining fields for the Route Stage option are
populated by default from the BOM associated with the parent item, or you can define them manually. With a Route Stage
line, a route stage code would be entered in the No. field of this line.
No.
Displays the number of the resource or item component.
To add a component, from the choose from list, select the desired item or resource, depending on the option you chose in the Type
field.
You can update the component details when the Production Order has the status Planned or Released; however, you cannot add
or edit backflush-issued components once transactions have taken place.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:10 AM
 Note
You can use a parent item as a component item in Special type production orders. Production orders with a parent item as the
component item are not included in MRP calculations and serial and batch number transactions reports.
Route Sequence
Displays the sequence number that is assigned to each routing stage. The sequence indicates the precise order in which the
routing stages must be performed during the production process.
This field will not be visible by default. The value of this field is automatically populated by the system on creating lines with a line
Type set to Route Stage.
The pull-down list will contain a list of all the other route sequence numbers that currently exist in this Bill of Materials grid. No
other numbers can be entered. A selection of another existing route sequence number in this field will switch all the lines
associated with the current route sequence with all the lines associated with the selected route sequence.
Base Qty
Quantity of the components necessary to manufacture the Bill of Materials of a single parent product. The origin of the value is the
Quantity field in the Bill of Materials window.
Additional Qty
Displays the quantity that is added to the total planned quantity of items and resources in the production order, regardless of the
quantity of the parent item produced.
The value is copied from the Additional Qty field in the Bill of Materials window, however, you can change it manually in the
production order.
 Note
Only components of the Manual issue method can have zero Base Qty and the Additional Quantity larger than zero.
 Note
The additional quantity for by-products is always zero.
Planned Qty
Planned quantity of the component for issue, which is the multiple of the base quantity and the planned quantity of the product
plus the additional component quantity.
You can enter a different quantity in the following circumstances:
Manually issued components - The Production Order has Planned or Released status.
Planned quantity cannot be updated to less than issued quantity.
Backflush components - No products are reported as Completed.
A grey field indicates that you cannot update the quantity.
Issued
Total component quantity already issued for the Production Order.
Available
Displays the available quantity of the item units in the specific warehouse, including outgoing and incoming orders.
For resources, it displays the total resource availability for the warehouse populated on the production order line.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:10 AM
UoM Code, UoM Name
Displays the inventory Unit of Measurement (UoM) for the item component.
Warehouse
Default warehouse from which you issue the components.
For manually issued components you can overwrite the value before you post the inventory transactions for the line.
Issue Method
Choose the issue method for the Production Order:
Manual – individual components of a parent item are issued manually. This enables you to post components issued to a
production order precisely when they are required in the production process. Serial or batch-managed items must be
issued manually.
Backflush – components of a parent item are automatically issued to the Production Order (as defined in this
Components tab) once you report the completion of the parent item.
Start Date
Displays the earliest date when the component is needed in the production process.
The value from the Start Date field on the header is copied into this field by default. You can change it manually, however, the date
cannot be earlier than the start date on the header. Both start and end dates on the rows are relevant for MRP, ATP and resource
reports.
End Date
Displays the latest date by which the component needs to be used in the production process.
By default, his date is the same as the one in Due Date on the header of the production order. You can change this date for each
component manually, however, it cannot be later than the Due Date specified in the header. MRP, ATP and resource capacity
reports take into consideration separately the date ranges defined for each component.
Distr. Rule
If required, specify a distribution rule for the row.
WIP Account
Displays the account to which costs of the component are posted during the production process.
If the production order lines are populated with components from a BOM, the account defined in the WIP Account field in the BOM
for the relevant component populates this field. If the WIP Account field for the relevant component is blank in the BOM, this
account is blank, too.
You can manually update the account in this field. The value of this field is then copied into the Account Code field of the issue for
production.
Run Time
Displays the quantity of the resource included in the production order expressed in time.
The Run Time is calculated according to the following formula:
Base Qty of the resource * Planned Qty of the parent item * (Time per Resource Unit / Resource Units per Time)
Additional Time
Displays the additional quantity of the resource needed to complete the production order, expressed in time. The value is
calculated according to the following formula:
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:10 AM
Additional Qty * Time per Resource Units / Resource Units per Time
Total Time
Displays the total sum of Run Time and Additional Time.
Project
Specify the project that you want to relate to each item. By default, the field displays the project specified for the item in the
corresponding Bill of Materials window.
Resource Allocation
The value of this field is taken from the relevant Resource Master Data window; however, you can update it manually.
For production orders with route stages, the value of this field (for all Resource type lines) is taken from the Routing Date
Calculation field in the general area of the production order and cannot be edited.
Select one of the following options:
On Start Date - The capacity of the resource is allocated to the start date of the production order. This means that the
value of the resource capacity in the Planned Qty field is counted as Committed capacity on the start date of the
production order.
On End Date - The capacity of the resource is allocated to the end date of the production order. This means that the value
of the resource capacity in the Planned Qty field is counted as Committed capacity on the end date of the production
order.
Start Date Forwards - The capacity of the resource is allocated to the start date when it is assigned to the production
order; however, if the Planned Qty is greater than the Single Run Capacity for the start date, the system allocates only as
much capacity as there is Single Run Capacitydefined for the start date and continues to allocate the remaining capacity
to the day after the start date. The process continues forwards for each day until it allocates all the remaining Planned Qty.
End Date Backwards - The capacity of the resource is allocated to the end date when it is assigned to the production order;
however, if the Planned Qty is greater than the Single Run Capacity for the end date, the system allocates only as much
capacity as there is Single Run Capacity defined for the end date and continues to allocate the remaining capacity to the
day before the end date. The process continues backwards for each day until it reaches the current system date and
allocates all the remaining Planned Qty to the current system date regardless of how much Single Run Capacity is defined
for that day.
 Note
The triggers for running the resource allocation process are the following:
Adding the production order.
Updating Planned Qty, Resource Allocation, and Warehouse on a resource line (only for the resource in question).
Updating the Due Date field triggers the resource allocation process for all resources in the production order.
Updating the internal capacity does not trigger resource allocation, hence if you have updated the internal capacity and want
the system to run the resource allocation process to update the allocated amounts, you need to update the production order as
described above.
Required Days
Displays the number of days required for a specific resource to complete the Planned Qty of a particular route stage. This field will
be automatically calculated for a production order that has at least one route stage, one resource line, and whose Routing Date
Calculation field is either Start Date Forwards or End Date Backwards.
The calculation of this field is based on Routing Date Calculation status and Single Run Capacity of the resources.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:10 AM
Waiting Day
Displays a period of time (in days) to wait after the completion of the route stage. This field is not visible by default. As soon as a
Route Stage type line is created, you can manually enter the number of waiting days.s
Status
Displays the line status for Item, Resource, or Route Stages. This field is not visible by default. The following options are available
for this field:
Planned
In Progress
Complete
For production orders without route stages, changing a status may affect the following operations:
A line with Complete status is read-only and cannot be deleted.
You can change the Complete status back to Planned or In Progress, unless the production order is Closed or Canceled.
When the Issued quantity is less than the Planned Qty, if you change to Complete status, you have the option to reduce
Planned Qty and update it with Issued quantity.
For routed production orders, besides the above-mentioned scenarios, changing a status may additionally affect the following
operations:
Upon a status change on Route Stage, all components belonging to that route stage will have the Status field automatically
set according to the Route Stage status.
When using Routing Date Calculation feature, route stages with Complete status are considered to be stages with zero
duration, and thus are not counted in the calculation. However, if there is any open quantity on the resource row of such
route stages, commitment of this resource still occurs.
More Information
Production Order Window
Production Order Window: Summary Tab
The Summary tab displays information about the released and closed production orders.
To access the tab, choose Production Production Order Summary .
Upon the completion of a production order, on the Summary tab, you can observe the product cost for this production order. The
product cost is calculated both from the completed product perspective (the Actual Product Cost field), and the consumed
component perspective (the Actual Component Cost field and the Actual Additional Cost field). The variance of the cost is
displayed in the Total Variance field.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Summary Tab Fields
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:10 AM
Costs
Actual Item Component Cost
Total value of all component items (not including non-inventory components) issued for the production order.
Actual component cost = Cost per component * Component issued quantity
 Note
Any item component which has been returned through the return components functionality in the Receipt from Production
window reduces the Actual Item Component Cost value by its cost.
Actual Resource Component Cost
Records the cost of all resource components which have been issued for production.
 Note
Any resource component which has been returned through the return components functionality in the Receipt from
Production window reduces the Actual Resource Component Cost value by its cost.
Actual Additional Cost
Total value of all non-inventory component items, for example, a service or labor cost.
The field is updated on production completion.
Actual Product Cost
Total value of all products (the completed parent items) received from the completed product order.
Actual product cost = Cost per component * Expected component usage quantity
The calculation of expected component usage quantity is based on the completed products, which may be equal to or different
from the component issued quantity for the product order. When the two quantities are different, the variance appears.
Expected component usage quantity = Planned component quantity * (Actual parent completed quantity / Planned parent
quantity)
 Example
Take the following data for example, you can observe the difference in calculating the Actual Product Cost and the Actual
Component Cost.
Parent Item Produced Quantity Component Item Issued Quantity
Planned Quantity 31500 40.95
Actual Quantity 30166 40
The cost per component is 100. According to the table above:
Actual Component Cost = 100 * 40 = 4000
This value is removed from inventory in respect of the component items consumed in the production.
Actual Product Cost = 100 * [40.95 * (30166 / 31500)] = 3921.58
This value enters into the inventory in respect of the parent items produced in the production.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:10 AM
Total Variance
Displays the difference between product cost and component cost.
If there is a difference between the value of the issued components and the received products, this results in production variance.
Total variance = Actual product cost - Actual component cost
Production variance often occurs because of the following:
Overconsumption: The quantity of components consumed in production was greater than planned. This causes a negative
variance.
Underconsumption: The quantity of components consumed in production was less than planned. This causes a positive
variance.
Receipt before issue: The receipt from production document is added before the issue for production. In this scenario, the
product cost is based on an estimation, which is derived from:
1. The current production order structure, in other words, the list of production order components together with their
planned quantities.
2. The current component costs.
 Note
If the production order structure or component costs change during the period between the addition of Issues for
Production and Receipts from Production, this results in production variance.
If the valuation method of your products is not set to Standard, when you close the production order, the following calculations are
performed:
1. The system sums the values of the received quantity of products and by-products from all receipts from production.
2. The system sums the values of the issued components from all issues for production and receipts of returned components.
If there is a difference between the two summed amounts, the difference is reflected as the Total Variance field value.
The Total Variance field is updated upon production completion. Upon closure of the production order, the product is revaluated
according to the actual cost of the issued components. Meanwhile, all estimated production costs are replaced with the actual
costs from the issues for production, and the production variance is usually cleared.
Click the link arrow to the left of the Total Variance field to open the Variance Report window and view the contribution of each
production component to the final production variance. For more information, see Variance Report.
 Note
The variance report is only available if you use perpetual inventory and there is at least one Issue for Production or Receipt
from Production transaction.
Actual By-Product Cost
Records the cost of all by-product items which have been received from production, including any rejected by-products.
Click to open the Inventory Posting List window and view the relevant cost breakdown for the posted by-products.
Variance Per Product
Displays the total variance divided by (quantity completed + quantity rejected).
Journal Remark
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:10 AM
Displays the product number, by default. The value is saved in the General Ledger and is displayed in the General Ledger
transactions and reports. You can modify the value of the field.
Relevant for companies that use perpetual inventory management.
Companies that do not use perpetual inventory have no General Ledger transactions.
Quantities
Planned Quantity
Total planned quantity of the production order.
Completed Quantity
Displays the total quantity reported as completed. Rejected quantities and completed quantities enter inventory and impact
inventory valuations in the same way.
Rejected Quantity
Total quantity rejected in the Production Order. Rejected quantities and completed quantities enter inventory and impact
inventory valuations in the same way. You can choose to remove rejected items from inventory manually.
Dates
Due Date
Displays the due date of the Production Order.
Actual Closing Date
Enter the date on which the Production Order was closed.
By default, the system sets this date to the system date.
Overdue
Number of days by which the actual close date was overdue.
Planned Times
Total Production Time, Total Additional Time, and Total Run Time
For a production order, it displays the corresponding values on the Components tab for the resource with the longest Total Run
Time.
Remarks
Enter any additional information regarding the production order.
More Information
Production Order Window
Variance Report
This report shows the contribution of each production component to the final production variance for a selected production order.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:10 AM
To open this report, in the Production Order window, choose the Summary tab and click the link arrow next to the Total Variance
field.
 Note
The variance report is only available if:
The Use Perpetual Inventory option is selected in Administration System Initialization Company Details Basic
Initialization tab.
There is at least one issue for production or receipt from production transaction.
If you need to perform a manual analysis of the product cost and production order variance, use the document creation date
instead of the posting date. This allows you to sort the transactions according to the order in which they were added.
The default view of the report displays the component rows related to the production order. You can expand any component row in
the default view to see second-level lines with additional data. Use the Expand All and Collapse All buttons to expand or collapse
all rows at once.
Variance Report Fields
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Type
Displays whether the row is for an item or resource type component, by-product, or product revaluation.
When Product Revaluation appears in the row, it reflects the amount behind the journal entry postings upon production order
closure. For more information about product revaluation, see the section Journal Entry Postings Behind Production Documents in
the topic Production Costing.
Serial or Batch Type
 Note
This field is only displayed for inventory lines and is not visible by default.
Displays Serial for serial number items, Batch for batch items, and Regular for items not managed by serial numbers or batches.
Cost
Displays the average cost calculated as the total or estimated total divided by the quantity.
Estimated Total
 Note
This field is displayed for all rows in the default view. For second-level lines in the expanded view, the field is only displayed for
contribution lines or product type lines. For more information, see Contribution Line.
Displays the estimated total transaction value. This field is not displayed by default.
Variance
Displays the cumulated variance per specific component. The sum of all component variances matches the amount in Total
Variance field.
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:10 AM
Inventory Valuation Method
For inventory lines, this field displays the inventory valuation method used at the time that the transaction was posted.
For non-inventory lines, this field displays Standard.
Issue Type
For component lines, this field displays the issue method (Backflush or Manual) specified in the production order.
Contribution Line
If there is a contribution value related to the finished product from an issue from production line, this field displays Yes.
Source Journal Entry No.
The journal entry number linked to the specific document represented by the line.
Target Document
 Note
This field is only displayed for contribution lines.
Displays the document type that generated the contribution to the source document.
Message ID
Displays the transaction identifier. The sequence of the Message ID numbering allows you to identify the transaction sequence.
Production Order Window: Attachments Tab
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
1. Right click the Target Path column to open the context menu. Choose Change Path.
2. The Browse For Folder window appears, displaying the target path folder and any available subfolders. You an create new
subfolders in this window, if needed (subject to respective authorizations).
3. Select the required subfolder and choose OK.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:10 AM
4. The Target Path in the document is updated accordingly and the attachment is stored in the newly defined folder.
5. Choose Update.
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Releasing a Production Order
Procedure
1. From the SAP Business One Main Menu, choose Production Production Order .
Switch to Find mode.
2. Enter either the production order number or the product number and choose Find to display the relevant production order
details.
3. You can update the production order type, component items, the planned and base quantity, the warehouse, and the issue
method.
4. Change the production order status from Planned to Released to release the production order to the shop floor.
5. When the production order is released, you can choose either Report Completion or Issue Components.
6. Choose Update to save the changes and choose OK to exit the window.
More Information
Production Orders
Production Order Window
Issuing Components to a Production Order
Procedure
You can issue components of the manual issue method to the Standard or Special production order.
1. Choose Production Production Order .
Switch to the Find mode.
2. Choose the released Production Order.
3. In the Go To menu, choose Issue Components.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:10 AM
 Note
Alternatively, from the Main Menu, choose Issue for Production and then from the list, choose the relevant open
Production Order.
The Issue for Production Window is displayed.
4. In the Issue Components - Selection Criteria window, specify the selection criteria for the components you want to add to
the production order.
5. Optionally, change the quantity value or the warehouse.
6. Choose Add to save the information.
7. Display the Production Order window and check the Summary tab for the changes.
 Note
You may return issued components to a warehouse, either to correct mistakes or return unused components.
More Information
Production Orders
Production Order Window
Reporting Production Order Completion
Procedure
1. Choose Production Production Order .
Switch to the Find mode.
2. Choose the Released Production Order.
3. On the Go To menu, choose Report Completion.
 Note
Alternatively, you can choose Receipt from Production from the Main Menu and choose the open Production Order
from the list.
The Receipt from Production window is displayed.
4. You can change the quantity and the warehouse values. You can also change the type to either Complete or Rejected.
Completed and rejected quantities are recorded separately on the Summary tab of Production Orders. Rejected quantities
and complete quantities enter inventory and impact inventory valuations in the same way. You can choose to remove
rejected items from inventory manually.
5. Choose Add to save the information.
6. Display the Production Order window and check the Summary tab for the changes.
 Note
You can also report disassembly for the Disassembly Production Order. In that case, you receive the components of the
disassembled Production Order in the warehouse and issue the product from the warehouse.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:10 AM
Related Information
Production Orders
Production Order Window
Closing a Production Order
Procedure
1. Choose Production Production Order .
Switch to the Find mode.
2. Enter the Production Order number and choose Find or enter the product number and choose Find to display the relevant
production order details.
3. Verify that you have completed all the steps of the Production Order.
4. Choose Close in the Status field.
5. Choose Update to save the changes.
6. Choose OK.
Related Information
Production Orders
Production Order Window
Including Additional Costs to a Production Order
Context
Apart from costs of inventory items that are consumed during production, you can also include additional costs, such as labor,
machinery and overheads, to a product order.
You can use the following options to apply overhead costs to the product cost:
Additional Quantity
Use this field in the production order to account for material that is consumed in the production line, or to reflect the scrap
of raw materials.
Non-inventory items
You can set an item to non-inventory and define the unit cost in the item master data document. You can do this in both
perpetual inventory and non-perpetual inventory systems. The unit cost can be different for each warehouse if you select
the checkbox Manage Item Cost per Warehouse on the Basic Initialization tab of the Company Details window. Non-
inventory items always use the Standard valuation method.
 Caution
If you have installed a patch, or upgraded SAP Business One, and the non-inventory item does not have an associated
WIP account, the system displays an error message when you open a Receipt from Production window. To solve this
issue, open the Production window and choose Update.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:10 AM
For information about the setup for non-inventory items, see the Procedure section below in this topic.
Resources
Use resource master data for commodity, machine, labor, or other assets. You can utilize more extensive and flexible
functions with resources than non-inventory items. You can split the resource cost into several portions and different G/L
accounts to them. The G/L accounts can be determined directly or by the advanced G/L account determination rules. You
can also track resource capacities and allocate them to production orders to specific dates, or you can calculate production
order due dates based on your current resource capacities. Resources are further utilized with the production routing
feature.
Linking resources to non-inventory items
The benefit of linking a resource to a non-inventory item is that the cost rate is defined in the resource master data and is
valid also for the linked non-inventory item. Moreover, you can also utilize this interlinked resource in sales and purchasing
documents.
For more details on features related to resources, production routing, and linking resources to non-inventory items, see the
guide How to Work with Resources and Production in SAP Business One 10.0.
Procedure
1. Set the Item to Non-Inventory.
Choose Inventory Item Master Data , and deselect Inventory Item.
2. Set the Valuation Method to Standard (for perpetual inventory only).
Choose Inventory Item Master Data , select the Inventory Data tab, and in the Valuation Method field, select
Standard.
3. Defined Expense, WIP Material, and WIP Variance accounts (for perpetual inventory only).
Choose Administration Setup Financials G/L Account Determination Inventory tab.
4. Defined the Standard Cost for the Item (for perpetual inventory only).
Choose Inventory Item Master Data , select the Inventory Data tab and in the Item Cost field, specify the cost.
5. Defined the Issue Method as Backflush.
Choose Inventory Item Master Data , select the General tab and in the Issue Method field, select Backflush.
 Note
Non-inventory items must use the backflush issue method.
6. Add the non inventory item to the BOM.
For more information, see Defining Bill of Materials (BOMs).
You can change the required additional costs value by changing the value in the Planned field.
You can set the price for the non-inventory item (for non-perpetual inventory only)
 Note
A non-inventory item cannot be a by-product.
Results
The Item WIP Material account is copied to the production order and cannot be changed.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:10 AM
 Note
A subsequent change to the WIP Material account does not influence the production order.
The expense account is taken from the Expense Account field on the Warehouse tab.
Related Information
Production Orders
Production Costing
Upon the completion of a production order, you can check the product cost figures of the production order in the Production Order
Window: Summary Tab.
The product cost calculation is determined using the valuation method:
Standard – When a product is valuated by standard cost, no calculation is made, and the cost is copied from the item
master data upon report completion.
The component cost does not affect the product cost. If there is a difference between the cost of the issued components
and the cost of the received products, a Total Variance value is displayed in the Summary tab of the production order. The
total variance will not be cleared upon production order closure.
Moving Average – When a product is valuated by moving average, two figures are required for product receipt into
inventory: receipt quantity and total value added to the inventory. The total value is the product cost, which is the sum of all
the component costs used for those products.
FIFO – When a product is managed by FIFO, each report completion opens a new cost layer for the product in the inventory.
The quantity in the layer is the quantity of the product that was just reported as completed. The cost of the product is the
sum of all the component costs used for the quantity of the completed product divided by the quantity of the product.
The cost of a FIFO or moving-average product is the sum of its component costs and additional costs (such as labor and
overhead). To ensure accurate calculations of product cost, even if the components were issued manually, SAP Business
One uses the cost of the items issued to the production order and not the cost of the items currently in inventory. This
avoids differences between the actual cost of the components used in the order and the value of the product.
 Note
Unless otherwise specified, the cost calculation method described here is only relevant for standard and special production
orders, but not for disassembly for companies managing perpetual inventory.
Using route stages in a production order has no impact on product costing.
Variables for Product Cost Calculation
On every report completion, the system checks the following variables for each manually issued component in interim
calculations:
Issued component quantity – The total quantity of a component that is already issued in all issues for production
documents based on the production order. This value is visible in the Production Order Window: Components Tab.
Expected component quantity –The quantity of a component that is required for completion of the quantity of the product
in a single receipt from production document that is yet to be added. For example, if you are about to add a receipt from
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:10 AM
production for 40% of the planned product quantity, the expected component quantity will be 40 % of the planned
component quantity. Expected component quantity = quantity of product to be received / planned product quantity x
planned component quantity. This value is invisible.
Applied component quantity –The total quantity of a component that has been reported for completion of the quantity of
the product in all receipts from production documents. For example, if you add a receipt from production for 40% of the
planned product quantity and a second receipt from production for 20% of the planned product quantity, the applied
component quantity will be 60% of the planned component quantity. Applied component quantity = total quantity of
received products in all receipts from production / planned product quantity X planned component quantity. This value is
invisible.
The issued component quantity consists of the applied component quantity and the excess component quantity. The excess
component quantity is extra quantity that can be "applied" in case you add further receipts from production. If no further receipts
from production are added, the product cost is increased by the value of the excess component quantity when the production
order is closed. Such an increase is only performed if the produced quantity is still in stock when the production order is closed. If
the product is sold or issued from stock before the closure of the production order and the in-stock quantity is zero, the stock
value will not be increased. If part of the produced quantity is in stock, only this part of the product quantity is revalued.
If the issued component quantity in all issues for production documents is less than what is required for the received quantity of
the product in all receipts from production documents, the applied component quantity will be higher than the issued quantity. If
the issued component quantity is higher than what is required for the received quantity of the product, only part of the issued
quantity, or the applied quantity, will be counted in the product value.
If the applied quantity is greater than or equal to the issued quantity, this means that all the issued quantity of components for the
production order have already been used, and the required quantity is yet to be reported as issued from the warehouse. Since the
cost of the items that were actually used for the products is unknown, SAP Business One takes the current prices from the
inventory.
If the issued quantity is greater than the applied quantity, SAP Business One finds the cost of the components that were issued
and not used, and uses them in the calculation of the product cost. When finding those components, the issuing order of the
components is taken into account, meaning that the first components to be issued are the first to be used. The components
following those that were used are the first to be used for the cost calculation.
If the sum of the expected quantity and applied quantity is greater than the issued quantity, meaning that not all needed quantity
was issued, SAP Business One needs to make an assumption for the component cost, so it takes the current prices from the
inventory.
 Example
Product AB consists of item A and item B with the manual issue method. When the production starts, three of item B are
initially issued and cannot be used in the production process. The three items go to waste and are represented in SAP Business
One as additional quantity. The production order is then released with the following parameters:
Planned Quantity (of the product): 3
Base Quantity (of both components): 1
Planned Quantity of components:
Item A: (base quantity x planned product quantity) + additional quantity = 1 x 3 + 0 = 3
Item B: (base quantity x planned product quantity) + additional quantity = 1 x 3 + 3 = 6
Scenario
1. You have issued the full planned quantities of the components for production. The issued quantity of item A is 3. The
issued quantity of item B is 6.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:10 AM
2. You add a receipt from production to receive one-third of the planned product quantity (in other words, one piece). The
system calculates the expected component quantity as follows:
Item A: 1
Item B: 2
3. After adding the receipt for production, the quantities of component A are as follows:
Issued component quantity = 3
Applied component quantity = 1
Excess component quantity = 2
Product Costing Principles
The production order lifetime refers to the period between when the production order status is set to Released and when it is set
to Closed.
Product cost is calculated in the following stages:
When a receipt from production is added.
When the production order is closed.
When Production Cost Recalculation Wizard is run.
When a receipt from production is added, the following principles apply to product cost calculation:
Product cost can be derived from the following:
The actual cost of the applied quantities of components.
The estimated cost of the expected component quantities. Estimation occurs when there are insufficient issued
component quantities.
The combination of actual and estimated costs. If part of the required quantities of components are already issued,
this part will be valuated with the actual cost. The remaining part which is not yet issued for production will be
valuated with the estimated cost.
When the component items are managed by the serial/batch valuation method and no component quantity has been
issued yet, the product is received with a zero cost rate.
Actual product cost is the sum of the issued component quantities multiplied by the component unit costs that were valid when
the components were issued for production.
Estimated product cost is calculated as the sum of the expected component quantities multiplied by the component unit costs
that are valid when the receipt from production is added.
In the following scenarios, the product cost is always based solely on the actual component costs (no cost estimation occurs):
All product components are issued by the backflush method.
The product and its components are in a Disassembly type of production order.
The product cost is determined by the Standard valuation method.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:10 AM
Journal Entry Postings Behind Production Documents
The following posting rules apply to the journal entries of different production documents:
Issue for production:
When you issue components for production, the component values are transferred from the inventory account (credit) to a
WIP (work-in-progress) inventory account (debit).
Receipt from production:
When you receive the product (or by-product), its value is transferred from the WIP account (credit) to the inventory
account (debit).
Production order:
Upon production order closure, any existing production variance is potentially cleared and the product cost is adjusted
according to this value. The posting behind the closure of a production order consists of the following steps:
1. If a difference exists between the value of the received product (and by-product) and the value of the issued
components, this difference is treated as total variance in SAP Business One. Component WIP accounts values are
zeroed and transferred to the WIP variance account of the product.
2. The WIP variance account is cleared against the product’s inventory account. In the case of a negative variance (for
example, component overconsumption), the product’s inventory account is debited. In the case of a positive
variance (for example, component underconsumption), the product’s inventory account is credited.
The amount behind the production order closure posting is reflected by the Product Revaluation type in the Variance
Report.
 Example
The tables below show information that is extracted from the variance report of a production order and a journal entry
generated upon the closure of the production order.
The product was received by a warehouse with a cost estimate of 10 US dollars. However, the total value of the issued
components was only 5 dollars. Upon the production order closure, the product cost is revalued: the WIP variance
account is cleared against the inventory account. The inventory account is credited to reflect the decrease in the
product value.
Variance Report
# Type No. Qty Cost Total Variance
2 Product Product 1.000 $ 10.00 $ 10.00 $ 0.00
3 Product Product 0.000 $ 0.00 $ -5.00 $ -5.00
Revaluation
Journal Entry
# G/L Acct/BP Name Debit Credit
1 Inventory - Work In Progress $ 5.00
2 WIP Material Variances $ 5.00
3 Inventory account $ 5.00
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:10 AM
# G/L Acct/BP Name Debit Credit
4 WIP Material Variances $ 5.00
However, in special cases where the produced quantity is no longer available in the warehouse when the production order is
closed, the product will not be revalued. The Product Revaluation type will not appear in the Variance Report. This occurs,
for instance, when the produced quantity is sold before the production order is closed. In such case, the total variance is
not transferred to the product value and remains allocated on the production order and the following accounts, based on
the product valuation method:
If the valuation method is Serial/Batch, the variance remains on the price difference account.
If the valuation method is Moving Average or FIFO, the variance remains on the WIP variance account.
If part of the produced quantity is available in the warehouse when the production order is closed, only this part of the
product quantity will be revalued. For example, if one third of the produced quantity leaves the warehouse with an A/R
invoice, only two thirds of the product quantity is revalued, while one third of the total variance retains on the production
order and is not transferred to the product value. This total variance amount will be posted to the following accounts,
depending on the product valuation method:
If the valuation method is Serial/Batch, the variance is posted to the price difference account.
If the valuation method is Moving Average or FIFO, the variance remains on the WIP variance account.
A product with the Standard valuation method are not revalued when a production order is closed. The total variance
retains on the production order in the WIP variance account.
For more information about production order closure, see the guide How to Work with Resources and Production in SAP
Business One 10.0.
Production Costing of Non-Perpetual Inventory Management
In companies that use non-perpetual inventory systems, the product cost can be defined in the receipt from production. You can
manually specify the product cost, or choose a price list from which the cost is derived. When you add a receipt from production,
the last purchased price is filled in for each product item.
You can also specify the prices of the product and component items in the Bill of Materials window, or by using the Update Parent
Item Prices Globally function.
When you add a receipt from production, no cost estimation occurs, and thus the total production variance is not cleared when the
production order is closed. You can check the product valuation using the inventory valuation report.
Related Information
Variance Report
Production Orders
Production Order Window
Journal Entry
Common Cases in Production Costing
Special Cases in Production Costing
Production Costing Cases for Disassembly Production Orders
Common Cases in Production Costing
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:10 AM
This topic lists frequently encountered scenarios, situations, or examples related to the calculation and analysis of costs in the
production process.
Context
You work for a manufacturing company. 6 item components have been received by your warehouses. A goods receipt document is
generated with the following information in the Contents tab:
| #   | Item No.         | Quantity | UDF Layer / Batch | Unit Price |
| --- | ---------------- | -------- | ----------------- | ---------- |
| 1   | C1 MAP           | 5        |                   | $ 2.00     |
| 2   | C2 FIFO          | 5        | layer 1           | $ 3.00     |
| 3   | C2 FIFO          | 5        | layer 2           | $ 4.00     |
| 4   | C3 S/B valuation | 5        | batch 1           | $ 3.00     |
| 5   | C3 S/B valuation | 5        | batch 2           | $ 4.00     |
| 6   | C4 STD           | 1        |                   | $ 5.00     |
The component items above are named according to their valuation methods:
C1 MAP: Moving Average
C2 FIFO: First In, First Out
C3 S/B valuation: Serial/Batch
C4 STD: Standard
As shown in the user-defined field UDF Layer / Batch, the FIFO items were received in two layers with different prices. The
component items valuated by batch were received in two batches with different cost rates.
For demonstration purposes, we add a user-defined field UDF Current Item Cost in the Components tab of the production
order to show the cost of each component.
Case 1: A Receipt from Production Is Added Before Components Are Issued
1. You create a production order for Product A with planned quantity 3. Product A consists of one component C1 MAP. You
specify the following details in the Components tab:
Type: Item
Base Quantity: 1
Issue Method: Manual
UDF Current Item Cost: 2 US Dollars
2. You release the production order.
3. You directly add a receipt from production to receive the planned quantity of 3 products, without issuing any components.
Result
You can see the following information in the Variance Report:
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:10 AM
# Type No. Qty Cost Total Variance
1 Item Component C1 MAP 0.000 $ 0.00 $ 0.00 $ 6.00
2 Product Product 3.000 $ 2.00 $ 6.00 $ 0.00
In the Variance Report, the product value shown in the Cost column is derived from an estimate of the component cost, which is
the component’s item cost when the receipt from production was added (in other words, 2 US dollars).
Case 2: Excess Quantity of Components Is Issued
1. You create a production order for Product A with planned quantity 3. Product A consists of one component C1 MAP. You
specify the following details in the Components tab:
Type: Item
Base Quantity: 1
Issue Method: Manual
UDF Current Item Cost: 2 US Dollars
2. You release the production order.
3. You issue 4 components, even though the planned quantity is only 3.
4. You receive the planned quantity of 3 products.
Result
You can see the following information in the Variance Report:
# Type No. Qty Cost Total Variance
1 Item Component C1 MAP -4.000 $ 2.00 $ -8.00 $ -2.00
2 Product Product 3.000 $ 2.00 $ 6.00 $ 0.00
In the Variance Report, the product value shown in the Cost column is calculated to be the expected component quantity
multiplied by its actual cost divided by the completed product quantity: 3 x 2 US dollars / 3 = 2 US dollars.
The excess quantity is not considered in the product value during receipt from production. If you do not add further receipts from
production, this excess quantity will only affect product cost upon closure of the production order.
Case 3: Product Cost Estimation of FIFO Components Received in Multiple
Shipments
1. You create a production order for Product FIFO with planned quantity 2.·Product FIFO consists of one component
C2 FIFO with base quantity 1. The component has 2 layers with different cost rates: 3 US dollars in layer 1 and 4 US dollars
in layer 2. Each layer has an in-stock quantity of 1.
2. You release the production order. The component is issued manually. Yet, you have not issued any quantity of the
component.
3. You create two receipts from production to receive the first and second planned product, respectively.
4. You view the Variance Report to check the product cost.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:10 AM
Result
In the Variance Report, the product cost estimate of the value shown in the Cost column is calculated from the cost of the earliest
FIFO layer 1 for both receipts (in other words, 3 US dollars). Even if you create one receipt from production for multiple production
orders with the same FIFO component simultaneously, the estimation still uses the same earliest available FIFO layer.
If you create multiple receipts from production, the estimation of the product cost upon each receipt is calculated independently
based on the corresponding earliest layer, without taking any previous estimations into account. In this example, since no
component has been issued, the product cost estimation still takes layer 1 as the earliest layer.
Case 4: Product Cost Estimation of Zero or Insufficient Available Quantity of
Components
You create a production order with one component. You have not added any issue for production yet, or the quantity of
components that you have issued is less than required. You receive the planned quantity of the product by adding a receipt from
production.
Result
The system posts the product cost based on an estimate derived from the current component cost of the on-hand component
quantity.
If the component is valuated by FIFO:
When an estimation is made, the expected component quantity is valued with the cost of the earliest FIFO layer that is on-
hand, followed by later on-hand FIFO layers. If the component has zero on-hand quantity, but has a specified cost, the most
recent FIFO layer will be used for the estimate.
If the component is valuated by Moving Average:
The current moving average value is used.
If the component is valuated by Serial/Batch:
The average value of issued component batches is used. If no components are issued, a zero value is used instead of an
estimate.
If the component has a zero on-hand quantity and the component has never been received in the warehouse (in other words, it
does not have a specific cost), then the product has zero cost.
Case 5: Impacts of Deleted Components on Product Cost
Your production order consists of 3 components. You delete a component from the production order.
Result
If you delete a component with zero issued quantity, it has different impacts on the product cost, depending on the deletion timing.
Zero issued quantity occurs when a receipt from production is added, but the component is still not issued for production. If the
deletion happens before receipt from production, the product cost is not impacted. However, if the deletion happens after receipt
from production, the deleted component affects the product cost as it contributes to part of the product cost estimate.
Deleted components are no longer visible in production order rows; however, you can view deleted components and their cost
impact in the production Variance Report. Additionally, deleted components (with or without a cost impact) are displayed in the
production order change log.
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:10 AM
Components with non-zero issued quantities cannot be deleted directly. To delete such a component, you need to return the
issued quantity by adding a receipt from production and choosing the Return Components button. Backflush components cannot
be returned.
Case 6: Impact of Returned Components on Product Cost
Your production order consists of components valuated by different methods. You issue these components for production. Upon
reporting product completion, you create a receipt from production to return some components from the production order.
Result
Returning components does not immediately affect product costing. The cost of the returned components in the receipt from
production is calculated differently according to the component valuation method:
Moving Average and FIFO
The returned component cost is equal to the issued component cost. The components issued last are returned first (LIFO
principle).
Batch/Serial
The cost of the received batch equals the cost of the issued batch. However, if you return components and create a new
batch, instead of receiving the originally issued batches, the new batch will be created with zero cost.
Case 7: Impact of By-Product on Product Cost
1. You add a production order with one component C1 MAP and one by-product.
2. You issue the planned quantity of 1 component at a cost of 3 US dollars.
3. You add a receipt from production, which includes the by-product and the information from the table below. You manually
enter 1 US dollar as the by-product cost.
Information from Contents Tab of Receipt from Production
| Item No.   | Quantity |     | Unit Price | Item Cost | By-Product          |     |
| ---------- | -------- | --- | ---------- | --------- | ------------------- | --- |
| Product    | 1        |     | $ 3.00     | $ 3.00    |                     |     |
| By-Product | 1        |     | $ 1.00     | $ 1.00    | <Checkbox Selected> |     |
4. You close the production order and check the Variance Report.
Result
The following information shows up in the Variance Report:
| #   | Type           | No.        | Qty    | Cost   | Total   | Variance |
| --- | -------------- | ---------- | ------ | ------ | ------- | -------- |
| 1   | By-Product     | By-Product | 1.000  | $ 1.00 | $ 1.00  | $ 1.00   |
| 2   | Item Component | C1 MAP     | -1.000 | $ 3.00 | $ -3.00 | $ 0.00   |
| 3   | Product        | Product    | 1.000  | $ 3.00 | $ 3.00  | $ 0.00   |
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:10 AM
| #   | Type    | No.     | Qty   |     | Cost   |     | Total   | Variance |
| --- | ------- | ------- | ----- | --- | ------ | --- | ------- | -------- |
| 4   | Product | Product | 0.000 |     | $ 0.00 |     | $ -1.00 | $ -1.00  |
Revaluation
As you can see from the variance report, if you define a cost for a by-product, it impacts the product cost when the production
order is closed. When the production order is closed, the product cost is reduced by the value of the by-product.
In our example, upon production order closure, the cost of the by-product, 1 US dollar, is subtracted from the product cost based
on the receipt from production, 3 US dollars. This calculation is displayed in the last row with the Product Revaluation type.
Case 8: The product Is Received by Different Warehouses; or the Product Warehouse
Is Changed Before the Production Order Is Closed
1. You have a production order with a single component C1 MAP. The product warehouse is 01. The planned product quantity
is 2. The base quantity of the component is 1. The component is issued manually.
2. You issue 3 components for production.
3. You add a receipt from production to receive and store 1 planned quantity of product in warehouse 02.
4. You add a second receipt from production to receive and store another planned quantity of product in warehouse 03.
5. As you have issued a higher quantity of components than planned, excess component quantity occurs.
Information from Components Tab of Production Order
| Type | No. | Base Qty | Planned Qty | Issued |     | Issue  | Warehouse | UDF     |
| ---- | --- | -------- | ----------- | ------ | --- | ------ | --------- | ------- |
|      |     |          |             |        |     | Method |           | Current |
Item Cost
| Item | C1 MAP | 1   | 2   | 3   |     | Manual | 01  | 2 US Dollars |
| ---- | ------ | --- | --- | --- | --- | ------ | --- | ------------ |
6. You close the production order and check the Variance Report. There is a 2 dollar difference between the total product cost
and the total component costs:
| Type           | No.     | Qty    |     | Cost   |     | Total    | Variance |     |
| -------------- | ------- | ------ | --- | ------ | --- | -------- | -------- | --- |
| Item Component | C1 MAP  | -3.000 |     | $ 2.00 |     | $ -6.000 | $ -2.00  |     |
| Product        | Product | 2.000  |     | $ 2.00 |     | $ 4.00   | $ 0.00   |     |
7. You close the production order. The G/L account on the product is set by warehouse. Each warehouse has its own separate
inventory account defined in the Accounting tab in the Warehouses - Setup window. You want to know if the system
revalues the product in both warehouses when you close the production order.
Result
In the Summary tab of the Production Order window, the Total Variance field value displays $ 0.00.
Choose the link arrow next to the Journal Remark field to open the journal entry. In the journal entry, you can see that the system
correctly revalues the product in each warehouse by the cost at which the product has been received.
Information from Journal Entry
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:10 AM
# G/L Acct/BP Name Debit Credit
1 Inventory - Work In Progress $ 2.00
2 WIP Material Variances $ 2.00
3 WIP Material Variances $ 1.00
4 Inventory account of warehouse $ 1.00
02
5 WIP Material Variances $ 1.00
6 Inventory account of warehouse $ 1.00
03
Case 9: A Standard-Valuated Product Is Revalued Between Two Partial Production
Receipts
Your production order consists of components valuated by the Standard method. You revalue the product in the interval between
two partial production receipts.
Result
Products are always received at the standard cost rate that is current when a receipt from production is added. If an inventory
revaluation occurs between two receipts from production, the second receipt takes the new cost rate which is set in the inventory
revaluation document.
Case 10: Component Cost Changes During Production Order Lifetime
You change the component cost during the production order lifetime.
Result
In general, component cost changes do not have immediate impact on the product cost. They are only reflected in the product cost
when a new receipt from production is created. The implications of component cost changes depend on whether the components
have already been issued for production or not:
When the component has already been issued for production:
To reflect the component cost change in the product cost, perform the following steps:
1. Return the issued components using the return components functionality.
2. Add inventory revaluation to change the component cost.
3. Issue the components again at the new cost rate.
When the component has not yet been issued for production:
If you have already received the product without issuing the components, the product cost was posted as an estimate
based on the initial component cost. The new component cost will only be reflected in the product after you complete the
following two steps:
1. Add the issue for production. The new component cost will be displayed.
2. Close the production order.
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:10 AM
Case 11: Changing Product Cost of Closed Production Order
You want to change the product cost of a closed production order in order to reflect an increase in the component cost.
Solution
You can use the product cost recalculation wizard to adjust the product cost of a closed production order due to an increase in the
component cost. However, the wizard can only be used to revalue product items with the Serial/Batch valuation method and with
at least one component valuated by the Serial/Batch method. For more information about the product cost recalculation wizard,
see How to Set Up and Use Serial/Batch Valuation Method in SAP Business One 10.0.
For products with other valuation methods, you can use the inventory revaluation document based on a manual calculation. Please
note that this will only revalue the product quantity that is available in stock.
Related Information
Production Costing
Special Cases in Production Costing
Production Costing Cases for Disassembly Production Orders
Special Cases in Production Costing
This topic lists unique, uncommon, or exceptional scenarios and examples related to the calculation and analysis of costs in the
production process.
Case 1: The Planned Quantity of the Parent Item Changes During Production
You create a production order. You change the planned quantity of the parent item during the production order lifetime.
Result
If there is zero additional quantity, the change in the planned product quantity has no impact on the product cost. This is because
when the planned product quantity is changed, the planned component quantities are increased accordingly.
While you can increase the planned product quantity at any time during the production order lifetime, there are restrictions on
situations where you can decrease the planned product quantity. For instance, if you have already issued some component
quantity, you cannot decrease the planned product quantity to a level that the issued component quantity is greater than the
planned component quantity.
Case 2: Costing of Rejected Product
In a receipt from production, you reject a certain produced quantity of a product by selecting the transaction type Reject in the
Trans. Type field.
Result
There is no difference in costing principles for rejected and completed quantities of a product.
However, you may consider decreasing the value of the rejected quantity of the product (for example, if the item did not pass the
quality check). If so, make sure that the option Manage Item Cost per Warehouse is selected ( Administration System
Initialization Company Details Basic Initialization tab). In the receipt from production, the rejected quantity of the product
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:10 AM
should be received by a special warehouse. After the production order is closed, you can add an inventory revaluation document to
decrease the cost of the faulty product.
You can find the total completed quantity and rejected quantity of a product from all receipts from production in the Quantities
section in the Summary tab of the Production Order window.
Case 3: The Additional Component Quantity Changes During Production
The additional component quantity changes during the lifetime of a production order.
Result
Additional component quantity is part of the planned component quantity and thus affects the product cost. While you can
increase the additional quantity at any time during the lifetime of a production order, there are restrictions on the situations where
you can decrease the additional quantity. For instance, you cannot decrease the additional component quantity to a level that the
issued quantity is greater than the planned component quantity.
Case 4: Changing the Planned Quantity of a Backflush Item
You need to change the planned quantity of a backflush item.
Solution
Once a component has been issued, you cannot change the planned quantity. If you need to issue a higher component quantity,
you can add a new row in the production order for the component and change the issue method to Manual.
Case 5: Changing the Valuation Method of a Component or Product During
Production
You want to change the valuation method of a component or a product during the production order lifetime.
Solution
You can change the valuation method for items if the items meet the conditions listed in the explanation for the Valuation Method
field in the Item Master Data: Inventory Data Tab. For production-related documents, the following conditions also apply:
You can change the valuation method of both product and component items if the production order is open and no receipt
from production or issue for production documents have been added.
You can change the valuation method of component items even if the production order is open and a receipt from
production or issue for production transaction exists.
You cannot change the valuation method of product items if the production order is open and a receipt from production or
issue for production transaction exists.
Case 6: Changing the Management Method of a Component or Product During
Production
You want to change the management method of a component or a product during the production order lifetime.
Solution
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:10 AM
If the relevant requirements for changing the management method are fulfilled, you can change the management method between
None, Serial Numbers, and Batches for an item through the Manage Item By dropdown list in the Item Master Data window.
However, you cannot change the management method of a serial/batch valuated product if you have already added a receipt from
production and the production order has not been closed.
Case 7: The Bills of Materials Are Redesigned During Production
The bills of materials are redesigned during the production order lifetime.
Result
Changes to bills of materials do not affect existing production orders. Bills of materials can even be deleted when the production
order status is open. Bills of materials only serve as a template when you create the production order.
Case 8: The Same Item or Resource Appears Multiple Times in a Production Order
The same item or resource appears in more than one row in the Components tab of a production order.
Result
This is a common scenario. There are no special implications on product costing. The planned component quantity can be broken
down into several rows in the Components tab of a production order.
Related Information
Production Costing
Common Cases in Production Costing
Production Costing Cases for Disassembly Production Orders
Production Costing Cases for Disassembly Production Orders
This topic lists cases related to the calculation and analysis of costs for Disassembly-type production orders.
Case 1: Cost of Received Components in Disassembly Production Order
You create a disassembly production order. The product is taken apart. The components are received with a certain cost.
Result
No cost estimation occurs with a disassembly production order. All postings are based on the actual cost.
The cost of the received components depends on the defined cost of the components:
If you are managing item cost by warehouse (on Company Details: Basic Initialization Tab, the Manage Item Cost per
Warehouse checkbox is selected), the system uses the item cost from the warehouse where an item was previously
received.
If you are managing item cost on the company level (on Company Details: Basic Initialization Tab, the Manage Item Cost
per Warehouse checkbox is deselected), the system uses the item cost from the item master data.
If you use the FIFO valuation method for your components, the following rules apply:
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:10 AM
If a FIFO item has defined costs and multiple FIFO layers available, the cost of the earliest layer is used for the
receipt of the component. In other words, the component cost is not dependent on the received quantity. The costs
of later FIFO layers are disregarded. All received quantity is considered in one single FIFO layer. The cost of this FIFO
layer is equal to the cost of the earliest available FIFO layer.
If a FIFO component has a defined cost and zero available quantity, the FIFO component takes the cost of the most
recent FIFO layer which has left the warehouse or company.
If you use the Batch/Serial valuation method for your components, the component cost depends on whether you create a
new batch/serial number or use an existing batch/serial number in the receipt from production document. If you create a
new batch/serial number to receive a component, the component has zero cost. If you receive a component with an
existing batch/serial-number, the component cost takes the current cost of the batch/serial-numbered component.
If you use the Standard valuation method for your components, the components are received at the current standard cost
that is valid in the receiving warehouse.
If a FIFO or Standard component does not have defined cost in the receiving warehouse, it is received with zero cost.
The product is issued at the current cost displayed in the issue for production document.
When a disassembly production order is closed, the production variance is not cleared (in other words, the cost of the received
components is not adjusted according to the actual cost of the issued product).
Case 2: Receipt from Production Is Not Displayed in Relationship Map
1. You add a disassembly type of production order with one single backflush component C1 MAP. The component is valuated
by the Moving Average method. The document number of the production order is 50. The planned quantity of the product
is 1. The product warehouse is 01.
2. In the Go To menu, choose Report Completion. Add the issue for production document that appears in order to ship the
product item to the inventory. The document number is 10.
3. Right click in the production order to open the context menu. Select Relationship Map in the context menu. In the
Relationship Map window that opens, you can view the relationship between the production order and the issue for
production. Yet, you do not see the receipt from production.
Cause
The receipt from production is only available for components with the manual issue method. In this example, as the issue method
of the component is backflush, the component item is received by the warehouse in the background. The receipt transaction does
not generate a dedicated receipt from production document. Both inventory movements (receipt and issue) are bound to the issue
for production.
If you want to display all inventory movements related to the production order, you need to generate the Inventory Posting List
report. To generate the report, right click in the production order to open the context menu. Select Inventory Posting List in the
context menu.
Report Example: Inventory Posting List by Production
Order #50
Document Whse Item No. Qty
SO 10 01 Product -1
SO 10 01 C1 MAP 1
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:10 AM
Production Costing
Common Cases in Production Costing
Special Cases in Production Costing
Work Orders
As of SAP Business One 2005, the Production Order has replaced the Work Order.
An automatic upgrade process means that if you worked with Work Orders in earlier versions of SAP Business One, you can move
seamlessly to the new Production Order. In addition, you can continue to view open Work Orders.
More Information
Upgrading from Work Orders to Production Orders
Upgrading from Work Orders to Production Orders
SAP Business One includes an automatic upgrade process from the old Work Order to the new Production Order. Only open work
orders are upgraded.
If you have previously worked with work orders, the upgrade facilitates a smooth transition to the Production module.
Comparison Between Fields in Work Order and Production Order
Upgrade from Work to Production Order
Work Order Production Order Description/Activity
Series Series The order of the series in the Work Order is
not maintained when upgrading to the
Production Order. All upgrades are created
according to default sequential numbering.
If several series exist in the Work
Order, all are added to the same
Production Order series.
If there are several series in the
Production Order, the Work Order
series are added to the last series.
If the last series has a number
limitation, it is removed.
No. Number The numbering in the Work Order is not
maintained when upgrading to the
Production Order. All upgrades are created
in the Production Order according to
default sequential numbering.
This field is not copied, but the next
available number for the selected
series is added.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:10 AM
| Work Order | Production Order | Description/Activity |
| ---------- | ---------------- | -------------------- |
If the Work Order includes several
rows, then each is a separate
Production Order.
The Work Order number is copied
to the Production Order remarks
field.
Est.Completion Date Due Date If the Est.Completion Date does not exist,
then the Due Date is the same as the Order
Date.
| Processor | User | If the user is defined as anonymous in the |
| --------- | ---- | ------------------------------------------ |
Work Order, then in the Production Order
this field contains, by default, the first super
user.
| Order Date | Posting Date | Renamed                             |
| ---------- | ------------ | ----------------------------------- |
| State      | Status       | Work Order is converted to Planned. |
Production Instruction is converted to
Released.
Work Completed is not upgraded.
|     | Origin | Upgraded Production Orders are defined |
| --- | ------ | -------------------------------------- |
here as Upgrade. Other options are Manual
and MRP.
| Item | Product No. | Each line item is copied to a separate |
| ---- | ----------- | -------------------------------------- |
Production Order.
Quantity Planned Quantity If the Quantity field in the Work Order is
positive, the system creates a standard
Production Order type, and the planned
quantity remains similar to the Work Order
quantity.
If the Quantity field in the Work Order is
negative, the system creates a Disassembly
Production Order type, and the planned
quantity remains the same as the Work
Order quantity, without the minus sign. For
example, -9 becomes 9 and order type
becomes disassembly.
| WH  | Warehouse |     |
| --- | --------- | --- |
Customer Ref. No. Remarks The customer reference number is copied
to the Remarks field.
| Completion Date  | Actual Closing Date |                                |
| ---------------- | ------------------- | ------------------------------ |
| Instruction Date |                     | Not copied in the upgrade      |
| Price            |                     | Not copied to Production Order |
In the Production Order the price for non
perpetual inventory system is determined
according to the product price in the BOM.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:10 AM
| Work Order |     | Production Order |     | Description/Activity |
| ---------- | --- | ---------------- | --- | -------------------- |
Manually changed product prices are not
reflected in the upgrade.
| Total            |     |     |     | Is not copied in the upgrade.            |
| ---------------- | --- | --- | --- | ---------------------------------------- |
| Instruction Date |     |     |     | Is not upgraded                          |
| Contact          |     |     |     | Is not upgraded                          |
| Additional Cost  |     |     |     | Is not upgraded; must be added manually. |

 Note
In the work order, each row represents a document. A -1 value indicates that this is disassembly. If the BOM includes a minus
value, it indicates a by-product. The production order does not use the minus symbol for the by-product, so the rows must be
removed manually.
Issue for Production
Issue for production is used to issue manual items to production orders, and to report the completion of disassembly orders.
When you add an issue for production, in addition to posting expenses for items, the same journal entry posts resource expenses.
Resource expenses are transferred from the resource expense account to the related resource WIP account. The total value posted
for each resource unit equals Total Std Resource Cost as defined in Resource Master Data. The actual posting is split across up to
ten resource expense accounts as defined by the advanced G/L account determination rules or the G/L account determination
and the WIP account that is defined in Account Code on the Issue for Production.

 Example
"ExampleResource1" has a "Total Std Resource Cost" of 100 per unit which is split between "Resource Std Cost 1" = 60
and "Resource Std Cost 2" = 40.
| Resource No.     | Total Std     | Std Cost  | Std Cost  |     |
| ---------------- | ------------- | --------- | --------- | --- |
|                  | Resource Cost | Expense 1 | Expense 2 |     |
| ExampleResource1 | 100           | 60        | 40        |     |
The journal entry in respect of the resource component consumption of 10 resource units is as displayed in the table
below.
| Account            | Debit | Credit |     |     |
| ------------------ | ----- | ------ | --- | --- |
| Std Cost Expense 1 |       | 600    |     |     |
| Std Cost Expense 2 |       | 400    |     |     |
| WIP Account        | 1000  |        |     |     |
The posting is added to the posting of any other item and resource component within a single journal entry that is
created when adding the issue for production. The total value that is posted to all the resource WIP accounts is added
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:10 AM
cumulatively to the Actual Resource Component Cost field on the Summary tab of the production order whenever an
issue for production is added.
Related Information
Issue for Production Window
Issue for Production Window
Use this window to issue manual items to production orders, and to report disassembly orders completion.
Backflush components are issued automatically.
To open the window, choose Production Issue for Production .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Issue for Production Fields
Number
Displays the sequential transaction number.
Series
Choose the series for the receipt from production.
Posting Date
Enter the transaction posting date. The current date is displayed by default.
Ref. 2
Enter any additional information regarding the issue for production.
Order No.
If you access the window from the Main Menu, specify the number of the open production order.
If you access the window from the Go To menu, the value is automatically displayed in the field.
Row No.
Specify the row number of the production order to report the issued quantity for that line.
Quantity
Specify the quantity of the issued items. The open quantity is displayed by default; however, you can update that value.
 Note
If the item is batch or serial number controlled, choose CTRL+TAB to update existing numbers or to create new serial and
batch numbers.
Whse
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:10 AM
Warehouse of the component item.
You can overwrite it before you post the inventory transactions for the line. To display Warehouses – (Default) – Setup, click .
Bin Location Allocation
 Note
The field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many component items are allocated from bin locations. You must allocate the same quantity of items from bin
locations as the quantity you specified in the document row; otherwise, the field is marked in red and you cannot add the
document.
To manually allocate items from bin locations, click to open one of the following windows:
Bin Location Allocation - Issue Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Number Selection Window
This window opens if the item in the document row is a serial item.
Batch Number Selection Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
Planned
Displays the planned quantity, which is the multiple of the planned product quantity and the base quantity.
Issued
Total quantity already issued to the production order.
Avail
Available quantity of the item in the specific warehouse.
Remarks
Enter any additional information regarding the issue of the production order.
Journal Remark
Displays the issue for production, by default. You can modify the value of the field.
For companies that do not use the perpetual inventory, there is a remark field in the transaction history file.
For companies that use the perpetual inventory, there is a remark field in the general ledger and the transaction history file.
Production Order
Displays the List of Production Orders window.
Select the required production order and choose the relevant items from the production order.
You can also use this window to issue components for several production orders in the same issue for production document.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:10 AM
Disassembly Order
Displays the List of Production Orders window for the disassembly production order. Choose the relevant items for the
disassembly.
Route Sequence
Displays the route sequence related to the item or resource component in the production order. The field is only visible when a
routed production order is selected for issuing.
Route Stage
Displays the route stage related to the item or resource component in the production order. The field is only visible when a routed
production order is selected for issuing.
Stage Description
Displays the description of the route stage related to the item or resource component in the production order. The field is only
visible when a routed production order is selected for issuing.
More Information
Production Orders
List of Production Orders
List of Production Order
In this window, choose items you want to issue for production or receive from production from a list of released production orders.
Select the required rows and select Choose.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
List of Production Order
Find
Use to search for a production order.
Document Number, Production Order Type, Start Date, Due Date, Item No., Item Description, Priority
Displays production order information.
More Information
Issue for Production Window
Receipt from Production
A receipt from production allows you to report the completion of a production order and post the finished product to the inventory.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:10 AM
Related Information
Receipt from Production Window
Receipt from Production Window
Use this window to report the completion of the product.
For Standard and Special production orders, post the finished product to the inventory.
For Disassembly production orders, post the components to the inventory.
To open the window, choose Production Receipt from Production .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Receipt from Production Fields
Number
Displays the sequential transaction number.
Series
Choose the series for the receipt from production.
Posting Date
Enter the transaction posting date. The current date is displayed by default.
Ref. 2
Enter any additional information regarding the receipt from production.
Order No.
If you access the window from the Main Menu, specify the number of the open production order.
If you access the window from the Go To menu, the value is automatically displayed in the field.
Item No., Item Description
Displays the item number and description after you enter the production order number.
Trans. Type
Choose the transaction type for the production order. Completed and rejected quantities are recorded separately on the Summary
tab of Production Orders. Rejected quantities and completed quantities enter inventory and impact inventory valuations in the
same way. You can choose to remove rejected items from inventory manually.
Complete: to report the completion of the product quantity.
Reject: to report the rejection of the product quantity
Quantity
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:10 AM
Specify the quantity of the completed or rejected items. The open quantity is displayed by default; however, you can update that
value.
 Note
If the item is batch or serial number controlled, choose CTRL + TAB to update existing numbers, or create new serial
and batch numbers.
You cannot update this field for by-products having the Backflush issue method. However, if you update the quantity of
the parent item, the quantity of the by-product is updated proportionally.
You can update this field manually for by-products having the Manual issue method. Updating the parent item's quantity
does not affect the received quantity of such by-products.
Unit Price
Information price of the item that is taken from the price list selected in the general area of the Goods Receipt window in the
Inventory module.
This filed is editable for by-products.
Item Cost
After adding the receipt from production, this field displays the following:
For parent items, the cost of the parent item which has been posted in the journal entry behind the receipt from production.
For by-products, the cost of the by-product which has been posted in the journal entry behind the receipt from production.
Whse
Warehouse of the reported product.
Bin Location Allocation
 Note
This field is available only if you have enabled bin locations for at least one warehouse.
If you have not enabled bin locations for the warehouse you specified in the document row, this field is blank and not editable.
Displays how many finished items are allocated to bin locations. You must allocate the same quantity of items to bin locations as
the quantity you specified in the document row; otherwise the field is marked in red and you cannot add the document.
To manually allocate items to bin locations, click to open one of the following windows:
Bin Location Allocation - Receipt Window
This window opens if the item in the document row is not managed by serials or batches.
Serial Numbers - Setup Window
This window opens if the item in the document row is a serial item.
Batches - Setup Window
This window opens if the item in the document row is a batch item.
Once the document is added, clicking the link arrow in this field opens Inventory Posting List.
Planned
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:10 AM
Planned quantity for the reported product.
Completed
Displays the quantity completed.
By-Product
A checkbox in this field indicates that the component item was entered with negative quantity in the bill of materials and
production order and therefore classified as by-product.
Remarks
Enter any additional information regarding the receipt from the production order.
Journal Remark
Displays the receipt from production, by default. You can modify the value of the field.
For companies that do not use perpetual inventory management, the receipt from production is displayed in the Remarks field in
the transaction history file.
For companies that use perpetual inventory, the receipt from production is displayed in the Remarks field in the General Ledger
and transaction history file.
Production Order
Displays the List of Production Orders. Choose the necessary production order from the list.
Return Components
Opens the List of Production Orders displaying the production and disassembly orders.
To return components, double-click the relevant order, and in the displayed Select Items to Copy window, select the items to
return.
More Information
Production Orders
List of Production Order
List of Production Order
In this window, choose items you want to issue for production or receive from production from a list of released production orders.
Select the required rows and select Choose.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
List of Production Order
Find
Use to search for a production order.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:10 AM
Document Number, Production Order Type, Start Date, Due Date, Item No., Item Description, Priority
Displays production order information.
More Information
Issue for Production Window
Production Std Cost Management
From the SAP Business One Main Menu, choose Production Production Std Cost Management to manage the following SAP
Business One functions:
Production Std Cost Rollup - Rolls up the total production standard costs of components included in the BOM, as well as those of
any sub-children, and updates the estimated production standard cost on the parent's item master data accordingly.
Production Std Cost Update - Updates the estimated production standard cost on the item master data record with the item cost.
Production Std Cost Rollup - Selection Criteria
Use this functionality to update a parent item's production standard cost with the sum of total production standard costs of its
BOM components. The system rolls up total production standard costs for all sublevel BOMs all the way until the last sublevel.
 Note
For sublevel BOMs that are not relevant for the standard cost rollup (the Include in Production Std Cost Rollup
checkbox in the Item Master Data window is deselected) the production standard cost in the parent item's master data
is not updated.
If in the selection criteria, you include a BOM that is not relevant for the standard cost rollup, the routine updates the
standard production cost on all its sublevel BOMs which are relevant for the routine (the Include in Production Std Cost
Rollup checkbox on the Item Master Data window is selected).
To access this window, from the SAP Business One Main Menu, choose Production Production Std Cost Management
Production Std Cost Rollup .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Production Std Cost Rollup - Selection Criteria Fields
Parent Item No. From... To
Specify the range of the parent items for which you want to run the production standard cost rollup.
More Information
Production Std Cost Management
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:10 AM
Production Std Cost Update - Selection Criteria
Use this functionality to update an item's estimated standard production cost with its item cost. After you run the standard
production cost update routine for an item, the system updates the Production Std Cost field in the Item Master Data window
accordingly.
The system updates the production standard cost in the following ways:
If you are managing item cost per warehouse (on Company Details: Basic Initialization Tab, the Manage Item Cost per
Warehouse checkbox is selected), the system uses the current item cost from the default warehouse. If you have not
defined the default warehouse for the item, the system uses the default warehouse on the company level.
If you are managing item cost per company (on Company Details: Basic Initialization Tab, the Manage Item Cost per
Warehouse checkbox is not selected), the system uses the current item cost from the item master data.
If the item has the serial/batch valuation method, the system updates the production standard cost with the average batch
or serial number cost across all batches or serial numbers.
If the item has the FIFO valuation method, the system updates the production standard cost with the average cost across
all open FIFO layers.
 Note
This function is available only if you are using the perpetual inventory system (on Company Details: Basic Initialization Tab, the
Use Perpetual Inventory checkbox is selected).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Production Std Cost Update - Selection Criteria Fields
Item No. From... To
Specify the range of items for which you want to update the production standard cost.
More Information
Production Std Cost Management
Production Cost Recalculation Wizard
The wizard enables you to recalculate production costs based on current cost values.
Components managed by serial/batch valuation method might be issued for production before their final cost is determined.
There could be a valuating cost price transaction such as Landed Cost, AP Invoice based on goods receipt PO (GRPO), Inventory
Revaluation that will change the component's price after it was issued for production.
These cost discrepancies impact production cost calculations that are made based upon current cost values. To deal with cost
discrepancies, the Production Cost Recalculation Wizard is available in SAP Business One to help you make any adjustments
required.
The Production Cost Recalculation Wizard enables the recalculation of production cost for:
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:10 AM
Products managed by the serial/batch valuation method
Products received from production
Any relevant production orders on which production receipts are based must already be closed
Products with at least one component in the corresponding issues for production managed by the serial/batch valuation
method
You can start the Production Cost Recalculation Wizard by either of the following ways:
From SAP Business One Main Menu, choose Production Production Cost Recalculation Wizard .
From SAP Business One Main Menu, choose Sales - A/R Gross Profit Recalculation Wizard , and the Production Cost
Recalculation Wizard will be initiated as part of the Gross Profit Recalculation Wizard.
The list below shows you how to run the Production Cost Recalculation Wizard. Choose each step for more details.
Please note that image maps are not interactive in PDF outputs.
Step 1: Selecting Wizard Options
On the Wizard Options page, select whether to run a simulation, start a new run, or load a saved run.
Wizard Options Fields
Run Production Cost Recalculation Simulation
Select to simulate a production cost recalculation run. The simulation gives you a preview of the expected results of the actual
wizard run.
Start Production Cost Recalculation Run
Select to create a new production cost recalculation run.
Load Saved Production Cost Recalculation Run
Select to view a saved production cost recalculation run which is not yet executed.
Related Information
Production Cost Recalculation Wizard
Step 2: Specifying Recalculation Parameters
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:10 AM
Step 3: Selecting Documents
Step 4: Viewing Material Revaluation Details
Step 5: Saving and Executing Recalculation Run
Step 2: Specifying Recalculation Parameters
On the Wizard Parameters page, specify parameters for the wizard run.
In this step, specify parameters for the wizard run. The parameters that you select will determine the range of receipts from
production to which the Production Cost Recalculation Wizard will be applied.
Production Cost Recalculation Name
Specify a name for the production cost recalculation run if required. The default name is a unique code automatically defined by
SAP Business One.
Date of Run
By default displays the current date and cannot be changed.
Remarks
Enter remarks about the production cost recalculation run if required.
Receipts from Production Posting Date From…To…
Specify the range of receipts from production posting date to filter the items that you want to recalculate production costs for.
Item No. From…To…
Specify the range of the item number to filter the items that you want to recalculate production costs for.
Group
Select an item group to filter the items that you want to recalculate production costs for.
Additional Filters Fields
Additional Filters
Select this checkbox and click the icon to add additional filters to narrow the search.
Find items with only the selected properties
Select this checkbox and properties you want to apply to the search.
Search Condition
Choose whether to search with And or Or condition.
Find Items With
Automatically summarizes the search condition and properties you have specified for the search.
Display Inactive Items
Select this checkbox to display items that do not appear in any of the selected sales documents since a specified date.
Search
Select this button to start searching.
 Note
Starting a new search will clear selections in the search results table.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:10 AM
Item List
Displays the search results – BoMs that are managed by the serial/batch valuation method and at least one of their components is
also managed by the serial/batch valuation method.
Selected Items
Displays the selected items that are moved from the Item List table.
 Note
You can use the buttons between the Item List table and the Selected Items table to move all rows or only selected rows
between the two tables.
Related Information
Production Cost Recalculation Wizard
Step 1: Selecting Wizard Options
Step 3: Selecting Documents
Step 4: Viewing Material Revaluation Details
Step 5: Saving and Executing Recalculation Run
Step 3: Selecting Documents
On the Recommendations page, select relevant documents.
In this step, you can select the documents in which the production cost needs to be adjusted to the current cost of the product
components managed by the serial/batch valuation method. Material revaluation document of type debit/credit will be created for
the serial/batch assigned to the selected receipt from production, debit/credit amount will correspond to the value in Total
Variance.
Related Information
Production Cost Recalculation Wizard
Step 1: Selecting Wizard Options
Step 2: Specifying Recalculation Parameters
Step 4: Viewing Material Revaluation Details
Step 5: Saving and Executing Recalculation Run
Step 4: Viewing Material Revaluation Details
On the Material Revaluation Details page, view the details of the material revaluation document, which adjusts production costs
to current cost of the components. Documents will only be created when Automatic Posting in the next step is selected.
Posting Date
Specify a posting date for the material revaluation document. The date displayed by default is the current date.
Document Date
Specify a document date for the material revaluation document. The date displayed by default is the current date.
Series
Use the dropdown list to determine the numbering series for the material revaluation document.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:10 AM
Reference 2
Specify an additional reference number if required.
Journal Remarks
Enter remarks for the journal entry.
Material Revaluation No.
Automatically determined by the selected numbering series.
Related Information
Production Cost Recalculation Wizard
Step 1: Selecting Wizard Options
Step 2: Specifying Recalculation Parameters
Step 3: Selecting Documents
Step 5: Saving and Executing Recalculation Run
Step 5: Saving and Executing Recalculation Run
On the Save and Execute Options page, choose Execute to recalculate the production cost. Or choose one of the save options to
save your predefined parameters or to save wizard recommendations for later review.
Save Wizard Parameters and Exit
Select to save the parameters for a future run and exit the wizard.
Save Wizard Simulation and Exit
Select to save the wizard simulation for later review of the simulated results, and exit the wizard.
Execute
Select to recalculate the gross profit and a system message will pop out:
Executing the wizard creates an inventory revaluation for adjustment of the production cost,
and a journal entry for adjusting costs of goods sold and gross profit. Creation of documents
depends on input data. Do you want to continue?
Press Yes to generate a new Material Revaluation (MRV) transaction to recalculate the production cost.
Wizard Parameters Name
Specify a name for the wizard parameters if required. The default name is a unique code automatically defined by SAP Business
One.
Description
Enter description for the wizard parameters if required.
Summary
After choosing Finish, you will see a wizard run summary which displays the results of the wizard run.
Related Information
Production Cost Recalculation Wizard
Step 1: Selecting Wizard Options
Step 2: Specifying Recalculation Parameters
Step 3: Selecting Documents
Step 4: Viewing Material Revaluation Details
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:10 AM
Update Parent Item Prices - Selection Criteria
Use this window to update prices of parent items according to changes in child item prices.
To access the window, choose one of the following:
Production Update Parent Item Prices Globally
Inventory Price Lists Special Prices Update Parent Item Prices Globally
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Update Parent Item Prices Selection Criteria
Price List From ... To...
Choose the range of the price lists to include in the report.
Code From ... To...
Specify the range of item codes to include in the report.
Parent Items
Filters the report by parent items.
In the selection criteria, SAP Business One displays all parent items that have child items with a new price in the price list.
Component Items
Filters the report by component (child) items.
SAP Business One finds all child items for which the price was changed and displays their parent items in the recommendation list.
Item Group
Choose an item group to include in the report.
Properties
Choose Properties and make relevant selections to use as selection criteria in the report.
More Information
Update Parent Item Prices Globally Window
Update Parent Item Prices Globally Window
This window displays a report listing child items for which prices have changed. It also creates a list of recommendations for new
parent item prices. You can accept or reject the changes.
To access the window,
1. Choose one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:10 AM
Production Update Parent Item Prices Globally Update Parent Item Prices – Selection Criteria
Inventory Price Lists Special Prices Update Parent Item Prices Globally Update Parent Item Prices –
Selection Criteria
2. Select the required criteria and choose the OK button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Update Parent Item Prices Globally Fields
Parent Item Code, Name
Name and code of the parent item, as defined in the Bill of Materials window.
Qty
Displays the quantity of the parent items as defined in the Bill of Materials.
Child Item Code, Name
Displays the name and the code of the child item.
Qty in BOM
Displays the quantity of the child items as defined in the Bill of Materials.
Current Price
Current price of the child item as defined in the Bill of Materials.
New Price
New price of child item entered in the price list.
Difference
Displays the difference between the new and old price in the price list.
Total Difference
Displays the Difference multiplied by the quantity of the child item in the Bill of Materials.
Parent Item Current Price
Current price of the parent item in the price list.
Suggested Price
Sum of the current parent price plus the cumulative total difference of the child items. You can change the suggested price
manually.
Price List
The price list associated with the Bill of Materials at the time the update takes place.
Update
Updates the parent item price in the price list associated with the bill of materials.
Remove
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:10 AM
Select this checkbox for parent items you do not wish to update. This parent item will not be displayed in the report, until
additional changes are been made in its child items.
More Information
Update Parent Item Prices - Selection Criteria
Bill of Materials
Production Reports
Use the reports listed under this menu entry to:
Generate the list of the bills of material
View open production orders
Related Information
Bill of Materials Report
Open Items List
Bill of Materials Report
This report provides the detailed list of all the bills of material that you have created.
Use this window to specify selection criteria for creating and displaying the list of bills of material.
To open the window, choose Production Production Reports Bill of Materials Report .
After defining the report, you can view it in the Bill of Materials Report window (see Bill of Materials Report Window).
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Properties
Opens the Properties window. Specify the item properties as selection criteria.
BOM Type
Choose the Bill of Materials type as a selection criterion.
To specify all types, choose All.
Bill of Materials Report Window
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:10 AM
This window displays the bill of materials report according to the defined selection criteria (`see Bill of Materials Report).
Bill of Materials Report
UoM
The unit of measure of the BoM item and its components, as defined in Inventory Item Master Data Inventory Data tab.
Quantity
Displays the quantity of parent items and their components.
Whse
Displays the warehouse from which the components are issued to produce or to sell the finished product. To display Warehouses
(Default) – Setup, click .
Price
Displays the purchase price of the components or the standard or moving average price when working in perpetual inventory
system.
Depth
Displays the level in the bill of materials. The finished product of the bill of materials is at level 1.
BOM Type
Displays the type of the bill of materials.
Route Sequence
Displays the route sequence copied from the Bill of Materials (BOM) screen. The field is only visible when routing is applied to the
BOM.
Route Stage
Displays the route stage copied from the Bill of Materials (BOM) screen. The field is only visible when routing is applied to the
BOM.
Open Items List
 Note
This topic contains SAP Notes that contain additional information.
This report lets you track the status of your sales and purchasing documents. You can find the customers that still need to pay for
their orders and the vendors that have not provided the items you ordered, and you can track your missing items in stock.
Use the report to view the following document types:
Open sales and purchasing documents, including A/P and A/R reserve invoices that are not yet fully paid or fully delivered
Documents that were partially copied to a target document
 Note
Closed or cancelled documents do not appear in the report.
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:10 AM
To access the window, choose one of the following:
Sales – A/R Sales Reports Open Items List
Purchasing - A/P Purchasing Reports Open Items List
Production Production Reports Open Items List
You can also use the open items list report to change the status of relevant documents, for example, to close or cancel open
documents. For production orders, you can change the status from Planned to Released or vice versa, or select multiple
production orders and change their status at once.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Open Items List Fields
Currency
Specify the currency in which you want to display the amounts.
Open Documents
Specify the type of document that you want to display.
Sales and purchasing documents
 Note
A/P and A/R Reserve Invoices have two different statuses:
Unpaid – Select this option to display all the open A/P or A/R reserve invoices that are not fully paid yet. This list
may include A/P or A/R reserve invoices that are already partially or fully delivered.
Not Yet Delivered – Select this option to display all the open A/P or A/R invoices that are not fully delivered yet.
This list may include A/P or A/R reserve invoices that are already partially or fully paid.
Production orders with the status Planned or Released
Missing items, that is, a list of all items with available quantity lower than zero.
After you close the window, the last document selection is saved and appears by default the next time you open the window.
Doc. No.
Reference number of the purchasing or sales document.
Installment No.
Appears only for A/P or A/R invoices and displays the successive installment number of the document.
Customer/Vendor
Customer or vendor name as it appears in the sales or purchasing document.
Days Overdue
Appears only for A/P or A/R invoices; displays the number of days beyond the due dates of the invoices.
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:10 AM
Customer/Vendor Ref. No.
The number of a customer sales or vendor purchasing document.
Due Date
Due date of the purchasing or sales document.
Amount
Open amount in the document, including tax that is still not drawn into the target document, or not yet paid.
Net
Open amount in the document excluding the tax amount from the Tax field in the general area of the document.
Tax
Open tax amount in the document.
Original Amount
Original total amount of the document, including tax.
Posting Date
Posting date of the document.
Document Date
Date of the document.
Blanket Agreement No.
Choose which blanket agreements to report on.
Open Item List – Production Orders
The following columns are displayed when you select the option Production Orders in the Open Documents field:
Doc. No.
The production order number.
Type
The type of production order: Standard, Special, or Disassembly.
Status
The current status of the production order.
Priority
The degree of importance of the production order indicated by integer numbers.
Open Item List – Missing Items
The following columns are displayed when you select the option Missing Items in the Open Documents field:
Item No.
Item code.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:10 AM
Item Description
Item description as defined in the item master data.
In Stock
Total quantity of the item as contained in all the defined company warehouses.
Ordered
Total open quantity of the item that appears in open purchase orders and open A/P reserve invoices not yet delivered.
Committed
Total open quantity of the item that appears in open sales orders and in open A/R reserve invoices that are not delivered yet.
Consignment
Number of items on consignation. The value in this field is a result of the quantity in open deliveries minus the quantity in open
returns
 Note
Drop ship warehouses are not considered in inventory reports and are therefore not included in the consignment quantity. You
can use a script to calculate the total consignation quantity of an item. For more information, see SAP Note 1773671 .
Available
The total available quantity of the item in all the company warehouses. The calculation is based on the following formula:
Qty in Stock + Qty Ordered – Qty Committed
Change To
To change the status of a document, select the checkboxes for the relevant documents, choose the Change To button, and choose
one of the following status options (depending on the document type and current status):
Planned (only relevant to production orders)
Closed
Canceled
 Note
Alternatively, you can cancel or close open documents in one the following ways:
In a document, open the context menu and choose Cancel or Close.
Select a document and choose Data main menu Cancel or Close.
The canceled/closed documents will not appear in the report again.
This is custom documentation. For more information, please visit SAP Help Portal. 72