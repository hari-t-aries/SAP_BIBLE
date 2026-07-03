6/8/26, 6:56 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:56:32 GMT+0000
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

6/8/26, 6:56 AM
Localization for India
This documentation describes features and functions in SAP Business One that are specific to the localization for India.
Information about general features and functions that are not localization-specific is available in the online help for SAP Business
One. You can also access the online help and localization-specific information directly in SAP Business One ( Help
Documentation Online Help and Help Documentation Country/Region Specific Information ).
GST
Goods and Services Tax (GST) is a new way of handling indirect taxation in India. GST replaces some existing tax regimes providing
benefits such as:
Reduced tax complexity
A simplified taxation system with fewer variables
Greater tax transparency
A reduced administrative burden
Unified taxation for the country/region and individual states
Economic and employment benefits
For details on working with GST, see the How to Guide for GST India document and collaboration group referred to in SAP Note
2194689 .
Tax Collected at Source (TCS)
Finance Bill 2020 has inserted a new provision - Sec 206C (1H) which provides that if a seller (being a person, whose turnover in
the previous financial year exceeds 10 Crores) makes a sale of “goods” whose value, either individually or in aggregate exceeds 50
Lacs, the seller shall collect tax at source at 0.1% on the value of sale consideration exceeding 50 Lacs from the buyer.
The new provision is applicable from 1st Oct 2020. For more information, see the SAP Notes in the References section of SAP Note
2971563 .
Dunning Wizard Enhancements
In SAP Business One and SAP Business One, version for SAP HANA, as of version 10.0 Support Package (SP) 2311, the following
enhancements are available when working with the dunning wizard:
In step 6: Recommended Service Documents, the new fields SAC for Interest and SAC for Fees enable you to specify the
SAC code to be applied to the dunning interest or fees for all recommended service invoices. If necessary, you can specify a
different SAC code for individual service invoices in the table.
In step 6: Recommended Service Documents, the new checkbox Create Drafts enables you to create drafts for all
recommended service invoices.
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:56 AM
Setup and Administration: India
This section describes the settings and definitions related to functions that are specific to India.
Information about settings and definitions related to general functions is available in the general online help file, under: Help
Documentation Online Help .
Company Details: Accounting Data Tab
Company Details, Accounting Data Tab: India
Tax Related Definitions
Tax Types - Setup Window
Tax Codes - Setup Window
Withholding Tax Codes - Setup Window
Sequence - Setup Window: India
Excise Register Numbering - Setup: India
Tax Code Determination - Setup Window
Tax Engine Configuration
TDS Related Definitions
Defining Financial Year Master: India
Defining Sections: India
Defining the Nature of Assessees: India
Defining Certificate Series: India
Freight Charges
The page Managing Freight Charges in the general online help file provided with SAP Business One describes the freight charges
functionality. In India, when creating sales and purchasing documents, the freight considers the location of the sales or purchasing
document for the respective journal entry.
Company Details, Accounting Data Tab: India
A tab for defining basic accounting information specific to India per its legal requirements.
To access this tab, choose Administration System Initialization Company Details Accounting Data .
General Subtab Fields
P.A.N. No.
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:56 AM
Specify the permanent account number.
P.A.N. Circle, Ward No.
Specify either the P.A.N. circle number or the ward number.
P.A.N. Assessing Officer
Specify the name of the P.A.N. assessing officer.
LST/VAT No.
Specify the local sales tax (LST) number or the value added tax (VAT) number.
CST No.
Specify the central sales tax (CST) number.
Exemption Number
If the company has a tax exemption number, enter that number in this field.
TAN No.
Specify the number of the tax deduction account.
Service Tax No.
Specify the registration number of the service tax.
Service Nature
You use this dropdown box to separate Service Distributor from Service Provider.
 Note
You cannot edit the Service Nature field after you select and confirm a value.
Assessee Type, Company Type
Specify the assessee or company type.
Nature of Business
Specify what the company deals with.
TIN No.
Specify the tax identification number.
To setup TIN no. for locations, users are required to maintain state information in the Locations - Setup window.
To setup TIN no. for business partners, users need to maintain state information in business partner master data’s Ship to
(Customer) / Pay to (Vendor) addresses.
Holidays
Select a set of company holiday dates as defined in the Holiday Dates window.
To define a new set of dates, select Define New.
Excise Subtab Fields
E.C.C. No., C.E. Registration No., C.E. Range, C.E. Division, C.E. Commissionerate, Manufacturers Code, Jurisdiction
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:56 AM
Specify excise registration information for future excise invoice printing and reports generation.
More Information
Company Details: Accounting Data Tab
Tax
You use the functions under this menu option to define tax-related settings, according to your country/region regulations. The
definitions you make here dictate the way tax is registered in the accounting transactions and how it is reflected in the different tax
reports.
To access tax definition functions choose Administration Setup Financials Tax .
Tax Types - Setup Window
Use this window to define additional tax types and select a Tax Parameter and a Tax Category for each one.
To access this window, choose Administration Setup Financials Tax .
Tax Types - Setup Window Fields
Tax Type Name
Specify a name for the tax type.
 Note
When a tax type is used in other modules, you can rename it, but you cannot delete it.
Tax Category
Specify the tax category for the respective tax type.
Tax Parameter
Specify a tax parameter for each tax type.
 Note
You can apply one tax parameter to several different tax types.
You cannot edit this field if the tax type is used in other modules.
Attribute Values
Opens the Define Values for Tax Attribute window.
 Note
If the return value is being used in a tax parameter, you cannot delete it.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:56 AM
Tax Category - Setup Window
Return Values - Setup Window
Attribute Values
Use the Attributes - Setup window for individual tax types to define tax attributes and control fields for tax posting.
To open this window, choose Administration Setup Financials Tax Tax Types , then select a tax type and choose
Attribute Values.
Tax Type Attributes for Brazil
Code
Specify a tax code.
Purchasing Tax Account
Specify a tax account for the purchasing transactions.
Sales Tax Account
Specify a tax account for the sales transactions.
Non Deductible %
Specify the non-deductible percentage.
 Note
This field is available only when Included in Price or Exempt is not selected. Otherwise, the value is 0.
Non Deductible Account
Define the account for non-deductible amounts.
 Note
This field is available only when Non Deductible % is not 0.
Effective From
Indicates the start of the current valid period.
Attribute x
Displays the attributes configured in Tax Type Definition by parameter.
Valid Period
Opens the Valid Period window for defining the validity period for each attribute.
Valid Period - Setup: Specific Tax Type Window
Effective From
Specify the start of the valid period.
Attribute x
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:56 AM
Displays the attributes configured in Tax Type Definition, by parameter.
 Note
If a numeric attribute type is left blank, the system takes 0 as its value.
More Information
Tax Types - Setup Window
Tax Category - Setup Window
Use this window to define tax categories.
To open this window, choose Administration Setup Financials Tax . In the displayed Tax Types - Setup window, choose
Define New in the Tax Category dropdown list.
Tax Category - Setup Window
Tax Category
Define additional tax categories.
 Note
You cannot change the predefined tax categories.
More Information
Tax Types - Setup Window
Specific Tax Type Attributes - Setup Window
Sequence - Setup Window: India
Use this window to define a sequence for a document.
To open this window, choose Administration Setup Financials Tax Sequence .
Sequence - Setup Window Fields
Document
Displays the document types for which you can define a sequence, including all transaction documents available for India.
 Note
Once a certain transaction document type is configured to support Sequence, user can select assigned sequences when using
the document.
Sequence
Default sequence name.
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:56 AM
Assign Sequence to Document
Choose to assign a sequence to a selected document in the Sequence window.
More Information
Sequence - Specific Document Window: India
Sequence - Specific Document Window: India
Use this window to define a new sequence, or set an existing sequence as default.
You can assign multiple sequences for one location.
To open this window, choose Assign Sequence to Document in Administration Setup Financials Tax Sequence .
Sequence Definition Fields
Assign
Sets the sequence as default.
Location
Specify a location for the sequence.
This field is mandatory.
You can:
Define multiple sequences for one location
Generate documents with the same sequence for different locations
 Example
You can generate a purchase order with Sequence 1 for both the Delhi Branch and the Mumbai Branch.
Prefix, Suffix
Specify the sequence prefix or suffix.
First
Specify the number to assign to the first document, of this document type, that you enter in the system.
Subsequent documents receive sequential system-assigned numbers.
Next
Displays the number that will be assigned to the next document of the corresponding type.
Value updated for each new document created in the system.
If the value in this column is not equal to the value in the First column, then:
Documents of this type have already been entered
The numbering of the corresponding document type can no longer be changed
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:56 AM
Last
Specify the last number that can be assigned to a document of this type. Use only when you need to define an additional series for
numbering.
Remarks
Provide additional information.
Lock
Locks the sequence for use.
Display Unlocked Sequence
Selected to display only unlocked sequences. Otherwise, all the sequences are displayed. The display is refreshed automatically.
Set as Default
In the Sequence - Setup window, sets the selected sequence as the default sequence for the specific document type.
 Note
After assigned sequence is used in documents, you can not modify its location.
More Information
Sequence - Setup Window: India
Default Sequence Window
Use this window to assign as default for users the sequence defined in Sequence - Specific Document Window: India. The location
of the assigned sequence is the default value for Location in the document.
Default Sequence Window
Set as default for current user
Sets the selected sequence as the default for the current user.
Set as default for all users
Sets the selected sequence as the default for all users.
Set as default for certain users
Sets the selected sequence as the default for the users you select in the Select Users window.
Excise Register Numbering - Setup: India
Use this window to define excise register numbers for the locations of manufacturers. Excise register numbers help generate
separate returns or reports for each location.
To open the window, choose Administration Setup Financials Tax Excise Register Numbering .
Excise Register Numbering – Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:56 AM
Location
Choose one location from those defined in the location setup window for manufacturers.
 Note
The excise register numbering is available for location that is marked as manufacturer or excise manufacturer (XM or EM is
selected).
 Note
The existing Excise Register Numbering from 2005 B will appear with no location designated, user needs to attach one location
with it. Irrespective of any conflict in the warehouse location with attached location (with existing generated excise register
numberings), the system will use warehouse location of the old transactions instead of newly attached location.
Excise Register
The following are the available excise register numbers:
RG23A Part I
RG23A Part II
RG23C Part I
RG23C Part II
First No., Next No., Last No.
The first/next/last excise register number.
 Note
You must assign a location to each excise register number.
Excise Register Numbering - Reset: India
Use this window to reset the excise register number for each location.
To access this window:
1. Choose Administration Setup Financials Tax Excise Register Numbering .
2. Do one of the following:
Double-click the relevant row.
Select the relevant row and choose Reset.
Excise Register Numbering - Reset
First No.
Specify a first number for the excise register number sequence.
Last No.
Enter a last number for the excise register number sequence.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:56 AM
The last number must larger than the next number of the location.
Tax Engine Configuration
Use this function to configure the tax engine.
More Information
Tax Parameter - Setup Window
Tax Formula - Setup Window
Tax Type Combination - Setup Window
Tax Parameter - Setup Window
Use this window to define tax parameters. (Tax Parameter = Attributes + Return Values)
To open this window, choose Administration Setup Financials Tax Tax Engine Configuration .
Tax Parameter - Setup Window Fields
Code
Specify a code for the tax parameter.
Description
Describe the tax parameter.
Attribute
Displays the Description value of each attribute.
Specify an attribute or create a new one.
 Note
If the tax parameter has been used by a tax type, you can still add attributes.
If the attribute is used in a tax parameter, you can only view the information in this window.
Mandatory Field
Indicates that the input of defined values for tax attributes is mandatory.
Return Value
Select a return value predefined by the application or create new ones.
 Note
Even if the return value is used in a tax parameter, you can view the information in this window and add a new value.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:56 AM
Attributes - Setup Window
Return Values - Setup Window
Return Values - Setup Window
Use this window for defining return values.
To open this window, choose Administration Setup Financials Tax Tax Engine Configuration . In the displayed Tax
Parameter - Setup window, choose Define New in the Return Values dropdown list.
Return Values - Setup Window Fields
Return Value Code
Define the code for the return value.
The first character must be ʻa...z’ or ʻA…Z’.
The other characters can be ʻ_’ or ʻa…z’ or ʻA…Z’ or ʻ1…9’.
Saving your changes prompts a system message informing you that this attribute is used in a tax parameter.
Description
Describe the return value.
Display in Sales/Purchasing Tax Amount Window
Displays the return values in the tax window in A/P or A/R documents.
 Note
If the default value for Tax Amount is selected, you cannot change it. However, you can change this checkbox anytime for other
return values.
 Note
You cannot delete a return value that is being used in a tax parameter.
More Information
Tax Parameter - Setup Window
Attributes - Setup Window
Use this window to define attributes for tax parameters.
To open this window:
1. Choose Administration Setup Financials Tax Tax Engine Configuration Tax Parameter .
2. In the Tax Parameter - Setup window, select Define New in the Attribute dropdown list.
Attributes - Setup Window Fields
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:56 AM
Data Type
Select one of the following data types from the dropdown list:
Amounts
Prices
Quantities
Percents
Integer
String
Measures
Attribute Code
Define a code for the attribute:
The first character must be ʻa...z’ or ʻA…Z’.
The other characters must be ʻ_’ or ʻa…z’ or ʻA…Z’ or ʻ1…9’.
Description
Describe the attribute.
 Note
You cannot delete an attribute used in a tax parameter.
The system predefines the Rate attribute. Its data type is percent, and only its description is editable.
More Information
Tax Parameter - Setup Window
Tax Formula - Setup Window Operation Field
Use this field in the Tax Formula - Setup window to select valid operations for the tax formula.
To open the window, choose Administration Setup Financials Tax Engine Configuration .
Arithmetic Operations
Operation Description Example Result
+ Addition X=2 3
X=X+1
– Subtraction X=2 3
X=5-X
* Multiplication X=4 20
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:56 AM
| Operation | Description |     | Example | Result |
| --------- | ----------- | --- | ------- | ------ |
X=X*5
| /   | Division |     | X=5     | 3;  |
| --- | -------- | --- | ------- | --- |
|     |          |     | X=15/X; | 2.5 |
X=5
X=X/2
| %   | Modulus (division remainder) |     | 5%2;    | 1;  |
| --- | ---------------------------- | --- | ------- | --- |
|     |                              |     | 10%8;   | 2;  |
|     |                              |     | 10%2;   | 0   |
| (,) | Priority                     |     | 5*(2+3) | 25  |
Round (Number, Decimals as A predefined function for Round (2.134,2); 2.13;
| Number) | rounding. |     |              |     |
| ------- | --------- | --- | ------------ | --- |
|         |           |     | Round (2.-1) | 0   |
The rounding rules follow these
settings:
Rounding Method field
in the Document
Settings window
Rounding field in the
Define Currencies
window
Decimal Place field in
the General Settings
window, Display tab
Round (Number, Type) A predefined function for Round (2.134, Amounts) 2.13
rounding.
If the setting of the Decimal
|     | You can choose only one of the |     | Place Amounts field is 2. |     |
| --- | ------------------------------ | --- | ------------------------- | --- |
following types:
Percents
Prices
Amounts
Quantities
The rounding rules follow the
settings of the Decimal Place
field in the General Settings
window, Display tab.
Condition Operations
| Operations | Description | Example | Result |     |
| ---------- | ----------- | ------- | ------ | --- |
| <          | Less than   | 5<8     | True   |     |
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:56 AM
| Operations | Description              | Example               | Result |
| ---------- | ------------------------ | --------------------- | ------ |
| <=         | Less than or equal to    | 5<=8                  | True   |
| ==         | Equal to                 | 5==8                  | False  |
| !=         | Not equal                | 5!=8                  | True   |
| >=         | Greater than or equal to | 5>=8                  | False  |
| >          | Greater than             | 5>8                   | False  |
| If…else    | Condition operate        | if (X<6) {X=X+2} else | 5      |
{X=X+1}
X=3
  Example
ICMS
Industrialization or Reselling or Consumption or Assets
ICMS Gross Amt = Item Net Value / (1-((ICMS rate/100)*(Base/100)))
ICMS Tax Amount = ICMS Gross Amount – Net Value
Base Amount = Item Net Value / (1-((ICMS rate/100)*(Base/100))*(1+(IPI rate/100)*(IPI Base/100)))
ICMS Amount = Base Amount * ((100-ICMS rate)/100)*(Base/100))
Grammar Rules
The language is case-sensitive.
1. Solo expressions are not supported. Only statements are valid.
Valid statements include:
Assignment
If
While
Compound
2. Rules for assignment statements:
a. The referred local variable must be initialized.
The following statements are invalid:
a = a + 1
/*the local variable 'a' is not assigned a value before */
b = a
/*the local variable 'a' is not assigned a value before */
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:56 AM
b. The referred external local variable in the block cannot be assigned a value with a different type.
The following statements are incorrect:
a = "124"
/*it is not correct because the type of the local variable 'a' is string, which can be determined by the latest
statement before the block*/
3. Rules for if / while statements:
a. The type of the expression enclosed within "(" and ")" must be of type boolean:
i. True
ii. False
iii. The result of the relationship expression.
b. The statements enclosed within "{" and "}" plus "{" and "}" consist of a block, so rule 2.b) is applicable.
4. Rule for functions:
a. This release supports only the "Round" function, which has two types of prototypes:
Round (Number, Decimals as Number)
/* The first parameter "number" includes integer and real and represents the rounding number; the second
parameter "integer" includes integer type and only represents the digitals after the decimal point */
Round (Number, Type)
/* The first parameter is the same as the first prototype; the value of the second parameter "type" must be
one of the following values: Percents, Prices, Amounts, or Quantities */
5. Rules for expressions:
a. Logic expression:
Operators: && > ||
Operands: value must be boolean
b. Relationship expression:
Operators: >, >=, ==, !=, <, <=
Operands:
If there is one string value between two operands, the non-string value is changed to the corresponding
string value before a comparison is made
If there is no string value between two operands, the values of integer, real and boolean can be compared
 Example
The value of ("truf" > true) is true. Here the second operand is converted to "true".
The value of (2 < "12") is false. Here the first operand is converted to "2".
The value of (2< true) is false. Here the second operand is converted to 1.
The value of (2>false) is true. Here the second operand is converted to 0.
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:56 AM
c. Arithmetic expression:
Operators: (*, /, %) > (+, -)
Operands:
The operands for "%" must be integer type\
The operands for the operators, except "%" and "+" , must be non-string type, including integer, real and
boolean
The operands for "+" can be any type. If there is a string value of the operands, the result will be string;
otherwise, the result will be numeric.
If two operands are both integer, the result of "/" will also be integer. For example, 2 / 4 = 0 (divide exactly)
d. Unary expression:
Operators: !, -
Operands:
For "!", it must be boolean value
For "-", it must be non-string value
e. Bracket expression: the highest priority expression
Operators: (, )
Their priority is: 1) < 2) < 3) < 4) < 5)
6. Other rules:
a. Strings cannot be assigned to the non-string output parameter
b. You cannot assign a value to the input parameter
c. Number overflow - when you exceed the maximum value 9223372036854
d. All output variables must be assigned values
Reserved Words (case sensitive)
if Percents ContinueNotice Round
else Prices ContinueNextPageNotice
while Amounts B1Notice
True Quantities
false
COMPILER B1
CHARACTERS
letter = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz" .
digit = "0123456789" .
cr = CHR(13).
tab = CHR(9) .
If = CHR(10) .
anyButQuote = ANY – “ ' ”
anyButApostrophe = ANY – “ ' ”
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:56 AM
COMMENTS FROM "/*" TO "*/"
IGNORE
cr + lf + tab
TOKENS
ident = letter {letter | digit | '_'} .
number = digit {digit}.
real = digit {digit} "." digit {digit}.
string = '"' {anyButQuote} '"' | "'" {anyButApostrophe} "'".
PRODUCTIONS
B1 = Body
Body = StatSeq
StatSeq = Stat [";"] {Stat [";"]}
CompoundStat = "{" StatSeq "}"
Stat = AssignStat | IfStat | WhileStat | CompoundStat.
AssignStat = Ident "=" Exp.
IfStat = "if" "(" Exp ")" CompoundStat [ "else" CompoundStat ].
WhileStat = "while" "(" Exp ")" CompoundStat.
Exp = ConExp.
ConExp = OrExp.
OrExp = AndExp { "||" AndExp }.
AndExp = RelExp { "&&" RelExp }.
RelExp = AddExp [ RelOp AddExp].
RelOp = ( "<" | "<=" | ">" | ">=" | "==" | "!=" ).
AddExp = MulExp { AddOp MulExp}.
AddOp = ( "+" | "-" ).
MulExp = Factor { MulOp Factor }.
MulOp = ( "*" | "/" | "%" ).
Factor = ("true" | "false" | integer | string | real |"(" Exp ")" | IdentOrFunction | Enum | UnaryO
IdentOrFunction = Ident (ParamList | ).
Ident = ident.
ParamList = "(" [Exp { "," Exp}] ")".
Enum = RoundTypeEnum | SystemStringEnum.
RoundTypeEnum = ("Percents" | "Prices" | "Amounts" | "Quantities").
SystemStringEnum = ("ContinueNotice" | "ContinueNextPageNotice" | "B1Notice").
UnaryOp = ("-" | "!").
END B1.
More Information
Tax Formula - Setup Window
Tax Formula - Setup Window
Use this window to define possible tax formulas for determining how the tax amount or other return values are calculated.
 Note
Each tax type in a tax type combination must have its own formula.
To access this window, choose Administration Setup Financials Tax Tax Engine Configuration .
General Area
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:56 AM
Code
Specify a code for the tax formula.
Description
Describe the tax formula.
Tax Type
To select the tax type that was defined in the tax type combination, click .
All the return value codes and attribute codes automatically appear in the variable grid.
You cannot change these return values.
After you save the formula, this field becomes non-editable.
Refresh Parameter
Updates the attributes and the return values of the tax type in the variable table.
Operation
To select an available operation, click .
For more information, see Tax Formula - Setup Window Operation Field.
Insert
Adds the selected operation to the formula.
Variable Table Fields
Variable
Specify a variable for the formula, either manually or by selecting from the list.
Formula Output
Click to display the formula return values.
Formula Input
Click to display the formula attributes.
Parameter
Specify the valid parameters, either by selecting from the list or by entering values manually.
Options include:
Parameters from marketing documents
Tax attributes code
Return values code
 Note
All the tax attributes and return values used in the formula should be listed in the tax parameter table.
A formula must include all the return values defined in the tax parameter table under Formula Output.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:56 AM
Entering an invalid parameter generates an error message when you try to save your changes. The system removes your entry
and opens the Choose from List window to let you select a valid parameter.
Data Type
Displays the data type for the tax calculation.
Formula Pan
Formula
Enter the formula for the tax calculation.
 Note
You can enter the formula manually, or use the Operation and Insert functions.
The system displays a warning message if you try to change a formula that has already been used in a tax code.
If you still want to save the changes, the system revalidates all related tax type combinations. If one does not pass the validation,
you cannot save the changes.
Formula Validation Message
When you choose OK or Update, the application validates the formula and displays either the validation message, or an error
message, as appropriate.
More Information
Tax Formula - Setup Window Operation Field
Tax Type Combination - Setup Window
Use this window to define tax type combinations. A tax type combination works like a validation rule for tax types.
To open this window, choose Administration Setup Financials Tax Tax Engine Configuration .
Tax Type Combination - Setup Window Fields
Code
Specify the code for the tax type combination.
Description
Describe the tax type combination.
#
Displays the line item number for the tax type. You must select the tax type in sequence.
 Note
The sequence of the tax types is important, as it is used in tax formula definitions.
Tax Type
Specify a tax type.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:56 AM
 Note
If the tax type combination has been used in a tax code, you cannot change the tax types.
Formula Code
Specify the defined tax formula.
 Note
You can change the tax formula at any time; however, the application issues a warning if the tax type combination has been
used in a tax code.
When you select a tax formula code, the application checks the formula. If the formula does not adhere to the following validation
rules, the application generates a warning, but allows you to continue the operation:
If return values of other tax types are used in this tax formula, those tax types must be defined prior to this line in the same
tax type combination.
If tax attributes of other tax types are used in this tax formula, those tax types must also be defined in the same tax type
combination.
When you choose OK or Update, the application validates the tax type combination. If the tax type combination does not adhere to
the following validation rules, you receive an error message and the data is not saved:
One tax type can be defined only once in the same tax type combination.
If return values of other tax types are used in one tax formula, those tax types must be defined before this line in the same
tax type combination.
If tax attributes of other tax types are used in one tax formula, those tax types must also be defined in the same tax type
combination.
More Information
Tax Types - Setup Window
Tax Formula - Setup Window
Setting Up Tax
Follow the below procedures to set up and use tax in purchasing and sales documents:
Setting Up and Using Tax Codes
Setting Up Default Tax Codes in Purchasing and Sales Documents
Setting Up and Using Tax Codes
Context
The following procedure describes how to define tax codes using the Tax Engine Configuration.
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:56 AM
Procedure
1. Define a tax parameter.
In this example, a tax parameter with the code Rate is defined.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Engine
Configuration Tax Parameter .
The Tax Parameter - Setup window appears.
b. In the Code field, specify Rate as the tax parameter code, and in the Description field, describe the tax parameter.
c. From the Attribute dropdown list, select Rate.
To define a new attribute, in the Attribute dropdown list, choose Define New to open the Attributes - Setup window.
d. From the Return Value dropdown list, select Tax Amount and Base Amount.
To define a new return value, in the Return Value dropdown list, choose Define New to open the Return Values -
Setup window.
e. To save the tax parameter, choose the Add button.
f. To close the window, choose the Cancel button.
For more information, see the following:
Tax Parameter - Setup Window
Attributes - Setup Window
Return Values - Setup Window
2. Define a tax type.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Types .
The Tax Types - Setup window appears.
b. In the Tax Type Name field, specify the tax type name.
c. From the Tax Category dropdown list, select the relevant tax category.
To define a new tax category, in the Tax Category dropdown list, choose Define New to open the Tax Category -
Setup window.
d. From the Tax Parameter dropdown list, select the relevant parameter. For more information about defining tax
parameters, see Defining a Tax Parameter above.
To define a new tax parameter, in the Tax Parameter dropdown list, choose Define New to open the Tax Parameter -
Setup window.
e. To save the tax types, choose the Update button.
 Note
After defining each tax type, you must choose the Update button before you can define the next tax type.
f. To close the window, choose the OK or Cancel button.
For more information, see the following:
Tax Types - Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:56 AM
Tax Category - Setup Window
Tax Parameter - Setup Window
3. Define a tax formula.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Engine
Configuration Tax Formula .
The Tax Formula - Setup window appears.
b. In the Code field, specify a code for the tax formula, and in the Description field, describe the tax formula.
c. From the Tax Type dropdown list, select the corresponding tax type for formula. For more information about
defining tax types, see Define a tax type above.
The return values and attribute of this tax type appear as Formula Output and Formula Input respectively.
d. In the variable table fields, open the List of Tax Parameters window by choosing Tab in the empty field of the
Parameter Code column, and select tax parameters for the tax formula by double-clicking the row or choosing the
OK button after selecting the row.
 Note
The List of Tax Parameters window from the Formula Input section shows all the parameters that can be used
as input parameters for this formula, including attributes defined for this tax type, attributes and return values
defined for other tax types, and document attributes.
e. In the formula pan on the right, define the formulas. Select variables by double-clicking the corresponding row in the
variable table fields, and enter arithmetic operators either through the keyboard or the Operation field.
f. Check the correctness of the formula by clicking before the Formula Validation Message field. If there is no
message shown, it means that the formula is correct.
g. Choosing the Add button checks the correctness of the formula first and saves the tax formula if the formula is
correct.
h. To close the window, choose the Cancel button.
For more information, see the following:
Tax Formula - Setup Window
Tax Formula - Setup Window Operation Field
4. Define a tax type combination.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Engine
Configuration Tax Type Combination .
The Tax Type Combination - Setup window appears.
b. In the Code field, specify the code for the tax type combination, and in the Description field, describe the tax type
combination.
c. From the Tax Type dropdown list, select the relevant type. For more information about defining tax types, see Define
a tax type above.
d. In the Formula Code field, open the List of window by choosing Tab , and select the corresponding formula code by
double-clicking the row or choosing the Choosing button after selecting the row.
e. To save the tax type combination, choose the Add button.
f. To close the window, choose the Cancel button.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:56 AM
For more information, see the following:
Tax Type Combination - Setup Window
5. Define a tax code.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Codes .
The Tax Codes - Setup window appears.
b. In the Code field, specify the tax code, and in the Description field, describe the tax code.
c. From the Tax Type Combination dropdown list, select the tax type combination you defined earlier. For more
information about defining tax type combinations, see Define a tax type combination above.
The tax types included in this tax type combination appear in the table.
d. In the Code field, open the List of Sales Tax Authorities window by choosing Tab , and select a code for each tax
type by double-clicking the row or choosing the Choose button after selecting the row.
If you need to define new attributes for the tax type, proceed as follows:
i. In the List of Sales Tax Authorities window, choose the New button to open the <Specific Tax Type>
Attributes - Setup window to define attributes for the corresponding tax type.
ii. In the corresponding fields, specify the name, purchasing tax account, sales tax account, and non deductible
%.
iii. Open the Valid Period - Setup: <Specific Tax Type> window by selecting a row and performing one of the
following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Valid Period .
Right-click the row you just selected and choose Valid Period.
Choose the Valid Period button.
iv. In the Effective From field, specify the effective date, and in the Rate field, specify the rate.
v. In the Valid Period - Setup: <Specific Tax Type> window, save the valid period for the rate by choosing the
Update button.
vi. To close the Valid Period - Setup: <Specific Tax Type> window, choose the OK or Cancel button.
vii. In the <Specific Tax Type> Attributes - Setup window, save the attributes for the tax type by choosing the
Update button.
viii. To close the <Specific Tax Type> Attributes - Setup window, choose the OK or Cancel button.
ix. In the List of Sales Tax Authorities window, select the newly defined attributes by double-clicking the row or
choosing the Choose button after selecting the row.
e. To save the tax code, choose the Add button.
f. To close the window, choose the Cancel button.
For more information, see the following:
Tax Codes - Setup Window
Specific Tax Type Attributes - Setup Window
6. Use tax codes in purchasing and sales documents.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:56 AM
a. From the SAP Business One Main Menu, choose Sales - A/R Sales Quotation, Sales Order, Delivery, Return,
A/R Down Payment Request, A/R Down Payment Invoice, A/R Invoice, A/R Credit Memo , or Purchasing -
A/P Purchase Order, Goods Receipt PO, Goods Return, A/P Down Payment Request, A/P Down Payment
Invoice, A/P Invoice, A/P Credit Memo .
b. Specify the customer in the Customer field (for sales documents), or the vendor in the Vendor field (for purchasing
documents), and the item in the Item No. field.
c. In the Tax Code field, open the List of Sales Tax Codes window by choosing Tab , and select the relevant tax code.
For more information about defining tax codes, see Define a tax code above.
If you need to see the total tax calculated for this document and a breakdown of each tax type, proceed as follows:
a. In the toolbar, click to display the Form Settings - <Specific Document> window.
b. On the Table Format tab, in the row Tax Amount (LC), select the Visible checkbox and choose the OK button.
c. In the Tax Amount (LC) field, click the orange arrow beside the entry to display the Define Tax Amount Distribution
window, which shows the base amount and the tax amount.
For more information, see the following:
Sales Document: Contents Tab
Purchasing Documents: Contents Tab
Setting Up Default Tax Codes in Purchasing and Sales
Documents
Context
Default tax codes appear in the Tax Code field automatically in purchasing and sales documents instead of you selecting the tax
codes in each document each time.
For more information, see the following:
Tax Code Determination for Marketing Transactions
Procedure
1. Define an item category.
a. From the SAP Business One Main Menu, choose Administration Setup Inventory Item Groups .
The Item Groups - Setup window appears.
b. In the Item Group Name field, specify an item group name.
c. At the bottom of the General tab, under the heading Item Category, select whether the item group is for Service
items or Material items.
d. To add the item group, choose the Add button.
e. To close the window, choose the Cancel button.
For more information, see the following:
Item Groups - Setup
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:56 AM
2. Define a tax code determination.
a. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code
Determination .
The Tax Code Determination - Setup window appears.
b. From the Determination Type dropdown list, select the determination type.
If you need to set the default tax codes in marketing documents for material items, in the Determination Type
dropdown list, select Material Item.
c. In the grid, define the priority and key fields that act as parameters for identifying the tax codes applicable to a
transaction by choosing parameters from the dropdown lists.
d. Open the Key Fields Value - Setup window by selecting a row and performing one of the following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Key Fields Value .
Right-click the row you just selected and choose Key Fields Value.
Choose the Key Fields Value button.
e. In each field, open the List of … window by choosing Tab , and select the exact parameters for the three key fields
of this combination by double-clicking the row or choosing the Choose button after selecting the row.
f. Open the Valid Period - Setup window by selecting a row and performing one of the following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Valid Period .
Right-click the row you just selected and choose Valid Period.
Choose the Valid Period button.
g. In the Effective From and Effective To fields, specify the first day and the last day of the validity period.
h. In the Tax Code field, open the List of Sales Tax Codes window by choosing Tab , and select the tax code
applicable for this determination by double-clicking the row or choosing the Choose button after selecting the row.
i. In the Valid Period - Setup window, save the valid period for the tax code by choosing the Update button.
j. To close the Valid Period - Setup window, choose the OK or Cancel button.
k. In the Key Fields Value - Setup window, save the values by choosing the Update button.
l. To close the Key Fields Value - Setup window, choose the OK or Cancel button.
m. In the Tax Code Determination - Setup window, save the changes by choosing the Update button.
n. To close the Tax Code Determination - Setup window, choose the OK or Cancel button.
For more information, see the following:
Tax Code Determination - Setup Window
Key Fields Value - Setup Window
Default WT Code - Setup Window
Tax Payment Wizard: India
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:56 AM
The tax payment wizard enables you to define required filter options and activate the tax payment run process.
To access the Tax Payment Wizard window, choose Banking Tax Payment Wizard .
More Information
Tax Payment Wizard - Wizard Options
Tax Payment Wizard - General Parameters
Tax Payment Wizard - Saving Options
Tax Payment Wizard - Tax Payment: CENVAT
Tax Payment Wizard - Tax Payment: Service Tax
Tax Payment Wizard - Tax Payment: VAT and Tax Category
Tax Payment Wizard - Tax Payment: Other
Tax Payment Wizard - Challan Information
Tax Payment Wizard - VAT Refund
Tax Payment Wizard - Confirm Message
Tax Payment Wizard - Wizard Options
Specify the required information in the first step of the Tax Payment Wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
Start New Wizard
Creates a new tax payment run process.
Load Saved Wizard
Lists the executed and saved tax payment with detailed information.
From Date, To Date
Specify the date range during which taxes were collected in transaction.
The default From Date value is the date of the oldest saved or executed wizard; the default To Date value is the current date.
Location
Selects location as a filter option for saved tax payment wizards.
Enabled only when Load Saved Wizard is selected.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:56 AM
Table Area of Wizard History
Wizard Name
Name of a previous payment run.
Date
Displays the date of the tax payment run, based on the status of the wizard: saved or executed.
Tax Category
Displays the tax types.
Status
Displays the status of the payment run:
S - saved
E - executed
RG23A Part II No.
RG23A Part II No. displays when Raw Materials Credit was used.
RG23C Part II No.
RG23C Part II No. displays when Capital Goods Credit was used.
After selecting to start a new wizard or to load an existing one, choose Next to access the General Parameters window.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - General Parameters
Use this window to enter general information for the tax payment wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Wizard Name
Specify the wizard name.
The default name is generated automatically.
From Date, To Date
Specify the date when the tax payment run process is activated. In this field, click on the choose-from list to pop up a window for
user to select financial periods (obtained from Posting Periods defined in System Initialization General Settings ).
Series No.
Automatically generated Tax Payment Series No.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:56 AM
Tax Category
Select tax category for tax payment wizard.
Location
Select the location for the tax payment wizard. This field is mandatory.
Seq. Name
Specify a sequence from the drop-down list. The system generates the sequence automatically.
 Note
This field appears only for documents that are assigned a sequence.
E.C.C. No.
A read-only field that appears when you select CENVAT in Tax Category.
Its value comes from E.C.C. No. of the location you select. The credit amount and payable amount will be calculated separately
based on Locations.
After entering information in all the fields, choose Next to continue.
 Note
If you open a saved wizard, the next step is saving options. If you open an executed wizard, the next step is tax payment based
on the tax category selected.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Saving Options
Tax Payment Wizard - Tax Payment: CENVAT
Tax Payment Wizard - Tax Payment: Service Tax
Tax Payment Wizard - Tax Payment: VAT and Tax Category
Tax Payment Wizard - Tax Payment: Other
Tax Payment Wizard - Saving Options
Use this window to specify whether you want to save the report for later use or execute it now.
Save Selection Criteria and Exit
Saves the criteria defined in the wizard and exits. The next time you display the saved wizard data, the recommendation report is
created according to these criteria.
Execute
Saves the recommendation report and executes it. Later, the report is displayed in view-only mode.
After selecting a save option, choose Next.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:56 AM
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Tax Payment: CENVAT
Tax Payment Wizard - Tax Payment: Service Tax
Tax Payment Wizard - Tax Payment: VAT and Tax Category
Tax Payment Wizard - Tax Payment: CENVAT
Use this window to check the detailed tax payment for each CENVAT component, so that later you can post the tax payment to the
accounts and generate a payment number.
Credit Available
Displays the various tax credit amounts for different tax components of CENVAT.
Credit amount for Raw Materials including raw materials and finished goods is calculated:
From the incoming excise invoice or manual journal entries
Up to the date defined in To Date in Tax Payment Wizard Step 2: General Parameters
Credit amount for Capital Goods is calculated:
From the incoming excise invoice or manual journal entries
Up to the date defined in To Date in Tax Payment Wizard Step 2 General Parameters
P.L.A. Remaining
Displays the current amount in the P.L.A account for each tax type.
Credit amount for P.L.A. is calculated up to current date.
Credit Utilization
Displays a matrix table of the CENVAT payable amount. You can specify the utilization amount of each component for credit
amount.
Payable
Displays payable amount in Credit Utilization for different tax components of CENVAT.
The payable amount are from journal entries of outgoing excise invoice and journal entries involving CENVAT Payable Account
which are posted in selected period but are still open for CENVAT payment.
 Note
Only when the sum of credit utilized amount and P.L.A. utilization amount is equal to the payable amount for each component,
can you go on with the next step.
After selecting the payment methods, choose Next.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:56 AM
Tax Payment Wizard: India
Tax Payment Wizard - Tax Payment: Service Tax
Use this window to choose the payment for each tax component.
Credit Available
Displays the various tax credit amounts by tax type.
Credit amount is calculated:
From partially or fully paid A/P invoices and A/P credit memos
Up to the date defined in To Date in Tax Payment Wizard Step 2: General Parameters
Credit Utilization
Displays a matrix table of the service tax payable amount. You can specify the utilization amount of each component for credit
amount.
 Note
The utilization amount cannot be:
Larger than the existing credit amount displayed in the Credit Available field
Negative
Payable
Displays payable amount in Credit Utilization for different tax component of service tax.
Payable amount is collected from the journal entries of closed or partially paid AR invoices and AR credit memos which are posted
in selected period and still open for service tax payment. AR invoices and credit memos generated before the current release are
still included. If the AR Invoice is partially paid, then the payable Service Tax is calculated proportionately.
After selecting the payment methods, choose Next.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Tax Payment: VAT and Tax Category
Use this window to specify the payment means for the tax payment.
Tax Category
Displays the tax categories.
Payable Amount
Displays the payable amount for different tax categories.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:56 AM
Payable amount is collected from journal entries of A/R invoices, A/R credit memos, and manual journal entries. The latter include
journal entries created from stock transfers and posted in a selected period, and which are still open for VAT payment.
 Note
Invoices or credit memos generated before the current release are also included.
Credit Amount
Displays the credit amount for different tax categories.
Credit amount is calculated:
From journal entries of A/P invoices, A/P credit memos, and manual journal entries
Up to the date defined in To Date in Tax Payment Wizard Step 2: General Parameters
Payment Amount
Displays the payment amount.
Direct Payment Amount
Displays the direct payment amount.
If this amount is above zero, choose in the toolbar to specify the payment means and the amount.
After you have settled the payment, choose Next.
 Note
The payment means amount must equal the direct payment amount; otherwise, an error message appears when you choose
Next.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Tax Payment: Other
Use this window to choose payment means for other tax payment.
Tax Category
Displays the tax categories.
Payable Amount
Displays the payable amount.
Payable amount is collected from journal entries of A/R invoices, A/R credit memos, and journal entries involving payable
accounts posted in selected periods and still open for relevant tax category payment.
 Note
A/R invoices and credit memos generated before the current SAP Business One release are still included.
Credit Amount
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:56 AM
Displays the credit amount.
Credit amount is calculated:
From journal entries of A/P invoices, A/P credit memos, and manual journal entries
Up to the date defined in To Date in Tax Payment Wizard Step 2: General Parameters.
Payment Amount
Displays the payment amount.
Direct Payment Amount
Displays the direct payment amount.
If this amount is above zero, choose in the toolbar to specify the payment means and amount.
 Note
The payment means amount must equal the direct payment amount; otherwise, the system displays an error message when
you press Next.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Challan Information
Use this window to specify Challan information for the tax payment run process.
Challan No., Challan Date, Bank Name, Remarks
Specify the necessary Challan information for tax payment.
After you have entered information in all the fields, choose Next to continue.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - VAT Refund
Tax Payment Wizard - VAT Refund
Use this window to specify refund information for the tax payment run process.
Refund Amount
Specify the refund amount.
Refund Account
Specify an account for depositing the refund amount.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:56 AM
If the refund account in this form has been specified before by any user in the company, the account from the last refund is
displayed here as the default value.
After you have entered information in all the fields, choose Next to continue.
More Information
Tax Payment Wizard: India
Tax Payment Wizard - Confirm Message
This window displays a system message indicating that the tax payment is saved or posted successfully.
Click Finish to confirm and close the window.
More Information
Tax Payment Wizard: India
TDS: India
TDS is the income tax deducted at source. It refers to any form of withholding tax.
During A/P process, you can do the following with TDS:
Make adjustments to the TDS amount per invoices, which can include A/P regular invoices and A/P down payment
Invoices.
Reverse TDS in A/P and A/R credit memo
Deduct TDS in A/P and A/R invoices
Deduct TDS in A/P down payment Invoices and A/P down payment requests
Deduct TDS on freight for both document and line level freight based on the applicability of WTax on freight
Deduct TDS in incoming and outgoing payments
Generate Form 16A and the eTDS report in SAP Business One
More Information
Defining Financial Year Master: India
Defining Sections: India
Defining the Nature of Assessees: India
Defining Certificate Series: India
Defining Financial Year Master: India
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:56 AM
Use this window to provide the data for creating an eTDS return report.
Procedure
1. To access the window, from SAP Business One Main Menu, choose Administration Setup Financials TDS
Financial Year Master .
2. In the Financial Year Master window, specify the following fields:
Code
Specify a unique code for the TDS financial year.
Description
Enter a description for the TDS financial year.
Start Date
Specify the start date of the financial year.
End Date
Specify the end date of the financial year.
Assessment Year
Enter a unique assessment year code for the TDS assessment year. The code should be a 6–digit number.
3. Choose the OK button.
Defining Sections: India
Use this window for determining the provisions for tax deduction .
Procedure
1. To access the function, from SAP Business One Main Menu, choose Administration Setup Financials TDS
Sections .
2. In the Sections window, specify the following fields:
Code
Specify the section code. It should be no more than 4 characters.
Description
Description of the section code you assigned.
eCode
Specify the ecode for the section code.
3. Choose the OK button.
Defining the Nature of Assessees: India
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:56 AM
Use this window to define the nature of assessee for the purpose of determining the tax deduction rate.
For the Indian localization, assessee means any person or entity by whom any tax or any other sum of money is payable under the
Income Tax Act, 1961. The assessee may fall under any of the following categories:
Individual
HUF (Hindu undivided family)
Company
Partnership firm
Association of firms
Local Authority such as Municipality and so on
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup Financials TDS Nature of Assessee .
2. In the Nature of Assessee window, specify the following fields:
Code
Specify the code for an assessee.
Description
Description of the assessee code.
Assessee Type
Specify an assessee type.
3. Choose the OK button.
Defining Certificate Series: India
Use this window to define the certificate series for creating a TDS report.
Procedure
1. To access the function, from the SAP Business One Main Menu, choose Administration Setup Financials TDS
Certificate Series .
2. In the Certificate Series window, specify the following fields:
Code
Specify a unique TDS series code.
Prefix
Specify the prefix of the series.
First No.
Specify the first number of the series.
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:56 AM
Next No.
Next number of the series.
Last No.
Specify the last number of the series.
Section Code
Select a section code. The drop down list displays all the values you defined in the Section Code - Setup window.
Location
Select a location for which the series is being created.
3. Choose the OK button.
Tax Codes - Setup Window
The following table describes the fields that appear in the Tax Codes - Setup window. You can define possible tax codes in this
window.
To access this window choose: Administration Setup Financials Tax .
Tax Codes - Setup Window Fields
Code, Description
Specify the code and short description of the tax.
Inactive
When the checkbox is selected, you cannot select the corresponding tax code in any window or add any document with an inactive
tax code. It is deselected by default.
Tax Type Combination
Specify the predefined tax type combination.
Tax Type
the tax types which have been defined in the tax type combination
Code
Specify the tax code.
Description
The description of the selected tax code
Formula Code
The formula code of the selected tax type
Sales Tax Account, Purchasing Tax Account, Non-Deductible Acct
G/L accounts defined for the tax code
Non Deductible %
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:56 AM
The non-deductible tax percentage defined for the tax code.
Effective From
The effective period of the tax code
Tax Code Determination
You set up determination orders of tax codes for the following:
Material items
For more information, see Setting Up Tax Code Determination for Material Items.
Service items
For more information, see Setting Up Tax Code Determination for Service Items or Service Documents.
Service documents
For more information, see Setting Up Tax Code Determination for Service Items or Service Documents.
Withholding taxes
For more information, see Setting Up Tax Code Determination for Withholding Tax: Brazil.
More Information
Tax Code Determination - Setup Window
Tax Code Determination for Marketing Transactions
When you enter item information in marketing documents, SAP Business One checks the item master data. If the item
classification for tax purposes is:
Material Item
The tax code determination for materials begins.
Service Item
The tax code determination for services begins.
When you enter service information in marketing documents, the tax code determination for service documents begins.
The key fields information for the tax code determination is according to your entries in the marketing documents, such as BP
Code, Item Code and so on.
 Note
Usage is a required value for tax code determination for material items.
The posting date of the marketing document is used to check the valid period of the tax code determination.
Based on information in these key fields, SAP Business One searches the priority table and checks the Priority 1 relevant tables.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:56 AM
To retrieve the tax code, SAP Business One proceeds as follows:
1. Finds a row matching these key fields in the valid period, it retrieves the tax code.
2. Cannot find any matching row in Priority 1, it checks Priority 2, then Priority 3 tables, and so on, until it finds a proper tax
code.
3. Cannot find any proper tax code in the priority table, it checks Default Tax Code for Sales or Default Tax Code for
Purchase.
4. Cannot find any proper tax code, it leaves the Tax Code field blank.
 Note
When you change any of the key fields in a marketing document, the tax code determination runs again to retrieve the correct
tax code.
More Information
Tax Code Determination
Setting Up Tax Code Determination for Material Items
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
Select the determination type as Material Item.
2. Select values for the Key Field 1,2,3 fields.
For more information, see Tax Code Determination - Setup Window.
3. Select one row and choose the Key Field Value button.
The Key Field Value - Setup window appears.
For more information, see Key Fields Value - Setup Window.
4. Specify key field values.
5. Select one row and choose the Valid Period button.
The Valid Period - Setup window appears.
For more information, see Valid Period - Setup Window.
6. Specify valid periods.
7. Select one row and choose the Tax Code by Usage button.
The Tax Code by Usage - Setup window appears.
For more information, see Tax Code by Usage - Setup Window.
8. Specify the tax code by usage.
9. To save your changes, choose the OK button, and then the Update button.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:56 AM
Tax Code Determination
Setting Up Tax Code Determination for Service Items or Service
Documents
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
2. Select either the Service Item or Service Document determination type.
3. Select values for the Key Field 1,2,3 fields.
For more information, see Tax Code Determination - Setup Window.
4. Select one row and choose the Key Field Value button.
The Key Field Value - Setup window appears.
For more information, see Key Fields Value - Setup Window.
5. Specify key field values.
6. Select one row and choose the Valid Period button.
The Valid Period - Setup window appears.
For more information, see Valid Period - Setup Window.
7. Specify valid periods.
8. To save your changes, choose the OK button, and then the Update button.
Related Information
Tax Code Determination
Tax Code Determination - Setup Window
Use this window to define and prioritize combinations of key fields, to which you can assign tax codes.
To access this window, choose Administration Setup Financials Tax Tax Code Determination .
Tax Code Determination - Setup Window Fields
Determination Type
From the drop-down box, select the tax type.
Priority
Displays the priority number.
Key Fields 1, 2, 3
From the drop-down box, select the first, second, or third key field in combination.
Description
Describe the key fields.
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:56 AM
Default Tax Code for Sales, Purchase
Click to assign a default tax code to all sales- or purchase-related documents.
Key Fields Value
1. Select a row.
2. Choose this button to open the Key Fields Value – Setup window.
3. Assign values to the selected key fields.
 Note
Only authorized users can use this window.
More Information
Key Fields Value - Setup Window
Tax Code Determination
Tax Code Determination - Setup (Determination Type: Material
Item)
Use this window to define the priority of key field combinations for tax code determination, enter key fields, and add tax codes for
the key fields.
To open this window, choose Administration Setup Financials Tax Tax Code Determination .
Tax Code Determination - Setup Window (Determination Type: Material Item) Fields
Determination Type
Specify a determination type.
Priority
Displays the fixed line number to indicate the priority for the determination.
To change the priority, click or .
 Note
Priority 1 is the highest priority for the tax code determination. Changes made here do not affect the key field definition.
Key Fields <n>
Specify the key fields for the tax code determination.
 Note
Insert the values one by one and follow the order strictly (Key Fields 1, Key Fields 2, Key Fields 3 and so on).
In the same priority line, the key fields must be different.
Description
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:56 AM
Describe the key field combination.
Default Tax Code for Sales
Specify a default tax code for sales transactions.
Default Tax Code for Purchase
Specify a default tax code for purchase transactions.
Key Fields Value
Opens the Key Fields Value- Setup window.
Key Fields Value - Setup Window
Use this window to specify values for the Key Fields <n>.
To open this window:
1. Select a row in the Tax Code Determination - Setup window.
2. Do one of the following:
Double-click the row you just selected.
From the menu bar, choose Goto Key Fields .
Right-click the row you just selected and choose Key Fields.
Choose the Key Fields Value button.
Key Fields <n>
Specify a value for the key field.
Key Fields <n> Description
Displays the description of the key field.
Valid Period
Only available for tax determination type as Material Item, Service Item or Service Documentation. Opens the Valid Period -
Setup window.
For more information, see Valid Period - Setup Window.
 Note
This window displays the column names for Key Fields <n>, according to the row you selected in the Define Tax Code
Determination - Setup window. The possible values are:
Business Partner
BP Code from the business partner master data.
Item
Item No. from the item master data.
Material Group
Material Group from the item master data.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:56 AM
State
State of ship-to address of customer or pay-to address of vendor.
NCM Code
NCM Code in the NCM code table.
Item Group
Item Group from the item master data.
Vendor Group
Vendor Group from the business partner master data.
Customer Group
Customer Group from the business partner master data.
Vendor Type
Vendor Type from the business partner master data.
Material Type
Material Type from the item master data.
Valid Period - Setup Window
To open this window:
1. In the Define Key Fields Value window, select a row.
2. Perform one of the following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Validity Period .
Right-click the row you just selected and choose Validity Period.
Choose Key Validity Period.
Effective From
Specify the first day of the validity period.
Effective To
Specify the last day of the validity period.
Tax Code by Usage
Only available for the tax determination type Material Item. Opens the Tax Code by Usage - Setup window.
Tax Code by Usage – Setup Window
Usage
List from the usage master data in the nota fiscal. You cannot edit this field.
Tax Code
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:56 AM
Specify the tax code.
Freight Tax Code
Specify a tax code for freight.
More Information
Tax Code Determination for Marketing Transactions
Tax Code Determination - Setup Window (Determination Type:
Service Document)
Use this window to define the priority of key field combinations for tax code determination, enter key fields, and add tax codes for
the key fields.
To access this window, choose Administration Setup Financials Tax Tax Code Determination .
Tax Code Determination - Setup Window (Determination Type: Service Item) Fields
Determination Type
Specify a determination type.
Priority
Displays the fixed line number to indicate the priority for the determination.
To change the priority, click or .
 Note
Priority 1 is the highest priority for the tax code determination. Changes made here do not affect the key field definition.
Key Fields <n>
Specify key fields for the tax code determination.
 Caution
Insert the values one by one and follow the order strictly (Key Fields 1, Key Fields 2, Key Fields 3, and so on).
In the same priority line, the key fields must be different.
Description
Describe the key field combination.
Default Tax Code for Sales
Specify a default tax code for sales transactions.
Default Tax Code for Purchase
Specify a default tax code for purchase transactions.
Key Fields Value
Opens the Key Fields Value - Setup window.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:56 AM
Key Fields Value - Setup Window
Use this window to specify values for the Key Fields <n>.
To open this window:
1. Select a row in the Define Tax Code Determination window.
2. Do one of the following:
Double-click the row you just selected.
From the menu bar, choose Goto Key Fields .
Right-click the row you just selected and choose Key Fields.
Choose Key Fields Value.
Key Fields <n>
Specify a value for the key fields.
Key Fields <n> Description
Displays a description of the key fields.
Valid Period
Opens the Valid Period - Setup window.
 Note
This window displays the column names for key fields <n>, according to the row you selected in the Define Tax Code
Determination window. The possible values are:
Business Partner
BP Code in the business partner master data
State
State of ship-to address of customer or pay-to address of vendor
County
County of ship-to address of customer or pay-to address of vendor
G/L Account
G/L Account in the marketing document line item
Vendor Group
Vendor Group in the business partner master data
Customer Group
Customer Group in the business partner master data
Valid Period - Setup Window
To open this window:
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:56 AM
1. In the Define Key Fields Value window, select a row.
2. Perform one of the following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Validity Period .
Right-click the row you just selected and choose Validity Period.
Choose Key Validity Period.
Effective From
Specify the first day of the validity period.
Effective To
Specify the last day of the validity period.
More Information
Tax Code Determination for Marketing Transactions
Tax Code Determination - Setup Window (Determination Type:
Service Item)
Use this window to define the priority of key field combinations for tax code determination, enter key fields, and add tax codes for
the key fields.
To open this window, choose Administration Setup Financials Tax Tax Code Determination .
Tax Code Determination - Setup Window (Determination Type: Service Item) Fields
Determination Type
Select Service Item from the drop-down box.
Priority
Displays the fixed line number to indicate the priority for the determination.
To change the priority, click or .
 Note
Priority 1 is the highest priority for the tax code determination. Changes made here do not affect the key field definition.
Key Fields <n>
Specify key fields for the tax code determination.
 Caution
Insert the values one by one and follow the order strictly (Key Fields 1, Key Fields 2, Key Fields 3, and so on).
In the same priority line, the key fields must be different.
Description
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:56 AM
Describe the key field combination.
Default Tax Code for Sales
Specify a default tax code for sales transactions.
Default Tax Code for Purchase
Specify a default tax code for purchase transactions.
Key Fields Value
Opens the Key Fields Value - Setup window.
Key Fields Value - Setup Window
Use this window to specify values for the Key Fields <n>.
To open this window:
1. Select a row in the Define Tax Code Determination window.
2. Do one of the following:
Double-click the row you just selected.
From the menu bar, choose Goto Key Fields .
Right-click the row you just selected and choose Key Fields.
Choose Key Fields Value.
Key Fields <n>
Specify a value for the key fields.
Key Fields <n> Description
Displays a description of the key fields.
Valid Period
Opens the Valid Period - Setup window.
 Note
This window displays the column names for key fields <n>, according to the row you selected in the Define Tax Code
Determination window. The possible values are:
Business Partner
BP Code in the business partner master data.
Item
Item No. in the item master data.
Service Group
Service Group in the item master data.
State
State of ship-to address of customer or pay-to address of vendor.
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:56 AM
County
County of ship-to address of customer or pay-to address of vendor.
Service Code
Service Code in the item master data.
Item Group
Item Group in the item master data.
Vendor Group
Vendor Group in the business partner master data.
Customer Group
Customer Group in the business partner master data.
Valid Period - Setup Window
To open this window:
1. In the Define Key Fields Value window, select a row.
2. Perform one of the following operations:
Double-click the row you just selected.
From the menu bar, choose Goto Validity Period .
Right-click the row you just selected and choose Validity Period.
Choose Key Validity Period.
Effective From
Specify the first day of the validity period.
Effective To
Specify the last day of the validity period.
More Information
Tax Code Determination for Marketing Transactions
Key Fields Value - Setup Window
Use this window to specify values for Key Fields 1, 2, 3 selected in the Tax Code Determination - Setup.
To open this window:
1. Choose Administration Setup Financials Tax Tax Code Determination
2. Select the values for Key Fields 1, 2, 3.
3. Select a row and do one of the following:
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:56 AM
Double-click the row you just selected.
From the menu bar, choose Goto Key Fields .
Right-click the row you just selected and choose Key Fields.
Choose the Key Fields Value button.
Key Fields Value - Setup Window Fields
BP Code, Item No., Material Group, Service Group, Item Group, Customer Group, Vendor Group, State Code, County Code, NCM
Code, G/L Account
Specify values for the key fields.
BP Name, Item Description, M.G. Description, S.G. Description, V.G Description, NCM Name, GL Name, Effective From, Effective
To, Tax Code
Describe the key fields.
BP: Business Partner; M.G.: Material Group; S.G.: Service Group; V.G.: Vendor Group; GL: General Ledger.
Valid Period
Only available for tax determination type as Material Item, Service Item or Service Documentation. Opens the Valid Period -
Setup window.
For more information, see Valid Period - Setup Window.
Default WT Code
Only available for the determination type as Withholding Tax. Opens the Default WT Code - Setup window for defining default
withholding tax codes.
For more information, see Default WT Code - Setup.
More Information
Valid Period - Setup Window
Default WT Code - Setup Window
Tax Code Determination - Setup Window
Valid Period - Setup Window
To open this window:
1. In the Key Fields Value - Setup window, select a row.
2. Do one of the following:
Double-click the row you just selected.
From the menu bar, choose Goto Validity Period .
Right-click the row you just selected and choose Validity Period.
Choose the Validity Period button.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:56 AM
Effective From
Specify the first day of the validity period.
Effective To
Specify the last day of the validity period.
Tax Code by Usage
Only available for the tax determination type Material Item. Opens the Tax Code by Usage - Setup window.
More Information
Tax Code by Usage - Setup Window
Tax Code Determination - Setup Window
Tax Code by Usage - Setup Window
You set up tax code by usage for only the tax code determination type as Material Item.
To open this window:
1. In the Valid Period - Setup window, select a row.
2. Do one of the followings:
Double-click the row you just selected.
From the menu bar, choose Goto Tax Code by Usage .
Right-click the row you just selected and choose Tax Code by Usage.
Choose the Tax Code by Usage button.
Usage
List from the usage master data in the nota fiscal. You cannot edit this field.
Tax Code
Specify the tax code.
Freight Tax Code
Specify a tax code for freight.
More Information
Tax Code Determination - Setup Window
Default WT Code - Setup Window
Use this window to define default withholding tax codes.
To open this window:
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:56 AM
In the Key Fields Value - Setup window, select a row.
Do one of the followings:
Double-click the row you just selected.
From the menu bar, choose Goto Default WT Code .
Right-click the row you just selected and choose Default WT Code.
Choose the Default WT Code button.
Default WT Code - Setup Window Fields
Code
All withholding tax codes
Description
Withholding tax description
Default
Sets the withholding tax as default.
More Information
Tax Code Determination - Setup Window
Locations - Setup: India
Use this window to specify the required information for the location defined in Accounting Data tab in Company Details.
General tab - specify demographic information for location
Accounting Data tab - specify accounting information for location as you define in Accounting Data tab in Company Details
Accounting Data Tab
General Subtab
Provide information for the following fields for TDS purpose.
P.A.N. No.
Specify the permanent account number, using a combination of 10 characters and digits.
TAN Circle No.
Specify the TAN Circle number.
TAN Ward No.
Specify the TAN Ward number.
TAN Assessing Officer
Specify the TAN Assessing Officer.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:56 AM
Excise Subtab
ECC No.
Specify the three parameters for ECC No.:
PAN No.: comes from PAN No. ( Accounting Data General )
Select from the following registration types:
XM: manufacturer location (default)
XD: dealer location
None: other location
EM: excise manufacturer. EM locations operate according to the same logic as XM locations.
ED: excise dealer. ED locations operate according to the same logic as XD locations.
SD: service tax. SD locations operate according to the same logic as None locations.
Enter 3-digit number; default value is blank.
 Note
This field is mandatory if Excisable is selected for Warehouse.
Once transactions exist for the location with this ECC No., you may not change the ECC No.
SSI Exemption
Select to indicate that the manufacturer is registered as a small scale industries (SSI) unit.
 Note
This checkbox appears only when you select XM or EM as the registration type. Once an outgoing or incoming excise invoice
exists for this location, you cannot change the checkbox status.
 Note
For locations upgraded from those without this checkbox, you can change this checkbox once, even if excise invoices exist for
this location.
TDS Subtab
CIT Address, CIT City, CIT Pin Code
Specify the CIT information to appear in Form 16A.
Tax Information: India
Use this window to specify the tax information of a company.
To open this window, choose Business Partners Business Partners Master Data Accounting Tax tab, and click .
Tax Information Fields
P.A.N. No.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:56 AM
Specify the permanent account number (PAN).
P.A.N. Circle No.
Specify the PAN circle number.
P.A.N. Ward No.
Specify the PAN ward number.
P.A.N. Assessing Officer
Specify the name of the PAN assessing officer.
LST/VAT No.
Specify either the local sales tax number or the value added tax number.
CST No.
Specify the central sales tax number.
TAN No.
Specify the tax deduction account number.
Service Tax No.
Specify the service tax registration number.
Company Type
Categorize the company.
Nature of Business
Specify what the business deals with.
Assessee Type
Categorize the assessee.
TIN No.
Specify the taxpayer identification number.
 Note
A newly-created marketing document contains the same tax information data as that found in Business Partner Master
Data Accounting Tax tab.
More Information
Business Partner Master Data: Accounting Tab, Tax
Vendor Type - Setup: India
Use this window to define new, or edit existing vendor types for a business partner.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:56 AM
You cannot delete default values.
Vendor Type - Setup Window
Vendor Type
Categorize the vendor.
Description
Describe the defined type.
More Information
Business Partner Master Data: Accounting Tab, General
Business Partner Master Data: Accounting Tab, Tax
Applying Point of Taxation Rules to Service Taxes
The Indian Central Government formulated the Point of Taxation Rules (PTR) vide Notification No. 18/2011-ST dated Mar. 01, 2011.
Amendments were carried out in these rules vide Notification No. 25/2011-ST dated Mar. 31, 2011.
According to Rule 3 in Notification No. 25/2011-ST, the point of taxation for service taxes shall be as follows:
(a) Date of invoice or payment, whichever is earlier, if the invoice is issued within the prescribed period of 14 days from the date of
completion of the provision of service.
(b) Date of completion of the provision of service or payment, if the invoice is not issued within the prescribed period as above.
 Note
For the A/P side, you can now use a new query to search for A/P invoices and A/P credit memos which are not fully paid within
3 months.
The following description is only relevant to the A/R side.
Glossary
To ensure the convergence with the legislation, SAP Business One has made the following interpretations of the legal terms in
Notification No. 25/2011-ST:
Term Definition
Point of taxation (POT) The “point of taxation” is the point of time when the tax is counted
as tax payables.
Therefore, the point of taxation for service taxes is the point of time
when the service taxes are counted as tax payables.
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:56 AM
Term Definition
Service tax Only the taxes of the Service Tax category are regarded as service
taxes.
To specify the tax category for a tax type, go to Administration
Setup Financials Tax Tax Types .
Completion of the provision of service The “completion of the provision of service” is signified by the
creation of deliveries with service taxes. Thus, the posting date of
such deliveries is considered as the “date of completion of the
provision of service”.
 Note
The delivery can be either Item or Service type. As long as a
service tax code is used, the delivery is considered as a
“completion of the provision of service” document.
Date of invoice The “date of invoice” is the posting date of either of the following
documents:
Service type of standalone A/R invoices with service taxes
A/R invoices based upon deliveries with service taxes
Date of payment The “date of payment” is the posting date of the payment created
for the following documents:
A/R invoices
Down Payment Invoices (DPI)
Down Payment Request (DPR)
And these documents must be created based upon
deliveries with service taxes.
Within the prescribed period of 14 days The “prescribed period of 14 days” counts from the service
completion date - posting date of the delivery. That is, the
“prescribed period of 14 days” ends only 13 days after the posting
date of the delivery.
 Example
1. Create a service tax delivery with posting date
Jan. 01, 2012.
2. Create an invoice based on delivery with one of the
following posting date:
Jan. 14, 2012
This invoice is considered as within the
prescribed period.
Jan. 15, 2012
This invoice is considered as NOT within the
prescribed period.
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:56 AM
Prerequisites
To apply the POT rules to service taxes in SAP Business One, make sure that you have completed the following:
1. From Main Menu, choose Administration System Initialization Company Details Basic Initialization . In the
Company Details window, on the Basic Initialization tab, select the checkbox Apply Point of Taxation Rules for Service
Taxes.
 Note
Before you select the checkbox, we recommend you to settle the existing delivery documents which are still open. The
point of taxation rules only apply to newly-created delivery documents. And, once you select the checkbox, you cannot
deselect it.
After you select the checkbox, a new menu entry Taxable Deliveries is available in Sales-A/R Sales Reports
Taxable Deliveries . You can use the taxable deliveries to post service taxes to journal entries for certain deliveries.
For more information, see the Taxable Deliveries section.
2. From the Main Menu, choose Administration Setup Financials G/L Account Determination .
In the G/L Account Determination window, on the General tab, specify the Service Tax Clearing Account where the service
tax amount is temporarily stored until the amount can be cleared upon the invoice creation.
For more information about when the service tax amount is posted to the service tax clearing account, see the Journal
Entry with Service Tax Posting section.
Taxable Deliveries
You can use the taxable deliveries to post service taxes to the service tax accounts for the deliveries whose tax amount is not
completely posted within 14 days. That is, you can post service taxes for deliveries that meet all the following conditions:
The delivery is created with service taxes.
The posting date of the delivery is at least 14 days earlier than the current system date.
The delivery is not fully copied to returns within 14 days.
The delivery is not fully copied to A/R invoices within 14 days.
The delivery is not fully paid (through the down payment invoice or down payment request) within 14 days.
The delivery meets the selection criteria specified in the Taxable Deliveries – Selection Criteria window.
To post services taxes to the service tax accounts, proceed as follows:
1. From SAP Business One Main Menu, choose Sales-A/R Sales Reports Taxable Deliveries . The Taxable Deliveries –
Selection Criteria window appears.
2. In the Taxable Deliveries – Selection Criteria window, specify the selection criteria for the deliveries and choose OK.
The Service Deliveries to Be Posted window appears with a list of deliveries for which you can post service taxes.
 Note
In the Service Deliveries to Be Posted window, the Tax Amount fields display the open tax amount of the delivery that
you can post to the service tax accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:56 AM
3. To post the open tax amount to the service tax accounts, choose Post Service Tax in the Service Deliveries to Be Posted
window.
A journal entry is created with the posting date of the delivery.
In the journal entry, the open tax amount is posted to the relevant service tax accounts.
For more information about the service tax posting journal entry, see the Journal Entry with Service Tax Posting section.
Journal Entry with Service Tax Posting
A new kind of journal entry is available with Service Tax Posting as Remarks.
This kind of journal entries debits the service tax clearing account, and credits the service tax accounts. The following shows an
example screenshot of such journal entry:
The service tax posting journal entry can be created both automatically and manually as follows:
Within 14 days from service tax delivery creation, any payment for the delivery (either through DPI or DPR) automatically
generates a service tax posting journal entry until the service taxes in the delivery are completely posted.
In the journal entry, the service tax clearing account is debited with the tax amount in the payment, and the service tax
accounts are equally credited.
The posting date of the journal entry is taken from the posting date of the payment.
Beyond the 14 days range of the service delivery creation, you need to manually create the service tax posting journal entry
for the deliveries whose tax amount is not completely posted. Otherwise, you cannot create invoices based on the delivery.
To manually create the service tax posting journal entry, use the taxable deliveries. For more information, see the Taxable
Deliveries section.
In the journal entry, the service tax clearing account is debited with the open tax amount in the delivery, and the service tax
accounts are equally credited.
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:56 AM
The posting date of the journal entry is taken from the posting date of the delivery.
Reversal of Journal Entry with Service Tax Posting
When you create return or A/R credit memo documents based on service tax deliveries, SAP Business One validates whether the
creation of these documents causes the posted tax amount to exceed the due tax amount in the deliveries. If this is the case, a
service tax posting journal entry reversal is automatically generated to reverse the unduly posted tax amount.
 Note
To view the service tax posting journal entries and the reversal journal entries related to a delivery, you can select Service Tax
Posting from the context menu in any of the following documents:
Service tax delivery
Payment created through DPI or DPR for the service tax delivery
Return based on the service tax delivery
A/R credit memo for an A/R invoice which is created based on the service tax delivery
POT Logic
To comply with Rule 3 in Notification No. 25/2011-ST, SAP Business One has adjusted the calculation logic of service taxes as
follows:
Within 14 days of the service delivery creation, the service taxes are posted to the service tax accounts when any of the
following conditions arise:
An A/R invoice is created based on the delivery, either partially or full
The invoice generates a journal entry with the date of the invoice. In the journal entry, the service tax amount in the
invoice is posted to the service tax accounts.
In such case, for the invoiced part of service taxes, the point of taxation is the date of the invoice.
A partial or full payment for the delivery, through DPI or DPR
The payment generates one EXTRA service tax posting journal entry with the date of the payment.
For more information, see the Journal Entry with Service Tax Posting section.
In the journal entry, the service tax amount in the payment is posted to the service tax accounts.
In such case, for the paid part of the service taxes, the point of taxation is the date of the payment.
 Note
If a payment is created for the delivery through A/R invoice, the payment does NOT generate an extra service tax
posting journal entry. This is because the service tax is already posted to the service tax accounts through the
invoice creation.
Beyond the 14 days range of the service delivery creation, if the service tax amount in the delivery is not fully posted to the
service tax accounts, you cannot create an invoice based on the delivery until you post the open service taxes to the service
tax accounts using Taxable Deliveries.
For more information, see the Taxable Deliveries section.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:56 AM
This way, the open service tax amount is posted to the service tax accounts.
In such case, for the open part of the service taxes, the point of taxation is the date of the delivery.
With the above two methods, for a service tax delivery, no matter if you create the invoices within or without 14 days, the point of
taxation always complies with the following legislations:
(a) Date of invoice or payment, whichever is earlier, if the invoice is issued within the prescribed period of 14 days from the date of
completion of the provision of service.
(b) Date of completion of the provision of service or payment, if the invoice is not issued within the prescribed period as above.
Deliveries Using Freight
When you copy service tax deliveries with freight to DPI or DPR, you can only include the freight as a new line as freight is not
available in DPI or DPR.
Currency
While you are creating any of the following documents related to a service tax delivery, you can only use the same currency as in
the delivery:
A/R invoice based on the service tax delivery
A/R credit memo for an A/R invoice which is created based on the service tax delivery
Down payment invoice or down payment request based on the service tax delivery
Payment created through DPI or DPR for the service tax delivery
Return based on the service tax delivery
Returns and A/R Credit Memos
 Note
When you create an A/R credit memo for an item in SAP Business One, you can decide whether the journal entry of the
credit memo reflects the inventory change or not by using the Without Qty Posting checkbox in the document rows.
However, after you enable the point of taxation rules, the Without Qty Posting checkbox is always selected for all
document rows when you create A/R credit memos for items,. This means that the creation of item type A/R credit
memos always influences the inventory.
When you create an A/R credit memo for an A/R invoice which is based on a service tax delivery, the A/R credit memo
must be fully created based on the invoice. In this case, you cannot copy an A/R credit memo partially from an A/R
invoice.
After you enable the point of taxation rules, you cannot create returns or A/R credit memos related to a service tax delivery if the
creation of these documents causes the open amount of the delivery to fall negative.
Financials and Banking: India
This section describes the financial and banking functions relevant to India.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:56 AM
Outgoing Excise Invoice: India
Use this window to create an excise invoice based on a delivery, goods return, or inventory transfer.
To open the window, choose Financials Tax Outgoing Excise Invoice .
 Note
The system automatically generates an outgoing excise invoice when you create the following documents:
A/P credit memo that is based on A/P invoices and contains items with CENVAT taxes
Cancellation document whose base document has been copied to an incoming excise invoice
 Note
SAP Business One provides a query that will show Inventory Transfer relevant OEIs that haven’t been copied to any IEI.
System Menu Tools Queries System Queries Open OEIs from Inventory Transfer Document
General Area
The first four fields contain information defined in the business partner master data.
Business Partner / To Warehouse
Specify whether the outgoing excise invoice is relevant to business partner or warehouse (default is Business Partner).
Contact Person
Name of the default contact person; editable field.
Excise Ref. No.
Specify the excise reference number.
No.
The left field displays the name of the selected numbering series; the right field displays the document number.
Status
Status of the current excise invoice.
Posting Date
Used to determine the time period for the document to be included in reports.
This field is uneditable and its value is the same as the posting date of the base document, for example, a delivery.
Excise Ref. Date
Specify the excise invoice date.
 Note
To add this document, you have to enter Excise Ref. No.
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:56 AM
Excise Removal Time
Specify the removal time of the excise invoice.
 Note
To add this document, you have to enter Excise Ref. No.
Currency
Choose the currency for displaying the amounts in the document.
When:
Customer currency = local currency, the drop-down list options are Local Currency or System Currency
Customer currency = a foreign currency, the drop-down list includes the option BP Currency
 Note
The selection does not change the original currency of the document.
Owner
Employee who owns the document.
Remarks
Additional document information; editable after the addition of the document.
Total Before Discount
Total amount of the document before calculating the discount.
If the discount is defined in the item or service row, the amount displayed in this field takes that discount into account.
% Discount
The left field displays the percentage of discount; the right field displays the discount amount. These fields are editable.
Rounding
This field appears only if the rounding method is defined as by Currency in the document settings.
Displays the difference between the original amount and the rounded amount obtained after the total document amount is
rounded, using the rounding method determined by the currency.
Tax
The tax amount for the document, calculated according to the set tax definitions.
Total
Total sum of the document, including tax and discounts.
Copy From
Specify a base document.
When the Business Partner / To Warehouse field is set to Business Partner:
If Business Partner is a customer, the option is Delivery
If Business Partner is a vendor, the option is Goods Returns
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:56 AM
When the field is set to To Warehouse, the option is Inventory Transfers. From pop-up window List of Inventory Transfers,
select the Inventory Transfer document you want to create OEI based on.
 Note
You cannot cancel an inventory transfer document if it has been copied to an outgoing excise invoice.
Once the Inventory Transfer document is copied in OEI, further operation is same as the existing functionality with following
exceptions:
User can change price copied from Inventory Transfer document
User can choose relevant Excise Tax code in OEI
Contents Tab
Item/Service Type
Choose:
Item to create a sales document for items defined in the Inventory module.
Service to create a sales document for a service that has not been defined as an Item in SAP Business One, such as a one-
time consultation.
The table view on this tab is different for each option.
To include items and services in the same sales document:
1. Enter the respective services as items in SAP Business One.
2. Enter the related items and services in one document, along with their respective prices and quantities.
3. Run the usual sales analysis and reports on these services.
Summary Type
Default value = No Summary
Choose By Documents to summarize rows with the same base documents into one row that displays the base document
number and reference.
An item appearing in the table more than once, and bearing the same price and description, is summarized to one row.
This option is available only when the documents are of type Item, and when you copy rows from base documents.
Table View for Document Type “Item”
Item No.
Displays the number of the selected item, as defined in the item master data.
Item Description
By default, displays the text from the item master data.
1. Modify as needed for the current sales document.
2. Press CTRL+TAB to save the change.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:56 AM
Changes do not affect the item master data.
Quantity
Displays the quantity in Sales Unit of Measure for the item, as defined in the item master data.
If the sales unit of measure contains more than one unit, the actual quantity of the units for the item is the number displayed in
this field multiplied by Items Per Sales Unit.
Price
Item price.
A blue price indicates a special price defined for this item, for this customer.
Tax Code
By default, displays the tax code linked to the item (see Inventory Item Master Data Sales Data tab). Choose a different tax
code, if required.
Total (LC)
Displays the total sum of the row in local currency, calculated according to this formula:
Quantity * Price * Exchange Rate - Discount for the Row (if defined).
WT Liable
Indicates if withholding tax is applicable in this document. You can manually select a value from the drop-down list.
Tax Amount (LC)
Tax amount in local currency.
Item WH
Displays Yes / No, depending on whether the item is defined as an inventory item in the item master data.
Distr. Rule
For certain dimensions, press Tab to open the List of Distribution Rules window, which:
Lists all the predefined distribution rules.
Lets you create new manual distribution rules.
 Note
To maintain the field Distr. Rule, you have to first maintain either Item No. under the document type Item or G/L Account
under the document type Service.
To define a manual distribution rule, you have to first provide the Total (LC) amount for both document types. The manual
distribution rule adopts the code form M+7 digits.
Once a certain distribution rule is chosen, a yellow arrow is added before the code, which enables you to retrieve the distribution
rule window for review or modification.
The distribution rule recorded here has an effective date that complies with the posting date of the sales document.
You can change the distribution rule for a specific row in the transaction.
RG23A Part I Number, RG23C Part I Number
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:56 AM
Specify the RG23A Part I Number, and RG23C Part I Number.
Logistic Tab
Ship To
Displays the customer's ship-to address, as defined in the business partner master data.
Pay To
Displays the customer's bill-to address, as defined in the business partner master data.
Shipping Type
Specify the required shipping type.
Accounting Tab
Journal Remark
By default, displays Outgoing Excise Invoice – XXX, where XXX is the BP code. If required, change this content.
BP Project
By default, displays the project name linked to the business partner in the business partner master data. If required, specify a
different project name.
Indicator
By default, displays the indicator linked to the business partner ( Business Partners Business Partner Master Data General
tab). The indicator is used as selection criteria in various reports. If required, choose a different indicator by clicking .
Order Number
Specify the order number of the chain, when you use the direct distribution method. This number is recorded in the file that you
send to the head office of the chain store.
Tax Tab
Tax Information
Click to open the Tax Information window for defining tax details.
Transaction Category
Displays the transaction category.
Form No.
Displays the form number.
Export
Segregates removals for export from other removals.
Duty Status
Specify whether this invoice is with or without payment of duty.
The system posts the CENVAT taxes at the time of the excise invoice creation. There is no posting for Without Payment of Duty.
Even if the removal is without payment of duty, you need to prepare an excise invoice as required.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:56 AM
To issue OEI without payment of duty, check Tax tab, then select Duty Status as Without Payment of Duty
If the OEI for a particular Stock Transfer is defined as without payment of duty the corresponding IEI will be treated as without
payment of duty and will copy data from OEI.
SSI Exemption
Select to exempt the outgoing excise invoice from CENVAT type taxes. By default, the checkbox is selected.
 Note
This checkbox appears only for outgoing excise invoices with the location marked as SSI Exemption. Once the document is
added, you cannot change the checkbox status.
Automatically Create IEI
Automatically creates an incoming excise invoice when you create an outgoing excise invoice.
IEI Ref. No.
Specify a reference number for creating an incoming excise invoice.
This is a mandatory field that appears when Automatically Create IEI is selected.
IEI Ref. Date
Specify the reference date for creating an incoming excise invoice.
This field appears when Automatically Create IEI is selected.
Incoming Excise Invoice: India
Use this window to create an excise invoice based on a goods receipt PO, return, or outgoing excise invoice.
 Note
The system automatically generates an incoming excise invoice when you create the following documents:
A/R credit memo that is based on A/R invoices and contains items with CENVAT taxes
Cancellation document whose base document has been copied to an outgoing excise invoice
To open the window, choose Financials Tax Incoming Excise Invoice .
General Area
The first four fields contain information defined in the business partner master data.
Business Partner / From Warehouse
Specify whether the incoming excise invoice is relevant to business partner or warehouse (default is Business Partner).
Contact Person
Name of default contact person; editable field.
Phone
Phone number of the contact person, or, if not listed, the customer.
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:56 AM
Excise Ref. No.
Specify the excise reference number.
No.
The left field displays the name of the selected numbering series; the right field displays the document number.
Status
Status of the excise invoice.
Posting Date
Used to determine the time period for the document to be included in reports.
This field is uneditable and its value is the same as the posting date of the base document, for example, a goods receipt PO or an
outgoing excise invoice.
Excise Ref. Date
Specify the excise invoice date.
 Note
To add this document, you have to enter Excise Ref. No.
Excise Removal Time
Specify the removal time of the excise invoice.
 Note
To add this document, you have to enter Excise Ref. No.
Currency
Specify the currency for displaying the amounts in the document.
When:
Customer currency = local currency, the drop-down list options are Local Currency or System Currency
Customer currency = a foreign currency, the drop-down list includes the option BP Currency
 Note
The selection does not change the original currency of the document.
Owner
Employee who owns the document.
Remarks
Additional information regarding the document; editable after the addition of the document.
Total Before Discount
Total amount of the document, before calculating the discount.
If the discount is defined in the row for the item or service, the amount displayed here takes that discount into account.
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:56 AM
% Discount
The left field displays the percentage of discount; the right field displays the discount amount. These values are editable.
Rounding
This field appears when the rounding method is defined as by Currency in the document settings.
When the total amount of the document is rounded, this field displays the difference between the original and the rounded
amounts.
Tax
Tax amount for the document, calculated according to the defined tax definitions.
Total
Total sum of the document, including tax and discounts.
Copy From
Specify a base document.
When the Business Partner/From Warehouse field is set to Business Partner:
If Business Partner is a customer, the option is Return.
If Business Partner is a vendor, the option is Goods Receipt PO.
When the field is set to From Warehouse, the option is Outgoing Excise Invoice. From pop-up window List of Outgoing
Excise Invoice, select the OEI document created previously.
Contents Tab
Item/Service Type
Choose:
Item to create a sales document for items defined in the Inventory module.
Service to create a sales document for a service that has not been defined as an item in SAP Business One, such as a one-
time consultation.
The table view on this tab is different for each option.
To include items and services in the same sales document:
1. Enter the respective services as items in SAP Business One.
2. Enter the related items and services in one document, along with their respective prices and quantities.
3. Run the usual sales analysis and reports on these services.
Summary Type
Default value = No Summary
Choose By Documents to summarize rows with the same base documents into one row that displays the base document
number and reference.
An item appearing in the table more than once, and bearing the same price and description, is summarized to one row.
This option is available only when the documents are of type Item, and when you copy rows from base documents.
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:56 AM
Table View for Document Type “Item”
Type
The type of row.
The options are:
T for a text row
Σ for a subtotal row
A for an alternative item row, if the sales document is a sales quotation
For a regular item row, this field is blank.
For more information about text row, subtotal row, and alternative item row, see the online help Sales - A/R or Purchasing - A/P
Goto Menu - Sales and Purchasing Documents Text Row / Subtotal Row / Alternative Item Row .
Item No.
Number of the selected item as defined in the item master data.
Item Description
By default, displays the text defined in the item master data.
To modify the information for the current sales document only:
1. Make the necessary changes.
2. Press CTRL+TAB to save the changes.
Quantity
Displays the quantity in Sales Unit of Measure for the item, as defined in the item master data.
If the sales unit of measure contains more than one unit, the actual quantity of the units for the item is the number displayed in
this field multiplied by the Items Per Sales Unit.
Price
Item price.
A blue price indicates a special price defined for this item for this customer.
Tax Code
Specify the tax code.
By default, displays the tax code linked to the item (see Inventory Item Master Data Sales Data tab).
Total (LC)
Total sum of the row in local currency, calculated according to this formula:
Quantity * Price * Exchange Rate - Discount for the Row (if defined).
WT Liable
Indicates if withholding tax is applicable in this document. You can manually select a value from the drop-down list.
Tax Amount (LC)
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:56 AM
Tax amount in local currency.
Item WH
Displays Yes / No, depending on whether the item is defined as an inventory item in the item master data.
Distr. Rule
For certain dimensions, press Tab to open the List of Distribution Rules window, which:
Lists all the predefined distribution rules.
Lets you create new manual distribution rules.
 Note
To maintain the field Distr. Rule, you have to first maintain either Item No. under the document type Item or G/L Account
under the document type Service.
To define a manual distribution rule, you have to first provide the Total (LC) amount for both document types. The manual
distribution rule adopts the code form M+7 digits.
Once a certain distribution rule is chosen, a yellow arrow is added before the code, which enables you to retrieve the distribution
rule window for review or modification.
The distribution rule recorded here has an effective date that complies with the posting date of the sales document.
You can change the distribution rule for a specific row in the transaction.
RG23A Part I Number, RG23A Part II Number, RG23C Part I Number, RG23C Part II Number
Specify the RG23A Part I Number, RG23A Part II Number, RG23C Part I Number, and RG23C Part II Number.
Logistic Tab
Ship To
Customer ship-to address, as defined in the business partner master data.
Pay To
Customer bill-to address, as defined in the business partner master data.
Shipping Type
Drop-down list of shipping types.
Accounting Tab
Journal Remark
By default, displays Incoming Excise Invoice – XXX, where XXX is the BP code. If required, change this content.
BP Project
By default, displays the project name linked to the business partner in the business partner master data. If required, specify a
different project name.
Indicator
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:56 AM
By default, displays the indicator linked to the business partner ( Business Partners Business Partner Master Data General
tab). The indicator is used as selection criteria in various reports. If required, choose a different indicator by clicking .
Order Number
Specify the order number of the chain, when you use the direct distribution method. This number is recorded in the file that you
send to the head office of the chain store.
Tax Tab
Tax Information
Click to open the Tax Information window, for defining tax details.
Transaction Category
Displays the transaction category.
Form No.
Displays the form number.
Duty Status
Specify whether this invoice is with or without payment of duty.
The system posts the CENVAT taxes at the time of excise invoice creation. There is no posting for Without Payment of Duty.
Even if the removal is without payment of duty, you need to prepare the excise invoice as required.
SSI Exemption
Select to exempt the incoming excise invoice from CENVAT type taxes. By default, the checkbox is selected.
 Note
This checkbox appears only for incoming excise invoices with the location marked as SSI Exemption. Once the document is
added, you cannot change the checkbox status.
TDS: India
In the SAP Business One Financial module, you can do the followings with TDS:
Make adjustments to the TDS amount per invoices which could be regular A/P invoices or A/P down payment Invoices.
Set up an acknowledgement number
Generate the Form 16A report
Generate an e-TDS file for e-TDS return
More Information
Processing Adjustment Entry: India
Setting Up Acknowledgement Numbers: India
Generating Form 16A: India
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:56 AM
Generating Quarterly eTDS File: India
Processing Adjustment Entry: India
You can make adjustments in the TDS amount per invoices. The invoices include A/P invoices and A/P down payment invoices. In
SAP Business One, you can post the adjustment journal entry for the fresh amount.
Procedure
1. To access the window, from the SAP Business One Main Menu, choose Financial TDS Adjustment Entry .
2. Specify the following fields:
Transaction Type
Select the type of the transaction to which you want to make an adjustment for TDS.
Transaction No.
Select the number of the transaction to which you want to make a change in TDS.
BP Code
Displays the business partner code.
Assessee Code
Displays the assessee code.
WTax Code
Displays the WTax Code of the original transaction.
Taxable Amount
Displays the taxable amount of the invoice.
Total Rate %
Displays the applicable total tax rate as a percent.
TDS Amount
Display the original TDS amount calculated on the invoice.
Surcharge Amount
Display the surcharge amount of the original transaction.
Cess Amount
Display the Cess amount of the original transaction.
HSC Amount
Display the HSC amount of the original transaction.
New TDS Amount
Specify the new TDS amount you want to add for the transaction. If the amount is negative, the new amount is to be
deducted from the existing amount.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:56 AM
New Surcharge Amount
Specify the new surcharge amount you want to add to for this transaction. If the amount is negative, the new amount is to
be deducted from the existing amount.
New Cess Amount
Display the new Cess amount you want to add for this transaction. If the amount is negative, the new amount is to be
deducted from the existing amount.
New HSC Amount
Display the new HSC amount you want for the transaction.
3. Choose the OK button.
More Information
TDS: India
Generating Form 16A: India
A certificate of deduction of tax at source must be issued to vendors. It lists the TDS deducted on the payment made to vendors.
This certificate is known as Form No. 16A.
Procedure
1. To generate the Form 16A, from the SAP Business One Main Menu, choose Financial TDS Form 16 A .
2. Specify the following fields:
Code
In the From...and To... fields, choose the vendors for whom you want to run the Form 16A report.
Section Code
Select a section code for which the Form 16 A certificate is being generated.
TDS Location
In the drop down list, select a location for which you want to generate the Form 16 A certificate.
Financial Year
Specify the financial year for the report.
Quarter
Specify the quarter in the financial year for the report.
 Note
Before generating the report, you must define the acknowledgement number for the selected quarter. For more
information, see Setting Up Acknowledgement Numbers: India.
Deductee Type
Select a deductee type from the drop down list.
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:56 AM
Person Responsible
Select the person responsible for deducting the tax.
Designation
Designation of the person responsible.
3. Choose the OK button.
More Information
Form 16 A Report Window
Form 16 A Report Window: India
Send this report to tax authorities for the TDS deduction.
Document No.
Document number of the entry.
Date of Payment/Credit
Posting date in each entry.
Document Date
Creation date of a document .
Taxable Amount
Taxable amount of a document.
Total Tax Deposit
Total tax deposited of the entry.
TDS Amount
TDS amount of each entry.
Surcharge
Surcharge tax amount of each entry.
Cess
Cess tax amount of the entry.
HSC
HSC tax amount of the entry.
Certificate No.
To print out the report, you must generate the TDS certificate number. To display the certificate number, choose the Generate
Cert. No. button in the bottom area.
Challan No.
Challan number with which the tax was deposited in outgoing payments.
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:56 AM
BSR Code
Bank serial number of each entry.
Cheque No.
Cheque number in the payment means of outgoing payments.
Generate Cert. No.
Generates the certificate series for the report.
More Information
Form 16 A: India
Setting Up Acknowledgement Numbers: India
Use the window to define the acknowledgement number to generate with the Form 16A report.
Procedure
1. To access the window, from SAP Business One Main Menu, choose Financial TDS Acknowledge Number .
2. Specify the following fields:
Financial Year
Select a financial year code.
Quarter
Select a quarter which you have defined in the Defining Financial Year Master window.
Acknowledgement No.
Specify the acknowledgement number for each quarter.
Location
Select a location for which an acknowledgement number is being obtained and for which a print out is required.
3. Choose the OK button.
Generating Quarterly eTDS File: India
Use this function to generate the quarterly eTDS files submitted to the taxation authorities.
To generate a quarterly report, proceed as follows:
Procedure
1. To access the window, from the SAP Business One Main Menu, choose Financials TDS Generate Quarterly eTDS File
2. Specify the fields in the table below.
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:56 AM
Financial Year
Select a financial year for which to generate the report.
Person Responsible
Select a person responsible for deducting the TDS.
Designation
Designation of the person responsible.
Deductor Type
Select a deductor type from the drop down list.
Quarter
Select a quarter for which to generate the report.
Book Entry
Specify if the TDS payment was made by book entry.
Return Type
Select the return type from the following two options:
26: quarterly statement of deduction of tax under the Act in respect of payments other than salary and non
residents for the quarter.
27: quarterly statement of deduction of tax under the Act in respect of payments other than salary made to non
residents for the quarter.
Location
Select a location for which the eTDS return is being generated.
Return Preparation Utility
The default value is SAP Business One <version no.>. You can edit this field. This value appears in the Name of
Return Preparation Utility field of the TDS statement for the non salary category (file header record).
Enter File Name
You can select the file directory and file name where the eTDS file can be stored. To change the directory, click the Browse
button and choose the file directory you want.
Generate eTDS File
Lets you to generates the eTDS file.
3. Click the Generate eTDS File button.
 Note
Before an eTDS return is generated, the following fields in SAP Business One are checked for values:
The STD Code, Telephone 1, and E-Mail fields in Administration System Initialization Company Details
General Local Language
The STD Code, Office Phone, Mobile Phone, and E-Mail fields in Human Resources Employee Master Data
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:56 AM
Manually Reconciling Bank Statements
 Recommendation
When you use this function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do not
simultaneously use the external bank statement processing function (see Recording Transactions from External Statements in
the general online help file provided with SAP Business One) and the standard function for manually performing an external
reconciliation (see Manually Performing External Reconciliations in the general online help file provided with SAP Business
One) for the same bank account. In addition, we recommend that you use exclusively either this function or the standard
function for manually reconciling bank statements.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
The External Bank Reconciliation - Selection Criteria window appears.
2. In the Account Code field, select an account code.
As a result, Account Name and Currency are displayed automatically in the respective fields. If the account currency is
defined as All Currencies, the local currency is displayed and is the reconciliation currency. You cannot edit the Currency
and the Last Balance fields. In addition, the Last Balance field automatically displays the updated balance from the
previous reconciliation.
In the Ending Balance field, specify the current balance received from the bank; in the End Date field specify the date to
which the current balance is updated.
3. Choose OK.
The Reconciliation Bank Statement window appears.
SAP Business One displays all the open deposits and payments in which the selected account is involved. View and specify
the information displayed.
4. Select the transactions to be cleared.
When you select a transaction, SAP Business One recalculates the value in the Difference field. Reconciliation is performed
only if the difference equals zero.
5. If the value in the Difference field is not zero, do one of the following:
Create an adjustment.
For more information, see Creating Adjustments.
Save your selection for future processing.
Choose the Save button. The next time you choose the same account in the External Bank Reconciliation -
Selection Criteria window, the Reconciliation Bank Statement window displays the saved selection.
6. To perform the reconciliation, choose the Reconcile button.
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:56 AM
 Note
You cannot re-create reconciliations created in the Reconciliation Bank Statement window.
Result
SAP Business One reconciles the selected transactions and sets the reconciliation type for this reconciliation to Manual.
More Information
Example: Manual Reconciliation of External Bank Statements
Creating Adjustments
To reflect transactions that are already in the bank statement but are not yet posted in SAP Business One, you can create a
balancing transaction or document.
 Recommendation
When you use this localized function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do
not simultaneously use the external bank statement processing function (see the Recording Transactions from External
Statements page in the general online help provided with SAP Business One) and the standard function for manually
performing an external reconciliation (see the Manually Performing External Reconciliations page in the general online help
provided with SAP Business One) for the same bank account. In addition, we recommend that you use exclusively either this
function or the standard function for manually reconciling bank statements.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
After you make the required adjustments, the difference between the ending balance in the bank statement and the account
balance in the books equals zero, and you can now reconcile the selected transactions.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
2. In the External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
3. In the Reconciliation Bank Statement window, make the required selections and choose Adjustments.
The Adjustments window appears.
4. Select one of the following types of transactions you want to create and choose OK:
Journal entry
Incoming payment
Outgoing payment
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:56 AM
Check for payment
Deposit
The window of the selected transaction type appears.
5. Create the required transaction and choose Add.
As a result, the created transaction is added to the table of the Reconciliation Bank Statement window, and it is also
selected. The value in the Difference field is updated accordingly.
6. To perform the reconciliation, choose the Reconcile button.
More Information
Manually Reconciling Bank Statements
Example: Manual Reconciliation of External Bank Statements
External Bank Reconciliation - Selection Criteria Window
Reconciliation Bank Statement Window
Example: Manual Reconciliation of External Bank Statements
On December 1, 2009, you decide to perform a reconciliation for your bank account. The last balance of this account was 100, and
the ending balance of this bank account for this date is 250.
The Reconciliation Bank Statement window displays 2 deposits that you can clear:
Date Transaction Number Deposit Amount
November 10, 2009 927 45
November 24, 2009 929 100
You need to reconcile transactions to match the value of the cleared book balance to the ending balance of this bank account. In
this case, you need to reconcile transactions with a total amount of 150 = 250 minus 100.
You select both transactions, but the total amount of the open transactions is 145 = 45 + 100.
You create a manual journal entry as an adjustment, debiting the bank account by the amount of 5.
As a result, an additional row is added to the list of transactions you want to clear. The difference between the cleared book
balance and the statement ending balance is now zero, enabling you to complete the reconciliation.
More Information
Creating Adjustments
External Bank Reconciliation - Selection Criteria Window
Use this window to define the selection criteria for manually reconciling bank statements.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:56 AM
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation .
External Bank Reconciliation – Selection Criteria Window Fields
Account Code, Account Name, Currency
Select the relevant account code.
After you select an account code, the account name and currency are displayed automatically in the respective fields. If the
account is defined as All Currencies, the local currency is displayed and is the reconciliation currency.
 Note
You cannot edit the Currency field (described above) and the Last Balance field (described below).
Bank Statement
This section contains the following fields:
Last Balance – Automatically displays the updated balance from the previous reconciliation.
Ending Balance – Specify the current balance received from the bank.
End Date – Specify the date to which the current balance is updated.
More Information
Reconciliation Bank Statement Window
Manually Reconciling Bank Statements
Reconciliation Bank Statement Window
This window displays all the open deposits and payments in which the account you chose in the External Bank Reconciliation -
Selection Criteria window is involved.
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation . In the
External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
General Area
Account Code
Displays the account code selected in the External Bank Reconciliation – Selection Criteria window.
Display
Determines what transactions are displayed. Select one of the following display options:
All – Both cleared and uncleared transactions
Cleared – Only cleared transactions
Uncleared – Only uncleared transactions
Find
Enables you to find a specific transaction in a sorted column.
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:56 AM
 Example
To find a transaction according to its number, sort the Trans. No. column. Then in the Find field, specify the relevant number.
SAP Business One highlights the first transaction that matches the value entered.
 Note
By default, the Date column is sorted.
Statement No.
Specify the number of the statement you received. This number is unique for each account. This means you can assign the same
number to statements created for different accounts; however, you can assign the same number only to one statement in each
account. You can create a statement without a number.
 Note
If a reconciliation is canceled, its statement number becomes available again and can be used for a new reconciliation.
Last Statement Balance
Displays the balance of the previous statement.
Payment, Deposit: Total No., Total Amount
The Total No. field displays the total number of selected transactions on the debit side (Payment) and on the credit side (Deposit).
The Total Amount field displays the cumulative debit amount and credit amount.
Cleared Book Balance
Displays the total cleared amount, considering the selected transactions.
Statement Ending Balance
Displays the value entered in the Ending Balance field in the External Bank Reconciliation – Selection Criteria window.
Difference
Displays the difference between the Cleared Book Balance and the Statement Ending Balance. This value depends on the
selected transactions.
Save
Saves the current reconciliation so that you can continue working on it later. The next time you choose the same account in the
External Bank Reconciliation – Selection Criteria window, the Reconciliation Bank Statement window displays the saved
selection.
Adjustments
Enables you to create any required bank adjustments by opening the Adjustments window. For more information, see Creating
Adjustments .
Table Area
Cleared
Select to indicate that the transaction has been cleared.
Type
Displays the transaction type:
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:56 AM
PS – represents payments, that is, transactions in which the selected account is credited
DP – represents deposits, that is, transactions in which the selected account is debited
Date
Displays the posting date of the transactions.
Trans. No.
Displays the number of the transaction and provides a link to the journal entry.
Reference No.
Displays the reference number as it appears in the Ref. 1 field in the Journal Entry window.
Payment
Displays the amount on the debit side in the transaction.
Deposit
Displays the amount on the credit side in the transaction.
Cleared Amount
After you select the transaction, the amount in the Payment/Deposit column is displayed here.
More Information
External Bank Reconciliation - Selection Criteria Window
Manually Reconciling Bank Statements
Outgoing Payments: P.L.A.: India
This option appears only in outgoing payments when the personal ledger account (P.L.A.) in G/L Account Determination is not
null.
To display this window, choose Banking Outgoing Payments Outgoing Payments ; then choose P.L.A.
General Area
No.
Displays the default numbering series and current number of the outgoing payment in the default numbering series.
Posting Date
Specify the posting date.
The current date is displayed by default.
Due Date
The value you specify will be the due date of the business partner row in the journal entry created by the document.
The current date is displayed by default.
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:56 AM
After you enter the details of the payment means in the Payment Means window, and return to the Outgoing Payment window,
this field is updated and displays the weighted average of the due dates defined for the payment means.
You can change this date, if required, before you add the document.
Reference
Specify another reference for this document, if required.
Transaction No.
Displays the number of the journal entry created by this document. The number appears after you add the outgoing payment.
Location
Select the location; default value is the location of the sequence. This field is mandatory.
 Note
P.L.A Remaining Amount is updated based on the location you select.
Seq. Name
Specify a sequence from the drop-down list. The system generates the sequence automatically.
 Note
This field appears only for documents that are assigned a sequence.
Project
Displays the project for this document.
Doc. Currency
Displays the currency for this document.
Challan No.
Displays the Challan No.
Challan Date
Displays the Challan date.
BSR Code
Specify the BSR Code received from the bank on deposit of Challan.
Bank Name
Displays the bank name.
Remarks
Enter any remarks regarding this outgoing payment.
Journal Remarks
Enter the information to display in the Details field of the journal entry. By default, this field contains the text: “Outgoing - P.L.A.”.
Total Amount Due
Displays the total amount to be paid through this document.
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:56 AM
Table Area
CENVAT Component
Displays all tax types for CENVAT.
Remaining Amount
Displays the remaining amount of CENVAT tax type by the location selected in the general area.
Deposit Amount
Specify the deposit amount to be posted into P.L.A. Account separately for each tax component.
More Information
Outgoing Payments
Creating Outgoing Payments: TDS: India
To record the TDS deposit in the government account during the booking of outgoing payments of vendors or customers, proceed
as follows:
Procedure
1. In the Outgoing Payment window, choose the TDS radio button.
2. Specify the following fields:
Section Code
Section code based on the codes you defined in the Withholding Tax Codes - Setup window.
Description
Displays the description of the TDS section codes.
Assessee Type
Displays the assessee types defined in the Nature of Assessee window.
Amount Payable
Displays the amount payable against each TDS section code, location and assessee type.
Deposit Amount
Displays the deposit amount against each amount payable.
Location
Select the location at which the TDS payment is being handled.
Bank Serial No.
Bank code number for the TDS deposit.
Challan No.
Displays the TDS deposit challan number which was issued by bank or transfer voucher number.
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:56 AM
Challan Date
Challan date of the TDS deposit.
Bank Name
Bank name of the TDS deposit.
3. To select more TDS entries for depositing tax amounts, choose the Pick TDS Entries button to open the TDS Entries
window.
4. In the TDS Entries window, to select the transactions you want, select the Choose checkbox of the line transactions.
Choose the OK button. You return to the Outgoing Payment: TDS window.
5. In the Outgoing Payment: TDS window, to deposit the TDS amount, choose the payment means button from the tool bar.
6. In the Payment Means window, you can make the payment as you want. For more information about payments, see
Payment Means.
7. After you finish with payment means, you return to the Outgoing Payment: TDS window. To continue, choose the Add
button.
More Information
TDS Entries
Payment Means
TDS Entries: India
In this window, you can select document entries for the TDS tax amount deposit.
To open the window, from the SAP Business One Main Menu, choose Banking Outgoing Payments , select the TDS radio
button and then click the Pick TDS Entries button.
 Note
Only fully paid down payment invoices appear in the window.
Choose
Includes this document for a TDS tax deposit.
Transact. Type
Document type of the TDS entry.
Document No.
Document number of the TDS entry.
Posting Date
Posting date of the TDS entry.
Base Amount
Base amount on the entry.
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:56 AM
Taxable Amount
Taxable amount of the entry.
Total Tax Amount
Total tax amount of the entry.
Total Tax Rate (%)
Total tax rate (%) based on the rate of the entry.
TDS Amount
TDS amount based on the tax amount of the entry.
Surcharge Amount
Surcharge tax amount based on the surcharge tax amount of the entry.
Cess Amount
Cess tax amount based on the Cess tax amount of the entry.
HSC Amount
HSC tax amount based on the HSC tax amount of the entry.
More Information
Outgoing Payments: TDS: India
Marketing Documents and Inventory: India
This section describes features and functions related to sales and purchasing documents and inventory that are relevant to India
only.
Information related to general sales, purchasing, and inventory functionality is available in the general online help file delivered
with SAP Business One, in Help Documentation Online Help .
 Note
A/R Reserve Invoice and A/P Reserve Invoice are described in the general online help file provided with SAP Business One.
These documents are not relevant for India and hence are not available in the SAP Business One software version for India.
Additional Information
Gross Amount
This field (in the Freight Charges window) is not editable.
When you change the value in the Net Amount field, the value in this field will be updated automatically according to the
predefined tax group.
Creating Sales and Purchasing Documents with Negative Totals
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:56 AM
Use
You can create invoices with negative totals. This allows you to bill and refund a customer or vendor in one single document. This
may be convenient for example, if you as a sales person are on the phone with a customer who is ordering certain items, but at the
same time wants to return some items that he ordered previously. In this case, instead of posting an A/R invoice and a credit
memo, you enter the items that the customer purchases as a positive quantity and the goods the customer intends to return as a
negative quantity.

 Recommendation
We recommend that you consider carefully whether you would like to record two opposite transactions in one document.
Posting two documents helps to improve transparency in accounting.
You can generate the following documents with a negative total:
A/R and A/P invoice
A/R and A/P credit memo
An A/R delivery
An A/R return
An A/P goods receipt
An A/P goods return
The inventory valuation behavior of the documents with negative totals is as outlined in the table below.
Inventory valuation behavior of documents with negative totals
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
| Goods receipt P/O | Goods return      | Inventory | Allocation |     |
| ----------------- | ----------------- | --------- | ---------- | --- |
| Goods return      | Goods receipt P/O | Inventory | Allocation |     |
A/P Invoice A/P credit memo Inventory Vendor Negative Adjustment
Account, Price
Differences Account
A/P credit memo A/P invoice Inventory Vendor Negative Adjustment
Account, Price
Differences Account
| Delivery        | A/R return      | Inventory    | COGS |     |
| --------------- | --------------- | ------------ | ---- | --- |
| Return          | Delivery        | Sales Return | COGS |     |
| A/R invoice     | A/R credit memo | Inventory    | COGS |     |
| A/R credit memo | A/R invoice     | Sales Return | COGS |     |
Goods receipt P/O based Goods return based on Inventory Allocation Negative Adjustment
| on goods return | goods receipt P/O |     |     | Account, Price |
| --------------- | ----------------- | --- | --- | -------------- |
Differences Account
Goods return based on Goods receipt P/O based Inventory Allocation Negative Adjustment
| goods receipt P/O | on goods return |     |     | Account, Price |
| ----------------- | --------------- | --- | --- | -------------- |
Differences Account
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:56 AM
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
| A/P invoice based on | Credit memo based on | No inventory transaction |     |
| -------------------- | -------------------- | ------------------------ | --- |
| goods receipt P/O    | goods return         |                          |     |
A/P credit memo based A/P invoice based on Vendor, Allocation Price Differences
| on goods return | goods receipt P/O |     | Account, Negative |
| --------------- | ----------------- | --- | ----------------- |
Adjustment Account
A/P credit memo based Invoice based on credit Inventory Vendor Negative Adjustment
| on A/P invoice | memo |     | Account, Price |
| -------------- | ---- | --- | -------------- |
Differences Account
Delivery based on return Delivery based on return Inventory COGS Negative Adjustment
Account
Return based on delivery Return based on delivery Sales Return COGS Negative Adjustment
Account, Price
Differences Account
| A/R invoice based on  | Credit memo based on | No inventory transaction |     |
| --------------------- | -------------------- | ------------------------ | --- |
| delivery              | return               |                          |     |
| A/R credit memo based | A/R invoice based on | No inventory transaction |     |
| on return             | delivery             |                          |     |
A/R credit memo based A/R invoice based on Sales Return COGS Negative Adjustment
| on invoice | credit memo |     | Account, Price |
| ---------- | ----------- | --- | -------------- |
Differences Account
Purchasing Documents, Tax Tab: India
Use this tab to specify sales tax information relevant for reports.
To access this tab, choose  Purchasing - A/P   Purchase Order, Goods Receipt PO, Goods Return, A/P Invoice, A/P Credit
Memo, A/P Down Payment Request, A/P Down Payment Invoice   Tax .
Sales Tax Relevant Fields
Tax Information
Click   to open the Tax Information window for viewing or modifying tax details.
Transaction Category
Specify a transaction category.
Form No.
Specify the form number.
Duty Status
Specify whether this invoice is with or without payment of duty.
If you define the duty status on the document level as with payment of duty, the checkboxes in the Duty Status column in the
Define Tax Amount Distribution window will be selected and non-editable by default.
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:56 AM
If you define the duty status on the document level as without payment of duty, the checkboxes in the Duty Status column in the
Define Tax Amount Distribution window will be deselected by default, and you can edit the checkboxes only for the Non-CENVAT
tax category, to post the tax amount.
 Note
When you copy a document, the duty status property of the target document inherits the value of the duty status property of
the base document and is not editable.
The Duty Status field can also be found in inventory transfer documents. When you copy an invoice transfer document to an OEI,
or copy an OEI to IEI, the duty status property inherits the value of the duty status property of the invoice transfer document, and
is not editable.
Import
Segregates purchase invoices for imports.
Excise Ref. No.
Specify the excise reference number.
Among all the purchasing documents, this field appears only in the following documents:
A/P credit memo that is based on A/P invoices and contains excisable items: The Excise Ref. No. field is not mandatory.
After adding the document, the system automatically generates an outgoing excise invoice.
Cancellation document of a goods return containing excisable items: If a goods return contains excisable items, you can
cancel it only after you have created an outgoing excise invoice based on the goods return. The Excise Ref. No. field on the
corresponding cancellation goods return is mandatory. After adding the cancellation goods return, the system
automatically generates an incoming excise invoice.
Sales Documents, Tax Tab: India
Use this tab to view and edit details regarding the sales tax information used in relevant reports.
To access this window, choose Sales A/R Sales Quotation, Sales Order, Delivery, Returns, A/R Invoice, A/R Credit Memo,
A/R Down Payment Request, A/R Down Payment Invoice Tax .
Sales Tax Relevant Fields
Tax Information
Click to open the Tax Information window in which you can view or change the tax information.
Transaction Category
Specify a transaction category.
Form No.
Specify the form number.
Duty Status
Specify whether this invoice is with or without payment of duty.
If you define the duty status on the document level as with payment of duty, the checkboxes in the Duty Status column in the
Define Tax Amount Distribution window will be selected and non-editable by default.
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:56 AM
If you define the duty status on the document level as without payment of duty, the checkboxes in the Duty Status column in the
Define Tax Amount Distribution window will be deselected by default, and you can edit the checkboxes only for the Non-CENVAT
tax category, to post the tax amount.
 Note
When you copy a document, the duty status property of the target document inherits the value of the duty status property of
the base document and is not editable. (Exception: When you copy a sales quotation to a sales order, this field is editable as
long as the document status is open.)
If you use the Document Generation Wizard, in order to consolidate documents having different duty statuses, in step 4 of the
wizard, in the Expanded Consolidation Options field, select Duty Status.
If you copy multiple documents to a single document, they must all have the same duty status.
The Duty Status field can also be found in inventory transfer documents. When you copy an invoice transfer document to an OEI,
or copy an OEI to IEI, the duty status property inherits the value of the duty status property of the invoice transfer document, and
is not editable.
Export
Enables you to segregate sales invoices for export.
Excise Ref. No.
Specify the excise reference number.
Among all the sales documents, this field appears only in the following documents:
A/R credit memo that is based on A/R invoices and contains excisable items
Cancellation document of a delivery containing excisable items
 Note
You can cancel a delivery only after you have created an outgoing excise invoice based on the delivery.
Form No. Batch Update: India
This report gives you batch update information on the Form No. in marketing documents.
Use this window to specify selection criteria for performing batch updates on the Form No. in marketing documents.
To open this window, choose Sales – A/R Form No. Batch Update , or Purchasing – A/P Form No. Batch Update , or
Inventory Inventory Transactions Form No. Batch Update .
 Note
In the Form Number Batch Update window, you see only those marketing documents for which you have authorization.
User
Specify a user name to display marketing documents created by this user, or choose All to display drafts created by all users.
Open Only
Displays in the Form No. Batch Update window only those marketing documents with the status Open.
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:56 AM
Sales-A/R, Purchasing- A/P
Lets you select additional marketing documents to be included in the report.
Inventory Transfer
Displays form numbers with inventory transfers.
Inventory Transfer Request
Displays form numbers with inventory transfer requests.
Location
Specify the location for the inventory transfer in the Form No. Batch Update window.
 Note
User can filter the selection by Locations.
Transaction Category
Specify a transaction category as predefined in Transaction Category – Setup window.
A number of Transaction Categories are predefined. This will help generation of Purchase and Sales Register reports. To view or
update the predefined Transaction Category, check Marketing Document Tax tab Transaction Category Define New
Default predefined Transaction Categories are:
Form C: This is issued by the purchasing dealer to the selling dealer, if the goods are covered in the registration certificate
of the purchasing dealer.
Form E-I and E-II: This is issued by the selling dealer to the purchasing dealer. The selling dealer makes declaration in E-I
form if it is a first sale and in E-II form if it is a subsequent sale.
Form F: This is issued by the transferring dealer. The dealer makes declaration in Form F, if the goods are dispatched to
another State on consignment basis or to branch of dealer in another State. This is only Inter State movement of goods and
not a sale and hence no CST is payable.
Form H: This is issued by the purchasing dealer (for Export) to the selling dealer, if the goods are sold in the course of
Export; the sale during course of export is exempt from CST.
Form No. Batch Update Window
This window displays marketing documents according to the defined selection criteria.
User can use Form No. Batch Update to maintain Form No. for VAT relevant Iinventory Transfers.
To see the details of a marketing document, double-click a row.
Form No.
The existing value in the marketing document.
Service Category - Setup: India
Use this window to define a new service category.
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:56 AM
Service Category - Setup Window
Service Category
Specify a name for the new service category.
 Note
You cannot remove a service category that is used in item master data.
Description
Provide information about the service category.
More Information
Item Master Data: General Tab
Chapter ID - Setup: India
Use this window to define a new Chapter ID. This information is needed when the material is defined as excisable.
Chapter ID - Setup Window
Chapter, Heading, Subheading, Description
Enter the excisable information for each field.
More Information
Item Master Data: General Tab
Message Documentation
Message documentation aims to provide you with the information you need to respond to system or error messages that may
appear in SAP Business One.
10000908
Message
Enter P.A.N. number for business partner
Diagnosis
1. From the SAP Business One Main Menu, you have chosen:
Business Partners Business Partner Master Data
2. In the Business Partner Master Data window, on the Accounting tab, on the Tax subtab , you have selected the Subject to
Withholding Tax checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:56 AM
3. You have chosen the Add or Update button.
However, you have not specified a P.A.N. number, and this is required for business partners who are subject to withholding
tax.
Procedure
To specify a P.A.N. number for a business partner who is subject to withholding tax:
1. On the Tax subtab of the Accounting tab in the Business Partner Master Data window, choose the button.
2. In the Tax Information window, in the P.A.N No. field, enter a number.
 Note
A P.A.N. number must contain 10 alphanumeric characters.
3. Choose the Add or Update button.
More Information
Locations - Setup: India
Business Partner Master Data: Accounting Tab, Tax
10000909
Message
PAN No. must be 10 alphanumeric characters
Diagnosis
1. You have created a new customer. In the Business Partner Master Data window, you have chosen the Tax subtab of the
Accounting tab.
2. You have chosen the Tax Information button. In the Tax Information window, you have specified a P.A.N. number that does
not consist of 10 alphanumeric characters.
3. You have chosen the Update button, or pressed TAB to exit this field.
Procedure
Specify a P.A.N. number that consists of 10 alphanumeric characters.
10000910
Message
All mandatory fields are required
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:56 AM
Diagnosis
In the Generate Quarterly e-TDS File window, you have left at least one of the mandatory fields empty, and chosen the Generate
eTDS File button.
Procedure
In the Generate Quarterly e-TDS File window make sure to fill in all the mandatory field, and then choose the Generate eTDS File
button.
 Note
All the fields in this window are mandatory except for Location. If you leave the Location field empty, all the locations are
considered for the file.
10000911
Message
File name is too long
Diagnosis
1. In the Generate Quarterly e-TDS File window, you have chosen the Browse button and specified in the Save As window a
file name that is longer than 12 characters.
2. You have chosen the Save button.
Procedure
In the Save As window, specify a file name up to 12 characters long.
10000912
Message
Financial year cannot be removed as it is in use by other users
Diagnosis
You have attempted to delete a financial year record but failed, because the record has been referenced in other transactions, such
as has been referenced in the Acknowledgement Number window.
Procedure
Stop deleting the record.
1. Choose Administration Setup Financials TDS Financial Year Master .
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:56 AM
2. In the Financial Year Master window, right click the line of the record you want to delete, and then in the pop up window,
choose the Yes button.
3. Choose the Update button. Then you get the error message.
4. To stop deleting the record, in the Financial Year Master window, choose the Cancel button.
More Information
Defining Financial Year Master: India
10000913
Message
[Column name] is missing
Diagnosis
You have tried to update the Financial Year Master - Setup window, but you have left one or more columns empty.
Procedure
Entering data in all the columns in the Financial Year Master - Setup window is mandatory.
Specify the required values in the empty columns and choose the Update button.
More Information
Defining Financial Year Master: India
10000914
Message
Enter start dates that do not overlap with other time periods
Diagnosis
In the Financial Year Master - Setup window, you have entered a start date that overlaps another time period.
Procedure
In the Financial Year Master - Setup window, enter start dates that do not overlap with other time periods.
10000921
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:56 AM
Message
In “Start Date” column, enter date that is the first of the month
Diagnosis
In the Financial Year Master - Setup window, in the Start Date column, you have attempted to enter a date that is not the first of
the month.
Procedure
In the Start Date column, enter a date that is the first of the month.
10000927
Message
You cannot remove nature of assessee in use
Diagnosis
In the Nature of Assessee - Setup window, you have attempted to remove a nature of assessee, but this is not allowed in SAP
Business One because the nature of assessee is in use.
10000990
Message
Financial year master data not found; check definition
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the Deposit Post. Date field and chosen the OK button. But the
financial year master data was not found.
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup Financials TDS Financial Year Master .
2. In the Financial Year Master window, define the TDS posting date.
3. From the SAP Business One Main Menu, choose Financials TDS Form 16A .
4. In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
More Information
Defining Financial Year Master: India
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:56 AM
Generating Form 16A: India
10000998
Message
In “Code” column, enter code of 1–6 numerals
Diagnosis
In the Financial Year Master - Setup window, in the Code column, you have entered a code containing one of the following:
One or more nonnumeric characters
More than six numerals
Procedure
In the Financial Year Master - Setup window, in the Code column, enter a code containing 1–6 numerals.
10001042
Message
Transactions exist in database. Change of Overlook status will result in wrong calculation. Continue?
Diagnosis
The status of the fields below should not be changed if the business partner has already had transactions for TDS. Otherwise,
errors can be brought to TDS calculation.
Threshold Overlook
Surcharge Overlook
Procedure
Change the over look status at the beginning of the financial year, and make sure there is no transaction in the financial year.
1. Choose Business Partners Business Partner Master Data Accounting Tax .
2. Select or deselect the checkboxes of the Threshold Overlook and Surcharge Overlook fields.
10001043
Message
Define financial year
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:56 AM
Diagnosis
You want to create an A/P invoice with TDS while the financial year master record is not defined yet.
1. You have created an A/P invoice and specified the Invoice in the category field of the withholding tax.
2. In the A/P Invoice window, you have chosen the Add button.
Procedure
Define the financial year as follows:
1. Go to Administration Setup Financial TDS Financial Year Master .
2. Specify the fields in the window and choose the OK button.
3. Create an A/P invoice again.
More Information
Defining Financial Year Master: India
10001044
Message
TDS amount for the invoice is already deposited
Diagnosis
We recommend that you not credit or cancel an invoice if the related TDS has been deposited to authority. If you do have the need
to credit or cancel an invoice, we recommend that you make the TDS adjustment accordingly later.
10001045
Message
Accumulated amount for withholding tax has been changed
Diagnosis
You have attempted to add an A/P invoice. In case the accumulated amount for TDS that displayed in the screen is different from
the amount in database, this error occurs. It happens when several users try to add an A/P invoice with TDS at the same time.
Procedure
1. Choose Purchasing A/P A/P Invoice .
2. In the A/P Invoice window, choose withholding tax code, and choose the Add button.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:56 AM
10001081
Message
Certificate number not generated, check definition
Diagnosis
In the Form 16A Report window, you have chosen the Generate Cert. No. field and chosen the OK button.
Procedure
1. In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
2. In the Form 16A Report window, choose the Generate Cert. No. button.
More Information
Generating Form 16A: India
Form 16A Report Window: India
10001082
Message
Not all invoices are in the same financial year
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the values in the Deposit Post. Date field but the range of this
posting period belongs to different TDS financial years.
Procedure
In the Form 16A - Selection Criteria window, specify the values in the Deposit Post. Date field.
More Information
Generating Form 16A: India
10001083
Message
Acknowledgement number is not found
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:56 AM
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the fields and chosen the OK button. But the acknowledgement is
not found.
Procedure
1. In the SAP Business One Main Menu, choose Financials TDS Acknowledgement Number .
In the Acknowledgement Number window, specify the required fields.
2. In the SAP Business One Main Menu, choose Financials TDS Form 16A .
In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
More Information
Setting up Acknowledgement Number: India
Generating Form 16A: India
10001084
Message
Employee's address not defined; check master data
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the fields and chosen the OK button.
Procedure
1. In the SAP Business One Main Menu, choose Human Resources Employee Master Data .
In the Employee Master Data window, on the Address tab, define the required fields.
2. In the SAP Business One Main Menu, choose Financials TDS Form 16A .
In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
More Information
Employee Master Data
Generating Form 16A: India
10001085
Message
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:56 AM
Employee master data does not contain state information; check definition
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the fields and chosen the OK button.
Procedure
1. In the SAP Business One Main Menu, choose Human Resources Employee Master Data .
In the Employee Master Data window, on the Address tab, specify a value in the State field.
2. In the SAP Business One Main Menu, choose Financials TDS Form 16A .
In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
More Information
Employee Master Data
Generating Form 16A: India
10001086
Message
Location not found; check definition
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the Location field and chosen the OK button. But the location data
is not found.
Procedure
1. In the SAP Business One Main Menu, choose Administration Setup General States .
In the States - Setup window, define TDS locations.
2. In the SAP Business One Main Menu, choose Financials TDS Form 16A .
In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
Related Information
Generating Form 16A: India
10001088
Message
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:56 AM
Location missing
Diagnosis
In the Form 16A — Selection Criteria window, you have left the Location field empty and chosen the OK button.
Procedure
Select the required option from the menu list next to the Location field, fill in the other details and choose the OK button.
More Information
Generating Form 16A: India
10001089
Message
Deductee Type missing
Diagnosis
In the Form 16A — Selection Criteria window, you have left the Deductee Type field empty and chosen the OK button.
Procedure
Select the required option from the menu list next to the Deductee Type field, fill in the other details and choose the OK button.
More Information
Generating Form 16A: India
10001093
Message
BP's name or address not defined; check master data
Diagnosis
In the Form 16A - Selection Criteria window, you have specified the fields and chosen the OK button.
Procedure
1. From the SAP Business One Main Menu, choose Business Partners Business Partners Master Data .
In the Business Partners Master Data window, on the Address tab, specify the required fields.
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:56 AM
2. From the SAP Business One Main Menu, choose Financials TDS Form 16A .
In the Form 16A - Selection Criteria window, specify the values in the required fields, and choose the OK button.
More Information
Business Partner Master Data: Address Tab
Generating Form 16A: India
10001102
Message
No entry found
Diagnosis
You have attempted to pick the TDS entries in the TDS page of Outgoing Payments window, but after you choose the Pick TDS
Entries button, no entries are found.
Procedure
In the TDS page of Outgoing Payments window, to find appropriate TDS entries, select the following fields again:
Loc.
Section Code
Assessee Type
More Information
Outgoing Payments: TDS: India
Withholding Tax Codes - Setup Window
10001103
Message
%s is missing
Diagnosis
You have attempted to create an outgoing payments for TDS. But one or more following fields are not specified:
Challan No
Challan Date
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:56 AM
BSR Code
Bank Name
Procedure
Make sure that you have specified the values in all the fields above.
More Information
Creating Outgoing Payments: TDS: India
10001104
Message
TDS can only be paid in local currency
Diagnosis
You cannot pay TDS in foreign currency.
You have attempted to make the payment in the Payment Means window, through the Outgoing Payment: TDS window. But you
have specified a foreign currency in the Currency field.
Procedure
In the Doc. Currency field, change the foreign currency to local currency (INR) and try to pay it again.
1. From the SAP Business One Main Menu, choose Banking Outgoing Payments Outgoing Payments , and select the
TDS radio button.
2. In the Outgoing Payments window, from the Doc. Currency dropdown list, choose INR.
3. In the toolbar or in the payment, choose the icon and make the payment again.
More Information
Creating Outgoing Payments: TDS: India
Payment Means
10001105
Message
Select TDS entries in the same financial year
Diagnosis
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:56 AM
You have attempted to pick several TDS entries in the TDS Entries window. But you have selected at least two TDS entries that are
not in the same financial year.
Procedure
Deselect the entries that not in the same financial year and try again.
More Information
TDS Entries
Defining Financial Year Master
10001107
Message
Enter valid location
Diagnosis
You have attempted to add or update all the certificate series, but the location you entered is not defined yet.
Procedure
Define locations first before you specify them in the certificate series.
1. Go to Administration Setup Inventory Locations and specify the following fields:
Loc. Name
fields in General tab
fields in Accounting tab
Choose the Add button.
2. Go to Administration Setup Financials TDS Certificate Series and in the Certificate Series window, specify the
location you have defined.
3. Choose the Add or Update button.
More Information
Locations - Setup: India
Defining Certificate Series
10001108
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:56 AM
Message
Enter a valid section
Diagnosis
You have attempted to add or update a certificate series, but the section you entered has not been defined yet.
Procedure
Make sure you have defined the relevant sections before you specify them in certificate series definition.
1. Go to Administration Setup Financials TDS Sections and specify the following fields:
Code
Description
eCode
Choose the Update button.
2. Go to Administration Setup Financials TDS Certificate Series and in the Section field, enter the section you
have defined.
3. Choose the Add or Updatebutton.
More Information
Defining Sections
Defining Certificate Series
10001109
Message
Duplicated certificate serial number code
Diagnosis
You have attempted to add a certificate series, but the certificate serial number code entered is duplicated with another certificate
series. Certificate serial number code must be unique.
Procedure
1. Go to Administration Setup Financials TDS Certificate Series
2. In the Code field, specify a value.
3. Choose the Add button.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:56 AM
Defining Certificate Series: India
10001110
Message
Deletion not permitted for certificate series already in use
Diagnosis
You have attempted to delete a certificate series which it's already in use.
Procedure
If Next No. is greater than First No. that means the Certificate Series is already in use, it cannot be deleted.
1. Go to Administration Setup Financials TDS Certificate Series
2. In the Code field, specify a value.
3. Choose the Add button.
10001111
Message
Invalid certificate serial number code
Diagnosis
You have attempted to add or update a certificate series but you do not enter an valid number in the Code field.
Procedure
1. In SAP Business One Main Menu, choose Administration Setup Financials TDS Certificate Series .
2. In the Certificate Series - Setup window, specify a value in the Code field.
3. Choose the Add button.
More Information
Defining Certificate Series: India
10001113
Message
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:56 AM
Combination of section and location already exists
Diagnosis
You have attempted to add a certificate series while the combination of one section and location already existed in the system.
Procedure
1. Go to Administration Setup Financials TDS Certificate Series
2. In the Section or Location fields, select another value.
3. Choose the Add button.
10001114
Message
%s is missing!
Diagnosis
You have attempted to add a certificate series while one of the following fields is empty:
Section
First No.
Default Series
Procedure
1. In SAP Business One Main Menu, choose Administration Setup Financials TDS Certificate Series
2. Enter a value in these fields:
Section
First No.
Default Series
3. Choose the Add button.
More Information
Defining Certificate Series: India
10001115
Message
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:56 AM
Enter a valid number
Diagnosis
You have attempted to add a certificate series with the First No. field defined with characters like “1A”.
Procedure
In the First No. field, enter a valid number.
More Information
Defining Certificate Series: India
10001116
Message
First No. or Next No. cannot be greater than Last No.
Diagnosis
You have attempted to add a certificate series with the First No. or Next No. greater than Last No.
Procedure
1. Go to Administration Setup Financials TDS Certificate Series .
2. In the Certificate Series window, specify these fields:
First No.
Next No.
Last No.
3. Choose the Add button.
10001117
Message
Are you sure you want to refresh all the certificate series?
Diagnosis
You have attempted to refresh all the certificate series by going to Administration Setup Financials TDS Certificate
Series and press the Refresh button.
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:56 AM
Procedure
Refreshing all the certificate series which can result in resetting the values of all Next No. to their corresponding First No.. This
operation is not reversible. Choose OK to reset Next No., otherwise, choose Cancel.
10001144
Message
TDS amount is greater than TDS Taxable amount; this is not allowed in eTDS report. Continue?
Diagnosis
You have generated the e-TDS report for withholding tax. When withholding tax is deducted based on accumulated transactions,
and the withholding tax amount entered is larger than the taxable amount, the report is not valid and does not pass the File
Validation Utility (FVU) check.
Procedure
You need to manually adjust the report to have it pass the FVU check.
10001157
Message
Invoice/DP invoice is already deposited with authority
Diagnosis
One or more TDS entries have already been deposited in previous transactions.
1. You have created an A/P invoice, and in the WT Tax Category window, you have selected a WTax code that is defined for
TDS.
You have chosen the Add button.
2. From the SAP Business One Main Menu, you have chosen Banking Outgoing Payments Outgoing Payments , and
have selected the TDS radio button.
3. In the Outgoing Payments window, you have specified the required fields.
4. You have chosen the Pick TDS Entries button.
5. In the TDS Entries window, you have selected the invoice created in step 1 and have chosen the OK button.
6. You have selected the same invoice to deposit but you have not added it.
7. You have added the first payment and then have tried to add the second payment.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:56 AM
Change the selection criteria of TDS entries and deposit again.
More Information
Creating Outgoing Payments: TDS: India
TDS Entries: India
10001158
Message
New Credit Memo/Adjustment entries exist against the selected invoices/DP invoices. Do you want to continue?
Diagnosis
A new credit memo or TDS adjustment exists for the selected TDS entries.
You have tried to add an approved draft of an outgoing payment that was created for an A/P invoice; however, by the time you have
tried to add it, the A/P invoice had already been partially credited.
Procedure
If you continue the deposit, the application will ignore the new credit memo and/or TDS adjustment. To include the new credit
memo and/or TDS adjustment, reselect the TDS selection criteria.
More Information
Creating Outgoing Payments: TDS: India
10001369
Message
“CST Code Incoming” is a mandatory field
Diagnosis
In the Tax Codes - Setup window, you have defined a tax code, and you have chosen the Update button. However, the CST Code
Incoming field is empty.
The CST Code Incoming field is mandatory when the tax type is linked with a tax category other than ICMS.
Procedure
In the CST Code Incoming field, specify the CST code.
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:56 AM
More Information
Tax Codes - Setup Window
10001423
Message
Select 'WTax Codes Allowed' with BP's Assessee Type
Diagnosis
You have upgraded your base with TDS upgrade tool, and in SAP Business One Main Menu, choose Business Partner Master
Data Accounting Tax , the assessee types of the WTax Codes Allowed area are not consistent with business partner's
assessee types.
Procedure
1. In the Business Partner window, Accounting tab, Tax sub-tab, choose the WTax Codes Allowed button.
2. Reselect business partner's assessee types and choose the Update button.
More Information
Business Partner Master Data: Accounting Tab, Tax
10001216
Message
The combination of Financial Year, Quarter and Location should be unique
Diagnosis
You have attempted to define an acknowledgement number, but you have chosen duplicated values in the following fields:
Financial Year
Quarter
Location
Procedure
1. In the SAP Business One Main Menu, choose Financials TDS Acknowledgement Number .
2. In the Acknowledgement Number - Setup window, specify the following fields:
Financial Year
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:56 AM
Quarter
Location
More Information
Setting Up Acknowledgement Number: India
10001215
Message
Zero adjustment is not supported
Diagnosis
You have attempted to make an adjustment entry, but you have not assigned any values to the TDS components.
Procedure
1. From the SAP Business One Main Menu, choose Financials TDS Adjustment Entry .
2. Specify valid values in the following fields:
New TDS Amount
New Surcharge Amount
New Cess Amount
New HSC Amount
More Information
Processing Adjustment Entry: India
10001214
Message
Base document does not exist or is not supported
Diagnosis
You have attempted to select a transaction to make an adjustment entry, but the selected transaction ID does not exist, or the
invoice contains no withholding tax information.
Procedure
1. From the SAP Business One Main Menu, choose Financials TDS Adjustment Entry .
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:56 AM
2. In the Adjustment Entry window, from the Transaction No. dropdown list, select an invoice.
More Information
Processing Adjustment Entry: India
10001213
Message
Not all tax components contain account information
Diagnosis
You have attempted to add an adjustment entry, but the selected invoice being processed lacks one or more of the TDS
component account properties you have defined in the Withholding Tax - Setup window.
Procedure
Make sure that all four TDS components of an invoice have an account defined.
More Information
Processing Adjustment Entry: India
10001212
Message
Cannot make adjustment; check whether the document exists or contains withholding tax information
Diagnosis
You have attempted to select a transaction to make an adjustment entry, but the selected transaction ID does not exist, or the
invoice contains no withholding tax information.
Procedure
1. From the SAP Business One Main Menu, choose Financials TDS Adjustment Entry .
2. In the Adjustment Entry window, from the Transaction No. dropdown list, select an option.
More Information
Processing Adjustment Entry: India
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 7:01 AM
SAP Business One 10.0
Generated on: 2026-06-08 07:01:49 GMT+0000
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

6/8/26, 7:01 AM
Localization for Central MENA/AE/EG/LB/OM/QA/SA
This documentation describes features and functions in SAP Business One that are specific to the localization for Central
MENA/AE/EG/LB/OM/QA/SA (Middle East and North Africa: United Arab Emirates/Egypt/Lebanon/Oman/Qatar/Saudi Arabia).
Information about general features and functions that are not localization-specific is available in the online help for SAP Business
One. You can also access the online help and localization-specific information directly in SAP Business One ( Help
Documentation Online Help and Help Documentation Country/Region Specific Information ).
Setup and Administration: Central
MENA/AE/EG/LB/OM/QA/SA
This section describes the settings and definitions related to functions that are specific to Central MENA /AE/EG/LB/OM/QA/SA.
Information about settings and definitions related to general functions is available in the general online help file, under: Help
Documentation Online Help .
Company Details
Accounting Data tab
Use Deferred Tax
Select if you want to recognize tax when the payment takes place and not when the invoice is created.
Extended Tax Reporting
Generates and saves the tax report for tax authorities.
Selecting this checkbox opens the Period Type for Report Generation dropdown list.
Period Type for Report Generation
Enabled when you select the Extended Tax Reporting checkbox.
Specify the period type for the report generation.
Basic Initialization tab
Use Bill of Exchange
Select to indicate that the company uses bills of exchange (BoE). If not selected, all references to BoE in SAP Business One are
hidden. When a BoE transaction is added, Use Bill of Exchange cannot be disabled.
Tax-Related Definitions
To set tax-related definitions choose: Administration Setup Financials Tax The following settings are available:
Tax Groups
Tax Code Determination
Withholding Tax Codes
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 7:01 AM
Defining BAS Codes
Tax Declaration Boxes - Setup Window
Tax Groups - Setup Window
Use this window to define your company's tax groups.
To open this window, choose Administration Setup Financials Tax Tax Groups .
Tax Groups – Setup Window
Code, Name
Specify a code and name for the tax group.
Inactive
Select to indicate that the tax group is inactive. Once the tax group is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
Category
Select one of the two tax groups:
Output Tax – tax groups for A/R documents
Input Tax – tax groups for A/P documents
EU
Select this option if the tax group is used for transactions with European Union countries (relevant only for Output Tax groups).
Triangular Deal, Goods Shipment, Service Supply
Select Goods Shipment, Triangular Deal, or Service Supply. These three fields are mutually exclusive.
Acquisition/Reverse
This column is relevant only for Input Tax groups (A/P). Select this option to define the tax group as pertaining to Acquisition /
Reverse.
Specifying the acquisition tax is a procedure used when you record goods purchased from EU countries. Tax is not calculated in
the document, but the correct amount is recorded in the journal entry and affects the tax report. In this case, the tax amount in the
rows and in the total of the A/P invoice would be 0.
Effective from, Rate %
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can create additional entries by double-clicking the row number of
the tax group and defining them in the Tax Definition window.
 Note
The tax amounts in the documents are calculated according to the tax group's effective date.
Non Deduct. %
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 7:01 AM
The rate of tax that was paid but not allowed as a deduction. The calculation of the non-deductible amount is based on the tax
amount. Relevant only for Input tax groups (A/P).
 Example
Rate of input tax group: 16%
Rate of non-deductible: 4%.
When creating an A/P invoice for total amount of 100, the amount of total tax is 16 from which 0.64 (=4%*16) is the non-
deductible amount and 15.36 is deductible.
When using a tax group defined as non-deductible, the total amount of tax is divided between the tax account and the non-
deductible tax account.
Non Deduct. Acct
Specify the account to which you want to post the non-deductible tax amounts.
Tax Account
Specify a G/L account to use in journal entries containing this tax group.
Acquisition Tax Account
Specify a G/L account to use in journal entries containing an acquisition tax.
Deferred Tax Account
Specify the account to which you want to post deferred tax amounts.
Group Description
Use this informative field to enter values, which could be used later as parameters in user queries.
Cash Discount Account
Specify the account to which you want to post cash discount amounts.
VAT Exemption Reason
This dropdown field is based on the PEPPOL VATEX code list, and allows you to create or select a reason for VAT exemption in the
Tax Exemption Letter section under Business Partner Master Data Accounting Tax .
Tax Definition - Setup Window
Use this window to specify tax information for a specific group or code.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Groups .
Select the required tax group and choose the Tax Definition button.
Tax Definition - Setup Window
Effective From, Rate
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can specify new values.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 7:01 AM
The tax amounts in the documents are calculated according to the tax group's effective date.
Tax Code Determination
In sales and purchasing documents, you must specify a tax code for items and services that are liable for taxes. SAP Business One
proposes a tax code by default, which depends on the localization you are using.
You can set up tax code determination rules that take precedence over the tax information in the business partner or item master
data, and G/L account determination. When you create a sales or purchasing document, the application proposes a tax code for
each item line based on the rules you defined, but you can overwrite this proposal.
In tax code determination, you can do the following:
Define tax code determination rules
Update tax code determination rules
Delete tax code determination rules
Change the order of tax code determination rules
Define tax code determination rules for freight charges
For more information, see Working with Tax Code Determination Rules.
If you do not define tax code determination rules, the tax code is determined as follows:
Item type documents Service type documents
1. Default tax code in business partner master data 1. Default tax code in business partner master data
2. Default tax code in item master data 2. Default tax code in account details
3. Default tax code in freight setup 3. Default tax code in freight setup
4. Default tax code in G/L account determination 4. Default tax code in G/L account determination
Working with Tax Code Determination Rules
You define tax code determination rules to determine how the application proposes tax codes in sales and purchasing documents.
 Caution
If several superusers are connected to the same company database and add a tax code determination rule at the same position
in the hierarchy, the database may become inconsistent.
Procedure
Defining Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 7:01 AM
2. Specify at least the following mandatory data:
Document Type
Business Area
Condition
You can specify up to five conditions, for example, ship-to address, item, or user-defined field (UDF), and their values
per rule.
 Note
If you create several rules with the same conditions, the application cannot apply the rule, because it is not
unique. For example, rule 1 has the condition Ship-To Address, and rule 2 also has the condition Ship-To Address.
Value
If you do not manage freight in documents: Line Tax Code.
If you manage freight in documents: Line Freight Tax or Header Freight Tax. In this case, specifying a line tax code is
optional.
Filling in the other columns is optional. For more information, see Tax Code Determination – Setup Window.
 Recommendation
Specify the data in the order given here, that is, first the document type, then the business area, and so on.
3. If you selected UDF as a condition, the User-Defined Fields Selection window appears. In this window, select the relevant
UDF.
4. Repeat step 2 for all tax code determination rules that you want to define. Note that you can copy, cut and delete several
rows at the same time by choosing CTRL plus the relevant option from the right-click menu.
5. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
6. To confirm the change, choose Yes.
Updating Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Change the relevant data.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Deleting Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 7:01 AM
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Select the line of the rule that you want to delete, right-click, and choose Delete Row. To delete several rules at the same
time, hold the CTRL key when clicking the tax code determination rule lines.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Changing the Order of Tax Code Determination Rules
Changing the order of tax code determination rules affects the process of tax code proposals in sales and purchasing documents.
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Select the tax code determination rule that you want to move. You can move only one rule at a time.
3. Drag and drop the rule to the desired location in the hierarchy.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Defining Tax Code Determination Rules for Freight Charges
You can define tax code determination rules for freight charges only if the Manage Freight in Documents field is selected in
Administration System Initialization Document Settings .
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Specify the data as described above in Defining Tax Code Determination Rules. In addition, enter the following data:
Line Freight Tax
Header Freight Tax
3. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
4. To confirm the change, choose Yes.
More Information
Tax Code Determination
Tax Code Determination – Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 7:01 AM
Tax Code Determination - Setup Window
Use this window to define tax code determination rules, according to which the application proposes tax codes in sales and
purchasing document lines.
Tax Code Determination – Setup Window Fields
Determination Order
The position of the tax code determination rule within the hierarchy of tax code determination rules. When determining the tax
code proposal in a sales or purchasing document, the application works its way through the rules starting at the highest position.
Document Type
Specify for which type of document, for example, item, service, or both, the tax code determination rule is relevant. This field is
mandatory.
Business Area
Specify whether the tax code determination rule is relevant for sales or purchasing, or both. This field is mandatory.
Condition
Select a condition based upon which the tax code is determined. The conditions that you can select depend on the localization you
are using. You can specify up to five conditions, for example, business partner, item, ship-to address, or user-defined fields.
If you select more than one condition, all conditions must be met for the tax code determination rule to be applied.
This field is mandatory.
Value
Specify a value for the condition you selected in the Condition column. This field is mandatory.
Depending on the condition you selected, you can either select a value from a list or enter a value. The value itself also depends on
the condition selected.
 Example
Condition Value or Action
Federal Tax ID Filled-in
Empty
Business Partner Select the relevant business partner code.
Ship-to Address Select the ship-to address defined in the business partner master
data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Description
If necessary, enter an additional explanation for the tax code determination rule.
Line Tax Code
Specify the tax code that should be proposed in sales or purchasing documents, if the tax code determination rule applies. Use
one of the tax codes defined in the application or create a new one. Depending on the business area you specified, you can only
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 7:01 AM
select a tax code relevant for that business area. For example, if you selected Sales as a business area, the application only
displays sales tax codes.
In the sales or purchasing document, you can change the tax code that is proposed by the tax code determination rule.
Line Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document lines.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
Header Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document headers.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
More Information
Working with Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
When defining tax code determination rules, you specify conditions and values that must apply for the application to propose a tax
code on sales and purchasing documents. The conditions and values you can specify depend on the localization of SAP Business
One that you are using as well as on the document type and business area. The table below lists the conditions and values that are
available for the different localizations.
You can specify values by using the dropdown list or, for some values, by entering free text. For some of the conditions and values,
if you have specified them once, you can select the value that was used last for the condition from the dropdown list.
Conditions and Values for Tax Code Determination Rules
Condition Value
Federal Tax ID
Filled in: The Federal Tax ID field on the sales or purchasing
document must contain a value.
Empty: The Federal Tax ID field on the sales or purchasing
document must be empty.
Ship-To Address Choose: Select the ship-to address defined in the business partner
master data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Ship-To Street / PO Box
Choose: Select a ship-to street / PO box defined in the
business partner master data.
Filled in: The Street / PO Box field in the ship-to address of
the sales or purchasing document must contain a value.
Not defined: The Street / PO Box field in the ship-to
address of the sales or purchasing document must not
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 7:01 AM
Condition Value
contain a value.
Ship-To City
Choose: Select a ship-to city defined in the business
partner master data.
Filled in: The City field in the ship-to address of the sales or
purchasing document must contain a value.
Not defined: The City field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Zip Code
Choose: Specify a ship-to zip code.
Filled in: The Zip Code field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The Zip Code field in the ship-to address of
the sales or purchasing document must not contain a
value.
Ship-To County
Choose: Select a ship-to county defined in the business
partner master data.
Filled in: The County field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The County field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To State
Choose: Select a ship-to state defined in the application.
Filled in: The State field in the ship-to address of the sales
or purchasing document must contain a value.
Not defined: The State field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Country/Region
Choose: Select a ship-to country/region defined under
Administration Setup Business Partners
Countries/Regions .
EU: The item is shipped to a member state of the European
Union.
Non-EU: The item is shipped to a country/region outside of
the European Union.
Item Choose: Select an item code from the list.
Item Group Choose: Select an item group from the list.
Business Partner Choose: Select a business partner from the list.
Customer Group Choose: Select the customer group the customer must be
associated with from the list.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 7:01 AM
Condition Value
Vendor Group Choose: Select the vendor group the vendor must be associated
with from the list.
Warehouse
Choose: Select a warehouse that the item must be shipped
from or to.
Filled in: The Warehouse field on the sales or purchasing
document must contain a value.
Not defined: The Warehouse field on the sales or
purchasing document must not contain a value.
G/L Account Choose: Select the G/L account that must be used on the sales or
purchasing document for the rule to apply.
Tax Status
Liable: The tax status field in the business partner master
data must contain the value Liable.
Exempt: The tax status field in the business partner master
data must contain the value Exempt.
EU/Acquisition: The tax status field in the business partner
master data must contain the value EU or Acquisition.
Freight Choose: Select a type of freight from the list.
UDF Choose: Select a user-defined field that you use on the sales or
purchasing document, business partner or item master data, for
warehouses, or item groups.
More Information
Tax Code Determination
Working with Tax Code Determination Rules
Tax Code Determination - Setup Window
Example: Tax Code Determination Rules Applied on Marketing
Docs
The following examples illustrate how the tax code determination (TCD) rules are applied when you create a sales or purchasing
document.
Tax code determination rule with line and header freight tax conditions defined
TCD rule definition Master data
Line Tax Code Line Freight Tax Header Freight Tax BP Item
A1 A4 A5 A2 A3
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 7:01 AM
TCD rule definition Master data
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A4                    | A5                      |     |     |     |
Tax code determination rule without line tax code defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| Not defined   | A2               | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A2            | A2                    | A2                      |     |     |     |
Tax code determination rule with one condition for header freight
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | A5                 | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A5                      |     |     |     |
Tax code determination rule without freight tax conditions defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A2                      |     |     |     |
Tax code determination rule without freight tax conditions defined – freight tax code defined in freight setup
| TCD rule definition |     |     | Master data |     | Freight Setup |
| ------------------- | --- | --- | ----------- | --- | ------------- |
Line Tax Code Line Freight Tax Header Freight Tax BP Item Freight Tax Code
| A1  | Not defined | Not defined | Not defined | Not defined | A6  |
| --- | ----------- | ----------- | ----------- | ----------- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 7:01 AM
TCD rule definition Master data Freight Setup
Tax code proposed on document
Item Tax Code Line Freight Tax Header Freight Tax
Code Code
A1 A6 A6
More Information
Tax Code Determination
Withholding Tax Codes - Setup Window
Use this window to define withholding tax codes for your company.
To open the window, choose Administration Setup Financials Tax Withholding Tax .
Withholding Tax Codes - Setup Fields
WT Code
Specify a code for the withholding tax.
Inactive
Select to indicate the withholding tax is inactive. Once the withholding tax is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
WT Name
Enter a description for the withholding tax code.
Category
Choose one of the following from the dropdown list:
Invoice – the withholding tax calculation appears in the invoice and is recorded in the journal entry when the invoice is
added.
Payment – the withholding tax calculation appears in the invoice, but is recorded in the journal entry when it is created by
the incoming payment based on that invoice.
Effective From
Enter the date from which a tax group rate (%) is effective.
Rate
Enter the rate of tax to be calculated from the date defined in the Effective From field.
Base Type
Choose either Gross (includes VAT) or Net from the drop-down list to determine from which amount the withholding tax will be
calculated.
% Base Amount
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 7:01 AM
Specify the percentage of the base amount that is subject to withholding tax. The default value is 100%.
Official Code
Specify the official code to be reported in the withholding tax report.
Account
Choose the G/L account code to be recorded in journal entries relevant for this withholding tax code.
Withholding Tax Definition
Choose this button to open the Withholding Tax Definition - Setup: <XXX> window, in which you can define the Effective From
date and the tax percentage for the selected withholding tax code.
Minimum Taxable Amount
Specify the minimum taxable amount for the withholding tax to take effect.
More Information
Tax Definition - <XXX> Window
Defining BAS Codes
Define the BAS codes you need for your business activity statement reporting. You can add or remove BAS codes, for example if
there are any changes in tax regulations.
Procedure
Adding New BAS Codes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Specify the following data:
Code
Name
Type
Summary field
Debit/credit
Formula syntax
3. Choose the BAS Code Definitions - Rows button and set additional parameters for the BAS code.
 Note
The BAS Code Definitions - Rows button is available for BAS codes of types VAT Group, Account, and Single Choice.
4. Choose Update and OK.
Modifying BAS Codes
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 7:01 AM
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Change the data in the table, for example, the debit/credit data or the formula syntax. For more information about these
fields, see BAS Code Definitions Window.
 Note
Depending on the type of tax code, you can only change certain items of information. For account type tax codes for
example, you can only change the debit/credit information, but not the summary field. The items that you cannot
change are grayed out as inactive.
Removing BAS Codes
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax BAS Code Definitions .
The BAS Code Definitions - Setup window appears.
2. Place your cursor in a row and choose Data Remove from the menu bar.
3. Choose Update and OK.
The BAS code is removed.
More Information
Business Activity Statement Reporting
BAS Code Definitions Window
In this window, you review the BAS codes used for business activity statement (BAS) reporting, modify or remove BAS codes, or
add new ones.
To open this window, choose Administration Setup Financials Tax BAS Code Definitions .
BAS Code Definitions Window
Effective From
Enables you to set up groups of BAS codes, with each group sharing one effective period. Proceed as follows:
1. Specify the date from which the group of BAS codes you want to create is effective. From the Effective From dropdown list,
select one of the following:
01.01.1900
01.01.2024: This date is displayed by default.
Define New: If you want to specify a date other than 01.01.1990 or 01.01.2024, define a new one.
Once you define a new date, the BAS code group that has the default Effective From date 01.01.2024 is copied to
the new group.
Similarly, every time you define a new date, the existing BAS code group that has the chronologically latest Effective
From date is copied to the new group.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 7:01 AM
The chronologically later Effective From date of one BAS code group automatically becomes the "Effective To” date for
the group with the early Effective From date.
For example, you only create two groups of BAS codes, group A and group B. The Effective From dates of group A and B
are set as 01.01.2009 and 01.01.2010, respectively. Therefore, 01.01.2010 automatically becomes the ”Effective To”
date of group A, that is, the effective period of group A is from 01.01.2009 to 01.01.2010.
2. If required, define the individual BAS codes within the group you create.
For each group, you can define different numbers of BAS codes, and each BAS code within the group can have individual
settings.
Code
Code of the tax category to be used in business activity statement reporting.
Name
Description of the tax category to be used in business activity statement reporting.
Type
Indicates how tax is calculated.
VAT Group: Use this type to report, group, and filter transactions by tax codes. You can combine tax groups and/or
constants in a formula using mathematical operations.
If you include a tax group of type Acquisition/Reverse in the formula, you can define the Acquisition/Reverse Tax Type of
the tax group to report only the input tax part (debit side), the output tax part (credit side), or both the input and output tax
parts (both debit and credit sides) of the transactions. To do so, double-click the BAS code row to define the details.
Account: Use this type to report, group, and filter transactions by G/L accounts. You can assign each account to only one
BAS code. This means, after you select an account for a BAS code, it is not displayed for another code selection. We
recommend that you select the Display only accts with postings checkbox in the Select accounts for group: <group
name> window to filter unused accounts.
Manual Input: Use this type if you want to manually enter an amount or a percentage rate, for example, as an adjustment to
a BAS code, in the BAS Report - Generation window.
If you enter a percentage rate, you can use decimals. However, if you enter an amount as an adjustment to a particular BAS
code, you can use decimals only if they are allowed for this BAS code.
Manual Text Input: Use this type if you want to manually enter a text in the BAS Report - Generation window. For this type
of BAS codes, a new column Text Data is available and editable in the BAS Report - Generation window.
Formula: Use this type if you want to combine the existing BAS codes and/or constants in a formula using mathematical
operations.
When you include BAS codes in a formula, use brackets “[]”as placeholders for each BAS code.
 Note
You cannot include a BAS code of type Single Choice in a formula.
 Example
G1, G2, G3, G4, G5, G6, and G7 are BAS codes; S1 and S2 are tax groups.
Among the BAS codes, G5, G6, and G7 are of type Formula.
[G5] = [G2] + [G3] + [G4]
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 7:01 AM
[G6] = [G1] – [G5]
[G7] = [G2] /11
G1 is of type VAT Group.
[G1] = [S1]+ [S2]
Single Choice: With this type, you can provide background information or additional remarks for certain BAS codes
according to legal regulations. You can specify a few legally valid options as reason codes and select only one of them for
reporting purposes.
 Example
1. You create the following BAS codes of type Manual Input:
F1: Varied fringe benefits tax installment, FBT code
F2: Estimated total fringe benefits tax payable, FBT code
2. To provide background information for F1 and F2, you create a BAS code F3 of type Single Choice, as follows:
F3: Reason for fringe benefits tax variation, FBT code
Reason Code 01: Benefits ceased/reduced and salary increased
Reason Code 02: Benefits ceased/reduced and no compensation to employees
Reason Code 03: Fewer employees
Reason Code 04: Increase in employee contribution
...
Position in Report
Specify the target XML node name.
Summary Field
Select an option to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount
Non-Deductible Amount
Debit/Credit
Determines which parts of the transactions that are calculated are added: for example, only the debit amount, only the credit
amount, or both.
Formula Syntax
Indicates the formula syntax to calculate the tax amount.
Sort Order
Indicates the position of the tax code in the BAS statement.
Absolute Value
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 7:01 AM
Displays the absolute amount for the relevant tax code in the report.
More Information
Defining BAS Codes
Tax Declaration Boxes - Setup Window
Use this window to define selection criteria for the tax declaration boxes appearing in the tax declaration box report.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax
Declaration Boxes .
Tax Declaration Boxes - Setup Window
Effective From
Enables you to set up groups of tax declaration boxes, with each group sharing one effective period. Proceed as follows:
1. Specify the date from which the group of tax declaration boxes you want to create is effective. From the Effective From
dropdown list, select one of the following:
01.01.1900
01.01.2024: This date is displayed by default.
Define New: If you want to specify a date other than 01.01.1990 or 01.01.2024, define a new one.
Once you define a new date, the tax declaration group that has the default Effective From date 01.01.2024 is copied
to the new group.
Similarly, every time you define a new date, the existing tax declaration box group that has the chronologically latest
Effective From date is copied to the new group.
 Note
The chronologically later Effective From date of one tax declaration box group automatically becomes the "Effective To”
date for the group with the early Effective From date.
For example, you only create two groups of tax declaration boxes, group A and group B. The Effective From dates of
group A and B are set as 01.01.2009 and 01.01.2010, respectively. Therefore, 01.01.2010 automatically becomes the
”Effective To” date of group A, that is, the effective period of group A is from 01.01.2009 to 01.01.2010.
2. If required, define the individual tax declaration boxes within the group you create.
For each group, you can define different numbers of tax declaration boxes, and each tax declaration box within the group
can have individual settings.
Code, Name
Enter a code and relevant description for the box.
Inactive
Select to indicate the tax declaration box is inactive. Once the tax declaration box is set as inactive, you cannot include it in the tax
declaration box report. By default, the checkbox is not selected.
Type
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 7:01 AM
Choose one of the following options:
Vat Group – summarizes VAT groups in the box
Box – summarizes several boxes in this box
Summary Field
Choose to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount – the actual tax amount
Non-Deductible Amount
Debit/Credit
Choose one of the following options to determine what to add of the transactions that will be calculated in the box:
Debit Side – only the debit amount
Credit Side – only the credit amount
Debit Side + Credit Side – both the credit and debit amount
Formula Syntax
The calculation formula of the box (the tax groups and the relations between them). For more information on the formula, go here.
Sort Order
Define the display order of the boxes in the report by entering their successive numbers. By default, the next successive number is
entered when you update the Tax Declaration Boxes - Setup window.
Absolute Value
Displays the absolute box amount in the report.
Box Definition - Rows
Opens the Box Definition – Rows window, in which you can define a formula for the selected box.
Box Definition - Rows - Setup Window
Use this window to define formulas for selected VAT groups or boxes.
To access this window, choose Administration Setup Financials Tax Tax Declaration Boxes . Double-click the relevant
box row.
Box Definition - Rows - Setup Window
VAT Group
Click the dropdown list and select the VAT group or box to include in the box.
Formula Sign
Click the dropdown list and select the arithmetic operation (+ or -) to define the relation between this VAT group or box, and the
one below it.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 7:01 AM
Choose Update to move to the next row.
After you have finished defining all VAT groups or boxes for the formula, choose Update to save your changes.
Transfer Posting Correction Wizard
The Transfer Posting Correction Wizard enables you to post corrections resulting from VAT changes, for amounts transferred from
revenue or expense accounts to new accounts.
This wizard guides you in defining parameters required to generate these postings.
To access the wizard, from the SAP Business One Main Menu, choose Administration Utilities Transfer Posting Correction
Wizard .
 Note
Ensure that you execute the wizard only once for the selected period and the selected accounts.
 Note
All documents that you post after executing the wizard and that are valid for this period, must be transferred manually. To
transfer the posting manually, create a journal entry.
More Information
Transfer Posting Correction Wizard - Selection Criteria
Transfer Posting Correction Wizard - Transaction Selection
Transfer Posting Correction Wizard - Transaction Confirmation
Transfer Posting Correction Wizard - Summary
Transfer Posting Correction Wizard - Selection Criteria Window
Use this window to specify the selection criteria for the wizard run.
Selection Criteria Fields
Date From... To...
Specify the date range for the wizard run. By default, the transactions within the posting date range are selected.
 Caution
There should be no overlap of the date ranges specified in different wizard runs; otherwise, you could correct the same posting
twice.
Doc. Date
Selects documents within the document date range.
 Caution
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 7:01 AM
Always use the selected option during the rest of the period; otherwise, you could correct the same posting twice.
Tax Rate
Specify the tax rate of the transaction – 16% or 19% – that the wizard uses to select documents.
Code
Tax group code
Name
Tax group name
Display
Deselect the tax group that you do not need in the wizard run.
 Note
Only those tax groups with the tax rate of 16% or 19% are valid for the wizard.
G/L Accounts
Limits the selection to specific G/L accounts only. Click to open the Accounts - Selection Criteria window where you can
select the needed G/L accounts.
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard: Transaction Selection
Window
Use this window to select the transactions that you want to include in the wizard run.
 Recommendation
After selecting the needed transactions, you should print the screen or export it to Excel; you may use it for future verification.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Selection Fields
App
Select the posting that you want to correct
G/L Account
The revenue or expense account relevant to a transaction
Tax Code
The tax group code associated with a transaction
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 7:01 AM
Tax %
The tax rate that was effective for the tax code at the time the transaction was posted
Doc. No.
The document number in SAP Business One
Debit, Credit (FC, SC)
The debit or credit tax amount (in terms of foreign currency or system currency)
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard: Transac. Confirmation
Window
Use this window to confirm the amount, accounts, and tax codes for which correction posting will be created.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Confirmation Fields
Interim Account
Specify the clearing account to be used during the correction posting process.
Expense Account
Specify the account to which the expense is posted.
Revenue Account
Specify the account to which the revenue is posted.
Input Tax Group
Specify the input tax group to be used in the correction posting.
Non-Deductible Tax Group
Specify the non-deductible tax group to be used in the correction posting.
Output Tax Group
Specify the output tax group to be used in the correction posting.
Deferred Tax Group (Input)
Specify the tax code which belongs to the input tax group and has a deferred tax account defined in the Tax Groups – Setup
window.
Deferred Tax Group (Output)
Specify the tax code which belongs to the output tax group and has a deferred tax account defined in the List of Tax Definitions
window.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 7:01 AM
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard - Summary Window
In this window, you can see how many journal entries have been made during the correction process. The number appearing is
twice the number of the corrected transactions because it includes the entries on both the debit and credit sides.
You can view the transactions created by the wizard in the Journal Entry window of the Financials module.
More Information
Transfer Posting Correction Wizard
Folio Number Assignment
Use this function to create legal documents such as invoices and credit memos that include the fiscal document number known as
Folio.
When a company is set up for Chile in Company Details and when printing marketing documents, the settings Obtain Printer
Settings from Default Printing Layout in Document Printing - Selection Criteria and Folio Number Assignment - Selection
Criteria are ignored for the last pages of marketing documents. This ensures that the correct folio number is assigned for
marketing documents during printing and that the folio number of the first page and last page is the same, no matter how many
rows exist in marketing documents.
Documents created with a Folio number have two numbers:
The internal number defined in document numbering (see Administration System Initialization Document
Numbering )
The Folio number that you can define using this function or when you create the document.
 Note
Only documents without folio numbers can be canceled. On the other hand, you cannot assign folio numbers to already
canceled documents and corresponding cancellation documents.
Prerequisites
You have selected the Use Folio Number checkbox on the Basic Initialization tab at Administration System Initialization
Company Details .
More Information
Assigning Folio Numbers
Checking Folio Numbering
Folio Number Assignment - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 7:01 AM
Folio Number Assignment: Printed Document Selection
Folio Number Assignment: Folio Number Determination
Assigning Folio Numbers
SAP Business One offers several ways of assigning folio numbers to documents, as described in the table below. If the Folio
Number field is editable in a document, you can take the first and fourth approaches; otherwise, you can take the second, third,
and fourth approaches.
Activities
Activity Procedure
Specifying Folio Number Directly in the Document
1. Display the document to which you want to assign a folio
number.
2. In the header area, enter the folio prefix and number in the
Folio Number field.
3. Choose the Update pushbutton.
Assigning Folio Number for One Document While Printing
1. Display the document to which you want to assign a folio
number.
2. To print the document, choose File Print .
The Print – Document window appears.
3. Select a printer and choose Print.
4. To assign a folio number in the Print – Document window,
choose OK.
If this is the first time you are printing a document of this
type, enter a folio prefix and a number to initialize a series
for this type of document. For example, IN – 000001 for
an A/R invoice. If you have already printed documents of
this type, you can no longer change the folio prefix.
The Folio Number Confirmation window appears, in which
you can confirm the folio number after you have checked
whether your printout was successful. If the printout was
not successful, for example, due to a paper jam, assign a
folio number at a later stage. For more information, see
Assigning Folio Numbers After Documents Are Printed.
5. If the printout was successful, make sure that the number
and prefix are correct and choose OK.
Assigning Folio Number for Many Documents During Printing
1. Choose Sales – A/R Document Printing . Make the
required selection in the Document Printing – Selection
Criteria window and choose OK
2. In the Print Documents window, select the documents you
wish to print and the first folio that will be used. Then
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 7:01 AM
Activity Procedure
choose Print.
3. Select the printing format for the documents.
The Folio Number Confirmation – Printed Document
Selection window appears.
4. Select the documents you wish to print and choose Next.
5. The Folio Number Confirmation – Folio Number
Determination window displays the selected documents
and their folio numbers assigned by SAP Business One. Edit
the folio numbers if required and choose Finish.
Assigning Folio Numbers After Documents Are Printed
1. Choose Sales – A/R Folio Number Assignment or
Purchasing – A/P Folio Number Assignment .
2. Make the required selection in the Folio Number
Assignment – Selection Criteria window and choose OK.
The window Folio Number Assignment – Printed
Document Selection appears. This window displays only
documents that have already printed but have no folio
numbers.
3. Select the documents for which you assign folio numbers
and choose Next.
4. The Folio Number Assignment – Folio Number
Determination window displays the selected documents
and their folio numbers assigned by SAP Business One. Edit
the folio numbers if required and choose Finish.
More Information
Document Printing - Selection Criteria
Print Document Window
Folio Number Confirmation: Printed Document Selection
Folio Number Confirmation - Folio Number Determination
Checking Folio Numbering
Prerequisites
Folio numbering has been activated.
Context
You can review which folio numbers have already been used and which numbers are still available.
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 7:01 AM
Procedure
1. From the SAP Business One Main Menu, choose Administration Utilities Check Folio Numbering .
2. In the Check Folio Numbering window, select the folio numbering range, the date, and the document types you want to
review.
The Document Serial Numbering List window displays the folio numbers per document type that have not been assigned
yet.
Related Information
Folio Number Assignment
Check Folio Numbering
You are enabled to check whether there are duplicated or missing folio numbers for documents created in SAP Business One.
Use the Check Folio Numbering window to define selection criteria for the check. If there are no duplicated or missing folio
numbers, a relevant message appears. If there are missing or duplicated numbers, they are displayed in a separate window.
To display this window, choose Administration Utilities Check Folio Numbering .
Check Folio Numbering Fields
Documents to Review
Select each document type for which you want to run the check.
Folio Number From... To
Define a range of folio numbers to be checked.
Date From... To
Define a range of posting dates to run the check on the documents carrying a posting date within that range.
Select All
Runs the check on all documents with folio numbers.
Clear Selection
Deselects all checkboxes.
Folio Number Assignment - Selection Criteria
Use this window to define the parameters for the documents to which you want to assign folio numbers.
Folio Number Assignment
Document Type
Specify the type of the document to which you want to assign a folio number.
Series
Specify an internal numbering series of the documents to which you want to assign Folio numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 7:01 AM
When Batch/Serial No. Exist, Print
Specify what you want to print on the document, when it contains a batch or serial number.
Posting Date From...To
Enter a range of posting dates for the documents to which you want to assign folio numbers.
Internal Number From...To
Enter a range of internal numbers for the documents to which you want to assign folio numbers.
Update Folio
Not selected by default. Documents are selected to update folio numbers.
Select Unprinted Documents
Not selected by default. Only available for selection if Update Folio is selected. When both Update Folio and Select Unprinted
Documents are selected, all (printed and not printed) marketing documents with relevant dates, series, and internal numbers are
displayed in folio number assignment.
More Information
Folio Number Assignment
Folio Number Assignment: Printed Document Selection
This window displays the documents to which folio numbers should be assigned and match the selection criteria you specified.
Printed Document Selection
Selection Column
Select the documents to which you want to assign folio numbers.
Document No., Posting Date, Due Date, BP Code, Total (LC)
General information regarding the documents that match the selection criteria you specified.
More Information
Folio Number Assignment
Folio Number Assignment: Folio Number Determination
This window displays all documents you select in the Folio Number Assignment - Printed Document Selection window.
Folio Number Determination Fields
Document No., Posting Date, Due Date, BP Code, Total (LC)
General information regarding the selected documents. You cannot edit these fields.
Folio Prefix, Folio Number
Enter the Folio Prefix and Folio Number.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 7:01 AM
More Information
Folio Number Assignment
Folio Number Confirmation: Folio Number Determination
This window displays all documents selected in the Folio Number Confirmation - Printed Document Selection window, with the
folio numbers assigned to them by SAP Business One.
Change the folio numbers if required.
Folio Number Determination
Document No., Folio Prefix, Folio Number, Posting Date, Value Date, BP Code, Total (LC)
Display general information regarding the selected documents. The values – except for the Folio Prefix and Folio Number – cannot
be edited.
Folio Number Confirmation: Printed Document Selection
This window displays the documents for which folio numbers should be assigned and fit the selection criteria.
Printed Document Selection Fields
Selection Column
Select the documents to which you want to assign folio numbers.
Document No., Posting Date, Value Date, BP Code, Total (LC)
Display general information regarding the documents that fit the selection criteria made by the user.
More Information
Folio Number Assignment
Banking
This section describes the features and functions under the Banking module that are specific to Turkey only.
Information about general features and functions in the Banking module is available in the general online help file provided with
SAP Business One, under Help Documentation Online Help
Postdated Check Deposit
Use this function to transfer to the cash account checks that were deposited as postdated.
To deposit postdated checks, choose Banking Deposits Postdated Check Deposit .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 7:01 AM
Postdated Checks Deposit Window
Depositing Postdated Checks
Procedure
1. Choose Banking Deposits Postdated Check Deposit .
2. In the general area of the window, fill in the fields so that the table displays the checks you want to deposit.
3. Specify the account to which the amount of the selected postdated checks should be transferred.
 Note
Only checks deposited as postdated checks in the Deposit window can be deposited from the Postdated Check Deposit
window.
4. Select the checks to be deposited.
5. To record the deposit in the database, choose Add.
Results
A journal entry transferring the deposited checks from the postdated checks account to the cash checks account is created. The
status of the checks is updated from Deposited as Deferred to Deposited as Cash.
Postdated Check Deposit Window
To open the Postdated Check Deposit window, choose Banking Deposits Postdated Check Deposit .
Postdated Check Deposit Window
Key
Successive number, starting from 1, for each postdated check deposit document.
Deposit Currency
To display only checks created with one currency, specify this currency. If you choose a foreign currency, a field displaying the
exchange rate appears. You can change the exchange rate if required.
Bank Account
Specify the account code to which the checks should be transferred.
Date
Due date of the checks. This is the current date by default. Change the date if required.
Display Until
Specify a date to display all checks that have reached their value date by this date.
Find Check No.
To trace a specific check, specify its number. SAP Business One marks the required check.
Date, Account Code, Check, Bank, Branch, Acct No., BP/Account Code, BP/Account Name, Check Amount, Incoming Payment
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 7:01 AM
Information about the postdated checks.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
Total for Deposit
Total amount of all checks selected for deposit.
No. of Checks
Number of checks selected for deposit.
Remarks
Remarks about this document.
Reconcile Amounts After Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Check Deposit
Postdated Credit Voucher Deposit
Use this function to transfer to the cash account credit card vouchers deposited to the deferred account.
To deposit postdated credit card vouchers, choose Banking Deposits Postdated Credit Voucher Deposit .
More Information
Postdated Credit Voucher Deposit Window
Depositing Postdated Credit Card Vouchers
Depositing Postdated Credit Vouchers
Context
Follow this procedure to deposit vouchers that were deposited as postdated to the cash account credit card.
Procedure
1. Choose Banking Deposits Postdated Credit Voucher Deposit .
2. In the general area of the window, specify the relevant parameters to display in the table the credit card vouchers to be
deposited.
3. Select the credit card vouchers you want to deposit.
4. If a commission is involved in the deposit, choose next to Total Commissions.
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 7:01 AM
5. In the Commission window, specify the commission details and choose Update.
6. To record the deposit in the database, choose Add.
Results
A journal entry that transfers the postdated credit card vouchers from the deferred account to the cash account is created. If the
deposit involves a commission, this is reflected in the journal entry.
Related Information
Postdated Credit Voucher Deposit Window
Postdated Credit Voucher Deposit Window
To open the Postdated Credit Voucher Deposit window, choose Banking Deposits Postdated Credit Voucher Deposit .
Postdated Credit Voucher Deposit Window
Key No.
Successive number, starting from 1, for each deposit of a postdated credit card voucher or postdated check.
Deposit Currency
To display credit card vouchers created with a particular currency, specify this currency.
No. of Vouchers
Number of vouchers selected for deposit.
Display Until
To display all credit card vouchers that have reached their value date by a certain date, specify this date.
Date
By default, the current date. You can change this date if necessary.
Find Voucher No
To find a credit card voucher by its number, sort the Doc. No. column and then specify the required number here. SAP Business
One places this voucher at the beginning of the list.
Date, Acct Code, Doc. No., Card Name, Ref., Payment Method, BP/Account Code, BP/Account Name, # Pymts, of, Total,
Incoming Payment
Information about the postdated credit card vouchers displayed.
Journal Remarks
Add any comments about the deposit.
Trans. No.
Number of the journal entry created by this document and a link to it. The number appears after you have added the document.
Total Commissions
Opens the Commission window where you can enter the amount of commission to be paid for the deposit.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 7:01 AM
Reconcile Amounts after Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Credit Vouchers Deposit
Commission Window
Setting Up Bill of Exchange Processing
Context
To activate bill of exchange processing in your company database, follow the steps below:
 Note
You cannot deactivate bill of exchange processing after you have recorded bill of exchange transactions.
Procedure
1. On the Company Details: Basic Initialization tab, select the Use Bill of Exchange checkbox.
2. On the Document Settings: Per Document tab, in the Document field, select Deposit from the dropdown list. Select the Bill
of Exchange Deposit checkbox if you want to split the business partner row in journal entries created by depositing several
bills of exchange in one deposit.
3. On the G/L Account Determination: Sales tab, click next to the Accounts Receivable field to open the Control
Accounts - Accounts Receivable window. Select the default controls accounts for your customers and choose the OK
button
4. On the G/L Account Determination: Purchasing tab, click next to the Accounts Payable field to open the Control
Accounts - Accounts Payable window. Select the default controls accounts for your vendors and choose the OK button
 Note
The control accounts you have defined in the G/L Account Determination window are set as the default for each
new business partner.
Purchasing control accounts should be located in the Liabilities drawer in the Chart of Accounts, and sales
control accounts should be located in the Assets drawer.
Bill of exchange related control accounts function as clearing accounts.
5. In the House Banks Accounts - Setup window, define bill of exchange related parameters.
6. In the Payment Methods - Setup window, define bill of exchange related parameters.
7. In the Business Partner Master Data Window, define bill of exchange related parameters:
On the General tab, in the Agent field, enter the agent code of the business partner. An agent is an employee in your
company who is responsible for bills of exchange (relevant only for Spain and Portugal).
On the Payment Terms tab, enter the bank account details of your business partners.
On the Accounting tab, General tab, click to open the Control Accounts window displaying the default control
accounts. You can change these G/L accounts manually if no journal entry has yet been created with these control
accounts for the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 7:01 AM
Results
After you have defined all the necessary settings, you can start processing bills of exchange.
Bill of Exchange Settings
The following fields are relevant for setting up and working with bill if exchange functionality.
Business Partner Master Data Accounting Tab, General
Bill of Exchange Discounted
Specify a G/L account for bill of exchange discounted.
Bill of Exchange on Collection
Specify a G/L account for bill of exchange collection.
Unpaid Bill of Exchange
Specify a G/L account for unpaid bill of exchange.
Bill of Exchange Presentation
Relevant for customers and leads only.
Bank Statement Processing
Working with bank statement processing requires defining internal bank operation codes (as well as additional settings). One of
the related parameters is “Posting Transaction”. The complete information about defining internal bank operation codes in
available in the general online help delivered with SAP Business One. Following bill of exchange specific information related to the
Posting Transaction field in the Internal Bank Operation Codes window.
“Posting Transaction ” is used as one of the criteria to define which transaction should be posted when identified by this internal
code. The specified posting transaction defines the available posting methods for the internal operation code. If the company uses
bills of exchange and a payment means, the following options are available in this field:
Incoming Bill of Exchange
Outgoing Bill of Exchange
They indicate that the internal code refers to transactions resulting either from receiving or from issuing bills of exchange. In both
cases, the applicable posting methods are Bank Interim Account from/to Bank Account and Ignore.
Working with Bills of Exchange
In SAP Business One, your company settings enable use of bills of exchange. A bill of exchange is a means of payment you can use
in incoming and outgoing payments. It is a document addressed by the vendor to the customer requiring the latter to pay a certain
amount on the due date.
A customer buys goods or services and agrees with the vendor that the payment method will be a bill of exchange. On the due
date, the vendor claims payment from the customer or asks the bank to claim it. If the customer pays, the process is completed. If
not, the bank informs the vendor, and the vendor duns the customer.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 7:01 AM
The bill of exchange is supported by the payment wizard.
Bills of exchange are reflected in various reports:
Cash Flow
Cash Flow Forecast Dashboard
To access bill of exchange-related functions, choose Banking Bill of Exchange .
More Information
Managing Bills of Exchange
Managing Bills of Exchange
Since paying or collecting bills of exchange is a process which requires several stages, you need to monitor and record the changes
made for each one of your incoming and outgoing bills of exchange.
After you set the required initial definitions, you can start working with the Bill of Exchange function:
You can monitor and record most bill of exchange-related activities in the Bill of Exchange Management window. This
window is designed as a chest of drawers, where each drawer represents a different bill of exchange status. You can take
required actions such as changing the bill of exchange status, defining bank data, setting posting and tax dates, and so on.
To access the Bill of Exchange Management window, choose Banking Bill of Exchange Bill of Exchange
Management . In the Bill of Exchange Management:— Selection Criteria window, specify your selection criteria and
choose the OK button.
Every change you make in one of your bills of exchange is recorded in the Bill of Exchange Transactions window. This
window is displayed automatically as you change a bill of exchange status.
To access the Bill of Exchange Transactions window, choose Banking Bill of Exchange Bill of Exchange Transactions
You can display and print your bills of exchange using the Bill of Exchange - Payables and Bill of Exchange - Receivables
windows. This function is required for sending a bill of exchange to be signed and approved by your customer, prior to you
depositing it in your bank.
To access the Bill of Exchange - Payables window, choose Banking Bill of Exchange Bill of Exchange — Payables
To access the Bill of Exchange - Receivables window, choose Banking Bill of Exchange Bill of Exchange —
Receivables
You can display data and history for each bill of exchange using the Bill of Exchange Register window.
To access the Bill of Exchange Register window, choose Banking Bill of Exchange Bill of Exchange Register .
Bill of Exchange Management: Selection Window
The following are the fields in the selection window of the Bill of Exchange Management function.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management .
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 7:01 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Management: Selection Window
Doc. Type
Specify whether to display bills of exchange created from incoming or outgoing payments.
Status
Specify a specific status to display only bills of exchange to which the selected status has been assigned.
Bill of Exchange No. From...To...
Specify a bills of exchange range according to their number.
Due Date From...To...
Specify a bills of exchange range according to their due date.
Reference No. From...To...
Specify a bills of exchange range according to their reference number.
Payment No. From.. To...
Specify a bills of exchange range according to the number of the payment documents linked to them.
Payment Posting Date From...To...
Specify a bills of exchange range according to the posing date of their linked payments.
BP Bank Code From... To...
Define the range of bills of exchange according to the bank code of their linked business partners. This field is displayed only when
the status Generated is selected.
Deposit No. From...To
Specify a bills of exchange range according to the numbers of their linked deposit documents. Only available with the status
Deposited or Paid.
Deposit Bank Acct No. From...To...
Specify range of bank account numbers to display only bills of exchange deposited to these accounts.
Deposit Type
Select to display bills of exchange according to their deposit type. Only available with the status Deposited or Paid.
Reconciled Only
Select to display only bills of exchange that are reconciled. Only available with the status Deposited or Paid.
Add Tolerance Days
Takes into account both the tolerance days defined in the House Bank Accounts – Definitions window and the defined value date
range. Only available with the status Deposited or Paid.
Payment Methods
All payment methods whose payment means are defined as bill of exchange. Select the payment methods to include in the Bill of
Exchange Management window.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 7:01 AM
More Information
Bill of Exchange Management
Bill of Exchange Management Window
The following are the fields in the Bill of Exchange Management window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management . Set the required parameters in the
selection window and choose OK.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Management Window
Sent, Generated, Deposited, Paid, Cancelled, Failed
Represents the statuses a bill of exchange can have:
When you select Incoming Payment as document type in the selection criteria, all the drawers appear.
When you select Outgoing Payment, only the following drawers appear:
Generated
Paid
Cancelled
Find Bill of Exchange No.
Specify a number to locate a bill of exchange by it.
Status
Groups the bills of exchange according to the statuses assigned to them. Only available if you selected the status All in the
selection criteria window.
Selection Column
Select the bills of exchange you want to process. Only available with one of the following statuses/drawers:
Sent
Generated
Deposited
Paid.
Due Date
Due date of the bill of exchange.
Posting Date
Posting date of the incoming/outgoing payment document.
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 7:01 AM
Bill of Exchange Total (LC)
Total amount paid by the bill of exchange - in local currency.
Remarks
Remarks as specified in the bill of exchange.
Reference No.
Reference number assigned to the bill of exchange in the Payment Means window.
Expand, Collapse
Expands or collapses the entire display of the window. Only available if you selected the status All in the selection criteria window.
Move To
Only available with the statuses/drawers, Sent, Generated, Deposited, and Paid. Specify how to process the selected bills of
exchange. The options available depend on the selected drawer:
Drawer - Sent:
Generated transfers the bill of exchange to the Generated drawer.
Cancelled cancels the bill of exchange and transfers it to the Cancelled drawer.
Drawer - Generated:
Deposited creates deposit documents for bills of exchange created from incoming payments.
Paid indicates that the amounts in the bills of exchange created from outgoing payments were transferred from
your account to the vendor’s account.
Cancelled cancels the bill of exchange and transfers it to the Cancelled drawer.
Drawer - Deposited:
Paid transfers the bills of exchange to the Paid drawer. Shows that the bill of exchange amount was transferred to
your bank account.
Generated cancels the deposit and transfers bills of exchange back to the Generated drawer.
 Note
You can only transfer back bills of exchange that have not been reconciled.
Drawer - Paid:
Deposited transfers the bills of exchange to the Deposit drawer. Cancels the indication that the bill of exchange
amounts were received at your bank account. Available only for incoming payments.
Failed cancels the incoming payment and transfers the bills of exchange to the Failed drawer.
Generated reverses the payment transaction and transfers the bills of exchange created by outgoing payments
back to the Generated drawer.
Posting Date, Document Date
By default, the current date. Available only with the drawers Sent, Generated, Deposited or Paid.
House Bank Country/Region, House Bank, House Bank Account, House Bank Branch
Only available when the Generated drawer is selected for incoming payments.
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 7:01 AM
Choose to open the Choose Bank window, in which you select the bank account for the bill of exchange transaction. The details
of the selected bank account are then displayed in the respective house bank fields.
Collection
Indicates that the bank collects the bill of exchange on its due date. Available only when the Generated drawer is selected for
incoming payments.
Discounted
Creates the deposit before the due date of the bill of exchange. Available only when the Generated drawer is selected for incoming
payments.
Norm
Specify the deposit norm number, which will be displayed in the OPEX file. Available only when the Generated drawer is selected
for incoming payments.
More Information
Bill of Exchange Management
Deposited - Details
Use this window to view additional details of selected deposited bills of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange Management Bill of Exchange Management ,
select and double-click the table row labeled Deposited.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Bank
Code, Name, Account Number, Branch, Control Key, Country/Region
Displays details of bank account in which bill of exchange was deposited.
Deposit
Type
Displays the type of deposit:
Collection – when the bank collects the Bill of Exchange on its due date.
Discounted – when you make an advanced deposit, that is, if you make a deposit before the due date of the bill of exchange.
Number
Displays deposit number from the Deposit window, general area.
Bill of Exchange
Number
Displays bill of exchange number from the Bill of Exchange — Receivables window.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 7:01 AM
Due Date
Displays bill of exchange due date from the Bill of Exchange — Receivables window.
Amount
Displays amount of the selected bill of exchange.
More Information
Bill of Exchange - Receivables
Bill of Exchange Transactions
This window appears each time you record transactions in the Bill of Exchange Management window. It displays the details
concerning the transactions you have just recorded.
To open the window, choose Banking Bill of Exchange Bill of Exchange Transactions .
More Information
Bill of Exchange Transactions Window
Bill of Exchange Transactions Window
Use this window to display information about transactions comprising the bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange Transactions .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Transactions Window
Transaction Number
Number of this transaction. Begins at 1 and runs sequentially.
Journal Entry No.
Number of the journal entry created by the transaction. A link to the journal entry is available for the following transactions:
Changing status from Generated to Deposited
Reconciliation
Changing status from Deposited to Paid
Changing status from Paid to Deposited
Status Changed From...To...
Previous and current status of the bill of exchange.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 7:01 AM
User Name
User who recorded the transaction.
Action
Action performed on the bill of exchange: status change or reconciliation.
Reference No.
Reference for the bill of exchange.
Due Date
Due date of the bill of exchange.
Posting Date
Posting date of the payment document.
Document Date
Document date for tax purposes.
Bill of Exchange Total
Total amount of the bill of exchange.
BP Bank Country/Region, BP Bank Code, BP Bank Name, BP Bank Account, BP Bank Branch
Bank details of the business partner linked to the bill of exchange.
BP Bank Control Key
Control key defined for the business partner’s bank account.
Remarks
Remarks for the bill of exchange.
Payment Method Code, Payment Method Description
Code and description of the payment method linked to the bill of exchange.
More Information
Bill of Exchange Transactions
Bill of Exchange - Receivables
When you create an incoming payment with bill of exchange as the payment means, a bill of exchange record is created. Use the
Bill of Exchange - Receivables window to view these records.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables .
More Information
Bill of Exchange – Receivables Window
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 7:01 AM
Bill of Exchange - Receivables Window
This window provides receivables information pertaining to a bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange – Receivables Window
Received from
Code and name of the customer who sent the bill of exchange.
Address
Pay to address specified in the Incoming Payment document.
Number
Number of the bill of exchange.
Reference
Reference for the bill of exchange and a link to the relevant incoming payment document.
Status
Current status of this bill of exchange.
Signature
User code of the person who recorded the bill of exchange.
Bill of Exchange - History
Opens the Bill of Exchange – History window with the historical statuses of the current bill of exchange and a link to each
transaction.
Remarks
Remarks in the A/R invoices paid by this bill of exchange (assuming the payment was based on an A/R invoice).
Total, Amount in Words
Total amount paid in this bill of exchange, the figure and in words.
Bank Account
Customer’s bank details linked to the bill of exchange.
Journal Remarks
Specify any comments regarding the journal entry posted by this bill of exchange.
More Information
Bill of Exchange - Receivables
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 7:01 AM
Bill of Exchange - History
Use this window to view historical transactions of each bill of exchange receivables/payables.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables/Payables . Display the required bill
of exchange. Choose Bill of Exchange – History.
More Information
Bill of Exchange - History Window
Bill of Exchange - History Window
The following are the fields in the Bill of Exchange – History window.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Receivables/Payables . Display the required bill
of exchange. Choose Bill of Exchange – History.
Bill of Exchange – History Window
Bill of Exchange No.
Number of the bill of exchange for which the transaction history is provided.
Reference No.
Reference assigned to the bill of exchange in the Payment Means window.
Transaction No.
Sequential number of the transaction. For a detailed view, choose .
Changed to Status
Status of the bill of exchange after the transaction was performed.
Date
Creation date of the transaction.
More Information
Bill of Exchange - History
Bill of Exchange - Payables
When you create an outgoing payment with bill of exchange as the payment means, a bill of exchange record is created. Use the
Bill of Exchange – Payables window to view these records.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Payables .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 7:01 AM
Bill of Exchange – Payables Window
Bill of Exchange - Payables Window
This window provides payables information pertaining to a bill of exchange.
To open the window, choose Banking Bill of Exchange Bill of Exchange – Payables .
Bill of Exchange – Payables Window
To Order of
Code and name of the vendor who received the bill of exchange.
Address
Address specified in the Pay to field in the Outgoing Payment.
Number
Number of the bill of exchange.
Reference
Reference for the bill of exchange and a link to the outgoing payment document.
Posting Date
Posting date of the bill of exchange.
Due Date
Due date of the bill of exchange.
Status
Current status of this bill of exchange.
Signature
User code of the person who recorded the bill of exchange.
Bill of Exchange - History
Opens the Bill of Exchange – History window, with all the historical statuses of the current bill of exchange and a link to each
transaction.
Remarks
Remarks entered in the incoming payment document.
 Example
Invoice number.
Total
Amount paid in this bill of exchange.
Amount in Words
Amount paid in this bill of exchange – in words.
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 7:01 AM
Country/Region, Bank, Account, Branch, Control Key
Details of the house bank linked to the bill of exchange.
Journal Remarks
Specify any comments regarding the journal entry posted by this bill of exchange.
More Information
Bill of Exchange - Payables
Bill of Exchange Register
SAP Business One uses the bill of exchange register to store information about all bills of exchange received and issued by the
company. The register reflects the current status of every bill of exchange and provides information regarding status history.
To access the bill of exchange register, choose Banking Incoming Payments Bill of Exchange Bill of Exchange Register
.
More Information
Bill of Exchange Register - Selection Criteria
Bill of Exchange Register Window
Bill of Exchange Register - Selection Criteria
The following are the fields in the Bill of Exchange Register – Selection Criteria window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Register .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Doc. Type
Select the bill of exchange type to display.
Status From...To...
Specify a range of statuses for the bills of exchange. The statuses available depend on the type of document selected:
With incoming payments: Sent, Generated, Deposited, Paid, Cancelled and Failed
With outgoing payments: Generated, Paid, Cancelled
Bill of Exchange No. From...To...
Specify a bills of exchange range according to their sequential numbers.
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 7:01 AM
Due Date From...To...
Specify a bills of exchange range according to their value dates.
Reference No. From...To...
Specify a bills of exchange range according to their reference numbers.
Payment No. From...To...
Specify a payment documents range for which you want to display the related bills of exchange.
Payment Posting Date From...To...
Specify a bills of exchange range according to the posting dates of the payment documents.
Deposit No. From...To...
Specify a bills of exchange range according to their deposit numbers.
Deposit Type
Specify to display bills of exchange according to their deposit type.
Reconciled Only
Displays only reconciled bills of exchange.
Payment Method
To display bills of exchange linked to specific payment methods, select the relevant payment methods.
More Information
Bill of Exchange Register
Bill of Exchange Register Window
Bill of Exchange Register Window
The following are the fields in the Bill of Exchange Register window.
To open the window, choose Banking Bill of Exchange Bill of Exchange Register . Specify the required parameters in the
Bill of Exchange Register – Selection Criteria window and choose OK.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Bill of Exchange Register Window
Number
Enter the number of a bill of exchange to view the details about this bill of exchange.
Currency
To display bills of exchange created for a specific currency, specify the relevant currency.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 7:01 AM
Status
To display only bills of exchange with a specific status, specify the relevant status.
Reference No.
Reference number of the bill of exchange.
Date
Due date of the bill of exchange.
Bank, Branch, Account No.
Bank details for the bill of exchange (house bank for outgoing payments, customer bank for incoming payments).
Status
Current status of the bill of exchange.
Amount
Amount of the bill of exchange.
Deposit
Details of the deposit, if the selected bill of exchange was deposited.
Deposit No. – number assigned to the deposit.
Deposit Date – deposit date.
G/L Account/BP Code – G/L account code or business partner code to which the bill of exchange was deposited.
Bank Country/Region, Bank, Branch, Account No. – information about the customer’s bank.
Payment
Details of the incoming/outgoing payment document linked to the selected bill of exchange:
Incoming/Outgoing Payment No. – number of the payment document.
Date – posting date of the document.
Customer/Vendor Code – code of the customer/vendor for which the payment was created.
Bill of Exchange Status
Displays the status history of the selected bill of exchange (one row for each status):
Bill of Exchange Trans. No. – number of the bill of exchange transaction and a link to it.
Bill of Exchange Status – status to which the bill of exchange was changed.
Date – date of the transaction.
More Information
Bill of Exchange Register
Bill of Exchange Register – Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 7:01 AM
Canceling a Bill of Exchange
You can cancel a bill of exchange that was received as an incoming payment but has not yet been deposited, or has been deposited
as postdated. To view the status of a bill of exchange, select the bill of exchange in the Bill of Exchange Register window, and view
the Status field.
Process
In the Bill of Exchange Management window, select the checkbox in the table row of the bill of exchange that you want to cancel,
then in the Move To dropdown list, select Canceled.
Result
The bill of exchange is transferred to the Canceled drawer in the Bill of Exchange Management window.
The incoming payment is canceled.
The A/R Invoice can be paid by other payment means.
A reverse journal entry is recorded.
Deposit: Bill of Exchange Tab
The Bill of Exchange tab in the Deposit window is available for deposit documents created for bills of exchange using the Bill of
Exchange Management window.
To view details on deposited bills of exchange, choose Banking Deposits Deposit . Then, select a deposit created for a bill of
exchange.
Deposit: Bill of Exchange Fields
Norm
Norm number of the deposit as defined in the Generated drawer in the Bill of Exchange Management window.
Collection/Discounted
Selection made in the Generated drawer in the Bill of Exchange Management window.
Due Date, Bill of Exchange, Bank, Branch, Account No., Customer Code, Amount
Information about the deposited bills of exchange. The total amount of the deposited bills of exchange is displayed in the row
below the table.
Payment Means: Bill of Exchange Tab
To access the Bill of Exchange tab in the Payment Means window, choose Banking Incoming Payments Incoming
Payments . Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment,
choose . In the Payment Means window, choose the Bill of Exchange tab.
Payment Means: Bill of Exchange Tab Fields
Bill of Exchange Accounts Receivables
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 7:01 AM
Account debited when the incoming payment is added. This account is defined in Administration Setup Financials G/L
Account Determination Sales General Accounts Receivable Control Accounts - Accounts Receivable .
Bill of Exchange Accounts Payable
Account credited when the outgoing payment is added. This account is defined in Administration Setup Financials G/L
Account Determination Purchase General Accounts Payable Control Accounts - Accounts Receivable .
Bill of Exchange No.
For incoming payment documents:
Unique number of the incoming payment, which can be changed if required. Two bills of exchange cannot be assigned to the same
number.
Bill of Exchange No. (op)
For outgoing payment documents:
Unique number of the outgoing payment, which can be changed if required. Two bills of exchange cannot be assigned to the same
number.
Bill of Exchange Due Date
For incoming payment documents:
Specify the date on which the bill of exchange is due.
If the payment is based on one or more A/R invoices with the same due date, the default due date is the due date of the
A/R invoice(s).
If the payment is based on several A/R invoices with different due dates, enter a due date manually.
 Note
After the bill of exchange is recorded, you can still change its due date. The updated due date will appear in the following places:
Due Date column in the table area of the corresponding journal entry
Due Date field in the general area of the payment
Due Date column for this bill of exchange in the Bill of Exchange Management window
Due Date column for this bill of exchange in the Cash Flow window
Bill of Exchange Due Date
For outgoing payment documents:
Specify the date on which the bill of exchange is due.
If the payment is based on one or more A/P invoices with the same due date, the default due date is the due date of the
A/P invoice(s).
If the payment is based on several A/P invoices with different due dates, enter a due date manually.
 Note
After the bill of exchange is recorded, you can still change its due date. The updated due date will appear in the following places:
Due Date column in the table area of the corresponding journal entry
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 7:01 AM
Due Date field in the general area of the payment
Due Date column for this bill of exchange in the Bill of Exchange Management window
Due Date column for this bill of exchange in the Cash Flow window
Reference
For incoming payment documents:
If the customer created the bill of exchange, specify its number here.
Reference (op)
For outgoing payment documents:
If the vendor creates the bill of exchange, specify its number here.
Payment Method
Specify the required payment method for the bill of exchange.
Status
When you choose the payment method, the status changes to Generated. This means that a journal entry for the payment will be
recorded and the invoice will be considered as paid (closed).
Reference 2
If another reference number exists, specify it here.
Remarks
Enter any remarks here.
BP Bank Data
Business partner bank details for the selected method of payment, showing the bank account to be credited at the end of the
process. You can change this bank account.
Total
Total amount paid in this bill of exchange.
Tax Reports: Central MENA/AE/EG/LB/OM/QA/SA
Following is information about tax reports required in Central MENA /AE/EG/LB/OM/QA/SA and additional information related to
tax handling in SAP Business One:
Tax Report
Withholding Tax Report
Tax Reconciliation Report
Tax Declaration Box Report
Business Activity Statement Reporting
Tax Report
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 7:01 AM
Use this report to display documents and manual journal entries that include tax amounts sorted by tax code. Tax reports can be
produced in an electronic format by choosing an electronic reporting option in Output Mode. The report includes the following
documents:
A/R and A/P invoices and credit memos
Inventory transfer documents – The inventory transfer transactions are displayed only in order to report the transactions in
the report because the tax percentage is 0.
Manual journal entries
Incoming payments and payments to vendors that are not based on invoices
Incoming payments and payments to vendors that include cash discounts
 Note
When printing the report, you can print the selection criteria on a separate page.
Use this window to specify selection criteria for the Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report . Alternatively, open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Selection Criteria Name
Criteria by which the report is created. Choose for a list of existing selection criteria, or press CTRL + A and specify new
selection criteria.
Date From...To..
Choose whether to generate the report according to Posting Date or Document Date or VAT Date or System Date, and specify the
date range for the report.
 Example
A/R invoice no. 15 was created with a posting date 25.3.19 and a document date 1.4.19. Generating the report according to
Posting Date and defining the date range as 1.1.19 – 31.3.19, includes A/R invoice no. 15 in the report. However, generating the
report according to Document Date and defining the same date range of 1.1.19 – 31.3.19, excludes A/R invoice no. 15, as the
Document Date assigned to it is not in the range.
Round Amount
Rounds the total amounts calculated in the report.
Series
Generates the report for documents created according to specific numbering series. After selecting, choose the ... button to open
the Series – Filter window in which you can define the required numbering series.
Transact.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 7:01 AM
Generates a report for specific document types.
After selecting, choose the ... button to open the Document Type window in which you can define the document types to include in
the report.
Output
This table displays all the tax groups defined as output tax groups ( Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report
- to change the order of the tax groups, highlight a group and click the arrows to position it
Input
This table displays all the tax groups defined as input tax groups (see Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report.
Button Up and Button Down - to change the order of the tax groups, highlight a group and click the arrows to position it.
Display Credit Memos in a Separate Column
The credit memos that were based on invoices from previous periods (previous to the range of dates defined in the Selection
Criteria window) appear in a separate section, at the end of the report.
Hide Tax Codes without Transactions
Excludes from the report those tax codes with no transactions related during the defined period.
Output Mode
Choose the type of report that you want to produce. You can choose an electronic tax report output here.
Only Display Documents with Externally Calculated Sales Tax
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Only includes in the report documents with an externally calculated tax amount on at least one row.
 Note
If you select this checkbox, the Externally Calculated Tax field is displayed in the tax report window.
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 7:01 AM
Update/ OK
When you change the preferences in the Tax Report – Selection Criteria window, the OK option changes to the Update mode.
Choose Update to save the report under the name you entered in the Report Name field.
The preferences chosen for the report are saved.
Tax Report Window
This window displays the tax report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report Window: Europe
Tax Code
Displays the tax code.
Choose to display a list of transactions involving this tax code.
EU
Indicates whether the tax group is used for transactions with other European Union countries, as defined in the EU field of the
Define Tax Groups window. Relevant only for output tax groups.
Tax %
Displays the tax rate of the tax group as a percentage.
Posting Date
Displays the posting date of the documents included in the report. Appears in expanded display only.
Document Date
Displays the document date defined for the document or transaction.
Base Amount
Total amount of the document, excluding tax; serves as the base value for the tax calculation.
Tax Amount
Tax amount calculated for the tax group: Total Tax field minus Non-Deductible field.
Total Tax
Displays the total amount of tax.
Non-Deductible
The tax amount that cannot be deducted.
Vendor Ref. No.
Displays the vendor’s reference number as recorded in the A/P invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 7:01 AM
Tax Report - Declaration
The following table describes the fields appearing in the Tax Report - Declaration window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Tax Declaration
option, set the other required parameters in the Tax Report - Selection Criteria window, then choose OK. Alternatively, open it
from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report - Declaration
Tax Code
Displays the code and the tax codes selected for the report.
Choose the icon to display a list of transactions involving that tax code.
EU
Indicates whether the tax code is EU relevant.
Tax %
Displays the tax rate as a percentage, as defined for the tax code.
Doc. No.
Displays the internal number of the document and its type. For example A/P invoice number 110007 is displayed as PU 110007.
Posting Date
Displays the posting date of the documents. If the Tax Date option is selected in the Selection Criteria window, this column
displays the tax date of the documents.
Base Amount
Total amount of the document before taxes, summarized for each tax code.
Tax Amount
Tax amount calculated for the tax group: Total Tax field minus Non Deductible field.
Total Tax
Displays the amount of the tax.
Non Deductible
The amount which cannot be deducted.
Account
Displays the control account in which the journal entry of the document is posted.
Vendor Ref. No.
Displays the vendor’s reference number from the document, if defined.
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 7:01 AM
Error Report
Choose to display error messages regarding the displayed report.
More Information
Tax Report
Tax Report - Register Book
The following table describes the fields appear in the Tax Report - Register Book window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Register Book
option and set the other required parameters in the Tax Report - Selection Criteria window, and then choose OK. Alternatively,
open it from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Register Book
Reg. No.
Displays the successive number of the records, beginning with the value defined in the Selection Criteria window.
Date
Displays either the posting date of the documents, or, if the Tax Date option is selected in the Selection Criteria window, the tax
date.
Doc. No.
Displays the internal number of the document and its type. For example, A/P invoice number 110007 is displayed as PU 110007.
Base Amount
Total amount of the document before taxes.
Tax %
The tax rate defined for the tax code, as a percentage.
Tax
Displays the amount of the tax in the document.
Non-Deductible
The amount of the non-deductible tax in the document, calculated according to the tax code definition.
Total Amount (LC)
Displays the total amount of the document in local currency.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 7:01 AM
Tax Report
Withholding Tax Report
This report displays the withholding tax amounts collected and paid during specific periods.
 Note
If a payment on account with withholding tax has been fully reconciled (that is, the reconciled amount equals the payment
amount), the withholding tax report does not include the payment information.
 Note
When you print the report, you can print the selection criteria on a separate page.
More Information
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner
Vendor Mode – Detailed Format Window
Withholding Tax Report by WTax Code
Withholding Tax Report - Selection Criteria
Use this window to specify selection criteria for the Withholding Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Withholding Tax Report. Alternatively,
open it from the Reports module.
New requirements for the Tax Summary Report and layouts are occasionally introduced by the authorities for different taxation
periods. Variations in selection criteria may exist for different taxation periods which result in different outputs.
After defining the report, you can view it in the Withholding Tax Report by Business Partner Window or the Withholding Tax Report
by WTax Code Window.
Selection Criteria
Selection Criteria Name
Specify the previously saved selection criteria you want to apply for the report, or press CTRL + A to specify new ones.
Date From...To...
Choose whether to include documents based on document date or posting date and specify the date range of the current year.
Declared Period
Specify the required declaration period.
Declaration Type
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 7:01 AM
Specify the type of declaration:
Original: The report includes all documents within the specified date range. When you approve the report, these documents
will be marked as printed.
Substitute: The report includes all documents within the specified date range, including documents already marked.
Complementary: The report includes only unmarked documents within the specified date range.
Vendors
Opens the Vendor Selection window, where you can select the vendors to include in the report.
Customers
Opens the Customer Selection window, where you can choose the customers to include in the report.
Doc. Type
Opens the Document Type window, where you can select the documents to include in the report.
Withholding Tax
Codes and names of all tax codes relevant for the report. Deselect tax codes that should be excluded.
 Note
To clear the entire column, click the column header.
To display subtotals for tax codes, select the relevant tax codes in the Amount column.
[Arrow Up/Down]
Determines the order of appearance of the tax codes in the report display and print layout.
Output Mode
Choose the required layout of the report.
The following display the report related to purchasing documents:
WTax Code Layout-Purchasing: grouped by tax codes
Vendor Layout-Purchasing: grouped by vendors
The following display the report related to sales documents:
WTax Code Layout-Sales: grouped by tax codes
Customer Layout-Sales: grouped by customers
Exceptional Event
Exceptional Event options are available for Withholding Tax Reports.
Save
Saves your selection criteria for future use.
Withholding Tax Report by Business Partner Window
This window displays the withholding tax report by business partners according to your defined selection criteria.
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 7:01 AM
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Report by Business Partner Window Fields
#
Double-click a row to open the Vendor Mode – Detailed Format window for detailed information about the relevant business
partner, grouped by document numbers.
BP Name
Displays the name of the business partner. Choose the icon to open the Business Partner Master Data window.
Federal Tax ID
Displays the federal tax ID of the business partner.
Document Amount
Displays the total document amount of the business partner.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Subject Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 7:01 AM
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
Vendor Mode - Detailed Format Window
Withholding Tax Table
Vendor Mode - Detailed Format Window
This window displays detailed information about the relevant business partner, grouped by document numbers.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Vendor Mode – Detailed Format Window Fields
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Example
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see the Transaction
Type Abbreviation Legend page in the general online help.
Date
Displays the posting date of the reconciled transaction or payment.
WTax Code, WTax %, Official Code
Displays the code, rate, and official code of the withholding tax that is included in the reconciled transaction or payment.
Invoice Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 7:01 AM
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Date
Displays the posting date of the payment.
Non-Subject Amount
Displays the following result: the base amount - the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
More Information
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner Window
Withholding Tax Table
Withholding Tax Report by WTax Code Window
This window displays the withholding tax report by withholding tax codes according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 7:01 AM
Withholding Tax Report by WTax Code Window Fields
WTax Code, WTax Name, WTax %
Displays the code, name, and rate of the withholding tax defined in the Withholding Tax Codes – Setup window according to your
selection criteria.
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Note
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see Transaction Type
Abbreviations Legend in the general online help, under: Help Documentation Online Help .
Document Date
Displays the posting date of the document.
Payment Date
Displays the posting date of the payment.
Document Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Sbj. Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 7:01 AM
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
Withholding Tax Table
Withholding Tax Table
This window appears when you create a document related to withholding tax-liable business partners. The window displays the
default ITW and VATW codes.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Table Fields
Code, Name
Code and name of the withholding tax codes defined as defaults for the business partner.
You can change these codes and choose any code that appears in the income tax withholding codes and in the VAT withholding
codes.
Type
Displays whether the WT code is an income tax withholding or VAT withholding.
Rate
Tax rate in percents.
Base Amount
Base amount of the document for tax calculation, depending on the base type defined for the WT code.
Taxable Amount
Amount of the document that is subject to tax. You can change this amount if required.
WTax Amount
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 7:01 AM
Tax amount calculated; editable value.
Category
Displays whether the tax code is related to the invoice category or the payment category.
Base Type
Base type of the WT code:
Net: Amount before taxes
VAT: Uses the VAT amount as the base amount
Criteria
Displays the selections made in the business partner master data.
Account
G/L account in which the journal entry for the tax is recorded.
More Information
Withholding Tax Codes – Setup Window
Tax Reconciliation Report
This report enables you to track the tax amounts that were posted in sales and purchasing documents and in manual transactions.
The report displays the G/L accounts involved in these transactions and calculates the tax amounts that should have been paid,
based on the tax codes defined for each transaction.
The report covers the following transactions:
A/P and A/R invoices
A/P and A/R credit memos
Manual journal entries
A/P and A/R down payment invoices
Incoming and outgoing payments
 Note
When saving a journal entry, if you deselect the Automatic Tax option in the Journal Entry window, you cannot view the journal
entry in this report.
 Note
When printing the report, you can print the selection criteria on a separate page.
 Note
Accounts are only displayed when there is at least one posting with a VAT code on the accounts within the respective period.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 7:01 AM
More Information
Tax Reconciliation Report - Selection Criteria
Accounts - Selection Criteria
Tax Report - Reconciliation Window
Tax Reconciliation Report - Selection Criteria
Use this window to specify selection criteria for the Tax Reconciliation report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Reconciliation Report . Alternatively,
open it from the Reports module.
After creating the report, you can view it in the Tax Report - Reconciliation window.
 Note
Only G/L accounts that have VAT transaction postings are considered in this report. Accounts are only subsequently displayed
in the report when there is at least one posting with a VAT code on the accounts within the respective period.
Selection Criteria
Selection Criteria Name
Click to select previously saved report selection criteria and use them to generate the report.
To save new selection criteria, press CTRL + A and enter a name in this field.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting Data tab of the Company
Details window Administration System Initialization Company Details ).
Opening Balance, Non-VAT Transactions
The report displays transactions grouped by G/L accounts and divided by tax codes, including non-tax transactions. This display
lets you crosscheck between the tax report, tax and tax based account balances, and the balance of the connected G/L account in
the system.
In addition, the report displays the opening balance of the specified tax based accounts, additional non-tax transactions that were
posted to this account, the document date, and the journal amount.
Select the Non-VAT Transactions checkbox to include the non-VAT transactions posted to the relevant G/L accounts in the report.
Date From...To
Define a date range for the report. By default, these fields display the start and end dates of the current fiscal year.
Document Date
Generates the report according to document, not posting date.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 7:01 AM
Round Amount
Report rounds off its amounts.
Series
Choose to select the series, for example, products, services, regions or brands, to include in the report.
Doc. Type
Choose to select the types of documents to include in the report.
Output
Codes and names of all the tax codes defined as output tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
Use the Amount column to select the tax codes for which you want to display subtotals.
Input
Codes and names of all the tax codes that are defined as input tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
Use the Amount column to select the tax codes for which you want to display subtotals.
[Arrow Up/Down]
Use these buttons to determine the appearance order of the selected tax codes in the report display and in the printed report.
G/L Accounts
Choose to open the Accounts – Selection Criteria window, in which you choose the G/L accounts to include in the report.
Save
Choose to save your report selection criteria for future use.
Related Information
Accounts - Selection Criteria
Accounts - Selection Criteria
Use this window to specify selection criteria for the current report.
To open this window, choose the button in the G/L Accounts field, in the Selection Criteria window of the relevant report.
Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 7:01 AM
Find
Opens the G/L Accounts window for selecting the G/L accounts to be displayed in the report. Selected accounts are marked with
an X.
Level
Choose the Level of the account display in the table.
Choosing Level 1 displays the highest level titles for the accounts. When you select a row in the table, you select all the accounts
that appear under this title.
Level
This column shows which accounts or titles have been selected.
If a row is marked with X, the specific account or group of accounts appears in the report.
To select an account, click in the selected row.
To cancel a selection, clear its X.
To clear all selections/select all accounts in the table, click the X in the column header.
Account
This column displays the codes and names of the accounts.
To view details of each account, use the arrow that appears next to the code and name.
More Information
Tax Reconciliation Report
Tax Report - Reconciliation Window
This window displays the Tax Reconciliation report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Reconciliation Window
#
Choose to expand or collapse the display of each account.
Tax Code
Displays the tax codes involved in the transactions included in the report, for each G/L account.
Click to display a list of the transactions involving that tax code.
Tax %
Displays the tax rate of the tax code.
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 7:01 AM
Posting Date
Displays the posting date of the document/journal entry.
If Tax Date is selected in the Selection Criteria window, this column displays the tax date of the document/journal entry.
Tax Base Amount
Displays the amount that is the basis for the tax calculation and was posted to the G/L account.
Tax Amount
Tax amount calculated for the report.
Deferred Tax Document
Indicates whether the document contains deferred tax.
Tax Declaration Box Report
This tax report should be generated monthly or quarterly. It includes transactions that involve tax and pertain to tax codes. The
following documents and transactions are covered in the report:
A/R and A/P invoices
A/R and A/P credit memos
Incoming payments and outgoing payments
Manual journal entries
Down payments
 Note
When printing the report, you can print the selection criteria on a separate page.
More Information
Tax Declaration Box Report - Selection Criteria
Tax Report - Declaration Window
Tax Declaration Box - Selection Criteria
Use this window to specify selection criteria for the Tax Declaration Box report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Declaration Box Report . Alternatively,
open it from the Reports module.
After creating the report you can view it in the Tax Report-Declaration window.
Selection Criteria
Selection Criteria Name
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 7:01 AM
Click to select previously saved report selection criteria and use them to generate the report. To save new selection criteria,
press CTRL + A and enter a name.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting tab of the Company
Details window ( Administration System Initialization Company Details ).
Adjustment
Select the adjusted version of a report.
Date From... To
Specify a range of posting dates or document dates or VAT dates or system dates to include specific transactions in the report. By
default, the From and To fields display the start and end dates of the current fiscal year.
If the specified From date falls into the effective period range of a tax declaration box group, all the tax declaration boxes within
this group are automatically displayed in the Tax Declaration Boxes table. For more information about the effective period of a tax
declaration box group, see the Effective From field in Tax Declaration Boxes - Setup window.
Round Amount
Report rounds off its displayed amounts.
Tax Declaration Boxes
This table displays the tax declaration boxes according to the specified From date. It includes the following columns:
Code – displays the code of the box
Name – displays the name of the box
Opening Balance - you can manually enter the opening balance relevant for each box
Display – all the checkboxes in this column are selected by default. Deselect the checkboxes of the boxes you want to
exclude from the report.
Save
Choose to save the Report Selection Criteria for future use.
More Information
Tax Declaration Box Report
Tax Report - Declaration Window
This window displays the Tax Declaration Box report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 7:01 AM
Tax Report – Declaration Window
Box Code
Displays the box code and a drill-down option to display the tax group or boxes that are combined to calculate the value for this
box.
Box Component Code
Displays the code of the component included in the box, and provides a drill-down icon that enables you to display the tax codes
included in each component.
Tax Code
This column displays tax codes only in expanded view mode.
Use the drill-down icon next to the tax code to display a list of documents which use that tax code.
Tax %
Displays the rate of each tax group.
Posting Date
Displays the posting date of each document.
Doc. Date
Displays the document date of each document.
VAT Date
Displays the VAT date of each document.
Credit Amount, Debit Amount
In a collapsed view mode, the credit column displays the cumulative amounts of both the credit and debit sides. A negative amount
indicates a greater debit side, and vice versa.
In an expanded view mode, these columns display the credit or debit amounts per row in the transaction created by each
document.
Summary Field
Displays the summary criteria defined in the Define Tax Declaration Box window.
Debit/Credit
Displays the choice made in the Credit/Debit column of the Define Tax Declaration Box window.
More Information
Tax Declaration Box Report
Business Activity Statement Reporting
Business activity statement (BAS) reporting is used by businesses in different countries for various purposes.
Usually, BAS reporting is done on a monthly, quarterly, or annual basis. However, it is also possible to report transactions, the dates
of which are beyond the range of the reported month, quarter, or year.
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 7:01 AM
Prerequisites
Initializing the BAS Reporting Function
To initialize the BAS reporting function, you have done the following:
1. You have selected the Extended Tax Reporting checkbox in Administration System Initialization Company Details
Accounting Data .
2. You have defined the period type for BAS reporting at the same location.
More Information
Defining BAS Codes
Generating BAS Reports
Retrieving BAS Reports and Saving Report Data
Generating BAS Reports
Procedure
1. Choose Financials Financial Reports Accounting Tax BAS Report Generation .
The BAS Report Generation - Selection Criteria window appears.
2. Specify the tax declaration type:
Original: To save the report for the first time in a given period.
Replacement: To correct a report that has already been saved.
Adjusted: To show only documents that have not yet been included in any previous report for a given period.
3. Specify the tax declaration name by selecting the appropriate year and period. For a replacement declaration, also select
the desired adjustment number.
4. Choose the date and date range according to which transactions should be included in the report, and choose OK.
The BAS Report - Generation window appears.
5. In this window, select the documents and transactions that you want to include in the report. The documents and
transactions are grouped by BAS code. You can change the values in the report for manual BAS codes and select one option
from “Single Choice” type codes.
6. To save the report, choose Add and OK.
Related Information
Business Activity Statement Reporting
Retrieving BAS Reports and Saving Report Data
Prerequisites
You have generated the BAS report for the desired reporting period.
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 7:01 AM
Context
You can retrieve BAS reports for review and, depending on the localization, save the report data to be submitted to the tax
authorities.
To retrieve and save the BAS reports, use the BAS report retrieval function. Proceed as follows:
Procedure
1. From the SAP Business One Main Menu, choose Financials Financial Reports Accounting Tax BAS Report
Retrieval .
The BAS Report Retrieval - Selection Criteria window appears.
2. Select the tax declaration name and the BAS codes you want to display, and choose OK.
The BAS Report - Retrieval window appears. It shows all documents included in the report, grouped by BAS code. To
display the individual transactions, click the down arrow for a BAS Code or choose Expand to display all documents.
3. To export the BAS amounts, choose Export. The BAS Report Export window appears. It displays the BAS codes and the
corresponding tax amount.
4. To export the values to Microsoft Excel, choose File Export MS-EXCEL . You can then open the file in Microsoft
Excel, fill in the electronic or paper form of the business activity statement and submit it to the tax authorities.
Related Information
Business Activity Statement Reporting
Generating BAS Reports
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:57 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:57:22 GMT+0000
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

6/8/26, 6:57 AM
Localization for Singapore
This documentation describes features and functions in SAP Business One that are specific to the localization for Singapore.
Information about general features and functions that are not localization-specific is available in the online help for SAP Business
One. You can also access the online help and localization-specific information directly in SAP Business One ( Help
Documentation Online Help and Help Documentation Country/Region Specific Information ).
Setup and Administration: Singapore
This section describes the settings and definitions related to functions that are specific to Singapore. Information about settings
and definitions related to general functions is available in the general online help file, under: Help Documentation Online
Help .
Company Details: Accounting Data Tab
Extended Tax Reporting
Generates and saves the tax report for tax authorities.
Selecting this checkbox opens the Period Type for Report Generation dropdown list.
Period Type for Report Generation
Enabled when you select the Extended Tax Reporting checkbox.
Specify the period type for the report generation.
G/L Account Determination
Checks Received
The G/L account defined in the Checks Received field on the G/L Account Determination Sales General sub-tab is set as
the default G/L account when creating incoming payment with bank transfer as the payment means.
Stock in Transit Account
Define a G/L account in the Stock in Transit Account field on the G/L Account Determination Inventory tab so that you can
copy an A/P reserve invoice to an A/P credit note.
Warehouses - Setup
Stock In Transit Account
The G/L account defined in the Stock In Transit Account field on the Warehouses - Setup Accounting tab is set as the
default G/L account when creating A/P Reserved Invoice.
This account is also displayed in the warehouses table on the Item Master Data Inventory Data tab.
Item Groups - Setup
Stock In Transit Account
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:57 AM
The G/L account defined in the Stock In Transit Account field on the Item Groups - Setup Accounting tab is set as the
default G/L account when creating A/P Reserved Invoice.
Document Numbering
Using the Manual option for assigning document number manually requires full authorization for Document Manual Numbering in
Administration System Initialization Authorizations General Authorizations .
Tax Groups - Setup Window
Use this window to define your company's tax groups.
To open this window, choose Administration Setup Financials Tax Tax Groups .
Tax Groups – Setup Window
Code, Name
Specify a code and name for the tax group.
Inactive
Select to indicate that the tax group is inactive. Once the tax group is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
Category
Select one of the two tax groups:
Output Tax – tax groups for A/R documents
Input Tax – tax groups for A/P documents
EU
Select this option if the tax group is used for transactions with European Union countries (relevant only for Output Tax groups).
Triangular Deal, Goods Shipment, Service Supply
Select Goods Shipment, Triangular Deal, or Service Supply. These three fields are mutually exclusive.
Acquisition/Reverse
This column is relevant only for Input Tax groups (A/P). Select this option to define the tax group as pertaining to Acquisition /
Reverse.
Specifying the acquisition tax is a procedure used when you record goods purchased from EU countries. Tax is not calculated in
the document, but the correct amount is recorded in the journal entry and affects the tax report. In this case, the tax amount in the
rows and in the total of the A/P invoice would be 0.
Effective from, Rate %
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
Since the tax percentage may change from time to time, you can create additional entries by double-clicking the row number of
the tax group and defining them in the Tax Definition window.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:57 AM
The tax amounts in the documents are calculated according to the tax group's effective date.
Non Deduct. %
The rate of tax that was paid but not allowed as a deduction. The calculation of the non-deductible amount is based on the tax
amount. Relevant only for Input tax groups (A/P).
 Example
Rate of input tax group: 16%
Rate of non-deductible: 4%.
When creating an A/P invoice for total amount of 100, the amount of total tax is 16 from which 0.64 (=4%*16) is the non-
deductible amount and 15.36 is deductible.
When using a tax group defined as non-deductible, the total amount of tax is divided between the tax account and the non-
deductible tax account.
Non Deduct. Acct
Specify the account to which you want to post the non-deductible tax amounts.
Tax Account
Specify a G/L account to use in journal entries containing this tax group.
Acquisition Tax Account
Specify a G/L account to use in journal entries containing an acquisition tax.
Deferred Tax Account
Specify the account to which you want to post deferred tax amounts.
Group Description
Use this informative field to enter values, which could be used later as parameters in user queries.
Cash Discount Account
Specify the account to which you want to post cash discount amounts.
VAT Exemption Reason
This dropdown field is based on the PEPPOL VATEX code list, and allows you to create or select a reason for VAT exemption in the
Tax Exemption Letter section under Business Partner Master Data Accounting Tax .
Tax Definition - Setup Window
Use this window to specify tax information for a specific group or code.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Groups .
Select the required tax group and choose the Tax Definition button.
Tax Definition - Setup Window
Effective From, Rate
The values displayed in these columns represent the date from which a tax group rate (%) is effective.
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:57 AM
Since the tax percentage may change from time to time, you can specify new values.
 Note
The tax amounts in the documents are calculated according to the tax group's effective date.
Tax Code Determination
In sales and purchasing documents, you must specify a tax code for items and services that are liable for taxes. SAP Business One
proposes a tax code by default, which depends on the localization you are using.
You can set up tax code determination rules that take precedence over the tax information in the business partner or item master
data, and G/L account determination. When you create a sales or purchasing document, the application proposes a tax code for
each item line based on the rules you defined, but you can overwrite this proposal.
In tax code determination, you can do the following:
Define tax code determination rules
Update tax code determination rules
Delete tax code determination rules
Change the order of tax code determination rules
Define tax code determination rules for freight charges
For more information, see Working with Tax Code Determination Rules.
If you do not define tax code determination rules, the tax code is determined as follows:
Item type documents Service type documents
1. Default tax code in business partner master data 1. Default tax code in business partner master data
2. Default tax code in item master data 2. Default tax code in account details
3. Default tax code in freight setup 3. Default tax code in freight setup
4. Default tax code in G/L account determination 4. Default tax code in G/L account determination
Working with Tax Code Determination Rules
You define tax code determination rules to determine how the application proposes tax codes in sales and purchasing documents.
 Caution
If several superusers are connected to the same company database and add a tax code determination rule at the same position
in the hierarchy, the database may become inconsistent.
Procedure
Defining Tax Code Determination Rules
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:57 AM
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Specify at least the following mandatory data:
Document Type
Business Area
Condition
You can specify up to five conditions, for example, ship-to address, item, or user-defined field (UDF), and their values
per rule.
 Note
If you create several rules with the same conditions, the application cannot apply the rule, because it is not
unique. For example, rule 1 has the condition Ship-To Address, and rule 2 also has the condition Ship-To Address.
Value
If you do not manage freight in documents: Line Tax Code.
If you manage freight in documents: Line Freight Tax or Header Freight Tax. In this case, specifying a line tax code is
optional.
Filling in the other columns is optional. For more information, see Tax Code Determination – Setup Window.
 Recommendation
Specify the data in the order given here, that is, first the document type, then the business area, and so on.
3. If you selected UDF as a condition, the User-Defined Fields Selection window appears. In this window, select the relevant
UDF.
4. Repeat step 2 for all tax code determination rules that you want to define. Note that you can copy, cut and delete several
rows at the same time by choosing CTRL plus the relevant option from the right-click menu.
5. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
6. To confirm the change, choose Yes.
Updating Tax Code Determination Rules
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Change the relevant data.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Deleting Tax Code Determination Rules
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:57 AM
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Go to the tax code determination rule you want to change. You can search for a rule by entering a search term (wild cards
are supported) in the search field and choosing the Find button. To go back to the full list, choose Show All.
3. Select the line of the rule that you want to delete, right-click, and choose Delete Row. To delete several rules at the same
time, hold the CTRL key when clicking the tax code determination rule lines.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Changing the Order of Tax Code Determination Rules
Changing the order of tax code determination rules affects the process of tax code proposals in sales and purchasing documents.
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Select the tax code determination rule that you want to move. You can move only one rule at a time.
3. Drag and drop the rule to the desired location in the hierarchy.
4. To save the change, choose Update and OK.
The application displays a system message asking you to confirm the change.
5. To confirm the change, choose Yes.
Defining Tax Code Determination Rules for Freight Charges
You can define tax code determination rules for freight charges only if the Manage Freight in Documents field is selected in
Administration System Initialization Document Settings .
1. From the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax Code Determination .
The Tax Code Determination Rule Setup window appears.
2. Specify the data as described above in Defining Tax Code Determination Rules. In addition, enter the following data:
Line Freight Tax
Header Freight Tax
3. To save your data, choose Update and OK.
The application displays a system message asking you to confirm the change.
4. To confirm the change, choose Yes.
More Information
Tax Code Determination
Tax Code Determination – Setup Window
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:57 AM
Tax Code Determination - Setup Window
Use this window to define tax code determination rules, according to which the application proposes tax codes in sales and
purchasing document lines.
Tax Code Determination – Setup Window Fields
Determination Order
The position of the tax code determination rule within the hierarchy of tax code determination rules. When determining the tax
code proposal in a sales or purchasing document, the application works its way through the rules starting at the highest position.
Document Type
Specify for which type of document, for example, item, service, or both, the tax code determination rule is relevant. This field is
mandatory.
Business Area
Specify whether the tax code determination rule is relevant for sales or purchasing, or both. This field is mandatory.
Condition
Select a condition based upon which the tax code is determined. The conditions that you can select depend on the localization you
are using. You can specify up to five conditions, for example, business partner, item, ship-to address, or user-defined fields.
If you select more than one condition, all conditions must be met for the tax code determination rule to be applied.
This field is mandatory.
Value
Specify a value for the condition you selected in the Condition column. This field is mandatory.
Depending on the condition you selected, you can either select a value from a list or enter a value. The value itself also depends on
the condition selected.
 Example
Condition Value or Action
Federal Tax ID Filled-in
Empty
Business Partner Select the relevant business partner code.
Ship-to Address Select the ship-to address defined in the business partner master
data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Description
If necessary, enter an additional explanation for the tax code determination rule.
Line Tax Code
Specify the tax code that should be proposed in sales or purchasing documents, if the tax code determination rule applies. Use
one of the tax codes defined in the application or create a new one. Depending on the business area you specified, you can only
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:57 AM
select a tax code relevant for that business area. For example, if you selected Sales as a business area, the application only
displays sales tax codes.
In the sales or purchasing document, you can change the tax code that is proposed by the tax code determination rule.
Line Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document lines.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
Header Freight Tax
Specify the tax code that should be proposed for freight charges in sales or purchasing document headers.
This field is only available if you have selected Manage Freight in Documents on the General tab of the Document Settings
window ( Administration System Initialization Document Settings ).
More Information
Working with Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
Conditions and Values in Tax Code Determination Rules
When defining tax code determination rules, you specify conditions and values that must apply for the application to propose a tax
code on sales and purchasing documents. The conditions and values you can specify depend on the localization of SAP Business
One that you are using as well as on the document type and business area. The table below lists the conditions and values that are
available for the different localizations.
You can specify values by using the dropdown list or, for some values, by entering free text. For some of the conditions and values,
if you have specified them once, you can select the value that was used last for the condition from the dropdown list.
Conditions and Values for Tax Code Determination Rules
Condition Value
Federal Tax ID
Filled in: The Federal Tax ID field on the sales or purchasing
document must contain a value.
Empty: The Federal Tax ID field on the sales or purchasing
document must be empty.
Ship-To Address Choose: Select the ship-to address defined in the business partner
master data. Note that you can only select the ship-to address as a
condition, if you selected business partner as condition no. 1.
Ship-To Street / PO Box
Choose: Select a ship-to street / PO box defined in the
business partner master data.
Filled in: The Street / PO Box field in the ship-to address of
the sales or purchasing document must contain a value.
Not defined: The Street / PO Box field in the ship-to
address of the sales or purchasing document must not
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:57 AM
Condition Value
contain a value.
Ship-To City
Choose: Select a ship-to city defined in the business
partner master data.
Filled in: The City field in the ship-to address of the sales or
purchasing document must contain a value.
Not defined: The City field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Zip Code
Choose: Specify a ship-to zip code.
Filled in: The Zip Code field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The Zip Code field in the ship-to address of
the sales or purchasing document must not contain a
value.
Ship-To County
Choose: Select a ship-to county defined in the business
partner master data.
Filled in: The County field in the ship-to address of the
sales or purchasing document must contain a value.
Not defined: The County field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To State
Choose: Select a ship-to state defined in the application.
Filled in: The State field in the ship-to address of the sales
or purchasing document must contain a value.
Not defined: The State field in the ship-to address of the
sales or purchasing document must not contain a value.
Ship-To Country/Region
Choose: Select a ship-to country/region defined under
Administration Setup Business Partners
Countries/Regions .
EU: The item is shipped to a member state of the European
Union.
Non-EU: The item is shipped to a country/region outside of
the European Union.
Item Choose: Select an item code from the list.
Item Group Choose: Select an item group from the list.
Business Partner Choose: Select a business partner from the list.
Customer Group Choose: Select the customer group the customer must be
associated with from the list.
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:57 AM
Condition Value
Vendor Group Choose: Select the vendor group the vendor must be associated
with from the list.
Warehouse
Choose: Select a warehouse that the item must be shipped
from or to.
Filled in: The Warehouse field on the sales or purchasing
document must contain a value.
Not defined: The Warehouse field on the sales or
purchasing document must not contain a value.
G/L Account Choose: Select the G/L account that must be used on the sales or
purchasing document for the rule to apply.
Tax Status
Liable: The tax status field in the business partner master
data must contain the value Liable.
Exempt: The tax status field in the business partner master
data must contain the value Exempt.
EU/Acquisition: The tax status field in the business partner
master data must contain the value EU or Acquisition.
Freight Choose: Select a type of freight from the list.
UDF Choose: Select a user-defined field that you use on the sales or
purchasing document, business partner or item master data, for
warehouses, or item groups.
More Information
Tax Code Determination
Working with Tax Code Determination Rules
Tax Code Determination - Setup Window
Example: Tax Code Determination Rules Applied on Marketing
Docs
The following examples illustrate how the tax code determination (TCD) rules are applied when you create a sales or purchasing
document.
Tax code determination rule with line and header freight tax conditions defined
TCD rule definition Master data
Line Tax Code Line Freight Tax Header Freight Tax BP Item
A1 A4 A5 A2 A3
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:57 AM
TCD rule definition Master data
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A4                    | A5                      |     |     |     |
Tax code determination rule without line tax code defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| Not defined   | A2               | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A2            | A2                    | A2                      |     |     |     |
Tax code determination rule with one condition for header freight
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | A5                 | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A5                      |     |     |     |
Tax code determination rule without freight tax conditions defined
TCD rule definition Master data
| Line Tax Code | Line Freight Tax | Header Freight Tax | BP  |     | Item |
| ------------- | ---------------- | ------------------ | --- | --- | ---- |
| A1            | Not defined      | Not defined        | A2  |     | A3   |
Tax code proposed on document
| Item Tax Code | Line Freight Tax Code | Header Freight Tax Code |     |     |     |
| ------------- | --------------------- | ----------------------- | --- | --- | --- |
| A1            | A2                    | A2                      |     |     |     |
Tax code determination rule without freight tax conditions defined – freight tax code defined in freight setup
| TCD rule definition |     |     | Master data |     | Freight Setup |
| ------------------- | --- | --- | ----------- | --- | ------------- |
Line Tax Code Line Freight Tax Header Freight Tax BP Item Freight Tax Code
| A1  | Not defined | Not defined | Not defined | Not defined | A6  |
| --- | ----------- | ----------- | ----------- | ----------- | --- |
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:57 AM
TCD rule definition Master data Freight Setup
Tax code proposed on document
Item Tax Code Line Freight Tax Header Freight Tax
Code Code
A1 A6 A6
More Information
Tax Code Determination
Withholding Tax Codes - Setup Window
Use this window to define withholding tax codes for your company.
To open the window, choose Administration Setup Financials Tax Withholding Tax .
Withholding Tax Codes - Setup Fields
WT Code
Specify a code for the withholding tax.
Inactive
Select to indicate the withholding tax is inactive. Once the withholding tax is set as inactive, you cannot select it in any new or draft
document. By default, the checkbox is not selected.
WT Name
Enter a description for the withholding tax code.
Category
Choose one of the following from the dropdown list:
Invoice – the withholding tax calculation appears in the invoice and is recorded in the journal entry when the invoice is
added.
Payment – the withholding tax calculation appears in the invoice, but is recorded in the journal entry when it is created by
the incoming payment based on that invoice.
Effective From
Enter the date from which a tax group rate (%) is effective.
Rate
Enter the rate of tax to be calculated from the date defined in the Effective From field.
Base Type
Choose either Gross (includes VAT) or Net from the drop-down list to determine from which amount the withholding tax will be
calculated.
% Base Amount
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:57 AM
Specify the percentage of the base amount that is subject to withholding tax. The default value is 100%.
Official Code
Specify the official code to be reported in the withholding tax report.
Account
Choose the G/L account code to be recorded in journal entries relevant for this withholding tax code.
Withholding Tax Definition
Choose this button to open the Withholding Tax Definition - Setup: <XXX> window, in which you can define the Effective From
date and the tax percentage for the selected withholding tax code.
Minimum Taxable Amount
Specify the minimum taxable amount for the withholding tax to take effect.
More Information
Tax Definition - <XXX> Window
Tax Declaration Boxes - Setup Window
Use this window to define selection criteria for the tax declaration boxes appearing in the tax declaration box report.
To open the window, from the SAP Business One Main Menu, choose Administration Setup Financials Tax Tax
Declaration Boxes .
Tax Declaration Boxes - Setup Window
Effective From
Enables you to set up groups of tax declaration boxes, with each group sharing one effective period. Proceed as follows:
1. Specify the date from which the group of tax declaration boxes you want to create is effective. From the Effective From
dropdown list, select one of the following:
01.01.1900
01.01.2024: This date is displayed by default.
Define New: If you want to specify a date other than 01.01.1990 or 01.01.2024, define a new one.
Once you define a new date, the tax declaration group that has the default Effective From date 01.01.2024 is copied
to the new group.
Similarly, every time you define a new date, the existing tax declaration box group that has the chronologically latest
Effective From date is copied to the new group.
 Note
The chronologically later Effective From date of one tax declaration box group automatically becomes the "Effective To”
date for the group with the early Effective From date.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:57 AM
For example, you only create two groups of tax declaration boxes, group A and group B. The Effective From dates of
group A and B are set as 01.01.2009 and 01.01.2010, respectively. Therefore, 01.01.2010 automatically becomes the
”Effective To” date of group A, that is, the effective period of group A is from 01.01.2009 to 01.01.2010.
2. If required, define the individual tax declaration boxes within the group you create.
For each group, you can define different numbers of tax declaration boxes, and each tax declaration box within the group
can have individual settings.
Code, Name
Enter a code and relevant description for the box.
Inactive
Select to indicate the tax declaration box is inactive. Once the tax declaration box is set as inactive, you cannot include it in the tax
declaration box report. By default, the checkbox is not selected.
Type
Choose one of the following options:
Vat Group – summarizes VAT groups in the box
Box – summarizes several boxes in this box
Summary Field
Choose to display one of the following amounts of the tax transactions in the report:
Base Amount
Tax Amount – the actual tax amount
Non-Deductible Amount
Debit/Credit
Choose one of the following options to determine what to add of the transactions that will be calculated in the box:
Debit Side – only the debit amount
Credit Side – only the credit amount
Debit Side + Credit Side – both the credit and debit amount
Formula Syntax
The calculation formula of the box (the tax groups and the relations between them). For more information on the formula, go here.
Sort Order
Define the display order of the boxes in the report by entering their successive numbers. By default, the next successive number is
entered when you update the Tax Declaration Boxes - Setup window.
Absolute Value
Displays the absolute box amount in the report.
Box Definition - Rows
Opens the Box Definition – Rows window, in which you can define a formula for the selected box.
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:57 AM
Box Definition - Rows - Setup Window
Use this window to define formulas for selected VAT groups or boxes.
To access this window, choose Administration Setup Financials Tax Tax Declaration Boxes . Double-click the relevant
box row.
Box Definition - Rows - Setup Window
VAT Group
Click the dropdown list and select the VAT group or box to include in the box.
Formula Sign
Click the dropdown list and select the arithmetic operation (+ or -) to define the relation between this VAT group or box, and the
one below it.
Choose Update to move to the next row.
After you have finished defining all VAT groups or boxes for the formula, choose Update to save your changes.
Transfer Posting Correction Wizard
The Transfer Posting Correction Wizard enables you to post corrections resulting from VAT changes, for amounts transferred from
revenue or expense accounts to new accounts.
This wizard guides you in defining parameters required to generate these postings.
To access the wizard, from the SAP Business One Main Menu, choose Administration Utilities Transfer Posting Correction
Wizard .
 Note
Ensure that you execute the wizard only once for the selected period and the selected accounts.
 Note
All documents that you post after executing the wizard and that are valid for this period, must be transferred manually. To
transfer the posting manually, create a journal entry.
More Information
Transfer Posting Correction Wizard - Selection Criteria
Transfer Posting Correction Wizard - Transaction Selection
Transfer Posting Correction Wizard - Transaction Confirmation
Transfer Posting Correction Wizard - Summary
Transfer Posting Correction Wizard - Selection Criteria Window
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:57 AM
Use this window to specify the selection criteria for the wizard run.
Selection Criteria Fields
Date From... To...
Specify the date range for the wizard run. By default, the transactions within the posting date range are selected.
 Caution
There should be no overlap of the date ranges specified in different wizard runs; otherwise, you could correct the same posting
twice.
Doc. Date
Selects documents within the document date range.
 Caution
Always use the selected option during the rest of the period; otherwise, you could correct the same posting twice.
Tax Rate
Specify the tax rate of the transaction – 16% or 19% – that the wizard uses to select documents.
Code
Tax group code
Name
Tax group name
Display
Deselect the tax group that you do not need in the wizard run.
 Note
Only those tax groups with the tax rate of 16% or 19% are valid for the wizard.
G/L Accounts
Limits the selection to specific G/L accounts only. Click to open the Accounts - Selection Criteria window where you can
select the needed G/L accounts.
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard: Transaction Selection
Window
Use this window to select the transactions that you want to include in the wizard run.
 Recommendation
After selecting the needed transactions, you should print the screen or export it to Excel; you may use it for future verification.
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:57 AM
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Selection Fields
App
Select the posting that you want to correct
G/L Account
The revenue or expense account relevant to a transaction
Tax Code
The tax group code associated with a transaction
Tax %
The tax rate that was effective for the tax code at the time the transaction was posted
Doc. No.
The document number in SAP Business One
Debit, Credit (FC, SC)
The debit or credit tax amount (in terms of foreign currency or system currency)
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard: Transac. Confirmation
Window
Use this window to confirm the amount, accounts, and tax codes for which correction posting will be created.
 Note
This topic includes explanations of some of the fields and other elements in this window.
Transaction Confirmation Fields
Interim Account
Specify the clearing account to be used during the correction posting process.
Expense Account
Specify the account to which the expense is posted.
Revenue Account
Specify the account to which the revenue is posted.
Input Tax Group
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:57 AM
Specify the input tax group to be used in the correction posting.
Non-Deductible Tax Group
Specify the non-deductible tax group to be used in the correction posting.
Output Tax Group
Specify the output tax group to be used in the correction posting.
Deferred Tax Group (Input)
Specify the tax code which belongs to the input tax group and has a deferred tax account defined in the Tax Groups – Setup
window.
Deferred Tax Group (Output)
Specify the tax code which belongs to the output tax group and has a deferred tax account defined in the List of Tax Definitions
window.
More Information
Transfer Posting Correction Wizard
Transfer Posting Correction Wizard - Summary Window
In this window, you can see how many journal entries have been made during the correction process. The number appearing is
twice the number of the corrected transactions because it includes the entries on both the debit and credit sides.
You can view the transactions created by the wizard in the Journal Entry window of the Financials module.
More Information
Transfer Posting Correction Wizard
Financial and Tax Reporting: Singapore
Following is information about financial and tax reports specific to SAP Business One software version for Singapore.
Tax Reports
The following tax reports are available:
Tax Report
Withholding Tax Report
Tax Reconciliation Report
Tax Declaration Box Report
Chart of Accounts
The general online help file mentions the checkbox Allow Multiple Linking to Financial Templates (in G/L Accounts Details
window) is not relevant to Singapore, and therefore is not included in the SAP Business One software version for Singapore.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:57 AM
Generating IRAS Audit File: Singapore
The IRAS audit file (IAF) is available for the Singapore localization.
Prerequisites
You have defined a default XML file folder on the Path tab of the General Settings window in Administration System
Initialization General Settings .
Procedure
To generate the IRAS audit file, proceed as follows:
1. From the SAP Business One Main Menu, choose Financials Financial Reports Electronic Report IRAS Audit File .
Alternatively, choose the file from the Reports module.
The IRAS Audit File - Selection Criteria window appears.
2. Specify the parameters, select the output format (XML or TXT), and choose the Generate button.
The audit file appears in your defined folder.
Tax Report
Use this report to display documents and manual journal entries that include tax amounts sorted by tax code. Tax reports can be
produced in an electronic format by choosing an electronic reporting option in Output Mode. The report includes the following
documents:
A/R and A/P invoices and credit memos
Inventory transfer documents – The inventory transfer transactions are displayed only in order to report the transactions in
the report because the tax percentage is 0.
Manual journal entries
Incoming payments and payments to vendors that are not based on invoices
Incoming payments and payments to vendors that include cash discounts
 Note
When printing the report, you can print the selection criteria on a separate page.
Use this window to specify selection criteria for the Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report . Alternatively, open it from the
Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:57 AM
Selection Criteria
Selection Criteria Name
Criteria by which the report is created. Choose for a list of existing selection criteria, or press CTRL + A and specify new
selection criteria.
Date From...To..
Choose whether to generate the report according to Posting Date or Document Date or VAT Date or System Date, and specify the
date range for the report.
 Example
A/R invoice no. 15 was created with a posting date 25.3.19 and a document date 1.4.19. Generating the report according to
Posting Date and defining the date range as 1.1.19 – 31.3.19, includes A/R invoice no. 15 in the report. However, generating the
report according to Document Date and defining the same date range of 1.1.19 – 31.3.19, excludes A/R invoice no. 15, as the
Document Date assigned to it is not in the range.
Round Amount
Rounds the total amounts calculated in the report.
Series
Generates the report for documents created according to specific numbering series. After selecting, choose the ... button to open
the Series – Filter window in which you can define the required numbering series.
Transact.
Generates a report for specific document types.
After selecting, choose the ... button to open the Document Type window in which you can define the document types to include in
the report.
Output
This table displays all the tax groups defined as output tax groups ( Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report
- to change the order of the tax groups, highlight a group and click the arrows to position it
Input
This table displays all the tax groups defined as input tax groups (see Administration Setup Financials Tax Define Tax
Groups Category column).
Code – displays the tax group code
Name – displays the tax group name
Display – displays the tax group in the report
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:57 AM
Amount – summarizes the total amount of the tax groups, from the beginning of the table until the selected tax group
included in the report.
Button Up and Button Down - to change the order of the tax groups, highlight a group and click the arrows to position it.
Display Credit Memos in a Separate Column
The credit memos that were based on invoices from previous periods (previous to the range of dates defined in the Selection
Criteria window) appear in a separate section, at the end of the report.
Hide Tax Codes without Transactions
Excludes from the report those tax codes with no transactions related during the defined period.
Output Mode
Choose the type of report that you want to produce. You can choose an electronic tax report output here.
Only Display Documents with Externally Calculated Sales Tax
 Note
This field is only displayed if you have selected the Allow External Calculation of Tax on A/R Documents checkbox (
Administration System Initialization Company Details Accounting Data tab ).
Only includes in the report documents with an externally calculated tax amount on at least one row.
 Note
If you select this checkbox, the Externally Calculated Tax field is displayed in the tax report window.
Update/ OK
When you change the preferences in the Tax Report – Selection Criteria window, the OK option changes to the Update mode.
Choose Update to save the report under the name you entered in the Report Name field.
The preferences chosen for the report are saved.
Tax Report - Declaration
The following table describes the fields appearing in the Tax Report - Declaration window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Tax Declaration
option, set the other required parameters in the Tax Report - Selection Criteria window, then choose OK. Alternatively, open it
from the Reports module.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report - Declaration
Tax Code
Displays the code and the tax codes selected for the report.
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:57 AM
Choose the icon to display a list of transactions involving that tax code.
EU
Indicates whether the tax code is EU relevant.
Tax %
Displays the tax rate as a percentage, as defined for the tax code.
Doc. No.
Displays the internal number of the document and its type. For example A/P invoice number 110007 is displayed as PU 110007.
Posting Date
Displays the posting date of the documents. If the Tax Date option is selected in the Selection Criteria window, this column
displays the tax date of the documents.
Base Amount
Total amount of the document before taxes, summarized for each tax code.
Tax Amount
Tax amount calculated for the tax group: Total Tax field minus Non Deductible field.
Total Tax
Displays the amount of the tax.
Non Deductible
The amount which cannot be deducted.
Account
Displays the control account in which the journal entry of the document is posted.
Vendor Ref. No.
Displays the vendor’s reference number from the document, if defined.
Error Report
Choose to display error messages regarding the displayed report.
More Information
Tax Report
Tax Report - Register Book
The following table describes the fields appear in the Tax Report - Register Book window.
To open the window, choose Financials Financial Reports Accounting Tax Tax Report , select the Register Book
option and set the other required parameters in the Tax Report - Selection Criteria window, and then choose OK. Alternatively,
open it from the Reports module.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:57 AM
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Register Book
Reg. No.
Displays the successive number of the records, beginning with the value defined in the Selection Criteria window.
Date
Displays either the posting date of the documents, or, if the Tax Date option is selected in the Selection Criteria window, the tax
date.
Doc. No.
Displays the internal number of the document and its type. For example, A/P invoice number 110007 is displayed as PU 110007.
Base Amount
Total amount of the document before taxes.
Tax %
The tax rate defined for the tax code, as a percentage.
Tax
Displays the amount of the tax in the document.
Non-Deductible
The amount of the non-deductible tax in the document, calculated according to the tax code definition.
Total Amount (LC)
Displays the total amount of the document in local currency.
More Information
Tax Report
Withholding Tax Report
This report displays the withholding tax amounts collected and paid during specific periods.
 Note
If a payment on account with withholding tax has been fully reconciled (that is, the reconciled amount equals the payment
amount), the withholding tax report does not include the payment information.
 Note
When you print the report, you can print the selection criteria on a separate page.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:57 AM
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner
Vendor Mode – Detailed Format Window
Withholding Tax Report by WTax Code
Withholding Tax Report - Selection Criteria
Use this window to specify selection criteria for the Withholding Tax Report.
To open the window, choose Financials Financial Reports Accounting Tax Withholding Tax Report. Alternatively,
open it from the Reports module.
New requirements for the Tax Summary Report and layouts are occasionally introduced by the authorities for different taxation
periods. Variations in selection criteria may exist for different taxation periods which result in different outputs.
After defining the report, you can view it in the Withholding Tax Report by Business Partner Window or the Withholding Tax Report
by WTax Code Window.
Selection Criteria
Selection Criteria Name
Specify the previously saved selection criteria you want to apply for the report, or press CTRL + A to specify new ones.
Date From...To...
Choose whether to include documents based on document date or posting date and specify the date range of the current year.
Declared Period
Specify the required declaration period.
Declaration Type
Specify the type of declaration:
Original: The report includes all documents within the specified date range. When you approve the report, these documents
will be marked as printed.
Substitute: The report includes all documents within the specified date range, including documents already marked.
Complementary: The report includes only unmarked documents within the specified date range.
Vendors
Opens the Vendor Selection window, where you can select the vendors to include in the report.
Customers
Opens the Customer Selection window, where you can choose the customers to include in the report.
Doc. Type
Opens the Document Type window, where you can select the documents to include in the report.
Withholding Tax
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:57 AM
Codes and names of all tax codes relevant for the report. Deselect tax codes that should be excluded.
 Note
To clear the entire column, click the column header.
To display subtotals for tax codes, select the relevant tax codes in the Amount column.
[Arrow Up/Down]
Determines the order of appearance of the tax codes in the report display and print layout.
Output Mode
Choose the required layout of the report.
The following display the report related to purchasing documents:
WTax Code Layout-Purchasing: grouped by tax codes
Vendor Layout-Purchasing: grouped by vendors
The following display the report related to sales documents:
WTax Code Layout-Sales: grouped by tax codes
Customer Layout-Sales: grouped by customers
Exceptional Event
Exceptional Event options are available for Withholding Tax Reports.
Save
Saves your selection criteria for future use.
Withholding Tax Report by Business Partner Window
This window displays the withholding tax report by business partners according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Report by Business Partner Window Fields
#
Double-click a row to open the Vendor Mode – Detailed Format window for detailed information about the relevant business
partner, grouped by document numbers.
BP Name
Displays the name of the business partner. Choose the icon to open the Business Partner Master Data window.
Federal Tax ID
Displays the federal tax ID of the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:57 AM
Document Amount
Displays the total document amount of the business partner.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Subject Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
Vendor Mode - Detailed Format Window
Withholding Tax Table
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:57 AM
Vendor Mode - Detailed Format Window
This window displays detailed information about the relevant business partner, grouped by document numbers.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Vendor Mode – Detailed Format Window Fields
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Example
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see the Transaction
Type Abbreviation Legend page in the general online help.
Date
Displays the posting date of the reconciled transaction or payment.
WTax Code, WTax %, Official Code
Displays the code, rate, and official code of the withholding tax that is included in the reconciled transaction or payment.
Invoice Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the business partner.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Date
Displays the posting date of the payment.
Non-Subject Amount
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:57 AM
Displays the following result: the base amount - the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
More Information
Withholding Tax Report - Selection Criteria
Withholding Tax Report by Business Partner Window
Withholding Tax Table
Withholding Tax Report by WTax Code Window
This window displays the withholding tax report by withholding tax codes according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Withholding Tax Report by WTax Code Window Fields
WTax Code, WTax Name, WTax %
Displays the code, name, and rate of the withholding tax defined in the Withholding Tax Codes – Setup window according to your
selection criteria.
Document No.
Displays the type and number of the reconciled transaction or payment. Choose the icon to open the transaction or payment.
 Note
IN represents a transaction resulting from the creation of an A/R invoice. For a complete list of origins, see Transaction Type
Abbreviations Legend in the general online help, under: Help Documentation Online Help .
Document Date
Displays the posting date of the document.
Payment Date
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:57 AM
Displays the posting date of the payment.
Document Amount
For reconciled transactions, displays the document amount.
For payments, displays the payment amount.
Taxable Amount
Displays the amount subject to tax.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
WTax Amount
Displays the withholding tax amount included in the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Payment Amount
Displays the payment amount of the reconciled transaction or payment.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Sbj. Amount
Displays the following result: the base amount − the total taxable amount in all rows of the Withholding Tax Table window + the
total amount from all document rows for which you selected No in the WTax Liable column.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
Non-Taxable Total
Displays the non-subject amount.
For reconciled transactions, it displays the reconciled amount.
For payments, it displays the unreconciled amount.
 Note
This field is not visible by default. You can set it visible through the Form Settings window.
Approved
Marks the report as reported to the authorities.
More Information
Withholding Tax Report
Withholding Tax Report - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:57 AM
Withholding Tax Table
Withholding Tax Table
You can check the details and break up of the withholding tax types involved in the document and also edit the withholding tax
information as needed. To open this window, in the relevant A/P or A/R transaction window, click beside the WTax Amount field.
WT Tax Category
Displays the withholding tax category from the business partner withholding tax setup.
Details
Specify any detailed information you want to put for the withholding tax.
Code
Display the code defined in the Withholding Tax Codes - Setup window and also selected for the business partner.
Name
Display the code description you have defined in the Withholding Tax Codes - Setup window.
Rate
Display the Effective Rate which is based on the rate defined in the Withholding Tax Codes - Setup window.
Base Amount
Display the base amount depending on the amount in the transaction.
Taxable Amount
Display the taxable amount in the transaction.
WTax Amount
Display the withholding tax amount which is calculated based on the taxable amount and the rate.
Category
Displays the document category.
Base Type
Displays the base type which you have defined in the Withholding Tax Codes - Setup window.
Criteria
Displays the criteria which you have defined for the business partner.
More Information
Withholding Tax Codes - Setup Window
Tax Reconciliation Report
This report enables you to track the tax amounts that were posted in sales and purchasing documents and in manual transactions.
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:57 AM
The report displays the G/L accounts involved in these transactions and calculates the tax amounts that should have been paid,
based on the tax codes defined for each transaction.
The report covers the following transactions:
A/P and A/R invoices
A/P and A/R credit memos
Manual journal entries
A/P and A/R down payment invoices
Incoming and outgoing payments
 Note
When saving a journal entry, if you deselect the Automatic Tax option in the Journal Entry window, you cannot view the journal
entry in this report.
 Note
When printing the report, you can print the selection criteria on a separate page.
 Note
Accounts are only displayed when there is at least one posting with a VAT code on the accounts within the respective period.
More Information
Tax Reconciliation Report - Selection Criteria
Accounts - Selection Criteria
Tax Report - Reconciliation Window
Tax Reconciliation Report - Selection Criteria
Use this window to specify selection criteria for the Tax Reconciliation report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Reconciliation Report . Alternatively,
open it from the Reports module.
After creating the report, you can view it in the Tax Report - Reconciliation window.
 Note
Only G/L accounts that have VAT transaction postings are considered in this report. Accounts are only subsequently displayed
in the report when there is at least one posting with a VAT code on the accounts within the respective period.
Selection Criteria
Selection Criteria Name
Click to select previously saved report selection criteria and use them to generate the report.
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:57 AM
To save new selection criteria, press CTRL + A and enter a name in this field.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting Data tab of the Company
Details window Administration System Initialization Company Details ).
Opening Balance, Non-VAT Transactions
The report displays transactions grouped by G/L accounts and divided by tax codes, including non-tax transactions. This display
lets you crosscheck between the tax report, tax and tax based account balances, and the balance of the connected G/L account in
the system.
In addition, the report displays the opening balance of the specified tax based accounts, additional non-tax transactions that were
posted to this account, the document date, and the journal amount.
Select the Non-VAT Transactions checkbox to include the non-VAT transactions posted to the relevant G/L accounts in the report.
Date From...To
Define a date range for the report. By default, these fields display the start and end dates of the current fiscal year.
Document Date
Generates the report according to document, not posting date.
Round Amount
Report rounds off its amounts.
Series
Choose to select the series, for example, products, services, regions or brands, to include in the report.
Doc. Type
Choose to select the types of documents to include in the report.
Output
Codes and names of all the tax codes defined as output tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
Use the Amount column to select the tax codes for which you want to display subtotals.
Input
Codes and names of all the tax codes that are defined as input tax and relevant for this report.
The codes in the Display column are selected by default.
Deselect the tax codes that should be excluded from the report.
To clear the entire column, click the column header.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:57 AM
Use the Amount column to select the tax codes for which you want to display subtotals.
[Arrow Up/Down]
Use these buttons to determine the appearance order of the selected tax codes in the report display and in the printed report.
G/L Accounts
Choose to open the Accounts – Selection Criteria window, in which you choose the G/L accounts to include in the report.
Save
Choose to save your report selection criteria for future use.
Related Information
Accounts - Selection Criteria
Accounts - Selection Criteria
Use this window to specify selection criteria for the current report.
To open this window, choose the button in the G/L Accounts field, in the Selection Criteria window of the relevant report.
Selection Criteria
Find
Opens the G/L Accounts window for selecting the G/L accounts to be displayed in the report. Selected accounts are marked with
an X.
Level
Choose the Level of the account display in the table.
Choosing Level 1 displays the highest level titles for the accounts. When you select a row in the table, you select all the accounts
that appear under this title.
Level
This column shows which accounts or titles have been selected.
If a row is marked with X, the specific account or group of accounts appears in the report.
To select an account, click in the selected row.
To cancel a selection, clear its X.
To clear all selections/select all accounts in the table, click the X in the column header.
Account
This column displays the codes and names of the accounts.
To view details of each account, use the arrow that appears next to the code and name.
More Information
Tax Reconciliation Report
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:57 AM
Tax Report - Reconciliation Window
This window displays the Tax Reconciliation report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Reconciliation Window
#
Choose to expand or collapse the display of each account.
Tax Code
Displays the tax codes involved in the transactions included in the report, for each G/L account.
Click to display a list of the transactions involving that tax code.
Tax %
Displays the tax rate of the tax code.
Posting Date
Displays the posting date of the document/journal entry.
If Tax Date is selected in the Selection Criteria window, this column displays the tax date of the document/journal entry.
Tax Base Amount
Displays the amount that is the basis for the tax calculation and was posted to the G/L account.
Tax Amount
Tax amount calculated for the report.
Deferred Tax Document
Indicates whether the document contains deferred tax.
Tax Declaration Box Report
This tax report should be generated monthly or quarterly. It includes transactions that involve tax and pertain to tax codes. The
following documents and transactions are covered in the report:
A/R and A/P invoices
A/R and A/P credit memos
Incoming payments and outgoing payments
Manual journal entries
Down payments
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:57 AM
When printing the report, you can print the selection criteria on a separate page.
More Information
Tax Declaration Box Report - Selection Criteria
Tax Report - Declaration Window
Tax Declaration Box - Selection Criteria
Use this window to specify selection criteria for the Tax Declaration Box report.
To open the window, choose Financials Financial Reports Accounting Tax Tax Declaration Box Report . Alternatively,
open it from the Reports module.
After creating the report you can view it in the Tax Report-Declaration window.
Selection Criteria
Selection Criteria Name
Click to select previously saved report selection criteria and use them to generate the report. To save new selection criteria,
press CTRL + A and enter a name.
Tax Declaration Name
Select one of the previously saved reports from the dropdown list.
 Note
This field is available only when the Extended Tax Reporting checkbox is selected on the Accounting tab of the Company
Details window ( Administration System Initialization Company Details ).
Adjustment
Select the adjusted version of a report.
Date From... To
Specify a range of posting dates or document dates or VAT dates or system dates to include specific transactions in the report. By
default, the From and To fields display the start and end dates of the current fiscal year.
If the specified From date falls into the effective period range of a tax declaration box group, all the tax declaration boxes within
this group are automatically displayed in the Tax Declaration Boxes table. For more information about the effective period of a tax
declaration box group, see the Effective From field in Tax Declaration Boxes - Setup window.
Round Amount
Report rounds off its displayed amounts.
Tax Declaration Boxes
This table displays the tax declaration boxes according to the specified From date. It includes the following columns:
Code – displays the code of the box
Name – displays the name of the box
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:57 AM
Opening Balance - you can manually enter the opening balance relevant for each box
Display – all the checkboxes in this column are selected by default. Deselect the checkboxes of the boxes you want to
exclude from the report.
Save
Choose to save the Report Selection Criteria for future use.
More Information
Tax Declaration Box Report
Tax Report - Declaration Window
This window displays the Tax Declaration Box report according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Tax Report – Declaration Window
Box Code
Displays the box code and a drill-down option to display the tax group or boxes that are combined to calculate the value for this
box.
Box Component Code
Displays the code of the component included in the box, and provides a drill-down icon that enables you to display the tax codes
included in each component.
Tax Code
This column displays tax codes only in expanded view mode.
Use the drill-down icon next to the tax code to display a list of documents which use that tax code.
Tax %
Displays the rate of each tax group.
Posting Date
Displays the posting date of each document.
Doc. Date
Displays the document date of each document.
VAT Date
Displays the VAT date of each document.
Credit Amount, Debit Amount
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:57 AM
In a collapsed view mode, the credit column displays the cumulative amounts of both the credit and debit sides. A negative amount
indicates a greater debit side, and vice versa.
In an expanded view mode, these columns display the credit or debit amounts per row in the transaction created by each
document.
Summary Field
Displays the summary criteria defined in the Define Tax Declaration Box window.
Debit/Credit
Displays the choice made in the Credit/Debit column of the Define Tax Declaration Box window.
More Information
Tax Declaration Box Report
Banking
This section describes the features and functions under the Banking module that are specific to Singapore only.
Information about general features and functions in the Banking module is available in the general online help file provided with
SAP Business One, under Help Documentation Online Help
Manually Reconciling Bank Statements
 Recommendation
When you use this function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do not
simultaneously use the external bank statement processing function (see Recording Transactions from External Statements in
the general online help file provided with SAP Business One) and the standard function for manually performing an external
reconciliation (see Manually Performing External Reconciliations in the general online help file provided with SAP Business
One) for the same bank account. In addition, we recommend that you use exclusively either this function or the standard
function for manually reconciling bank statements.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
The External Bank Reconciliation - Selection Criteria window appears.
2. In the Account Code field, select an account code.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:57 AM
As a result, Account Name and Currency are displayed automatically in the respective fields. If the account currency is
defined as All Currencies, the local currency is displayed and is the reconciliation currency. You cannot edit the Currency
and the Last Balance fields. In addition, the Last Balance field automatically displays the updated balance from the
previous reconciliation.
In the Ending Balance field, specify the current balance received from the bank; in the End Date field specify the date to
which the current balance is updated.
3. Choose OK.
The Reconciliation Bank Statement window appears.
SAP Business One displays all the open deposits and payments in which the selected account is involved. View and specify
the information displayed.
4. Select the transactions to be cleared.
When you select a transaction, SAP Business One recalculates the value in the Difference field. Reconciliation is performed
only if the difference equals zero.
5. If the value in the Difference field is not zero, do one of the following:
Create an adjustment.
For more information, see Creating Adjustments.
Save your selection for future processing.
Choose the Save button. The next time you choose the same account in the External Bank Reconciliation -
Selection Criteria window, the Reconciliation Bank Statement window displays the saved selection.
6. To perform the reconciliation, choose the Reconcile button.
 Note
You cannot re-create reconciliations created in the Reconciliation Bank Statement window.
Result
SAP Business One reconciles the selected transactions and sets the reconciliation type for this reconciliation to Manual.
More Information
Example: Manual Reconciliation of External Bank Statements
Creating Adjustments
To reflect transactions that are already in the bank statement but are not yet posted in SAP Business One, you can create a
balancing transaction or document.
 Recommendation
When you use this localized function for manually reconciling bank statements, to avoid creating duplicate reconciliations, do
not simultaneously use the external bank statement processing function (see the Recording Transactions from External
Statements page in the general online help provided with SAP Business One) and the standard function for manually
performing an external reconciliation (see the Manually Performing External Reconciliations page in the general online help
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:57 AM
provided with SAP Business One) for the same bank account. In addition, we recommend that you use exclusively either this
function or the standard function for manually reconciling bank statements.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
After you make the required adjustments, the difference between the ending balance in the bank statement and the account
balance in the books equals zero, and you can now reconcile the selected transactions.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manual
Reconciliation .
2. In the External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
3. In the Reconciliation Bank Statement window, make the required selections and choose Adjustments.
The Adjustments window appears.
4. Select one of the following types of transactions you want to create and choose OK:
Journal entry
Incoming payment
Outgoing payment
Check for payment
Deposit
The window of the selected transaction type appears.
5. Create the required transaction and choose Add.
As a result, the created transaction is added to the table of the Reconciliation Bank Statement window, and it is also
selected. The value in the Difference field is updated accordingly.
6. To perform the reconciliation, choose the Reconcile button.
More Information
Manually Reconciling Bank Statements
Example: Manual Reconciliation of External Bank Statements
External Bank Reconciliation - Selection Criteria Window
Reconciliation Bank Statement Window
Example: Manual Reconciliation of External Bank Statements
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:57 AM
On December 1, 2009, you decide to perform a reconciliation for your bank account. The last balance of this account was 100, and
the ending balance of this bank account for this date is 250.
The Reconciliation Bank Statement window displays 2 deposits that you can clear:
Date Transaction Number Deposit Amount
November 10, 2009 927 45
November 24, 2009 929 100
You need to reconcile transactions to match the value of the cleared book balance to the ending balance of this bank account. In
this case, you need to reconcile transactions with a total amount of 150 = 250 minus 100.
You select both transactions, but the total amount of the open transactions is 145 = 45 + 100.
You create a manual journal entry as an adjustment, debiting the bank account by the amount of 5.
As a result, an additional row is added to the list of transactions you want to clear. The difference between the cleared book
balance and the statement ending balance is now zero, enabling you to complete the reconciliation.
More Information
Creating Adjustments
External Bank Reconciliation - Selection Criteria Window
Use this window to define the selection criteria for manually reconciling bank statements.
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation .
External Bank Reconciliation – Selection Criteria Window Fields
Account Code, Account Name, Currency
Select the relevant account code.
After you select an account code, the account name and currency are displayed automatically in the respective fields. If the
account is defined as All Currencies, the local currency is displayed and is the reconciliation currency.
 Note
You cannot edit the Currency field (described above) and the Last Balance field (described below).
Bank Statement
This section contains the following fields:
Last Balance – Automatically displays the updated balance from the previous reconciliation.
Ending Balance – Specify the current balance received from the bank.
End Date – Specify the date to which the current balance is updated.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:57 AM
Reconciliation Bank Statement Window
Manually Reconciling Bank Statements
Reconciliation Bank Statement Window
This window displays all the open deposits and payments in which the account you chose in the External Bank Reconciliation -
Selection Criteria window is involved.
To open the window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation . In the
External Bank Reconciliation - Selection Criteria window, specify the relevant account information and choose OK.
General Area
Account Code
Displays the account code selected in the External Bank Reconciliation – Selection Criteria window.
Display
Determines what transactions are displayed. Select one of the following display options:
All – Both cleared and uncleared transactions
Cleared – Only cleared transactions
Uncleared – Only uncleared transactions
Find
Enables you to find a specific transaction in a sorted column.
 Example
To find a transaction according to its number, sort the Trans. No. column. Then in the Find field, specify the relevant number.
SAP Business One highlights the first transaction that matches the value entered.
 Note
By default, the Date column is sorted.
Statement No.
Specify the number of the statement you received. This number is unique for each account. This means you can assign the same
number to statements created for different accounts; however, you can assign the same number only to one statement in each
account. You can create a statement without a number.
 Note
If a reconciliation is canceled, its statement number becomes available again and can be used for a new reconciliation.
Last Statement Balance
Displays the balance of the previous statement.
Payment, Deposit: Total No., Total Amount
The Total No. field displays the total number of selected transactions on the debit side (Payment) and on the credit side (Deposit).
The Total Amount field displays the cumulative debit amount and credit amount.
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:57 AM
Cleared Book Balance
Displays the total cleared amount, considering the selected transactions.
Statement Ending Balance
Displays the value entered in the Ending Balance field in the External Bank Reconciliation – Selection Criteria window.
Difference
Displays the difference between the Cleared Book Balance and the Statement Ending Balance. This value depends on the
selected transactions.
Save
Saves the current reconciliation so that you can continue working on it later. The next time you choose the same account in the
External Bank Reconciliation – Selection Criteria window, the Reconciliation Bank Statement window displays the saved
selection.
Adjustments
Enables you to create any required bank adjustments by opening the Adjustments window. For more information, see Creating
Adjustments .
Table Area
Cleared
Select to indicate that the transaction has been cleared.
Type
Displays the transaction type:
PS – represents payments, that is, transactions in which the selected account is credited
DP – represents deposits, that is, transactions in which the selected account is debited
Date
Displays the posting date of the transactions.
Trans. No.
Displays the number of the transaction and provides a link to the journal entry.
Reference No.
Displays the reference number as it appears in the Ref. 1 field in the Journal Entry window.
Payment
Displays the amount on the debit side in the transaction.
Deposit
Displays the amount on the credit side in the transaction.
Cleared Amount
After you select the transaction, the amount in the Payment/Deposit column is displayed here.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:57 AM
External Bank Reconciliation - Selection Criteria Window
Manually Reconciling Bank Statements
Bank Reconciliation Report - Selection Criteria Window
The compares the ending balance of a bank statement with the adjusted balance of the G/L account that represents the bank
account as of the statement date. It lists the cleared transactions in the bank statement and the uncleared transactions in the G/L
account as of the statement date. This report uses only external reconciliations created with the function for manually reconciling
bank statements.
Use this window to specify selection criteria for the Bank Reconciliation report.
Bank Reconciliation Report – Selection Criteria Window
Account Code
From the dropdown list, select the G/L account for which you want to check external reconciliations. The list shows the account
code and the account name.
 Note
The list displays only the following accounts:
With external reconciliations created using the localized function for manually reconciling bank statements.
That represent house bank accounts.
Reconciliation Number
From the dropdown list, select the reconciliation that you want to include in the report for the selected G/L account.
The list displays the reconciliation number and its due date in the Recon. and Due Date fields respectively for the selected G/L
account.
Related Information
Bank Reconciliation Report Window
Bank Reconciliation Report Window
This report compares the ending balance of a bank statement with the adjusted balance of the G/L account that represents the
bank account as of the statement date. It lists the cleared transactions in the bank statement and the uncleared transactions in
the G/L account as of the statement date.
 Note
This report uses only external reconciliations created with the function for manually reconciling bank statements.
This window displays the Bank Reconciliation report according to your selection criteria.
It consists of the following sections:
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:57 AM
Report header – displays the criteria selected in the Bank Reconciliation Report - Selection Criteria window and other
relevant information.
Reconciliation summary – displays the summarized information of cleared checks, payments, deposits, and credits in the
bank statement; and uncleared checks, payments, deposits, and credits in the G/L account, and the balances and variance.
Report body – displays the detailed information of cleared checks, payments, deposits, and credits; uncleared checks,
payments, deposits; and credits; subtotals of each section; and totals of cleared and uncleared transactions.
 Note
Amounts in brackets indicate negative amounts.
Report Header
G/L Account
Displays the code and name of the selected G/L account.
Reconciliation Number
Displays the number of the reconciliation that you specified in the selection criteria window.
Statement Date
Displays the date specified in the End Date field in the External Bank Reconciliation – Selection Criteria window for this
reconciliation under Banking Bank Statements and External Reconciliations Manual Reconciliation .
Statement Number
Displays the number specified in the Statement No. field in the Reconciliation Bank Statement window for this reconciliation.
To open this window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation , specify
relevant information, and choose the OK button.
Date, Time
Displays the date and time when you run the report.
Reconciliation Summary
Beginning Balance
Displays the number in the Last Statement Balance field in the Reconciliation Bank Statement window for this reconciliation.
To open this window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation , specify
relevant information, and choose the OK button.
Cleared Checks and Payments
Displays the cleared amount of outgoing transactions in this reconciliation, that is, transactions in which the selected G/L account
is credited.
Cleared Deposits and Credits
Displays the cleared amount of incoming transactions in this reconciliation, that is, transactions in which the selected G/L account
is debited.
Ending Balance
Displays the number in the Statement Ending Balance field in the Reconciliation Bank Statement window for this reconciliation.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:57 AM
To open this window, choose Banking Bank Statements and External Reconciliations Manual Reconciliation , specify
relevant information, and choose the OK button.
Account Balance
Displays the balance on the selected G/L account as of the statement date.
Uncleared Checks and Payments
Displays the uncleared amount of outgoing transactions in this reconciliation, that is, transactions in which the selected G/L
account is credited.
Uncleared Deposits and Credits
Displays the uncleared amount of incoming transactions in this reconciliation, that is, transactions in which the selected G/L
account is debited.
Adjusted Account Balance
Displays the result of Account Balance + Uncleared Checks and Payments – Uncleared Deposits and Credits.
Variance
Displays the difference between the Ending Balance and the Adjusted Account Balance.
Report Body
Type
Displays the transaction type:
PS represents outgoing transactions, that is, transactions in which the selected G/L account is credited (such as checks
and bank transfers issued to vendors).
DP represents incoming transactions, that is, transactions in which the selected G/L account is debited (such as deposits
made of checks and bank transfers received from customers).
Trans. No.
Displays the number of the transaction and provides a link to the journal entry.
Posting Date
Displays the value as it appears in the Posting Date field in the Journal Entry window for this transaction.
Payee/Account Name, BP Code/Account Code
Displays the name and code of the business partner or account that acts as the offset account to the selected G/L account.
Ref. No.1, Ref. No.3
Displays the values as they appear in the Ref.1 and Ref.3 fields in the expanded mode of the Journal Entry window for the selected
G/L account.
Check No.
When the transaction is a check, displays the value as it appears in the Internal ID field in the Checks for Payment window for this
check under Banking Outgoing Payments Checks for Payment .
Remarks
Displays the value as it appears in the Remarks field in the expanded mode of the Journal Entry window for the selected G/L
account.
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:57 AM
Deposit
Displays the amount on the debit side of the selected G/L account.
Payment
Displays the amount on the credit side of the selected G/L account.
Balance
Displays the total cumulative amount calculated by adding deposits and subtracting payments.
Related Information
Bank Reconciliation Report - Selection Criteria Window
Postdated Check Deposit
Use this function to transfer to the cash account checks that were deposited as postdated.
To deposit postdated checks, choose Banking Deposits Postdated Check Deposit .
More Information
Postdated Checks Deposit Window
Depositing Postdated Checks
Procedure
1. Choose Banking Deposits Postdated Check Deposit .
2. In the general area of the window, fill in the fields so that the table displays the checks you want to deposit.
3. Specify the account to which the amount of the selected postdated checks should be transferred.
 Note
Only checks deposited as postdated checks in the Deposit window can be deposited from the Postdated Check Deposit
window.
4. Select the checks to be deposited.
5. To record the deposit in the database, choose Add.
Results
A journal entry transferring the deposited checks from the postdated checks account to the cash checks account is created. The
status of the checks is updated from Deposited as Deferred to Deposited as Cash.
Postdated Check Deposit Window
To open the Postdated Check Deposit window, choose Banking Deposits Postdated Check Deposit .
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:57 AM
Postdated Check Deposit Window
Key
Successive number, starting from 1, for each postdated check deposit document.
Deposit Currency
To display only checks created with one currency, specify this currency. If you choose a foreign currency, a field displaying the
exchange rate appears. You can change the exchange rate if required.
Bank Account
Specify the account code to which the checks should be transferred.
Date
Due date of the checks. This is the current date by default. Change the date if required.
Display Until
Specify a date to display all checks that have reached their value date by this date.
Find Check No.
To trace a specific check, specify its number. SAP Business One marks the required check.
Date, Account Code, Check, Bank, Branch, Acct No., BP/Account Code, BP/Account Name, Check Amount, Incoming Payment
Information about the postdated checks.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
Total for Deposit
Total amount of all checks selected for deposit.
No. of Checks
Number of checks selected for deposit.
Remarks
Remarks about this document.
Reconcile Amounts After Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Check Deposit
Postdated Credit Voucher Deposit
Use this function to transfer to the cash account credit card vouchers deposited to the deferred account.
To deposit postdated credit card vouchers, choose Banking Deposits Postdated Credit Voucher Deposit .
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:57 AM
More Information
Postdated Credit Voucher Deposit Window
Depositing Postdated Credit Card Vouchers
Depositing Postdated Credit Vouchers
Context
Follow this procedure to deposit vouchers that were deposited as postdated to the cash account credit card.
Procedure
1. Choose Banking Deposits Postdated Credit Voucher Deposit .
2. In the general area of the window, specify the relevant parameters to display in the table the credit card vouchers to be
deposited.
3. Select the credit card vouchers you want to deposit.
4. If a commission is involved in the deposit, choose next to Total Commissions.
5. In the Commission window, specify the commission details and choose Update.
6. To record the deposit in the database, choose Add.
Results
A journal entry that transfers the postdated credit card vouchers from the deferred account to the cash account is created. If the
deposit involves a commission, this is reflected in the journal entry.
Related Information
Postdated Credit Voucher Deposit Window
Postdated Credit Voucher Deposit Window
To open the Postdated Credit Voucher Deposit window, choose Banking Deposits Postdated Credit Voucher Deposit .
Postdated Credit Voucher Deposit Window
Key No.
Successive number, starting from 1, for each deposit of a postdated credit card voucher or postdated check.
Deposit Currency
To display credit card vouchers created with a particular currency, specify this currency.
No. of Vouchers
Number of vouchers selected for deposit.
Display Until
To display all credit card vouchers that have reached their value date by a certain date, specify this date.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:57 AM
Date
By default, the current date. You can change this date if necessary.
Find Voucher No
To find a credit card voucher by its number, sort the Doc. No. column and then specify the required number here. SAP Business
One places this voucher at the beginning of the list.
Date, Acct Code, Doc. No., Card Name, Ref., Payment Method, BP/Account Code, BP/Account Name, # Pymts, of, Total,
Incoming Payment
Information about the postdated credit card vouchers displayed.
Journal Remarks
Add any comments about the deposit.
Trans. No.
Number of the journal entry created by this document and a link to it. The number appears after you have added the document.
Total Commissions
Opens the Commission window where you can enter the amount of commission to be paid for the deposit.
Reconcile Amounts after Deposit
Automatically performs reconciliation of the amounts deposited.
More Information
Postdated Credit Vouchers Deposit
Commission Window
Creating Sales and Purchasing Documents with Negative Totals
Use
You can create invoices with negative totals. This allows you to bill and refund a customer or vendor in one single document. This
may be convenient for example, if you as a sales person are on the phone with a customer who is ordering certain items, but at the
same time wants to return some items that he ordered previously. In this case, instead of posting an A/R invoice and a credit
memo, you enter the items that the customer purchases as a positive quantity and the goods the customer intends to return as a
negative quantity.
 Recommendation
We recommend that you consider carefully whether you would like to record two opposite transactions in one document.
Posting two documents helps to improve transparency in accounting.
You can generate the following documents with a negative total:
A/R and A/P invoice
A/R and A/P credit memo
An A/R delivery
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:57 AM
An A/R return
An A/P goods receipt
An A/P goods return
The inventory valuation behavior of the documents with negative totals is as outlined in the table below.
Inventory valuation behavior of documents with negative totals
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
| Goods receipt P/O | Goods return      | Inventory | Allocation |     |
| ----------------- | ----------------- | --------- | ---------- | --- |
| Goods return      | Goods receipt P/O | Inventory | Allocation |     |
A/P Invoice A/P credit memo Inventory Vendor Negative Adjustment
Account, Price
Differences Account
A/P credit memo A/P invoice Inventory Vendor Negative Adjustment
Account, Price
Differences Account
| Delivery        | A/R return      | Inventory    | COGS |     |
| --------------- | --------------- | ------------ | ---- | --- |
| Return          | Delivery        | Sales Return | COGS |     |
| A/R invoice     | A/R credit memo | Inventory    | COGS |     |
| A/R credit memo | A/R invoice     | Sales Return | COGS |     |
Goods receipt P/O based Goods return based on Inventory Allocation Negative Adjustment
| on goods return | goods receipt P/O |     |     | Account, Price |
| --------------- | ----------------- | --- | --- | -------------- |
Differences Account
Goods return based on Goods receipt P/O based Inventory Allocation Negative Adjustment
| goods receipt P/O | on goods return |     |     | Account, Price |
| ----------------- | --------------- | --- | --- | -------------- |
Differences Account
| A/P invoice based on | Credit memo based on | No inventory transaction |     |     |
| -------------------- | -------------------- | ------------------------ | --- | --- |
| goods receipt P/O    | goods return         |                          |     |     |
A/P credit memo based A/P invoice based on Vendor, Allocation Price Differences
| on goods return | goods receipt P/O |     |     | Account, Negative |
| --------------- | ----------------- | --- | --- | ----------------- |
Adjustment Account
A/P credit memo based Invoice based on credit Inventory Vendor Negative Adjustment
| on A/P invoice | memo |     |     | Account, Price |
| -------------- | ---- | --- | --- | -------------- |
Differences Account
Delivery based on return Delivery based on return Inventory COGS Negative Adjustment
Account
Return based on delivery Return based on delivery Sales Return COGS Negative Adjustment
Account, Price
Differences Account
| A/R invoice based on | Credit memo based on | No inventory transaction |     |     |
| -------------------- | -------------------- | ------------------------ | --- | --- |
| delivery             | return               |                          |     |     |
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:57 AM
Type of Transaction Similar Transaction Inventory Account Balance Account Profit & Loss Account
A/R credit memo based A/R invoice based on No inventory transaction
on return delivery
A/R credit memo based A/R invoice based on Sales Return COGS Negative Adjustment
on invoice credit memo Account, Price
Differences Account
Message Documentation
Message documentation aims to provide you with the information you need to respond to system or error messages that may
appear in SAP Business One.
10000397
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the Output
Tax Group field empty.
Procedure
In step no. 4, specify the required tax group in Output Tax Group field, and choose Run.
10000398
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run, but you have left the Input Tax
Group field empty.
Procedure
In step no. 4, in the Input Tax Group field, specify the required tax group and choose Run.
10000399
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:57 AM
Message
Enter valid acquisition tax group
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step 4, the Transaction Confirmation window, you have chosen
the Run button. However, the Acquisition Tax Group field is either empty or contains an invalid tax group.
Procedure
In step 4, the Transaction Confirmation window, in the Acquisition Tax Group field, specify the required tax group, and choose the
Run button.
More Information
Transfer Posting Correction Wizard - Transaction Confirmation Window
10000400
Message
Tax group is invalid
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the Non—
Deductible Tax Group field empty.
Procedure
In step no. 4, specify the required tax group in Non-Deducible Tax Group field, and choose Run.
10000401
Message
Missing or invalid account
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the
Interim Account field empty.
Procedure
In step no. 4, specify the required G/L account in the Interim Account field, and choose Run.
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:57 AM
10000402
Message
Missing or invalid account
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the
Revenue Account field empty.
Procedure
In step no. 4, specify the required G/L account in Revenue Account field, and choose Run.
10000403
Message
Missing or invalid account
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step no. 4, you have chosen Run however, you have left the
Expense Account field empty.
Procedure
In step no. 4, specify the required G/L account in Expense Account field, and choose Run.
10000979
Message
In “From” and “To” fields, enter dates
Diagnosis
You have opened the Transfer Posting Correction Wizard — Selection Criteria window, and have chosen the Next button, but you
have not specified dates in the From and To fields. To continue to the next step, you must specify a valid date range since SAP
Business One retrieves data in ascending order from the earliest date to the latest date.
Procedure
In the Transfer Posting Correction Wizard — Selection Criteria window, specify dates in the From and To fields.
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:57 AM
More Information
Transfer Posting Correction Wizard - Selection Criteria Window
10000982
Message
In “Tax Rate” field, enter number greater than zero
Diagnosis
You have tried to run the Transfer Posting Correction Wizard. In step 2, the Selection Criteria window, you have chosen the Next
button. However, the Tax Rate contains a negative value.
Procedure
In step 2, the Selection Criteria window, enter a number greater than zero in the Tax Rate field, and choose the Next button.
 Note
Only tax groups with a tax rate of 16% or 19% are valid for the wizard.
More Information
Transfer Posting Correction Wizard - Selection Criteria Window
This is custom documentation. For more information, please visit SAP Help Portal. 55