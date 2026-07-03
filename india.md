6/12/26, 12:22 PM
Localization for India
Generated on: 2026-06-12 12:22:07 GMT+0000
SAP Business One | 10.0
Public
Original content: https://help.sap.com/docs/SAP_BUSINESS_ONE/fe9004e23275471b868395b412ad5f80?locale=en-
US&state=PRODUCTION&version=10.0
Warning
This document has been generated from SAP Help Portal and is an incomplete version of the official SAP product documentation.
The information included in custom documentation may not reflect the arrangement of topics in SAP Help Portal, and may be
missing important aspects and/or correlations to other topics. For this reason, it is not for production use.
For more information, please visit https://help.sap.com/docs/disclaimer.
This is custom documentation. For more information, please visit SAP Help Portal. 1

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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

6/12/26, 12:22 PM
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