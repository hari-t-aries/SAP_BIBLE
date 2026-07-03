6/8/26, 6:08 AM
SAP Business One 10.0
Generated on: 2026-06-08 06:08:01 GMT+0000
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

6/8/26, 6:08 AM
Banking
Use this component to perform all monetary transactions that involve bank accounts, including the following:
Manual and automatic creation of incoming and outgoing payments for various payment means
Manual and automatic performance of internal and external reconciliations
Postdated and cash deposits of checks and credit card vouchers
Batch and single check printing
In the interactive graphics below, you can hover over each area for short description and choose the highlighted areas for more
information.
Basic Operations
Please note that image maps are not interactive in PDF outputs.
Reports and Other Functions
This is custom documentation. For more information, please visit SAP Help Portal. 2

6/8/26, 6:08 AM
Please note that image maps are not interactive in PDF outputs.
Incoming Payments Main-Menu Option
Use the features listed under this function to:
Create incoming payments for customers, vendors and accounts for various payment means
Trace, update, and endorse received checks and credit card vouchers
Create, trace, and process drafts of incoming payment documents
To use the features, choose Banking Incoming Payments .
All the images here in this topic are interactive. Hover over each area for a short description. Choose the highlighted areas for more
information.
Operation of Incoming Payments:
Please note that image maps are not interactive in PDF outputs.
Operations of Received Checks and Credit Card Vouchers:
This is custom documentation. For more information, please visit SAP Help Portal. 3

6/8/26, 6:08 AM
Please note that image maps are not interactive in PDF outputs.
More Information
Payment Drafts Report
Check Register Report
Incoming Payments
Use this window to create a record each time your company receives a payment from a customer, vendor, or account.
An incoming payment document can be created for the following payment means:
Cash
Check
Credit card
Bank transfer
When you add an incoming payment, an appropriate journal entry is created.
You can create an incoming payment to clear the debt of an open A/R invoice or an opening balance. You can also create an
incoming payment for a down payment received before the goods or services were provided.
When you create an incoming payment to clear (fully or partially) a document or transaction, internal reconciliation takes place
automatically.
To open the window, choose Banking Incoming Payments Incoming Payments .
More Information
Creating Incoming Payments for Specific A/R Invoice(s)
Creating Incoming Payments on Account
Creating Incoming Payments for All Currency Customer
Creating Incoming Payments for Partial Amount
Cancelling an Incoming Payment
Incoming Payments: Customer
Incoming Payments: Vendor
This is custom documentation. For more information, please visit SAP Help Portal. 4

6/8/26, 6:08 AM
Incoming Payment: Account
Payment Means
Creating Incoming Payments for All Currency Customers
Context
Use the procedure to create an incoming payment document for an All currency customer.
Procedure
1. Choose Banking Incoming Payments Incoming Payments .
2. Select Customer.
3. In the Code field, enter the customer code.
4. Specify other relevant details.
5. To create a payment for specific invoice(s), select the relevant invoice(s) in the table.
The Amount Due (FC) and Amount Due (LC) fields are updated accordingly.
 Note
If you select more than one document in more than one currency, the Amount Due (FC) field displays *****.
If the payment received was without reference to a specific document, select Payment on Account, and enter the
amount paid without any currency sign ($, £). The Amount Due (LC) is updated automatically, and displays the amount
entered.
6. Choose to display the Payment Means window.
7. Specify the currency for the payment.
If you choose a foreign currency, a field displaying the exchange rate as defined in Administration Exchange Rates and
Indexes appears. Change the rate if necessary.
8. Choose the relevant tab for the means of payment.
 Note
The G/L account you enter in the Payment Means window should be in the currency selected.
9. Specify the details about the means of payment.
10. Choose OK to return to the Incoming Payments window.
The Amount Due (FC) field displays the paid amount in the selected currency.
The Amount Due (LC) field displays the paid amount in local currency, calculated according to the exchange rate defined in
the Payment Means window.
11. Choose Add.
Results
An appropriate journal entry is created.
If the incoming payment was created for specific document(s)/transaction(s) the following occurs:
This is custom documentation. For more information, please visit SAP Help Portal. 5

6/8/26, 6:08 AM
If the selected document(s) are fully paid, the status of it becomes closed.
The Applied Amount and Open Balance/Balance Due fields in the document(s)are updated accordingly.
The transactions for the incoming payments and the paid document(s)/transaction(s) are reconciled internally.
If the exchange rate of the invoice(s) is different from the exchange rate of the incoming payments, SAP Business
One automatically performs an exchange rate differences transaction.
Related Information
Incoming Payments
Canceling Incoming Payments
Context
Follow this procedure to cancel Incoming Payments created for cash, bank transfers, and checks.
 Note
When a payment on account is included in a payment order run, you cannot cancel it.
 Note
When a payment contains canceled or endorsed checks, you cannot cancel it.
 Note
When a payment contains checks that are deposited through the Postdated Check Deposit window, you cannot cancel the
payment through the Incoming Payments window. However, you can cancel the other checks of the payment, whether
deposited or not deposited, through the Check Register window.
Procedure
1. From the SAP Business One Main Menu, choose Banking Incoming Payments Incoming Payments and display the
payment you want to cancel.
2. In the document, right-click and choose Cancel.
3. When asked whether to cancel the incoming payment, choose Yes to complete the cancellation.
 Note
If the payment means is check, and the checks are already deposited, another message appears asking whether to
credit the checks received account for any deposited amount. Choose Yes to complete the cancellation.
 Note
If the current system date is not the original document date, the Cancellation Options window appears.
Select one of the following:
Current System Date – to assign to the transaction resulting from the cancellation the current date
Original Document Date – to assign to the transaction resulting from the cancellation the same date (posting
date, due date, and document date) as is assigned to the canceled document
This is custom documentation. For more information, please visit SAP Help Portal. 6

6/8/26, 6:08 AM
Choose OK to complete the cancellation.
Results
A reverse journal entry is created in order to cancel the journal entry created when the incoming payment was added. The
date assigned to this transaction is according to the selection you made in the Cancellation Options window. The Remarks
field of this journal entry indicates that this is a reverse transaction for a specific incoming payment.
If the canceled incoming payment was created for specific transactions or documents, the reconciliation performed as a
result of adding the incoming payment is canceled, and the balance due amounts in the transactions/documents paid are
updated accordingly. Documents paid and closed by the canceled incoming payment are reopened.
If the payment means is check, and the checks are not deposited, the cancellation of this incoming payment cancels the
checks. To view the status of a check, select the check in the Check Register window, and select the Check Status tab.
If the payment means is check, and the checks are already deposited, the cancellation of this incoming payment does not
cancel the deposited checks and deposits. The cancellation of this incoming payment cancels the internal reconciliation
between the incoming payment and the deposit.
 Note
If you want to cancel the deposited checks and deposits together with the incoming payment, see Canceling Checks.
The Journal Remarks field in the canceled incoming payment displays the text: Cancelled.
Creating Incoming Payments on Account
Context
Use the procedure to create incoming payments for payments received with no reference to specific invoice(s) and/or other
transactions.
 Note
When a payment on account is included in a payment order run, you cannot cancel it.
Procedure
1. From the SAP Business One Main Menu, choose Banking Incoming Payments Incoming Payments .
2. Select Customer or Vendor.
3. In the Code field, specify the business partner code.
4. Select Payment on Account.
5. In the field next to Payment on Account, specify the received amount.
6. Specify all other required details and choose to open the Payment Means window.
7. On the relevant payment means tab, specify the required details and choose OK.
8. To add the incoming payment document to the database, choose Add.
Results
This is custom documentation. For more information, please visit SAP Help Portal. 7

6/8/26, 6:08 AM
The appropriate journal entry is created.
Creating Incoming Payments for Partial Amount
Procedure
1. Choose Banking Incoming Payments Incoming Payments , and select the Customer button.
2. In the Code field, specify the customer code. The invoices still to be paid are displayed in the table.
3. Select the invoice for which you want to create the partial payment. In the Total Payment column, change the original
amount to the amount that is actually being paid and press Tab .
The amounts displayed in Amount Due (FC) and in Amount Due (LC) are updated accordingly.
4. Choose to open the Payment Means window, and specify the required details.
5. Choose OK, and in the Incoming Payments window, choose Add to add the document to the database.
Results
A journal entry is created, crediting the customer for the amount paid.
The amount in the Balance Due field of the partially paid invoice is updated, and displays only the amount still to be paid.
The invoice status remains open.
Related Information
Incoming Payments
Creating Incoming Payments from Vendors
Use the procedure to create an incoming payment from a vendor based on an A/P credit memo, or on an A/P invoice and A/P
credit memo when a partial amount is returned.
This might occur when you return to the vendor (completely or partially) goods you purchased and paid for.
 Caution
You cannot create this type of document through the payment wizard.
Procedure
1. Choose Banking Incoming Payments Incoming Payments .
2. In the Incoming Payments window, choose Vendor and specify the vendor from which the payment is received.
The table displays open documents and, if you selected Display all Transactions, transactions that are not reconciled yet:
A/P invoices, A/P down payment invoices, and manual journal entries in which the vendor is on the credit side are
presented with a negative sign.
The following are presented with a positive sign:
A/P credit memos not based on A/P invoices
This is custom documentation. For more information, please visit SAP Help Portal. 8

6/8/26, 6:08 AM
Manual journal entries in which the vendor is on the debit side
Outgoing payments that are not based on invoices
Amounts that were deposited to the vendor and not to the bank
Checks for payment
 Note
Down payment requests and opening balances transactions are not represented in the table.
3. Select the documents on which you want to base the incoming payment and change the Total Payment amount as
required.
4. Choose to open the Payment Means window, and specify the payment details.
5. Choose OK and then Add.
Result
The open amounts in the base documents are updated according to the payment amount.
If the base documents were fully paid through the incoming payment, the documents are closed and their journal entries
are automatically reconciled.
If the base documents were fully paid, but the payment amount did not match the definition made in the Incoming Amt
Diff. Allowed or Incoming % Diff. Allowed field of the Currencies - Setup window under Administration Setup
Financials Currencies , the following occurs:
Differences caused by a payment amount larger than the amount due (gain) are posted to the account, as defined in
Administration Setup Financials G/L Account Determination Sales General Overpayment A/R
Account .
Differences caused by a payment amount smaller than the amount due (loss) are posted to the account, as defined
in Administration Setup Financials G/L Account Determination Sales General Underpayment A/R
Account .
Example
You received from your vendor an A/P invoice for 994.3 (LC). You paid the exact amount, and then returned the goods and received
an A/P credit memo for 994.3 (LC). You entered the A/P credit memo. The vendor is about to pay you 994.5 (LC) in cash. The table
in the incoming payment document for this vendor is displayed as follows:
Documents for Payment
Document Balance Due Document Type Total Payment
1234 994.3 PC (=A/P Credit Memo) 994.3
The payment amount is actually 994.5 (LC). The amount defined in Administration Setup Financials Currencies
Incoming Amt Diff. Allowed is 1 (LC). The journal entry created by the payment will be:
Journal Entry
G/L Account/BP Debit Credit
Cash on Hand 994.5
This is custom documentation. For more information, please visit SAP Help Portal. 9

6/8/26, 6:08 AM
Overpayment A/R Account 0.2
Vendor 994.3
The journal entries of the A/P credit memo and the incoming payment are reconciled, and the A/P credit memo is closed.
More Information
Incoming Payments
Creating Incoming Payments for Specific Invoices
Context
The following procedure explains how to create an incoming payment for a customer against a specific invoice(s).
Procedure
1. Choose Banking Incoming Payments Incoming Payments .
The Incoming Payments window appears.
2. Choose Customer, and in the Code field, select the required customer code.
The Documents for Payment table displays all unpaid invoices created for the customer.
3. Choose the invoice(s) against which the payment is made.
The cumulative amount of the selected invoices is displayed in the Total Amount Due field.
4. Specify the required details, and choose to open the Payment Means window.
5. Select the appropriate payment means tab, and specify the required details.
6. Choose OK and in the Incoming Payments window, choose Add to add the document to the database.
Results
An incoming payment document is created.
A journal entry that credits the customer and the tax accounts (if tax is involved), and debits the receivable account, is
created.
The journal entries of the incoming payments and the paid invoices are reconciled.
The paid invoices are closed; they no longer appear in the Open Items list and in the Incoming Payments window as
documents for payment.
Related Information
Incoming Payments
Incoming Payments: Customer & Vendor
This is custom documentation. For more information, please visit SAP Help Portal. 10

6/8/26, 6:08 AM
The following fields appear in the general area of the Incoming Payments window.
To open the window, choose Banking Incoming Payments Incoming Payments . Select Customer or Vendor.
Incoming Payments: Customer & Vendor
Name, Bill to
Editable business partner details. To move to the next field, press CTRL+TAB .
Contact Person
Default contact person defined for the business partner. Specify another contact person if required.
Project
To relate the incoming payment to a specific project, specify the required project.
Blanket Agreement
Choose the relevant blanket agreement.
No.
Default numbering series and current number of the incoming payment in the default numbering series. Specify another series if
required.
To document a receipt that was originally created in a notebook, select Manual, then copy the number from the original receipt to
the number field.
Posting Date, Document Date
Current date by default, which you can change as required.
Due Date
By default, the current date, which will be the due date of the business partner row in the journal entry created by the document.
 Note
After you enter the details of the payment means in the Payment Means window and return to the Incoming Payment window,
this field is updated with the weighted average of the due dates defined for the payment means.
If required, you can change this date before you add the document.
Reference
Specify the business partner's reference number for this payment.
Transaction No.
Number of the journal entry created by this document. The number appears after you have added the incoming payment.
Remarks
Enter any remarks about this incoming payment.
Journal Remarks
Enter any details to be displayed in the Remarks field of the journal entry. Displays by default:
Incoming - <business partner code>.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 11

6/8/26, 6:08 AM
If the incoming payment has been generated by the payment wizard, the default display is
Incoming Payments - <business partner code> — <payment run name>.
The payment run name is copied from the Payment Wizard, General Parameters window.
Control Account
Specify the control account for the incoming payment. The control account affects only the amount that is not based on the
invoice in the journal entry of the payment. The default account varies according to your selection of documents.
If you have not selected any invoice or, if the first document that you have selected is a manual journal entry, the default
control account is the one set in the business partner master data.
If you have selected invoices, the default control account is that of the first invoice you have selected.
Created By Payment Wizard
Indicates whether or not the incoming payments were created through the payment wizard. You cannot edit it. Only available when
the option Customer is selected.
Payment on Account
Creates an incoming payment not based on any transaction or document appearing in the table. When you select this option, the
Control Account field appears where you can specify the control account for the incoming payment.
 Note
When a payment on account is included in a payment order run, you cannot cancel it.
Branch
Select a branch from which you want to choose the customer/vendor.
 Note
This field is available only if you have enabled multiple branches.
Total Amount Due
Amount of the payment in local currency, when the incoming payment is created for a local currency business partner.
Total Amount (LC), Total Amount (FC)
Amount of the payment in the foreign currency and in the local currency, according to the defined exchange rate.
Available when the incoming payment is created for an All currency or foreign currency business partner.
Open Balance
Reflects the difference between the amount paid and the amount due, in case it is greater than the amount specified in the
Incoming Amt Diff. Allowed or Incoming % Diff. Allowed field in the Currencies - Setup window under Administration Setup
Financials Currencies .
Add in Sequence
If the payment is not against a specific documents/transactions, closes the documents/transactions according their display order
in the table.
Only available if the Incoming Payment is created for a customer.
Referenced Document (<Number of Documents That the Current Document Refers To>)
This is custom documentation. For more information, please visit SAP Help Portal. 12

6/8/26, 6:08 AM
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Incoming Payments
Incoming Payments: Customer & Vendor - Contents Tab
The following fields appear in the Contents tab of the Incoming Payments window.
To open the window, choose Banking Incoming Payments Incoming Payments , and select Customer or Vendor.
This is custom documentation. For more information, please visit SAP Help Portal. 13

6/8/26, 6:08 AM
Contents Tab Fields
Document No.
Displays the document number. Click to display the document. This column is displayed only when the Customer Ref. No is
deselected.
Installment
Displays the successive number of the installment within the total number of the installments included in the specific invoice. The
invoice is displayed several times according to the number of installments still to be paid.
If not all installments are paid in the same document, the invoice will not be reconciled automatically.
Date
Displays the posting date of the document/transaction.
*
An asterisk is displayed in the line of every invoice or installment whose due date has passed.
Overdue Days
If the open item due date is earlier than the posting date of the manual payment, the number of overdue days is displayed in
red.
If the open item due date is equal to the posting date of the manual payment, 0 is displayed in black.
If the item is not overdue (that is, the open item due date is after the posting date of the manual payment), the number of
overdue days is displayed in black, preceded by a minus (-) sign.
Total
Displays the total amount due for the document/transaction.
WT Amount
Displays the withholding tax amount included in the document.
Balance Due
Displays the amount still to be paid from the document/transaction.
If a partial payment for that record has already been made, or if a credit memo was created for a partial amount, this value is lower
than the value displayed in the Total field.
Blocked
Displays an asterisk (*) if you selected Y in either of the following fields:
The Payment Block field of the manual journal entry line
The Payment Block field on the Accounting tab of the marketing document
Cash Discount %
Displays the rate of the cash discount defined for the business partner, depends on the incoming payment date and the invoice
date. Change if required.
Document Type
Displays the type of document or transaction. For example, IN represents A/R invoice.
This is custom documentation. For more information, please visit SAP Help Portal. 14

6/8/26, 6:08 AM
Total Payment
Displays the amount that is outstanding on an invoice. Change this amount if the incoming payment is only for part of the invoice
amount. The system proposes the balance due as the amount to be paid.
Total Rounding Amount
This column is displayed only when the selected rounding method is By Currency. In this case, the amount displayed in this field is
the difference between the original amount of the document and its rounded amount.
Distr. Rule
If required, specify a distribution rule for the row.
Project
Displays the project specified in the document.
Payment Order Run
Displays whether this transaction is included in a payment order run. You will be warned when creating payments for such
transactions.
More Information
Incoming Payments
Incoming Payments: Account
The following are the fields in the Incoming Payments window.
To open the window, choose Banking Incoming Payments Incoming Payments and select Account .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Incoming Payments for Account
No.
Default numbering series and current number of the incoming payment in the default numbering series. Specify another series if
required.
To document a receipt originally created in a note book, choose Manual and copy the number from the original receipt to the
number field.
Posting Date, Document Date
Current date by default. Change the dates if required.
Due Date
By default the current date, which will be the due date of the customer row in the journal entry created by the document.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 15

6/8/26, 6:08 AM
After you enter the details of the payment means in the Payment Means window, and return to the Incoming Payment window,
the field is updated with the weighted average of the due dates defined for the payment means.
If required, you can change this date before you add the document.
Reference
Enter any additional reference if required.
Transaction No.
Number of the journal entry created by this document. The number appears after you have added the incoming payment.
Branch
Select a branch from which you want to choose an account.
 Note
This field is available only if you have enabled multiple branches.
Project
To relate the incoming payment to a specific project, specify the required project.
Doc. Currency
Document’s currency, by default in the local currency Specify another currency if required.
If you choose foreign currency, the exchange rate defined in the Exchange Rates and Indexes table for the selected currency for
the document's posting date is displayed. You can change this rate if required.
Remarks
Enter any remarks about this incoming payment.
Journal Remarks
Enter the details to be displayed in the Remarks field of the journal entry. Includes by default: Incoming – Account Code. If
the incoming payment is for more than one account, the code is the last account in the document.
Doc. Remarks
Enter any relevant details regarding the amount paid for this account.
Amount
Specify the amount referred to the account.
Total Amount Due
Total amount of the payment in local currency.
Appears only when the selected document currency is the local currency.
Amount Due (FC), Amount Due (LC)
Amount of the payment in the selected foreign currency or local currency depending on the exchange rate defined in the
document. Appear if the document currency is other than the local currency.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 16

6/8/26, 6:08 AM
Incoming Payments
Incoming Payments: Attachments Tab
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
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Payment Means
Use this window to record and view the details of the means of payment combined to make an incoming or outgoing payment. The
following payment means are supported in all localizations:
Check
This is custom documentation. For more information, please visit SAP Help Portal. 17

6/8/26, 6:08 AM
Bank transfer
Credit card
Cash
Bill of Exchange is supported by the SAP Business One software versions for the relevant countries/regions. Details are available in
the localization-specific online help file under Help Documentation Localization-Specific Info .
To open the window, choose Banking Incoming Payments Incoming Payments . Alternatively, choose Banking
Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose .
Payment Means: General Area
Use this window to specify payment details. To open the general area of the Payment Means window, choose Banking
Incoming/Outgoing Payments Incoming/Outgoing Payments .
On the toolbar or in the payment, choose .
Payment Means General Area Fields
Currency
Currency of the payment, as defined in the Incoming/Outgoing Payments window. Specify another currency if required. If the
currency defined for the G/L account/business partner is the local currency, the displayed currency cannot be changed.
Overall Amount
Amount to be paid, comprising:
Invoices selected for payment
Information in the relevant Payments window
Any amounts that are not contained in incoming or outgoing invoices (only if Display Journal Entries was selected)
Balance Due
When the amounts to be covered by the different payment means have been entered, the balance due is equal to zero.
Bank Charge
Specify the amount of bank charge for the particular payment.
Paid
Total amount paid, which is the sum of the amounts entered in the Payment Means window.
Payment Means: Check Tab
To access the Check tab of the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Check tab.
Payment Means: Check Tab Fields
G/L Account
This is custom documentation. For more information, please visit SAP Help Portal. 18

6/8/26, 6:08 AM
For incoming payment documents:
Specify the account to be debited when the incoming payment is added. The account displayed is defined in Administration
Setup Financials G/L Account Determination Sales General Checks Received .
G/L Account (Table Area)
For outgoing payment documents:
Account defined for the selected bank in the House Bank Accounts – Setup window. To have a different account credited when the
outgoing payment is added, press TAB and select the required account. You can issue checks from different accounts within the
same outgoing payment if required.
Search by Bank Code
Searches for the required bank by bank code instead of bank name.
Due Date
The current date is the default date for the first check. Change if necessary.
Country/Region
Specify the country/region where the bank issuing the check is located.
Bank Name
Specify the relevant bank. Available options are banks defined for the selected country/region in the Banks – Setup window.
Branch, Account, Check No.
For incoming payment documents:
Specify the numbers of the branch, account, and check as printed on the check received.
Branch, Account
For outgoing payment documents:
Numbers of the branch and bank account of the credited G/L account. These details are taken from the House Bank Accounts –
Setup window.
Manual Check
For outgoing payments only:
To manually specify the check number, select the checkbox. This is useful if the check is not printed through SAP Business One,
but written manually.
Check No.
Incoming Payments
Specify the number of the check received.
Outgoing Payments
If you print checks from SAP Business One, this field is disabled and the check number is zero until the check is printed, when the
check number is updated automatically.
If you issue checks manually, select the checkbox Manual Check and specify here the check number.
Endors.
Specify whether endorsement of the check should be allowed or not.
This is custom documentation. For more information, please visit SAP Help Portal. 19

6/8/26, 6:08 AM
The default value of this column is determined by the Endorsable Checks from This BP checkbox on the Payment Terms tab of
the Business Partner Master Data window. When the Endorsable Checks from This BP checkbox is selected, in the payments
created for this business partner, the Endors. column is set to Yes by default. However, you can always change the Endors. status
before adding the payment.
Amount
Specify the amount of the check.
Originally Issued By
For incoming payments only:
Enter the original issuer of the check. This information is helpful if an incoming check bounces.
 Note
This column is available in most of the localizations. For additional information, see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Fiscal ID
For incoming payments only:
Enter the fiscal ID of the original issuer of the check. This information is helpful if an incoming check bounces.
 Note
This column is available in most of the localizations. For additional information, see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Endorse
For outgoing payments only:
Select the checkbox to enable the Endorsable Check No. field, from which you can choose an endorsable check and endorse it to
the business partner of the outgoing payment.
This checkbox is available only if you have selected the This BP Accepts Endorsed Checks checkbox on the Payment Terms tab of
the Business Partner Master Data window for the business partner of the outgoing payment.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This checkbox is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Endorsable Check No.
For outgoing payments only:
Press TAB to open the List of Checks window, in which you can select an endorsable check and endorse it to the business
partner of the outgoing payment. After you choose an endorsable check, its information appears in the line, and you cannot edit it.
This field is available only if you have selected the Endorse checkbox on the Check tab of the Payment Means window.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 20

6/8/26, 6:08 AM
This checkbox is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
More Information
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Bank Transfer Tab
To access the Bank Transfer tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Bank Transfer tab.
Payment Means: Bank Transfer Tab Fields
G/L Account
Specify the G/L account from the chart of accounts to/from which the bank transfer is to be posted.
Transfer Date
Specify the bank transfer date.
Reference
Specify a reference, such as the intended purpose, for the bank transfer.
Total
Specify the bank transfer amount.
More Information
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Credit Card Tab
To access the Credit Card tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Credit Card tab.
 Note
If you choose to pay by credit card or receive a payment through credit card, the corresponding journal entry will be non-
changeable.
Payment Means: Credit Card Tab Fields
Credit Card Name
This is custom documentation. For more information, please visit SAP Help Portal. 21

6/8/26, 6:08 AM
Specify the credit card used to make the payment.
G/L Account
Incoming Payments
The account defined for the selected credit card in the Credit Card – Setup window. If required, specify another account.
Outgoing Payments
Specify the account to be credited when the outgoing payment is added.
Credit Card No., Valid Until
For incoming payment documents:
Specify the number and valid-until date (in the format MM/YY) of the credit card.
ID No., Telephone No.
Specify the ID number and the phone number of the card owner.
Payment Method
Specify the required payment method.
Amount Due
Specify the amount paid with the credit card.
No. of Payments, First Partial Payment, Each Add. Payment
Specify the number of partial payments for this transaction, and the amount of the first partial payment.
SAP Business One automatically calculates the amount that is to be paid with future payments, and displays it in the Each Add.
Payment field. Rounding results are added to the first payment.
 Note
Available for incoming payment documents only if the selected payment method enables the creation of multiple partial
payments.
Voucher No.
Specify the number of the credit card voucher.
Transaction Type
For incoming payment documents:
Specify whether the transaction is a telephone transaction or a regular transaction.
Split Credit Voucher
For outgoing payment documents:
Creates a separate row in the journal entry for each partial payment.
Vouchers
All credit cards defined in the Credit Cards – Setup window. The credit card selected in the Credit Card Name field is marked. To
create vouchers for an additional credit card, choose Define New in this list.
Tel. for Approval, Company ID
This is custom documentation. For more information, please visit SAP Help Portal. 22

6/8/26, 6:08 AM
Telephone number for approval as defined for the credit card, and company ID that should be used when calling for approval.
Total
Total amount paid with this transaction.
More Information
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Cash Tab
To access the Cash tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Cash tab.
Payment Means: Cash Tab Fields
G/L Account
For incoming payment documents, one of the following is displayed:
Account defined in the Cash on Hand field on the General subtab of the Sales tab in the G/L Accounts Determination
window.
Default account defined for the user in the Cash Acct field on the Defaults tab in the User Default window.
If required, select another account. The selected account is debited once the incoming payment is added.
G/L Accounts (op)
For outgoing payment documents, specify the account to be credited when the outgoing payment is added.
Total
Specify the total amount of the cash payment.
More Information
Payment Means
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Check Register
SAP Business One uses the check register to store information about all checks that have been received in the company. The
check details are recorded in the Payment Means window during the creation of an incoming document, and updated when the
check is deposited.
This is custom documentation. For more information, please visit SAP Help Portal. 23

6/8/26, 6:08 AM
The check register reflects the current status of every check received, which means that you can find out at any time when and
where the check was deposited, or whether it was endorsed or canceled.
More Information
Check Register – Selection Criteria
Check Register Window
Endorsing Checks Using Manual Journal Entry
Prerequisites
The check to endorse has not been canceled or deposited.
Context
The check endorsement function enables you to forward an incoming check (for example, from a customer) to a third party (a
vendor) without having to deposit it first.
You can also select an endorsable third-party check in an outgoing payment as a payment means. For more information, see
Endorsing Checks in Outgoing Payments.
Procedure
1. Choose Banking Incoming Payments Check Register.
2. In the Check Register – Selection Criteria window, specify the relevant parameters and choose OK.
3. Select the check to endorse. If the value in the Endorsable field is No, change the entry to Yes.
4. Choose Endorsement.
The Journal Entry window appears.
5. SAP Business One automatically creates the first row of the journal entry and credits the check fund account. To debit the
endorsee business partner/account, add another row.
6. To create the journal entry, choose Add.
Results
After you have endorsed a check, you can no longer deposit or cancel it.
Related Information
Check Register
Canceling Checks
You can cancel a check that was received as an incoming payment together with the incoming payment document, whether the
check is deposited or not.
This is custom documentation. For more information, please visit SAP Help Portal. 24

6/8/26, 6:08 AM
To view the status of a check, select the check in the Check Register window, and select the Check Status tab.
Procedure
Non-Deposited Check Cancellation
To cancel non-deposited checks, follow the procedure below:
1. From the SAP Business One Main Menu, choose Banking Incoming Payments Check Register .
2. In the Check Register – Selection Criteria window, specify the required parameters and choose OK.
3. In the table, right-click the check you want to cancel, and choose Cancel Check.
4. When asked whether to cancel the check, choose Yes to complete the cancellation.
 Note
If the current system date is not the original document date, the Cancellation Options window appears.
Select one of the following:
Current System Date – to assign to the transaction resulting from the cancellation the current date
Original Document Date – to assign to the transaction resulting from the cancellation the same date (posting
date, due date, and document date) as is assigned to the canceled document
Choose OK to complete the cancellation.
Deposited Check Cancellation
To cancel deposited checks, follow the procedure below:
 Note
You cannot cancel checks that are deposited through the Postdated Check Deposit window.
1. From the SAP Business One Main Menu, choose Banking Incoming Payments Check Register .
2. In the Check Register – Selection Criteria window, specify the required parameters and choose OK.
3. In the table, right-click the check you want to cancel, and choose Cancel Deposit and Payment.
4. When asked whether to cancel the check, choose Yes to complete the cancellation.
 Note
If the current system date is not the original document date, the Cancellation Options window appears.
Select one of the following:
Current System Date – to assign to the transaction resulting from the cancellation the current date
Original Document Date – to assign to the transaction resulting from the cancellation the same date (posting
date, due date, and document date) as is assigned to the canceled document.
Choose OK to complete the cancellation.
Result
This is custom documentation. For more information, please visit SAP Help Portal. 25

6/8/26, 6:08 AM
A reverse journal entry is created in order to cancel the journal entry created when the incoming payment was added. The
date assigned to this transaction is according to the selection you made in the Cancellation Options window. The Remarks
field of this journal entry indicates that this is a reverse transaction for a specific incoming payment.
If the check is the only payment means related to the incoming payment, the Journal Remarks field in the related incoming
payment displays the text: Canceled.
For deposited check cancellation, a reverse deposit document of negative amount is created. The date assigned to this
deposit is according to the selection you made in the Cancellation Options window. It contains only the check you have
chosen to cancel.
For deposited check cancellation, in the deposit document in which the check is canceled, the Canceled column for the
canceled check displays the text: Yes.
More Information
Check Register
Check Register - Selection Criteria
Use this window to specify selection criteria for the Check Register.
To open the window, choose Banking Incoming Payments Check Register .
Selection Criteria
Check Date From...To...
To locate a check according to its date, specify a range of due dates.
Date of Receipt From...To...
To find checks received on specific dates, specify a date range for postings of incoming payments.
Check Number From...To...
To find a check according to its check number, specify a range of check numbers.
Check Amount From...To
To locate checks within a range of amounts or of a specific amount, specify a range of amounts.
Deposit Status
Specify the kind of checks to be retrieved:
Only deposited checks
Only checks that still are to be deposited
Both deposited and to be deposited (select All).
Endorsed
Specify the kind of checks to be retrieved:
Only endorsed checks
Only checks that are not endorsed
This is custom documentation. For more information, please visit SAP Help Portal. 26

6/8/26, 6:08 AM
Only endorsable checks
Only checks that are not endorsable
All checks
 Note
This checkbox is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Check Register Window
This window displays the Check Register according to the defined selection criteria.
Check Register Window
Check No.
Search for a specific check by its number.
Currency
Specify a currency to display only checks created in this currency.
Deposit Status
Specify whether to display deposited checks, checks that have not been deposited, or both. This selection criterion is active only
for checks appearing in this window.
Sequence No., Date, Check No., Bank, Branch, Account, Endorsed, Amount
Details regarding each check displayed.
Total
Total amount of all checks shown in the window.
 Note
Since not all checks documented in the check fund are displayed, this total is not equal to the check fund balance.
Date, Check No., Bank, Branch, Account, Endorsable, Amount
Details about the check selected in the table.
Deposit
Details regarding the selected check, if it has been deposited:
Deposit number
Deposit date
Account or business partner for which the check was deposited
Bank, branch and account in which the check was deposited
All details are taken from the deposit document as posted in SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 27

6/8/26, 6:08 AM
Payment
Details regarding the incoming payment document that was created for the selected check, and the outgoing payment document
in which the check was endorsed, if the selected check is used as a third-party check in the outgoing payment.
 Note
The outgoing payment information is available in most of the localizations. For additional information see the localization-
specific online help file under: Help Documentation Localization-Specific Info .
Endorsed, Deposited, Canceled
Information about whether the selected check has been endorsed, deposited, or canceled.
Cancellation Journal Entry
Number of the journal entry that cancels the one created when the incoming payment of a check is added.
Rejected by Bank
Select Yes if the bank rejects to cash the check.
 Note
This field is available for most of the localizations. For additional information see the localization-specific online help file under:
Help Documentation Localization-Specific Info .
Endorsement
Opens a journal entry window with a partial transaction that you must complete in order to perform the check endorsement.
Available only if the selected check is endorsable.
Credit Card Management
SAP Business One uses the credit card management function to store information about all credit card vouchers that are recorded
in the Payment Means window when an incoming payment document is created. When a credit card voucher is deposited, this
information is updated.
The credit card management function reflects the current status of every credit card voucher recorded, which means that you can
find out at any time when a credit card voucher was deposited, and where, or whether it was endorsed.
More Information
Credit Card Management – Selection Criteria
Credit Card Management Window
Cancelling Credit Card Vouchers
Procedure
1. Choose Banking Incoming Payments Credit Card Management .
2. In the Credit Card Management – Selection Criteria window, specify the required parameters and choose OK.
3. Select the credit card voucher you want to cancel.
This is custom documentation. For more information, please visit SAP Help Portal. 28

6/8/26, 6:08 AM
 Note
If the value in the Split Credit Voucher field in the Payment Means window was Yes, separate credit card vouchers were
created for each payment and are displayed in separate rows in the Credit Card Management window.
If the value in this field was No, a row representing all credit card payments is displayed, and cancellation is available for
the entire amount.
4. Right-click the voucher and choose Cancel.
The Journal Entry window appears. It automatically displays rows that represent the cancelled credit card vouchers.
5. Complete the journal entry and choose Add to record it.
Results
The selected credit card voucher is cancelled. The credit card register account is credited, and the G/L account/business partner
you selected when completing the journal entry is debited.
Related Information
Credit Card Management
Endorsing Credit Card Vouchers
Prerequisites
You can endorse only credit card vouchers that are not deposited yet.
Context
The credit card voucher endorsement function enables you to forward an incoming credit card voucher (for example, from a
customer) to a third party (a vendor) without having to deposit it first.
Procedure
1. Choose Banking Incoming Payments Credit Card Management .
2. In the Credit Card Management – Selection Criteria window, specify the required parameters and choose OK.
3. Select the credit card voucher to be endorsed.
 Note
If the value in the Split Credit Voucher field in the Payment Means window is Yes, a separate credit card voucher is
created for each payment. The payments are displayed in separate rows in the Credit Card Management window.
If the value in this field is No, a row representing all credit card payments is displayed, and cancellation is available for
the entire amount.
4. Choose Endorsement.
The Journal Entry window appears. The row(s) displayed in the Journal Entry window credit the credit card register and
represent the credit card voucher(s) included in the selected payment.
5. Complete the journal entry by debiting the relevant G/L account/business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 29

6/8/26, 6:08 AM
6. To create the journal entry, choose Add.
Results
The selected credit card payment is endorsed and cannot be deposited.
Related Information
Credit Card Management
Credit Card Management - Selection Criteria
Use this window to specify selection criteria for Credit Card Management.
To open the window, choose Banking Incoming Payments Credit Card Management .
Selection Criteria
Credit Card From...To...
To display the vouchers created for a range of credit cards, specify that range here.
Date From...To...
To display vouchers whose dates fall within a particular range, specify these dates here.
Display Undeposited Vouchers Only
Displays vouchers that have not been deposited. If you do not select this option, both deposited and undeposited vouchers are
displayed.
Credit Card Management Window
This window displays Credit Card Management according to the defined selection criteria.
Credit Card Management Window
Sequence No., Card Name, Voucher No., Date, Card No., Payment Method, Total
Information relating to the selected range of credit card vouchers.
Find Voucher No.
Specify the number of the voucher you want to trace. SAP Business One marks the required voucher. If a voucher with this number
cannot be found, the voucher with the closest number is marked.
Currency
To view only the credit card vouchers created for a specific currency, specify this currency.
Credit Card
To view only the credit card vouchers created for a specific credit card, specify this credit card.
Credit Card, Voucher No., Date, Card No., Ref., Payment Method, # of Paym., Total, First Payment, Each Add. Payment, Total Not
Paid
This is custom documentation. For more information, please visit SAP Help Portal. 30

6/8/26, 6:08 AM
This information about the marked voucher is displayed when you select a credit card voucher from the table. The information is
taken from the Payment Means window.
Incoming Payment No., Date, Customer Code, Customer Name.
Information regarding the incoming payment document through which the selected credit card voucher was created.
Transaction Type
Transaction type of the credit card payment: regular or telephone transaction. This information is taken from the Payment Means
window.
Cancelled
Shows whether or not the credit card voucher was cancelled.
Deposited
Indicates whether or not the credit card voucher was deposited.
Deposit No., Deposit Date, G/L Account / BP
Information about the deposit document made for the selected credit card voucher.
Endorsed
Indicates whether or not the credit card voucher was endorsed.
Bank, Branch, Account
Information from the corresponding fields of the deposit document, if the credit card voucher was deposited.
Endorsement
Endorses the selected credit card voucher. A journal entry window with a partial transaction appears. To perform the endorsement,
complete the transaction.
Credit Card Summary
Use this function to display and update credit card voucher references that are received from credit card companies.
More Information
Credit Card Summary – Selection Criteria
Credit Card Summary Window
Credit Card Vouchers for Update Window
Updating References for Credit Card Vouchers
Context
Use the procedure to update the references received from the credit card company in the credit card vouchers.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 31

6/8/26, 6:08 AM
1. Choose Banking Incoming Payments Credit Card Summary .
2. In the Credit Card Summary – Selection Criteria window, specify the parameters required to display the credit card
vouchers to update.
3. Choose OK.
The Credit Card Summary window appears, displaying the credit card vouchers according to your selection criteria.
4. In the Reference column, specify the appropriate reference for each credit card voucher.
5. Choose Update.
Related Information
Credit Card Summary
Credit Card Summary - Selection Criteria
Use this window to specify selection criteria for the Credit Card Summary.
To open the window, choose Banking Incoming Payments Credit Card Summary .
Selection Criteria
Creation Date From...To
To display all credit card vouchers created within a particular date range, specify these dates here.
Currency
To display credit card vouchers created for a specific currency, specify the relevant currency.
Vendor
To display credit card vouchers assigned to a specific credit vendor, specify the relevant credit vendor.
Display Documents with No Reference Only
Displays only credit card vouchers to which a reference has not yet been assigned.
Credit Card Summary Window
This window displays the Credit Card Summary according to your defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Credit Card Summary Window
Date, Currency
Creation date and currency of the incoming payment.
No. of Vouchers, Total
This is custom documentation. For more information, please visit SAP Help Portal. 32

6/8/26, 6:08 AM
Number of vouchers created in each incoming payment document and total amount of the vouchers.
 Note
If the incoming payment document contains an additional means of payment (for example, cash), the amount displayed in the
Total column is different from the total amount of the incoming payment document.
Reference
Specify a reference for the credit card vouchers. This reference is relevant for all vouchers included in the incoming payment
document.
Credit Card Vouchers for Update Window
The following are the fields in the Credit Card Vouchers for Update window.
To open the window, choose Banking Incoming Payments Credit Card Summary . In the Credit Card Summary –
Selection Criteria window, specify the required parameters and choose OK. In the Credit Card Summary window, double-click the
required row .
Credit Card Vouchers for Update
Date, Credit Card, Voucher Number, Total
Details from the credit card vouchers, which cannot be edited.
Reference
Specify the reference number received from the credit vendor.
More Information
Credit Card Summary
Deposit
Use this function to deposit received checks, credit card vouchers, and cash.
To create or view deposits, choose Banking Deposits Deposit .
In the interactive graphics below, you can hover over each area for a short description and choose the highlighted areas for more
information.
This is custom documentation. For more information, please visit SAP Help Portal. 33

6/8/26, 6:08 AM
Please note that image maps are not interactive in PDF outputs.
Deposit Window
Use the different tabs in this window to deposit received checks, credit card vouchers, and cash.
To open the window, choose Banking Deposits Deposits .
Deposit: General Area
Deposit No., Series
Deposit number according to the selected numbering Series.
Deposit Date
Specify the date of the deposit. The current date is displayed by default.
Considered From...To...
Available only if Postdated Checks is selected on the Checks tab. Specify the date range within which checks are to be considered
as postdated.
Considered Until
Available only if Cash Checks is selected on the Checks tab. Enter a date to specify that all checks with a due date equal to or
earlier than this date should be considered as cash.
Date From...To...
Available only if the Credit Card tab is selected. Enter a date range to specify that credit card vouchers within this range should be
deposited.
Deposit Currency
Specify the currency of the deposit. Once a currency is selected, only checks/credit card vouchers/cash of this currency may be
deposited.
[G/L Account/BP]
When the Checks tab or Credit Card tab is selected, choose whether to perform the deposit to a bank account or to a business
partner, and specify the G/L account or BP code.
This is custom documentation. For more information, please visit SAP Help Portal. 34

6/8/26, 6:08 AM
 Note
If you want to deposit checks to business partners, ensure that the checks are endorsable. After being deposited to business
partners, a check is considered as both deposited and endorsed. When this kind of check is canceled, it is also considered as
not endorsed.
Deferred Pmt Acct
Specify the account to which credit card vouchers with a due date later than the deposit date should be deposited. Available only if
the Credit Card tab is selected.
Bank, Branch, Account
Specify the details of the bank in which the deposit was made, as displayed on the deposit form.
Bank Reference
Specify the reference assigned to the deposit by the bank.
Payer
Specify the name of the person who made the deposit.
Branch
Select a branch for which you want to create the deposit.
 Note
This field is available only if you have enabled multiple branches.
Journal Remarks
Specify any remarks relevant to the journal entry created by the deposit.
Trans. No.
Journal entry number for this deposit.
Total Commissions
Clicking opens the Commission window, where you can define the commission rate that should be paid for the deposit.
Available only if the Credit Card tab is selected.
Reconcile Amounts After Deposit
Automatically performs reconciliation of the amounts deposited. Available only if the Checks or Credit Card tab is selected.
Deposit: Checks Tab
To access the Checks tab in the Deposit window, choose Banking Deposits Deposit Checks .
Deposit Window: Check Tab Fields
Display Checks From
Specify whether to display checks received by all check funds or by a specific check fund.
Find Check No.
To trace a specific check, specify the number of the required check. SAP Business One marks the required check.
This is custom documentation. For more information, please visit SAP Help Portal. 35

6/8/26, 6:08 AM
Cash Checks
Displays checks with due dates earlier than or the same as the date entered in the Considered Until field.
Postdated Checks
Displays checks with due dates later than or the same as the date entered in the Considered Until field.
Date, Check, Bank, Branch, Account No., BP/Account Code, BP/Account Name, Check Amount, Project, Incoming Payment
Relevant information regarding the checks to be deposited. The details are taken from the checks themselves.
Canceled
Cancellation status of the deposit row.
 Note
This field is not visible by default. You can set it to visible through the Form Settings window.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
More Information
Deposit
Deposit: Credit Card Tab
To access the Credit Card tab in the Deposit window, choose Banking Deposits Deposit Credit Card .
Deposit: Credit Card Tab
Find Voucher No.
To trace a specific credit card voucher, specify the number of this voucher. SAP Business One marks the required voucher.
Display the Following Vouchers
Specify the credit card fund in which the credit card vouchers for deposit are found. All displays all credit card vouchers that meet
the other parameters defined.
Voucher No., Date, Card Name, Ref., Payment Method, BP/Account Code, BP/Account Name, # of Payments, Total, Project,
Incoming Payment
Information about the credit card vouchers to be deposited. The details are from the incoming payment documents relating to the
displayed vouchers.
The row below the table displays the number of credit card vouchers selected and their cumulative amount.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 36

6/8/26, 6:08 AM
Deposit
Commission Window
Commission Window
To open the Commission window, choose Banking Deposits Deposit Credit Card Total Commissions .
Commission Window Fields
Commission Account, Standard Commission Amount
Specify the account used for commission payment and the amount of commission to be paid.
Tax Account, Tax Amount
If you also need to pay tax, specify the tax account and tax amount.
 Note
The tax account should be defined previously for processing all currencies if taxes in non-Local Currencies are handled.
Commission Due Date
Specify the due date for the commission entry in the transaction.
Project
If required, specify the project to which the commission is allocated.
Distr. Rule
If required, specify the distribution rule for the commission. By default, this field is empty.
If you define the distribution rule here, it appears in the Distr. Rule field for the corresponding journal entry row.
If you leave this field empty, the default distribution rule for the commission G/L account appears in the Distr. Rule field for
the corresponding journal entry row.
More Information
Deposit
Deposit: Cash Tab
To access the Cash tab in the Deposit window, choose Banking Deposits Deposit Cash .
Deposit Window: Cash Tab Fields
G/L Account
Cash on Hand account from which the deposit is defined. The account is defined in Administration Setup Financials G/L
Account Determination Sales . If required, you can select another account.
Balance
This is custom documentation. For more information, please visit SAP Help Portal. 37

6/8/26, 6:08 AM
Balance of the selected cash account. If the balance is negative, there is a debit balance, which is the maximum amount that can
be deposited.
Amount
Specify the amount you want to deposit. You cannot deposit an amount that is larger than the cash fund balance.
Primary Form Item
If the bank account you specified is cash flow relevant, you can specify the cash flow line item or define a new assignment in the
Combined Cash Flow Assignment window.
More Information
Deposit
Deposit: Attachments Tab
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
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
This is custom documentation. For more information, please visit SAP Help Portal. 38

6/8/26, 6:08 AM
Related Information
General Settings: Path Tab
Depositing Checks
Follow this procedure to deposit cash and postdated checks.
Procedure
1. Choose Banking Deposits Deposit Checks.
2. Select one of the following:
Cash Checks – if you want to deposit checks as cash. If you select this option, go to step 3.
Postdated Checks – if you want to deposit checks as postdated. If you select this option, go to step 4.
3. In the Considered Until field, specify the date until which checks with the same or an earlier due date are considered as cash
checks. The current date is displayed by default. Go to step 5.
4. In the Consider From...To... fields, specify a date range. All checks with a due date within this range are considered as postdated
checks. The dates of the next day and the last day of the fiscal year are displayed by default.
5. To display in the table the check you want to deposit, specify all the parameters (Currency, Display Checks From).
6. Select the checks to be deposited.
7. To record the deposit in the database, choose Add.
Result
When a deposit is added, the following occur:
A journal entry is created. Its number is displayed on the deposit document.
The status of the deposited checks changes. When you view these checks in the check fund, you see the details of the
deposit.
More Information
Deposit
Depositing Cash
Procedure
1. Choose Banking Deposits Deposit Cash .
2. Select the deposit currency and the bank account to which the money should be deposited.
3. Select the G/L account from which the deposit is made and enter the deposit amount.
This is custom documentation. For more information, please visit SAP Help Portal. 39

6/8/26, 6:08 AM
 Note
You cannot deposit amounts larger than the account balance.
4. Enter all relevant details and choose Add.
Results
When you add a cash deposit, a journal entry that transfers the deposited amount from the G/L account to the bank account is
created.
Related Information
Deposit
Depositing Credit Card Vouchers
Procedure
1. Choose Banking Deposits Deposit Credit Card .
2. Specify a date range to display vouchers within the range. If you do not define a range, all vouchers are displayed.
3. Select the G/L account or business partner to which the selected vouchers whose due date is the same as or earlier than
the current date will be deposited.
4. Select the G/L account to which the selected vouchers whose due date is later than the current date will be deposited.
5. Select the vouchers you want to deposit.
6. If a commission is involved in the deposit, choose next to Total Commissions and choose Update.
7. In the Commission window, specify the relevant data.
8. Choose Add.
Results
A journal entry is created.
The status of the deposited vouchers is updated. When you display them in Credit Card Management, the value in the
Deposited field is Yes.
If Reconcile Amount After Deposit was selected in the Deposit window, the transactions created by the deposit and by the
incoming payments are reconciled.
Related Information
Deposit
Canceling Deposits from Checks
Follow these procedures to fully or partially cancel a deposit from checks.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 40

6/8/26, 6:08 AM
Canceling deposits does not cancel related checks or payments. However, if related incoming payments were already canceled,
canceling deposits does cancel related checks.
 Note
When a deposit contains checks that are deposited through the Postdated Check Deposit window, you cannot fully cancel the
deposit. However, you can cancel the other part of the deposit using the Cancel Row option in the Deposit window or the
Cancel Deposit option in the Check Register window.
Procedure
Full Cancellation
To fully cancel a deposit from checks, follow the procedure below:
1. From the SAP Business One Main Menu, choose Banking Deposits Deposit and display the deposit you want to
cancel.
2. In the document, right-click and choose Cancel.
3. When asked whether to cancel the deposit, choose Yes to complete the cancellation.
 Note
If the deposit contains canceled checks (that is, the deposit was already partially canceled), this deposit will be canceled
excluding the canceled checks.
Partial Cancellation
To partially cancel a deposit from checks, do one of the following:
Cancel the deposit through the Deposit window:
1. From the SAP Business One Main Menu, choose Banking Deposits Deposit and display the required deposit.
2. In the table, right-click the row that you want to cancel, and choose Cancel Row.
3. When asked whether to partially cancel the deposit, choose Yes to complete the cancellation.
Cancel the deposit through the Check Register window:
1. From the SAP Business One Main Menu, choose Banking Incoming Payments Check Register .
2. In the Check Register – Selection Criteria window, specify the required parameters and choose OK.
3. In the table, right-click the check the deposit of which you want to cancel, and choose Cancel Deposit.
4. When asked whether to partially cancel the deposit, choose Yes to complete the cancellation.
Result
A reverse deposit document of negative amount is created. If it is a partial cancellation, the reverse deposit only contains
the check the deposit of which you have chosen to cancel. The Journal Remarks field of the reverse deposit displays the
text:
<journal remarks of the canceled deposit>, Reverse Entry for Deposit No. <deposit number
of the canceled deposit>
.
This is custom documentation. For more information, please visit SAP Help Portal. 41

6/8/26, 6:08 AM
The Journal Remarks field in the fully canceled deposit displays the text: Canceled.
The Canceled column for the canceled row displays the text: Yes.
The internal reconciliation performed as a result of adding the deposit is canceled.
More Information
Deposit
Outgoing Payments Main-Menu Option
Use the features listed under Outgoing Payments to:
Create outgoing payments for customers, vendors and accounts for various payment means
Create and void checks for a payment for miscellaneous purposes, such as a present for an employee
Create, trace and process drafts of outgoing payment documents and drafts of checks for payment
To use the features, choose Banking Outgoing Payments .
All the images here in this topic are interactive. Hover over each area for a short description. Choose the highlighted areas for more
information.
Operation of Outgoing Payments:
Please note that image maps are not interactive in PDF outputs.
Operations of Checks for Payment:
Please note that image maps are not interactive in PDF outputs.
More Information
Payment Drafts Report
Check Register Report
This is custom documentation. For more information, please visit SAP Help Portal. 42

6/8/26, 6:08 AM
Outgoing Payments
Use this window to create a record each time your company issues a payment to a customer, vendor or account.
The outgoing payment document can be created for the following payment means:
cash
check
credit card
bank transfer
Once the outgoing payment is added, an appropriate journal entry is created.
When creating an outgoing payment to clear (fully or partially) a specific document or transaction, an internal reconciliation
automatically takes place.
To open the window, choose Banking Outgoing Payments Outgoing Payments .
More Information
Creating Outgoing Payments
Outgoing Payments: Vendor
Outgoing Payments: Account
Outgoing Payments: Customer
Payment Means
Creating Outgoing Payments for Multiple G/L Accounts
When outgoing payments are created, it may be necessary to credit more than one G/L account, and to split the amount paid
among several projects and cost centers using a distribution rule.
 Example
Employee salary payment, payment or electrical expenses that should be split among cost centers of several departments.
Procedure
1. Choose Banking Outgoing Payments Outgoing Payments .
The Outgoing Payments window appears.
2. Select Account.
3. In the To Order of and Pay To fields, specify the relevant details and choose the document currency.
4. In the table area, select each G/L account to be involved in the payment, and assign the relevant amount.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 43

6/8/26, 6:08 AM
The available accounts are those with the same currency as the document currency and the ones defined as All
currency.
5. To allocate the amount assigned to each account to the required cost center or project, do the following:
a. Open the Form Settings – Outgoing Payments window, select the options Visible and Active for the columns Distr.
Rule and/or Project, and choose OK.
The columns are added to the table area.
 Note
If you selected the In Separate Columns radio button on the Cost Accounting tab of the General Settings
window under Administration System Initialization General Settings , you can select the options Visible
and Active for the XXX columns, where XXX is the descriptions of active dimensions.
If you defined a project and/or distribution rule for the accounts appearing in the table (in Financials Chart of
Accounts ), it is displayed in the respective fields by default.
b. Specify the required distribution rule and/or project for each account (you can change the default values).
6. Open the Payment Means window, specify the relevant details, and choose OK.
7. Choose Add.
 Note
To assign the same project to all the G/L accounts in the table, choose the required project in the Project field in the
general area. When asked whether to apply the selection to all rows, choose Yes to approve.
Result
Once the outgoing payment is added, the accounts selected in the table are credited, and the respective amounts are allocated to
the relevant cost centers and/or project if defined.
Example
You pay 1000 (LC) in electrical expenses, which should be split among cost centers of three departments; each has its own
electrical expenses G/L account.
QA - consumes 40%
Development - consumes 40%
Administration - consumes 20%
The table in the outgoing payment is as follows:
Payment to Multiple G/L Accounts
G/L Account Amount Profit Center
Electricity Exp. Admin. 200 Admin.
Electricity Exp. QA 400 QA
Electricity Exp. Dev. 400 Dev
This is custom documentation. For more information, please visit SAP Help Portal. 44

6/8/26, 6:08 AM
If the payment is made in cash, the journal entry created by the outgoing payment is as follows:
Journal Entry
G/L Account Debit Credit
Cash on Hand 1000
Electricity Exp. Admin. 200
Electricity Exp. QA 400
Electricity Exp. Dev. 400
More Information
Outgoing Payments
Creating Outgoing Payments for Customer
Use the procedure to create an outgoing payment to a customer based on an A/R Credit Memo, or on A/R Invoice and A/R Credit
Memo when only a partial amount is returned.
This might occur when goods purchased and already paid for by the customer were returned to the company (completely or
partially).
 Caution
You cannot create this type of document through the payment wizard.
Procedure
1. Choose Banking Outgoing Payments Outgoing Payments .
The Outgoing Payments window appears.
2. Select Customer, and choose the customer for which the payment is issued.
The table area displays the open documents and transactions (if you selected the option Display all Transactions) that are
not reconciled yet:
A/R Invoices, A/R Down Payment Invoices, manual journal entries in which the customer is on the debit side, and
amounts deposited to the customer and not to the bank that are presented with a negative sign.
A/R Credit Memos that are not based on A/R Invoices, manual journal entries in which the customer is on the
credit side, incoming payments that are not based on invoices, and checks for payment that are presented with a
positive sign.
 Note
Down Payment Requests and Opening Balances transactions are not represented in the table.
3. Select the documents on which you want to base the outgoing payment and change the Total Payment amount if required.
4. Open the Payment Means window, specify the payment details and choose OK.
5. Choose Add.
This is custom documentation. For more information, please visit SAP Help Portal. 45

6/8/26, 6:08 AM
Result
Applied Amount and Open Balance/Balance Due in the document(s) are updated accordingly.
If the base documents were fully paid through the outgoing payment, the documents get the status Closed.
The transactions of the outgoing payment and the paid document(s)/transaction(s) are reconciled internally.
If base documents were fully paid, but the payment amount did not match the definition made in the Outgoing Amt Diff.
Allowed or Outgoing % Diff. Allowed field of the Currencies - Setup window under  Administration     Setup    Financials
|     Currencies | :   |     |     |
| -------------- | --- | --- | --- |
Differences caused by a payment amount bigger than the amount due (loss) are posted to the account defined in
Administration     Setup     Financials     G/L Account Determination     Purchasing     General    Overpayment
A/P Account .
Differences caused by a payment amount smaller than the amount due (gain) are posted to the account defined in
Administration     Setup     Financials     G/L Account Determination     Purchasing    General
Underpayment A/P Account .
Example
You issued your customer an A/R Invoice for 285.27 (LC).
The customer paid the exact amount, and then returned part of the items, for which you issued an A/R Credit Memo for 120.06
(LC) (the credit memo is not based).
The customer now is entitled to a payment of 120.06 (LC), but you paid in cash only 120 (LC). The following is the table in the
Outgoing Payment document for this customer:
Documents for Payment
| Document | Balance Due | Document Type         | Total Payment |
| -------- | ----------- | --------------------- | ------------- |
| 1234     | 120.06 (LC) | CN (=A/R Credit Memo) | 994.3         |
The amount specified in  Administration     Setup     Financials    Currencies   Outgoing Amt Diff. Allowed  is 1 (LC).
The journal entry created by the payment will be:
Journal Entry
| G/L Account/BP          | Debit  | Credit |     |
| ----------------------- | ------ | ------ | --- |
| Cash on Hand            |        | 120    |     |
| Underpayment A/PAccount | -0.06  |        |     |
| Customer                | 120.06 |        |     |
The journal entries of the A/R Credit Memo and Outgoing Payment are reconciled, and the A/R Credit Memo is closed.
More Information
Outgoing Payments
This is custom documentation. For more information, please visit SAP Help Portal. 46

6/8/26, 6:08 AM
Creating Outgoing Payments
Procedure
1. From the SAP Business One Main Menu, choose Banking Outgoing Payments Outgoing Payments .
The Outgoing Payments window appears.
2. Select whether to create the outgoing payment for a vendor (default), customer, or account.
3. Specify the required data. If you selected Vendor, you can create the outgoing payments either by basing them on specific
documents or without basing them on any invoice.
4. On the toolbar or in the payment, choose .
The Payment Means window opens.
5. Specify details for the payment means of the outgoing payment and choose OK.
6. To add the outgoing payment document, choose Add.
Results
An appropriate journal entry is created.
If the means of payment was a check, the relevant check is created and can be:
Viewed in the Checks for Payment window ( Banking Outgoing Payments Checks for Payment )
Printed from the Checks for Payment window and the Document Printing function ( Banking Document Printing )
 Note
If the outgoing payment was created for a vendor for whom you defined a payment-consolidating business partner ( Business
Partners Business Partner Master Data Accounting General ), the journal entry is recorded to the consolidating
business partner.
If the outgoing payment was based on one or more specific invoices that were fully paid, the following is performed:
The transaction(s) of the paid invoice(s) and the transaction of the outgoing payment are reconciled automatically.
The Amount Due and the Paid/Credited fields in the paid invoice(s) are updated, and the status of the invoice(s) becomes
Closed.
If the outgoing payment was created for a foreign-currency vendor, a transaction for exchange rate differences is created.
 Note
The behavior described above applies whether Split BP/Account in Journal Entry (in Administration System Initialization
Document Settings Per Document Outgoing Payments ) is selected or not.
Related Information
Outgoing Payments
Incoming Payments
Outgoing Payments: Vendor & Customer
This is custom documentation. For more information, please visit SAP Help Portal. 47

6/8/26, 6:08 AM
The following fields appear in the general area of the Outgoing Payments window.
To open the window, choose Banking Outgoing Payments Outgoing Payments , and select Vendor or Customer.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
Name
Business partner's name. Press CTRL + TAB to move to the next field.
Pay to
Default pay to address defined for the business partner. Change it if required. If you choose the option Bank, the bank details
defined for the business partner appears.
Contact Person
Default contact person defined for the business partner. Change it if required.
Project
To relate the outgoing payment to a specific project, specify the required project.
Display Invoices with Matching Billing Address/Bank
Displays in the table only invoices with pay to address/bank details identical to the address/bank selected in the Pay To field.
Only available when the outgoing payment is created for a vendor.
No.
Default numbering series and current number of the outgoing payment in the default numbering series. Specify another series if
required.
Posting Date, Document Date
Current date by default. Change it if required.
Due Date
By default, the current date, which will be the due date of the business partner row in the journal entry created by the document.
 Note
When you enter the details of the payment means in the Payment Means window, and return to the Outgoing Payment window,
this field is updated with the weighted average of the due dates defined for the payment means.
If required, you can change the date before you add the document.
Reference
Specify another reference for this document if required.
Transaction No.
Number of the journal entry created by this document. The number appears when you have added the outgoing payment.
Branch
This is custom documentation. For more information, please visit SAP Help Portal. 48

6/8/26, 6:08 AM
Select a branch from which you want to choose a customer/vendor.
 Note
This field is available only if you have enabled multiple branches.
Pro Forma
Relevant for vendor only.
Indicates that the outgoing payment is created as down payment.
Remarks
Enter any remarks about this outgoing payment.
Journal Remarks
Enter the details to be displayed in the Remarks field of the journal entry. By default, the text:
Outgoing – <business partner code> appears.
 Note
If the outgoing payment has been generated by the payment wizard, the default display is
Outgoing Payments - <business partner code> — <payment run name>.
The payment run name is copied from the Payment Wizard, General Parameters window.
Control Account
Specify the control account for the outgoing payment. The control account affects only the amount that is not based on the invoice
in the journal entry of the payment. The default account varies according to your selection of documents.
If you have not selected any invoice or, if the first document that you have selected is a manual journal entry, the default
control account is the one set in the business partner master data.
If you have selected invoices, the default control account is that of the first invoice you have selected.
Created by Payment Wizard
Indicates whether the outgoing payments were created through the payment wizard or not. Only applicable for vendors. You
cannot edit it.
Payment on Account
Creates an outgoing payment not based on any transaction or document appearing in the table. When you select this option, the
Control Account field appears where you can specify the control account for the outgoing payment.
 Note
When a payment on account is included in a payment order run, you cannot cancel it.
Amount Due (FC), Amount Due (LC)
Total amount to be paid through this document, in foreign and local currency.
Add in Sequence
If the payment is not against specific documents/transactions, closes documents/transactions according to their display order in
the table.
Available only when the outgoing payment is created for a vendor.
This is custom documentation. For more information, please visit SAP Help Portal. 49

6/8/26, 6:08 AM
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
More Information
Outgoing Payments
Outgoing Payments: Vendor & Customer - Contents Tab
The following fields appear in the Contents tab of the Outgoing Payments window.
To open the window, choose Banking Outgoing Payments Outgoing Payments . Select Vendor or Customer.
This is custom documentation. For more information, please visit SAP Help Portal. 50

6/8/26, 6:08 AM
Contents Tab Fields
Document No.
Displays the document number. Click to display the document. This column is displayed only when the option
Customer/Vendor Reference Number is de-selected.
Installment
Displays the successive number of the installment within the total number of the installments included in a specific invoice. The
invoice is displayed several times according to the number of installments still to be paid.
If not all installments are paid in the same document, the invoice will not be reconciled automatically.
Date
Displays the posting date of the document/transaction.
*
An asterisk is displayed in the line of every invoice or installment whose due date has passed.
Overdue Days
If the open item due date is earlier than the posting date of the manual payment, the number of overdue days is displayed in
red.
If the open item due date is equal to the posting date of the manual payment, 0 is displayed in black.
If the item is not overdue (that is, the open item due date is after the posting date of the manual payment), the number of
overdue days is displayed in black, preceded by a minus (-) sign.
Total
Displays the total amount due for the document/transaction.
WT Amount
Displays the withholding tax amount included in the document.
Balance Due
Displays the amount still to be paid from the document/transaction.
If a partial payment for that record has already been made, or if a credit memo was created for the partial amount, this value is
lower than the value displayed in the Total field.
Blocked
Displays an asterisk (*) if you selected Y in either of the following fields:
The Payment Block field of the manual journal entry line
The Payment Block field on the Accounting tab of the marketing document
Cash Discount %
Displays the cash discount rate to which the business partner is entitled. This value is determined by the payment term linked to
the invoice, taking into account the date of payment in respect to the posting date of the invoice. You can change it if required.
Document Type
This is custom documentation. For more information, please visit SAP Help Portal. 51

6/8/26, 6:08 AM
Displays the type of document or transaction. For example, IN represents A/R invoice. For the complete list of document types,
see the help topic, Transaction Type Abbreviations Legend.
Total Payment
Displays the amount that is still outstanding on an outgoing invoice. Change this amount if the incoming payment is only for part of
the invoice amount. The application proposes the balance due as the amount to be paid.
Total Rounding Amount
This column is displayed only when the selected rounding method is By Currency. In this case, the amount displayed in this field is
the difference between the original amount of the document and its rounded amount.
Distr. Rule
If required, specify a distribution rule for the row.
Project
Displays the project specified in the document.
Payment Order Run
Displays whether this transaction is included in a payment order run. You will be warned when creating payments for such
transactions.
More Information
Outgoing Payments
Transaction Type Abbreviations Legend
Outgoing Payments: Account
The following fields appear in the Outgoing Payments window.
To open the window, choose Banking Outgoing Payments Outgoing Payments ; then choose Account.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Outgoing Payments for Account
Project
To relate the outgoing payment to a specific project, specify the required project.
Doc. Currency
Document’s currency. The default value is the local currency. Specify another currency if required.
If you specify a foreign currency, the exchange rate defined in the Exchange Rates and Indexes table for the selected currency for
the document's posting date is displayed. Change this rate if required.
No.
This is custom documentation. For more information, please visit SAP Help Portal. 52

6/8/26, 6:08 AM
Default numbering series and current number of the outgoing payment in the default numbering series. Specify another series if
required.
Posting Date, Document Date
Current date by default. Change the dates if required.
Due Date
Current date by default, which will be the due date of the account row in the journal entry created by the document.
After you specify the details of the payment means in the Payment Means window, and return to the Outgoing Payment window,
this field is updated and displays the weighted average of the due dates defined for the payment means.
If required, change this date before you add the document.
Reference
Enter an additional reference if required.
Transaction No.
Number of the journal entry created by this document. The number appears after you have added the outgoing payment.
Branch
Select a branch from which you want to choose an account.
 Note
This field is available only if you have enabled multiple branches.
Doc. Remarks
Enter any details regarding the amount paid for this account.
Amount
Specify the amount referred to the account.
Total Amount Due
Total amount of the payment in local currency. Appears only when the selected document currency is the local currency.
Amount Due (FC), Amount Due (LC)
Amount of the payment in the selected foreign currency and in local currency according to the exchange rate defined in the
document.
Appear if the document currency is other than the local currency.
Remarks
Enter any remarks regarding this outgoing payment.
Journal Remarks
Enter the details to be displayed in the Remarks field of the journal entry. Includes by default the text:
Outgoing – Account Code. If the outgoing payment is for more than one account, the code is for the last account in the
document.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 53

6/8/26, 6:08 AM
Outgoing Payments
Outgoing Payments: Attachments Tab
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
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
General Settings: Path Tab
Endorsing Checks in Outgoing Payments
Prerequisites
The check to endorse has not been canceled or deposited.
This is custom documentation. For more information, please visit SAP Help Portal. 54

6/8/26, 6:08 AM
For the customer or vendor you selected in the outgoing payment, on the Payment Terms tab of its master data, you have
selected the This BP Accepts Endorsed Checks checkbox.
Context
 Note
This feature is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info
The check endorsement function enables you to use an endorsable incoming check in an outgoing payment as a payment means.
Procedure
1. Choose Banking Outgoing Payments Outgoing Payments .
The Outgoing Payments window appears.
2. Choose a vendor or customer, and specify the required data.
3. On the toolbar or in the payment, choose .
The Payment Means window appears.
4. On the Check tab, select the Endorse checkbox, and in the Endorsable Check No. field, press Tab .
The List of Checks window appears, listing all the checks that are endorsable, not endorsed, not deposited, not canceled,
and not overdue.
5. In the List of Checks window, choose a check to endorse in the outgoing payment.
The check information appears in the line.
6. [Optional] You may specify other payment means in the Payment Means window, and choose the OK button.
7. To add the outgoing payment, choose the Add button.
Results
After you have endorsed a check, you can no longer deposit or cancel it.
Related Information
Payment Means: Check Tab
Payment Means
Use this window to record and view the details of the means of payment combined to make an incoming or outgoing payment. The
following payment means are supported in all localizations:
Check
Bank transfer
Credit card
Cash
This is custom documentation. For more information, please visit SAP Help Portal. 55

6/8/26, 6:08 AM
Bill of Exchange is supported by the SAP Business One software versions for the relevant countries/regions. Details are available in
the localization-specific online help file under Help Documentation Localization-Specific Info .
To open the window, choose Banking Incoming Payments Incoming Payments . Alternatively, choose Banking
Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose .
Payment Means: General Area
Use this window to specify payment details. To open the general area of the Payment Means window, choose Banking
Incoming/Outgoing Payments Incoming/Outgoing Payments .
On the toolbar or in the payment, choose .
Payment Means General Area Fields
Currency
Currency of the payment, as defined in the Incoming/Outgoing Payments window. Specify another currency if required. If the
currency defined for the G/L account/business partner is the local currency, the displayed currency cannot be changed.
Overall Amount
Amount to be paid, comprising:
Invoices selected for payment
Information in the relevant Payments window
Any amounts that are not contained in incoming or outgoing invoices (only if Display Journal Entries was selected)
Balance Due
When the amounts to be covered by the different payment means have been entered, the balance due is equal to zero.
Bank Charge
Specify the amount of bank charge for the particular payment.
Paid
Total amount paid, which is the sum of the amounts entered in the Payment Means window.
Payment Means: Check Tab
To access the Check tab of the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Check tab.
Payment Means: Check Tab Fields
G/L Account
For incoming payment documents:
Specify the account to be debited when the incoming payment is added. The account displayed is defined in Administration
Setup Financials G/L Account Determination Sales General Checks Received .
This is custom documentation. For more information, please visit SAP Help Portal. 56

6/8/26, 6:08 AM
G/L Account (Table Area)
For outgoing payment documents:
Account defined for the selected bank in the House Bank Accounts – Setup window. To have a different account credited when the
outgoing payment is added, press TAB and select the required account. You can issue checks from different accounts within the
same outgoing payment if required.
Search by Bank Code
Searches for the required bank by bank code instead of bank name.
Due Date
The current date is the default date for the first check. Change if necessary.
Country/Region
Specify the country/region where the bank issuing the check is located.
Bank Name
Specify the relevant bank. Available options are banks defined for the selected country/region in the Banks – Setup window.
Branch, Account, Check No.
For incoming payment documents:
Specify the numbers of the branch, account, and check as printed on the check received.
Branch, Account
For outgoing payment documents:
Numbers of the branch and bank account of the credited G/L account. These details are taken from the House Bank Accounts –
Setup window.
Manual Check
For outgoing payments only:
To manually specify the check number, select the checkbox. This is useful if the check is not printed through SAP Business One,
but written manually.
Check No.
Incoming Payments
Specify the number of the check received.
Outgoing Payments
If you print checks from SAP Business One, this field is disabled and the check number is zero until the check is printed, when the
check number is updated automatically.
If you issue checks manually, select the checkbox Manual Check and specify here the check number.
Endors.
Specify whether endorsement of the check should be allowed or not.
The default value of this column is determined by the Endorsable Checks from This BP checkbox on the Payment Terms tab of
the Business Partner Master Data window. When the Endorsable Checks from This BP checkbox is selected, in the payments
created for this business partner, the Endors. column is set to Yes by default. However, you can always change the Endors. status
before adding the payment.
This is custom documentation. For more information, please visit SAP Help Portal. 57

6/8/26, 6:08 AM
Amount
Specify the amount of the check.
Originally Issued By
For incoming payments only:
Enter the original issuer of the check. This information is helpful if an incoming check bounces.
 Note
This column is available in most of the localizations. For additional information, see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Fiscal ID
For incoming payments only:
Enter the fiscal ID of the original issuer of the check. This information is helpful if an incoming check bounces.
 Note
This column is available in most of the localizations. For additional information, see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Endorse
For outgoing payments only:
Select the checkbox to enable the Endorsable Check No. field, from which you can choose an endorsable check and endorse it to
the business partner of the outgoing payment.
This checkbox is available only if you have selected the This BP Accepts Endorsed Checks checkbox on the Payment Terms tab of
the Business Partner Master Data window for the business partner of the outgoing payment.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This checkbox is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
Endorsable Check No.
For outgoing payments only:
Press TAB to open the List of Checks window, in which you can select an endorsable check and endorse it to the business
partner of the outgoing payment. After you choose an endorsable check, its information appears in the line, and you cannot edit it.
This field is available only if you have selected the Endorse checkbox on the Check tab of the Payment Means window.
For more information about endorsing checks in outgoing payments, see Endorsing Checks in Outgoing Payments.
 Note
This checkbox is available in most of the localizations. For additional information see the localization-specific online help file
under: Help Documentation Localization-Specific Info .
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 58

6/8/26, 6:08 AM
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Bank Transfer Tab
To access the Bank Transfer tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Bank Transfer tab.
Payment Means: Bank Transfer Tab Fields
G/L Account
Specify the G/L account from the chart of accounts to/from which the bank transfer is to be posted.
Transfer Date
Specify the bank transfer date.
Reference
Specify a reference, such as the intended purpose, for the bank transfer.
Total
Specify the bank transfer amount.
More Information
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Credit Card Tab
To access the Credit Card tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Credit Card tab.
 Note
If you choose to pay by credit card or receive a payment through credit card, the corresponding journal entry will be non-
changeable.
Payment Means: Credit Card Tab Fields
Credit Card Name
Specify the credit card used to make the payment.
G/L Account
Incoming Payments
The account defined for the selected credit card in the Credit Card – Setup window. If required, specify another account.
This is custom documentation. For more information, please visit SAP Help Portal. 59

6/8/26, 6:08 AM
Outgoing Payments
Specify the account to be credited when the outgoing payment is added.
Credit Card No., Valid Until
For incoming payment documents:
Specify the number and valid-until date (in the format MM/YY) of the credit card.
ID No., Telephone No.
Specify the ID number and the phone number of the card owner.
Payment Method
Specify the required payment method.
Amount Due
Specify the amount paid with the credit card.
No. of Payments, First Partial Payment, Each Add. Payment
Specify the number of partial payments for this transaction, and the amount of the first partial payment.
SAP Business One automatically calculates the amount that is to be paid with future payments, and displays it in the Each Add.
Payment field. Rounding results are added to the first payment.
 Note
Available for incoming payment documents only if the selected payment method enables the creation of multiple partial
payments.
Voucher No.
Specify the number of the credit card voucher.
Transaction Type
For incoming payment documents:
Specify whether the transaction is a telephone transaction or a regular transaction.
Split Credit Voucher
For outgoing payment documents:
Creates a separate row in the journal entry for each partial payment.
Vouchers
All credit cards defined in the Credit Cards – Setup window. The credit card selected in the Credit Card Name field is marked. To
create vouchers for an additional credit card, choose Define New in this list.
Tel. for Approval, Company ID
Telephone number for approval as defined for the credit card, and company ID that should be used when calling for approval.
Total
Total amount paid with this transaction.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 60

6/8/26, 6:08 AM
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Payment Means: Cash Tab
To access the Cash tab in the Payment Means window, choose Banking Incoming Payments Incoming Payments .
Alternatively, choose Banking Outgoing Payments Outgoing Payments . On the toolbar or in the payment, choose . In
the Payment Means window, choose the Cash tab.
Payment Means: Cash Tab Fields
G/L Account
For incoming payment documents, one of the following is displayed:
Account defined in the Cash on Hand field on the General subtab of the Sales tab in the G/L Accounts Determination
window.
Default account defined for the user in the Cash Acct field on the Defaults tab in the User Default window.
If required, select another account. The selected account is debited once the incoming payment is added.
G/L Accounts (op)
For outgoing payment documents, specify the account to be credited when the outgoing payment is added.
Total
Specify the total amount of the cash payment.
More Information
Payment Means
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Checks for Payment
Use this function to:
Print outgoing checks created through the Outgoing Payments window
Create checks for payment without having the proper journal entry created
Create drafts for checks for payment
Print checks created through this window
More Information
Checks for Payment Window
This is custom documentation. For more information, please visit SAP Help Portal. 61

6/8/26, 6:08 AM
Printing Checks for Payment
Adding Checks for Payment
Context
Use the procedure to create checks for payment for G/L accounts or business partners – with or without the creation of the
appropriate journal entry.
Procedure
1. Choose Banking Outgoing Payments Checks for Payment .
The Checks for Payment window appears.
2. Fill in the To Order of field:
If the check is for a G/L account, press TAB and select the required G/L account code.
If the check is for business partner, press CTRL + TAB and select the required business partner code.
3. If you do not want the check-for-payment transaction to create a journal entry, deselect Create Journal Entry.
4. In the table, specify the G/L account to be credited and the tax group required.
 Note
You can credit more than one G/L account in the same check for payment as long as the amounts related to credited
accounts are of the same currency (any of the following combinations is allowed: All Currencies + Foreign Currency
accounts, if the amounts are in the specific foreign currency or All Currencies + Local Currency accounts if the amounts
are in local currencies)
5. Specify the due date and credited bank details.
 Note
When documenting a check that was issued manually, select Manual and enter the number of the check issued,
otherwise, the Check No. field is disabled and will be updated automatically when the check is printed.
6. Choose Add.
Results
The check for payment is added and, when Create Journal Entry is selected, the appropriate journal entry is recorded in the
database.
Related Information
Checks for Payment
Checks for Payment Window
Use this window to define details of checks that you need to pay. Some fields already display default values. Use the information
below to guide you in specifying field values.
This is custom documentation. For more information, please visit SAP Help Portal. 62

6/8/26, 6:08 AM
To open the window, choose Banking Outgoing Payments Checks for Payment .
General Area Fields
To Order Of
For check created through this window - Specify the business partner code or G/L account code for which the check is
created. Press TAB to open the Choose from List window for G/L accounts, and CTRL + TAB to open the List of
Business Partners window for business partners.
For check created through an Outgoing Payment document – Code and name/description of the business partner/G/L
account for which the outgoing document was created. These details cannot be changed.
Pay To
Default Bill To address defined for the selected business partner. If required, you can specify another address.
If a G/L account was selected, enter the mailing address you want to print on the check.
Internal ID
Successive numbers to checks for payment, starting at 1.
Reference
For check created through this window: By default, the number of the Internal ID field. Change it if required.
For check created through the Outgoing Payment document: Number of the outgoing payment document.
Posting Date
For check created through this window: By default, the current date. Change it if required.
For check created through the Outgoing Payment document: Posting date of the outgoing payment document through
which the check was created. This date cannot be changed.
Referenced Document (<Number of Documents That the Current Document Refers To>)
Choose to open the Reference Information window. In this window, you can specify the reference documents for the current
document and view the documents that reference the current document.
Document Referenced To tab:
Lets you specify other documents across different business modules as the reference documents for your current
document. The types of other documents and your current one can be either the same or different.
Document Referenced By tab:
Lets you see which documents are using the current document as a reference
To specify Document B1 as a reference document for Document A1, proceed as follows:
1. Go to the Document Referenced To tab of Document A1.
2. Choose Transact. Type and select the document type of Document B1.
The supported documents are those with the Referenced Document function in their respective windows. For example,
journal entries, landed costs and incoming payments are unavailable here.
3. In the Doc. Number field, specify the document number B1.
4. Choose Update.
This is custom documentation. For more information, please visit SAP Help Portal. 63

6/8/26, 6:08 AM
5. Document B1 appears on the Document Referenced To tab of Document A1. Accordingly, Document A1 appears on the
Document Referenced By tab of Document B1.
After you add the document, you can view and keep track of the reference relationships in the Relationship Map.
In addition, if you use the Duplicate option in the context menu or the Data menu in the menu bar to duplicate a marketing
document, you will see a message: Do you want to create a reference between the original and duplicate
documents? If you confirm the message, the original document is automatically set as a referenced document. You can view the
reference relationship through both the Reference Information window and the relationship map.
If you duplicate any document with existing document references, the document references are automatically copied from the
original document to its duplicate by default.
To cancel copying document references from original documents to their duplicates, go to the SAP Business One Main Menu
Administration System Initialization Document Settings General tab, and deselect the checkbox Copy Document
References from Original Documents to Duplicates.
 Note
The Copy To functionality does not copy the reference links, as the references are specific to the document for which they are
created.
Trans. No, Create Journal Entry
For check created through this window: If Create Journal Entry is selected, the appropriate journal entry is created when
this document is added. The number of the journal entry is displayed in the Trans. No. field.
For check created through the Outgoing Payment document: The Trans. No. field displays the number of the journal entry
created while the Outgoing Payment document was added. The Create Journal Entry is then disabled.
Contents Tab Fields
Remarks
For check created through this window: Specify relevant details for the check. The details will be printed on the check.
For check created through Outgoing Payment document: Numbers of the A/P invoices paid by this outgoing payment. This
text will be printed on the check.
Amount
For check created through this window: Specify the required amount.
For check created through an Outgoing Payment document: Amount as determined in the outgoing payment document.
Row Total
Total amount to be credited including tax.
Total
Total of the amounts appearing in the Contents tab.
Total Tax
Total amount of tax included in the check.
Amount Due
Total amount of the checks including possible taxes.
This is custom documentation. For more information, please visit SAP Help Portal. 64

6/8/26, 6:08 AM
Journal Remarks
For check created through this window: By default, the text: Check for Payment is displayed. Change it if required.
For check created through an Outgoing Payment document: Specify relevant remarks regarding the check.
Signature
Specify the name of the authorized signatory.
Total
Total amount of the check.
Pay to Order of
Text from the To Order of field, which will be printed on the check. Change it if required.
Amount In Words
Total amount in words, which is printed on the check in this format.
Due Date
For check created through this window: Specify the due date for the check. If Create Journal Entry is selected, this is also
the value date. The current date is the default. Change it if necessary.
For check created through an Outgoing Payment document: Due date of the check as determined in the Payment Means
window when the outgoing payment document was created.
Endors.
Specify whether the check should be endorsable or not.
Country/Region, Bank, Account, Branch
For a check created through this window, specify:
The details of the check and bank
The required country/region, bank, and account
For a check created through an Outgoing Payment document, specify bank account details as determined in the Payment
Means window when the Outgoing Payment document was created.
Manual
To manually specify the check number, select the checkbox. This is useful if the check is not printed through SAP Business One,
but written manually.
Check No.
If you print checks from SAP Business One, this field is unavailable and the check number is zero until the check is printed, when
the check number is updated automatically.
If you issue checks manually, select the Manual checkbox and specify here the check number.
Print on Blank Paper
Prints the check on blank paper.
Printing / Spacing
This is custom documentation. For more information, please visit SAP Help Portal. 65

6/8/26, 6:08 AM
Since the print margins can vary depending on the manufacturer of the printer, you can set the spacing here. Print out a check to
test it. Change the spacing by clicking the triangles. The setting is displayed on the right of the icon.
More Information
Checks for Payment
Combined Cash Flow Assignment Window
Cash Flow Line Items - Setup
Checks for Payment: Attachments Tab
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
File Name
The name of the file attached.
Attachment Date
The date on which the file is attached.
Related Information
This is custom documentation. For more information, please visit SAP Help Portal. 66

6/8/26, 6:08 AM
General Settings: Path Tab
Choose Bank Window
Use this window to choose bank accounts from grouped categories.
To open the window, choose the icon in banking-related windows, for example, Checks for Payment and Check Number
Confirmation.
Choose Bank Window
Display Account Selected for House Bank
If this option is selected (this is the default setting), you see only those accounts that meet the selection criteria you specified in
the previous window.
 Example
You specify a country/region and a bank and then choose . Only the accounts defined in the selected bank are displayed.
To display all house bank accounts defined in SAP Business One, deselect this option.
Country/Region
Country/region in which the accounts are located. Choose to display the banks located in this country/region.
Bank
Bank in which the accounts are located. Choose to display the accounts located in this bank.
Account No., IBAN, BIC/SWIFT Code
Displays the account number, IBAN, and the BIC/SWIFT code, as defined in the House Bank Accounts – Setup or the Business
Partner Bank Accounts – Setup window.
Void Checks for Payment
Use this function to void a single check or a number of checks in succession, as an alternative to using the Checks for Payment or
Outgoing Payments windows.
You need this function in the following situations:
The printed check number does not match the number assigned to it by SAP Business One.
A check was cancelled before it was delivered or cashed to or by a business partner.
To access the function, choose Banking Outgoing Payments Void Checks for Payment .
More Information
Void Checks for Payment – Selection Criteria
Void Checks for Payment Window
This is custom documentation. For more information, please visit SAP Help Portal. 67

6/8/26, 6:08 AM
Voiding Checks for Payment
Context
Use the procedure to void a single check or a number of checks in succession.
Procedure
1. Choose Banking Outgoing Payments Void Checks for Payment .
The Void Checks for Payments – Selection Criteria window appears.
2. Specify the required parameters and choose OK.
The Void Checks for Payment window appears.
3. Select the checks to be voided.
 Note
When selecting a check that is one of several checks created through the same outgoing payment document, all
additional checks created through this outgoing payment document are automatically selected and will be voided.
4. Specify the date to be considered as the check's cancellation date.
5. Choose Void.
6. When asked whether you want to void the selected checks, choose Continue to void the checks.
Results
The Voiding Checks for Payment window appears, displaying the selected checks. The Cancelled column indicates whether the
check was voided or not.
The selected checks are voided, and the appropriate journal entries are created. The word Cancelled is recorded in the Journal
Remarks field in the Checks for Payment window.
The Details field in the journal entry created contains the following text: Reverse Entry for Check No.XXX.
Related Information
Voiding Checks for Payment
Void Checks for Payment - Selection Criteria
The following are the fields in the Void Checks for Payment – Selection Criteria window.
To open the window, choose Banking Outgoing Payments Void Checks for Payment .
Selection Criteria
Posting Date From...To...
Specify a posting date range to display only checks for payment created within the range.
Check Number From...To...
This is custom documentation. For more information, please visit SAP Help Portal. 68

6/8/26, 6:08 AM
Specify a check number range to display only the checks with numbers within the range.
Check Internal ID
Internal number assigned automatically to the check by SAP Business One at the time of creation.
Bank Code
Opens the Bank Codes window, where you select whether to display checks for payment created for all banks or to display just the
checks created for a selected bank or banks.
More Information
Void Checks for Payment
Bank Codes Window
Bank Codes Window
To open the Bank Codes window, choose Banking Outgoing Payments Voiding Checks for Payment , then Bank Code.
Bank Codes Window
Code, Bank Name
Bank codes and names as defined in the Banks – Setup window.
More Information
Voiding Checks for Payment
Void Checks for Payment Window
The following are the fields in the Void Checks for Payment window.
To open the window, choose Banking Outgoing Payments Void Checks for Payment . Specify your selection criteria and
choose OK.
Void Checks for Payment Window
[Selection Column]
Select the checks to void.
Check No., Bank No, Due Date, BP/Account Code, BP/Account Name, Total, Check Internal ID
Relevant details about the checks for payment.
Doc. No.
Number of the document through which the check was created. This can be a check for payment or an outgoing payment.
Add. Payments
If a check for payment was created through an outgoing payment document, and in the same document another means of
payment were involved, the amount covered by the other means of payment is displayed here.
This is custom documentation. For more information, please visit SAP Help Portal. 69

6/8/26, 6:08 AM
Cancel Checks on:
Specify the cancellation date of the journal entry to be created during the voiding process:
Cancellation Date – Cancellation date of the journal entry will be the current date.
Check's Posting Date – Posting date of the journal entry will be the original creation date of the selected check for
payment.
More Information
Void Checks for Payment
Voiding Checks for Payment Window
The following are the fields in the Voiding Checks for Payment window after SAP Business One voids the selected checks.
To open the window, choose Banking Outgoing Payments Void Checks for Payment . Specify your selection criteria and
choose the OK button. In the Void Checks for Payment window, select the checks to be voided and choose the Void button.
Voided Checks for Payment
Doc. No., Check No., BP/Account Name, Total
Details of the checks selected for voiding.
Cancelled
Yes indicates that the check was voided.
Display Voided Checks Only
Displays only checks that were actually cancelled.
 Example
If the date of a check deviates from the date range of the current period, the check will not be voided and the value in the
Cancelled column is No.
More Information
Void Checks for Payment
Checks for Payment Drafts
Use this function to process drafts created for checks for payment.
To access the function, choose Banking Outgoing Payments Checks for Payment Drafts .
More Information
Checks for Payment Drafts Window
This is custom documentation. For more information, please visit SAP Help Portal. 70

6/8/26, 6:08 AM
Checks for Payment Drafts Window
To open the Checks for Payment Drafts window, choose Banking Outgoing Payments Checks for Payment Drafts .
Checks for Payment Drafts Window
Date
Due date of the check draft.
Pay to Order of
BP/Account code to which the check draft is issued.
Total
Total amount of the check draft, including taxes.
More Information
Checks for Payment Drafts
Working with the Payment Wizard
The payment wizard enables you to generate incoming and outgoing payments in batches according to the selected A/R and A/P
open transactions and the selected payment methods.
When creating incoming or outgoing payments using the payment wizard, you can partially pay specific transactions, as when
working manually.
Payment wizard runs cover A/P and A/R transactions that are partially paid, credited, or reconciled, as well as
unreconciled/allocated payments on account.
The following transaction types are considered in the payment wizard run:
A/R: A/R invoices, A/R correction invoices, A/R credit memos, A/R down payment requests, A/R down payment invoices,
A/R reserve invoices, manual journal entries with at least one row posted to a customer
If the customer is debited with positive amounts or credited with negative amounts, the journal entry is considered
as an A/R invoice with a positive total.
If the customer is debited with negative amounts or credited with positive amounts, the journal entry is considered
as an A/R credit memo with a positive total.
A/P: A/P invoices, A/P correction invoices, A/P credit memos, A/P down payment requests, A/P down payment invoices,
A/P reserve invoices, manual journal entries with at least one row posted to a vendor.
If the vendor is credited with positive amounts or debited with negative amounts, the journal entry is considered as
an A/P invoice with a positive total.
If the vendor is debited with positive amounts or credited with negative amounts, the journal entry is considered as
an A/P credit memo with a positive total.
Payments on account: Incoming and outgoing payments not allocated or reconciled to specific transactions are also
considered in the payment wizard run.
For more information about paying a negative total in the payment wizard, see Paying Negative Totals Using the Payment Wizard.
This is custom documentation. For more information, please visit SAP Help Portal. 71

6/8/26, 6:08 AM
Prerequisites
To use the payment wizard, make sure you have set up the following:
1. Banks
2. House Bank Accounts
3. Payment Methods
4. Payment methods on Business Partner Master Data: Payment Run Tab
Process
1. From the SAP Business One Main Menu, choose Banking Payment Wizard .
The first window provides a brief introduction to the payment wizard. Choose Next to start the payment wizard.
2. Make the required choices in each step. To move to the next step, choose the Next button.
For procedural descriptions, you can choose the interactive image below and go to the specific topics.
Please note that image maps are not interactive in PDF outputs.
This is custom documentation. For more information, please visit SAP Help Portal. 72

6/8/26, 6:08 AM
Result
Once a payment run is executed, the following occurs:
The relevant incoming payment and/or outgoing payments are created. The Created by Payment Wizard checkbox in these
documents is selected.
The fully paid A/R and/or A/P transactions are closed and the Applied Amount field is updated accordingly.
The partially paid A/R and/or A/P transactions are still open and the Applied Amount field is updated accordingly.
After creating a payment order, you can see detailed informaiton in the payment orders report, as described in Generating
the Payment Orders Report.
Step 1 - Selecting Payment Run Options
The following are the fields in the first step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 1 - Payment Run Selection
Start New Payment Run
Select to create a payment run.
Load Saved Payment Run
Select to view the selection criteria/recommendation report of a payment run not yet executed.
For payment runs with saved selection criteria, the table displays the payment run name, the date on which the selection criteria
were saved, and the status of the payment run Saved.
For payment runs with saved selection criteria and recommendation report, the table displays the payment run name, the date on
which the selection criteria and the recommendation report were saved, the total amount including the bank charges amount of
the payment run, and the status of the payment run Recommended.
For payment order runs, the table displays the payment order run name, the date on which the payment order run was executed,
the total amount including the bank charges amount of the payment order run, and the status of the payment order run
Payment Order Run.
View Executed Payment Run
Select to view an already executed payment run.
The table displays the payment run name, the date on which the payment run was executed, the total amount including the bank
charges amount of the payment run, the number of payments created by the payment run, and the status of the payment run
Executed.
Find
This function is available when you select the Load Saved Payment Run or View Executed Payment Run radio button.
Double-click a column in the table to sort the column first, and specify texts that you want to use as a selection criterion for the
column. The first line that matches the entered texts is highlighted in orange.
Go to Final Step
This is custom documentation. For more information, please visit SAP Help Portal. 73

6/8/26, 6:08 AM
This function is available when you select the Load Saved Payment Run or View Executed Payment Run radio button. Select to go
directly to the final step.
For payment runs whose status is Saved, the final step is Step 2 - Defining General Parameters.
For payment runs whose status is Recommended, and for payment order runs, the final step is Step 6 - Viewing
Recommendation Report.
For payment runs whose status is Executed, the final step is Step 8 - Viewing and Printing Payment Run Summary.
More Information
Working with the Payment Wizard
Step 2 - Defining General Parameters
The following are the fields in the second step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 2 - General Parameters
Payment Run Name
Specify a name for the payment run. The default name is a unique code automatically defined by SAP Business One.
Payment Run Date
Specify the date of the payment run. This date becomes the posting date of incoming/outgoing payments to be created by the
payment run. The default date is the current date.
Next Payment Run Date
Specify the date of the next payment run. This is used as a filtering criterion for transactions to be paid.
 Recommendation
Use this field to benefit from cash discounts. For a transaction, if you can get the same cash discount on both the payment run
date and the next payment run date, this transaction will not be included in the recommendation report of the current payment
run.
If this field is left blank, which is the default value, SAP Business One will ignore this setting and list out all transactions that meet
your selection criteria.
This field is available in most of the localizations. Additional information may be found in the localized online help file under: Help
Documentation Localization-Specific Info .
Branch
Select a branch for which you want to run the payment wizard.
 Note
This field is available only if you have enabled multiple branches.
Payment Type
Specify the payment type to be created by the payment run.
This is custom documentation. For more information, please visit SAP Help Portal. 74

6/8/26, 6:08 AM
Select Outgoing to display all open A/P transactions matching your other selection criteria.
Select Incoming to display all open A/R transactions matching your other selection criteria.
Payment Means
Specify the payment means to be used in the payment run.
For the payment type Outgoing, you can select the payment means Check or Bank Transfer.
For the payment type Incoming, only the payment means Bank Transfer is available.
Document Numbering Series
Specify the numbering series to be used in the incoming/outgoing payments.
When you first open the Payment Wizard window, the default value is the default series for incoming/outgoing payments defined
in Administration System Initialization Document Numbering .
After you executed a payment run, the default value is the document numbering series you used for your last executed payment
run.
Min. Payment Amount
Specify the minimum amount for a single incoming/outgoing payment generated by the current payment run.
If the field is left blank, which is the default value, there will be no payment amount limitation.
Bank File Path
Specify the destination path for the bank transfer file. This appears only when you selected the Bank Transfer checkbox in the
Payment Means section.
BP Reference Number
Select the checkbox to display the Cust./Vendor Ref. No. column instead of the Document No. column in the generated
payments.
For payments, selecting the checkbox is the same as selecting the BP Reference Number checkbox on Form Settings –
Outgoing/Incoming Payments Document General subtab.
More Information
Working with the Payment Wizard
Step 3 - Specifying Business Partners
The following are the fields in the third step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
 Note
Business Partners that meet both of the following criteria are not available for selection:
The business partners have a zero balance.
The business partners have no open down payment requests.
This is custom documentation. For more information, please visit SAP Help Portal. 75

6/8/26, 6:08 AM
Step 3 - Business Partner - Selection Criteria
Code From... To...
Specify a range of business partners that you want to include in the payment run.
Expanded Selection Criteria
Select the checkbox to specify up to 5 additional selection criteria from the dropdown lists.
Customer Group
From the dropdown list, select the customer group that you want to include in the payment run. The dropdown list appears only
when you selected the Incoming checkbox in Step 2 - Defining General Parameters.
Vendor Group
From the dropdown list, select the vendor group that you want to include in the payment run. The dropdown list appears only when
you selected the Outgoing checkbox in Step 2 - Defining General Parameters.
Properties
Choose to open the Properties window, in which you can select the business partner properties as selection criteria.
Include Vendors with Debit and Customers with Credit Balance
Select to include business partners with credit balances. By default, the checkbox is unselected.
Add To List
Choose to add the business partners that meet the selection criteria you have specified to the existing table.
Remove From List
Choose to delete the business partners that meet the selection criteria you have specified from the existing table.
Remove Entire List
Choose to clear the existing table.
Business Partner Code, Name, Balance (FC) / (LC)
Displays the code, name, and current balance for the business partner.
More Information
Working with the Payment Wizard
Step 4 - Defining Document Parameters
The following are the fields in the fourth step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 4 – Document Parameters
Selection Priority
From the dropdown list, select the field by which the transactions are sorted in the payment run.
A/P Transaction
This is custom documentation. For more information, please visit SAP Help Portal. 76

6/8/26, 6:08 AM
The section appears only when you selected the Outgoing checkbox in Step 2 - Defining General Parameters.
A/P transactions complying with the following parameters will be included in the payment run:
Posting Date From…To… - Specify a posting date range to include A/P transactions or manual journal entries whose
posting date is within this range.
Due Date From…To… - Specify a due date range to include A/P transactions or manual journal entries whose due date is
within this range. If tolerance days were defined, the due date To date for the payment run will be calculated as follows: <the
original due date To date> minus <the tolerance days>.
Apply to Cash Discount Trans. - Select the checkbox to apply the due date range for all A/P transactions. When the
checkbox is deselected, the due date range will not apply to A/P transactions with cash discounts, that is, when the cash
discount of an A/P transaction is available on the posting date of the payment run, even if its due date is outside the due
date range you specify, the A/P transaction will still be recommended. This checkbox is deselected by default.
This option is available only in localizations where cash discount functionality is supported. Additional information may be
found in the localized online help file under Help Documentation Localization-Specific Info .
Tolerance Days - Specify the number of days to adjust the due date range of A/P transactions or manual journal entries. If
tolerance days were defined, the due date To date for the payment run will be calculated as follows: <the original due date
To date> minus <the tolerance days>.
Min. Cash Discount % - Specify the minimum cash discount percentage to include A/P transactions or manual journal
entries whose cash discount is equal to or greater than this value.
This option is available only in localizations where cash discount functionality is supported. Additional information may be
found in the localized online help file under Help Documentation Localization-Specific Info .
Document Date From…To… - Specify a document date range to include A/P transactions or manual journal entries whose
document date is within this range.
Balance Due (LC) From…To… - Specify a balance due range to include A/P transactions or manual journal entries whose
balance due is within this range.
Document No. From…To… - Specify a document number range to include A/P transactions or manual journal entries whose
document number is within this range.
Blanket Agreement No. From... To... - Specify an agreement range if you want to refine the selection by blanket agreement.
A/R Transaction
The section appears only when you selected the Incoming checkbox in Step 2 - Defining General Parameters.
A/R transactions complying with the following parameters will be included in the payment run:
Due Date From...To... - Specify a due date range to include A/R transactions or manual journal entries whose due date is
within this range.
Document No. From...To... - Specify a document number range to include A/R transactions or manual journal entries whose
document number is within this range.
Blanket Agreement No. From... To... - Specify an agreement range if you want to refine the selection by blanket agreement.
Include Manual Journal Entries
Select to include manual journal entries. The checkbox is selected by default.
Include Negative Transactions Within Cumulative Positive BP Balances
Select to include negative transactions for business partners who have an overall positive balance (that is, vendors with a credit
balance or customers with a debit balance). The checkbox is selected by default.
This is custom documentation. For more information, please visit SAP Help Portal. 77

6/8/26, 6:08 AM
More Information
Working with the Payment Wizard
Step 5 - Specifying Payment Method
The following are the fields in the fifth step of the payment wizard. The step lists all the payment methods that match your
selection criteria. The payment methods are grouped first by the G/L accounts linked to their house bank accounts, and then by
their payment types.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 5 - Payment Method - Selection Criteria
[Selection Column]
Select the payment methods to include in the current payment run.
G/L Bank Acct, G/L Intm Acct
Displays the G/L account and G/L interim account linked to the house bank account for the current payment method.
Code, Description
Displays the code and description of the payment method.
Country/Region, Bank Code, Account No.
Displays the country/region, code, and account number defined for the house bank of the specific payment method. You can
specify a different house bank account for the current payment method in the List of House Bank Account window.
In the List of House Bank Account window, you can choose the button in the toolbar to select the fields that you want to
display and group them.
Max. Incoming Amt
Available only for the payment methods whose payment type is Incoming. Specify the maximum amount to be recorded in the G/L
account or the maximum amount for the corresponding payment method for the current payment run.
 Note
If the maximum incoming amount for the G/L account is zero, all the payment methods under this G/L account will be treated
as there is no amount restriction. Otherwise, all the payment methods under this G/L account will be processed according to
the value limitation in the field.
Max. Outgoing Amt
Available only for the payment methods whose payment type is Outgoing. Specify the maximum amount to be recorded in the G/L
account or the maximum amount for the corresponding payment method for the current payment run.
The default amount is the current debit balance (if it exists) of the selected house bank account, which is the maximum amount
that can be paid from your selected house bank account. You can overwrite this value.
 Note
If the maximum incoming amount for the G/L account is zero, all the payment methods under this G/L account will be treated
as there is no amount restriction. Otherwise, all the payment methods under this G/L account will be processed according to
the value limitation in the field.
This is custom documentation. For more information, please visit SAP Help Portal. 78

6/8/26, 6:08 AM
G/L Balance
Displays the current balance of the G/L account linked to the house bank account of the payment method.
G/L Interim Acct Bal.
Displays the current balance of the G/L interim account linked to the house bank account of the payment method.
Expected G/L Balance
If the Include G/L Interim Acct Balance checkbox is unselected, displays the expected G/L account balance as a combination of
the current G/L account balance displayed in the G/L Balance field, and the amount you specified in the Max. Incoming Amt or
the Max. Outgoing Amt field.
For incoming payments, displays the result of the G/L balance plus the maximum incoming amount for the payment
method.
For outgoing payments, displays the result of the G/L balance minus the maximum outgoing amount for the payment
method.
If the Include G/L Interim Acct Balance checkbox is selected, displays the expected G/L account balance as a combination of the
current G/L account balance displayed in the G/L Balance field, the amount you specified in the Max. Incoming Amt or the Max.
Outgoing Amt field, and the current G/L interim account balance displayed in the G/L Interim Acct Bal. field.
For incoming payments, displays the result of the G/L balance plus the maximum incoming amount plus the G/L interim
account balance for the payment method.
For outgoing payments, displays the result of the G/L balance minus the maximum outgoing amount plus the G/L interim
account balance for the payment method.
Bank File Format Type
Displays the format type of the bank file. There are two types of format: DLL format, and EFM – BPP format.
 Note
If you have not installed the Payment Engine add-on, only the EFM format of bank files can be generated with the Payment
Wizard.
Include G/L Interim Acct Balance
Select to take the G/L interim account balance into consideration when calculating the expected G/L balance.
[Arrow Up/Down]
Choose the buttons to change the payment method orders in the G/L bank account groups. For the same G/L bank account, the
payment methods will be processed by sequence in the following steps, that is, the first selected payment method will be
processed first.
More Information
Working with the Payment Wizard
Step 6 - Viewing Recommendation Report
The following are the fields in the sixth step of the payment wizard.
The transactions are grouped in the following order:
This is custom documentation. For more information, please visit SAP Help Portal. 79

6/8/26, 6:08 AM
1. By business partners
2. By payment methods
3. By the grouping options you defined in the payment methods. For more information, see Payment Methods - Setup.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 6 - Recommendation Report
Find
Sort a column first, and specify the texts that you want to use as a selection criterion for the column. The first line that matches
the entered texts is highlighted in orange. If you do not sort a column, SAP Business One searches the texts in the BP Code column
by default.
To sort a column in the report, double-click the column name. The column name will be marked with or . Transactions will be
sorted within its payment document.
[Selection Column]
Select the payments or open transactions to be included in the payment run.
Pmt No.
Displays the numbers countering the payments recommended for creation. Choose to view the related documents.
Status
Displays one of the following three icons for each payment:
A green icon indicates that a payment method you selected in step 5 is used.
You can go on creating a payment.
A yellow icon indicates that the payment total is negative and the payment method you selected in step 5 is updated to its
negative payment method.
You can go on creating an opposite payment for the business partner, that is, an incoming payment will be created for a
vendor, or an outgoing payment will be created for a customer.
A red icon indicates that the payment total is negative and the payment method you selected in step 5 cannot be updated
to its negative payment method due to various reasons. To see the specific reason why the validation failed, hover your
mouse over the icon for the tooltip. For more information about payment method validation, see Payment Methods - Setup.
You cannot continue creating a payment.
For more information, see Paying Negative Totals Using the Payment Wizard.
G/L Account Code
Displays the offsetting account in the journal entry to be created by the payment. This is either the G/L account or the G/L interim
account, depending on the payment method definition.
Installment No.
Displays the sequential number of the installment to be paid.
Total
Displays the total amount of the transaction or specific installment.
Balance Due
This is custom documentation. For more information, please visit SAP Help Portal. 80

6/8/26, 6:08 AM
Displays the balance due of the transaction or specific installment.
Discount %
Displays the cash discount specified in the transaction. You can overwrite this value.
Discount Due Date
Displays the last day when you can get the cash discount calculated according to the payment terms linked to the specific
transaction.
It displays the document due date when one of the following situation applies:
The cash discount is no longer applicable, that is, the posting date of the payment wizard is later than the latest cash
discount due date.
There is no payment terms information for the specific transaction, for example, a manual journal entry.
No cash discount is defined in the payment terms linked to the specific transaction.
The cash discount due date is later than the document due date.
To view all potential cash discounts, right-click a transaction row, and choose Possible Cash Discount.
Document Amount
Displays the balance due amount after discount of the transaction. You can overwrite this value.
If this amount is changed, the value in the Pmt Amount field is updated accordingly and a partial payment will be created. After the
payment run is executed, the values in the Applied Amount and the Balance Due fields of the transactions are updated
accordingly.
Document Type
Displays the type of the transaction. For example, IN represents A/R invoice. For the complete list of document types, see
Transaction Type Abbreviations Legend.
Payment Currency
Select a currency for the payment.
BP Ref. No.
For A/P or A/R transactions, displays the value in the Vendor Ref. No. or Customer Ref. No. field in the general area of the
corresponding window.
For journal entries, displays the value in the Ref. 2 field for the business partner row of the Journal Entry window in the
expanded editing mode.
 Note
The field is not visible by default. You can set it visible through the Form Settings window.
Reference
Specify a reference for the payment. It will appear in the Ref. 3 field for the G/L account row in the expanded editing mode of the
journal entry to be created by this payment.
 Note
This field is available only for bank transfers.
This is custom documentation. For more information, please visit SAP Help Portal. 81

6/8/26, 6:08 AM
Distribution Rule
Specify a distribution rule for the transaction.
*
If the due date of the open transaction is earlier than or equal to the payment wizard posting date (that is, the item is
overdue), the column displays an asterisk (*).
If the due date of the open transaction is later than the payment wizard posting date (that is, the item is not overdue), the
column is empty.
Overdue Days
If the open item due date is earlier than the posting date of the payment wizard, the number of overdue days is displayed in
red.
If the open item due date is equal to the posting date of the payment wizard, 0 is displayed in black.
If the item is not overdue (that is, the open item due date is later than the posting date of the payment wizard), the number
of overdue days is displayed in black, preceded by a minus (-) sign.
Bank Charge, Bank Charge (FC)
Specify the amount of bank charge for the payment. The default value is calculated as the payment amount multiplied by the bank
charge rate you defined in Payment Methods - Setup.
 Note
The fields are not visible by default. You can set them visible through the Form Settings window.
 Note
The fields are not available for bills of exchange.
Project
Specify the project code for the payment.
 Note
The field is not visible by default. You can set it visible through the Form Settings window.
Pmt Amount, Pmt Amount (FC)
Displays the payment amount in the local and foreign currency.
For incoming payments, the payment amount is calculated as the document amount minus the bank charge amount.
For outgoing payments, the payment amount is calculated as the document amount plus the bank charge amount.
SEPA Seq. Type
SEPA Seq. Type (Single Euro Payment Area Sequence Type) is the sequence type of a direct debit mandate. SEPA Seq. Type is
determined by the setting chosen in Business Partner Bank Accounts - Setup Window but can be changed in the wizard. The
options for SEPA Seq. Type include:
FRST: first
FNAL: final
OOFF: one-off
This is custom documentation. For more information, please visit SAP Help Portal. 82

6/8/26, 6:08 AM
RCUR: recurring
If two or more payments of the same mandate are arranged, the first payment needs to be marked as FRST and the next payment
needs to be marked as RCUR or FNAL. SEPA Seq. Type is applicable to SEPA-relevant localizations only.
No. of Checks
Displays the number of checks to be created by this payment run. You can overwrite this value.
A change affects the values in the First Check and Next Check fields because the amounts will be recalculated for the new number
of checks.
 Note
This field is available only for checks.
First Check
Displays the amount of the first check.
If there is only one check, this field displays the value in the Pmt Amount field. You cannot change this value.
If there is more than one check, this field displays the value in the Pmt Amount field divided by the number of checks
defined in the No. of Checks field. You can change this value.
 Note
This field is available only for checks.
Next Check
Displays the amount of the second check.
If there is only one check, this field displays 0. You cannot change this value.
If there is more than one check, this field displays the result of the following: (the value in the Pmt Amount field – the value
in the First Check field)/(the value in the No. of Checks field – 1). You can change this value.
 Note
This field is available only for checks.
Payment Order Status
Displays the status of the payment order rows. C stands for closed, which means the balance dues of all the documents in this
payment order row are zero, that is, the documents are fully paid, credited, or internally reconciled. This appears only after you
choose the Close Payment Order Rows button.
Primary Form Item
For G/L accounts or interim G/L accounts that are cash flow relevant, you can specify the cash flow line item or define a new
assignment in the Combined Cash Flow Assignment window.
The default value is the primary form cash flow line item you defined for incoming/outgoing payments on the Cash Flow tab of the
General Settings window.
Bank File Format Type
Displays the format type of the bank file. There are two types of format: DLL format, and EFM – BPP format.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 83

6/8/26, 6:08 AM
If you have not installed the Payment Engine add-on, only the EFM format of bank files can be generated with the Payment
Wizard.
Non-Included Trans.
Choose to open the Non-Included Trans. Report window displaying all transactions not included in the recommendation report
with errors.
Refresh
Choose the button to recalculate the recommendation report and the non-included transaction report according to the current
data.
Add Manual Row
Choose to create a payment document or a payment order row between a house bank account and a business partner or a target
account without referencing any documents in SAP Business One.
To change an already added manual row, double-click the payment order row, and make changes in the Payment Row - Details
window.
 Caution
If you go to any previous steps in the payment wizard, and then come back to the recommendation report, the manually-added
rows will disappear.
Close Payment Order Rows
Choose the button to close payment order rows in which all the documents have a zero balance due.
More Information
Working with the Payment Wizard
Non-Included Trans. Report
Step 7 - Saving Options
The following are the fields in the seventh step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Wizard: Step 7 - Save Options
Save Selection Criteria Only
Select to save the selection criteria without the recommendation report. After choosing Next and closing the system message,
choose Finish to end the payment wizard session.
This does not reserve the selected open transactions for this payment run. You can still clear the transactions either using the
incoming/outgoing payment documents or using a new payment run. When loading a saved payment run, it does not display
transactions that are already cleared.
Save Recommendations
Select to save both the selection criteria and the recommendation report. After choosing Next, Step 8 - Viewing and Printing
Payment Run Summary appears, in which you can view and print various simulated Payment Wizard Reports.
This is custom documentation. For more information, please visit SAP Help Portal. 84

6/8/26, 6:08 AM
This reserves the selected open transactions for this payment run only, which means that open transactions saved by this option
cannot be cleared using the incoming/outgoing payment documents or a new payment run.
 Note
To delete a recommended payment run, in Step 1 - Selecting Payment Run Options, select the payment run, right-click and
choose Cancel.
Execute Payment Order Run
Select to generate a payment order. After choosing Next and closing the system message, Step 8 - Viewing and Printing Payment
Run Summary appears, in which you can view and print various simulated Payment Wizard Reports.
This option enables you to generate electronic outbound bank files without creating payment documents. This reserves the
selected open transactions for this payment order run only. You cannot include the open transactions in another payment run or
payment order run. You will be warned when you clear the open transactions using the incoming/outgoing payment documents
and when you internally reconcile the open transactions. You can clear the open transactions via the BSP function. When the open
transactions are cleared, the payment order run remains open unless you close the open transactions using the Close Payment
Order Rows button in Step 6 - Viewing Recommendation Report.
 Note
Before generating electronic outbound bank files, you need to install and start the Payment add-on. The bank files are the same
as those generated for payment runs except for the following situation: when the bank file includes payment document number,
as the payment documents are not created in SAP Business One yet, the payment document number will be replaced by a
payment order number.
 Note
To delete a payment order run, in Step 6 - Viewing Recommendation Report, right-click on payment order rows one by one, and
choose Remove, until all the checkboxes are unselected in the selection column. Alternatively, in Step 1 - Selecting Payment
Run Options, select the payment order run, right-click and choose Cancel.
Execute Payment Run
Select to generate payments and payment documents. After choosing Next and closing the system message, Step 8 - Viewing and
Printing Payment Run Summary appears, in which you can view and print various Payment Wizard Reports.
More Information
Working with the Payment Wizard
Step 8 - Viewing and Printing Payment Run Summary
The following are the fields in the eighth step of the payment wizard.
To open the payment wizard, from the SAP Business One Main Menu, choose Banking Payment Wizard .
Payment Run Summary Section
Payments were added
Number of payments created in the payment run.
If this is a simulation of the payment run summary, displays 0.
This is custom documentation. For more information, please visit SAP Help Portal. 85

6/8/26, 6:08 AM
Checks were added
Number of checks created in the payment run.
If this is a simulation of the payment run summary, displays 0.
Bank transfers were added
Number of bank transfers created in the payment run.
If this is a simulation of the payment run summary, displays 0.
Document and Report Printing Section
Outgoing Payments, Incoming Payments
Select to print the outgoing and/or incoming payments created in the payment run.
If this is a simulation of the document and report printing, the checkboxes are not available.
Non-Included Transactions, Country/Region Summary, Currency Summary, BP Summary, Payment Method Summary, Bank
Account Summary, Payment Summary
Select to print the Payment Wizard Reports. Choose the button to display each report.
Checks
Select to view the check-related information and print the checks created in the payment run. The check-related information
includes the bank name, the bank account for which the check was created, and the range of check numbers drawn from the bank
account.
If this is a simulation of the document and report printing, the checkbox is not available.
Print
Choose to open the standard Microsoft Windows Print window.
Bank File
You can generate bank files at the end of the payment run.
 Note
If you have already executed the payment wizard run, the Bank File button is disabled. To enable it, first choose the Recreate
File button in Step 8 to update OPEX and Payment Wizard tables.
 Note
To use the Payment Engine without the Payment add-on, you require full authorization for the window.
To assign authorization for the Payment Engine to users, from the SAP Business One Main Menu, choose Administration
System Initialization General Authorizations . In the General Authorizations window, choose Banking Payment
System Payment Wizard Payment Engine .
To generate a bank file, follow these steps:
1. In the Payment Wizard, choose the Bank File button. The Payment Engine window opens.
2. In the Select Path field, define a folder in which to save your bank files. The path is stored for each client and is used as a
default path. In each case, the last path that you define in the Select Path field is stored.
3. Select the Test Run radio button.
This is custom documentation. For more information, please visit SAP Help Portal. 86

6/8/26, 6:08 AM
 Note
You must always successfully complete a test run before starting a production run.
4. To start a test run, choose the Create Files button.
 Note
After you complete a successful test run, temporary bank files are generated for the test run, and the radio button
switches to Production Run automatically.
5. On the Protocol tab, view the test run results.
6. On the Preview tab, view the location of the generated files.
 Note
Double-clicking a file in the list opens the file content on the Payment File tab. On the Payment File tab, view the file
content.
7. To generate the bank files, make sure that the Production Run radio button is selected.
 Note
After you complete a successful production run, the Preview tab changes to the Created Files tab.
8. On the Created Files tab, view the location of the generated files.
 Note
Double-clicking a file in the list opens the file content on the Payment File tab.
9. On the Payment File tab, view the file content. To save your changes, choose the Update button.
More Information
Working with the Payment Wizard
Payment Wizard Reports
Use payment wizard reports to view detailed information about different aspects of payment wizard runs.
Prerequisites
In the eighth step of the payment wizard: Payment Run Summary and Printing, you have chosen the button to display one of
the following reports:
Non-Included Trans. Report
Country/Region Summary Report
Currency Summary Report
BP Summary Report
Payment Method Summary Report
This is custom documentation. For more information, please visit SAP Help Portal. 87

6/8/26, 6:08 AM
Bank Account Summary Report
Payment Summary Report
Non-Included Trans. Report
The following are the fields in the Non-Included Trans. Report window, which you can open in both the sixth and the eighth step of
the payment wizard. The window can be displayed only when there are invoices that cannot be included in the payment run.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Non-Included Trans. Report
Installment
Displays the sequential number of the installment.
Posting Date
Displays the posting date of the transaction.
Amount
Displays the amount of the transaction or installment.
Country/Region Summary Report
The following are the fields in the Country/Region Summary Report window, which can be displayed and printed in the eighth step
of the payment wizard.
Country/Region Summary Report
Country/Region Code, Country/Region Name
Displays the code and name of the countries/regions of the business partners for which the payments were created.
Paid Amount (LC), Paid Amount (FC)
Displays the total amount including the bank charges amount paid to and/or by business partners in each country/region.
Currency Summary Report
The following are the fields in the Currency Summary Report window, which can be displayed and printed in the eighth step of the
payment wizard.
Currency Summary Report
Currency Code, Currency Name
Displays the code and name of the currencies involved in the payment run.
This is custom documentation. For more information, please visit SAP Help Portal. 88

6/8/26, 6:08 AM
Paid Amount
Displays the total amount including the bank charges amount paid in each currency.
BP Summary Report
The following are the fields in the BP Summary Report window, which can be displayed and printed in the eighth step of the
payment wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
BP Summary Report
Posting Date, Due Date
Displays the posting date and due date of the transaction involved in the payment run.
Document No.
Displays the document number in SAP Business One. You can choose to open the transaction.
Installment ID
Displays the sequential number of the installment.
Document Amount, Document Amount (FC)
Displays the document amount of the transaction or installment.
Applied Amount, Applied Amount (FC)
Displays the total amount excluding the bank charges amount paid for the transaction or installment in the payment run.
Bank charges amounts are paid at the payment level, so for information at the document level, there is only the applied amount.
Payment Method Summary Report
The following are the fields in the Payment Method Summary Report window, which can be displayed and printed in the eighth
step of the payment wizard.
Payment Method Summary Report
Payment Method, Description
Displays the code and description of the payment method involved in the payment run.
Bank Name
Displays the name of the bank linked to the payment method. The bank is taken from Payment Wizard: Step 5 - Payment Methods.
Paid Amount (LC), Paid Amount (FC)
Displays the total amount including the bank charges amount paid through the payment method.
This is custom documentation. For more information, please visit SAP Help Portal. 89

6/8/26, 6:08 AM
Bank Account Summary Report
The following are the fields in the Bank Account Summary Report window, which can be displayed and printed in the eighth step
of the payment wizard.
Bank Account Summary Report
Bank Name, Bank Account Number
Displays the name of the bank and bank account involved in the payment run.
Paid Amount (LC), Paid Amount (FC)
Displays the total amount including the bank charges amount paid through the bank account.
Payment Summary Report
The following are the fields in the Payment Summary Report window, which can be displayed and printed in the eighth step of the
payment wizard.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Checks Summary Report
Bank Name, Bank Account Number
Displays the name of the bank and the bank account involved in the payment run.
Internal Check No.
Displays the document number of the check created by the payment run. You can choose to open the Checks for Payment
window. If this is a simulation of the checks summary report, this field is empty.
Check No.
Displays 0. Check numbers are assigned only after the printing takes place. If this is a simulation of the checks summary report,
this field is empty.
No. of Documents
Displays the number of transactions paid by the check. If this is a simulation of the checks summary report, this field is empty.
Payment Amount, Payment Amount (FC), Payment Amount (SC)
Displays the check amount including the bank charges amount in local currency, foreign currency, and system currency. The values
are calculated according to the exchange rate of the payment run date.
Bank Transfer Summary Report
Bank Name, Bank Account Number
Displays the name of the bank and the bank account involved in the payment run.
Payment Doc. No.
This is custom documentation. For more information, please visit SAP Help Portal. 90

6/8/26, 6:08 AM
Displays the document number of the incoming or outgoing payment created by the payment run. You can choose to open the
Incoming Payments or Outgoing Payments window. If this is a simulation of the bank transfer summary report, this field is empty.
No. of Documents
Displays the number of transactions paid by the bank transfer. If this is a simulation of the bank transfer summary report, this field
is empty.
Payment Amount, Payment Amount (FC), Payment Amount (SC)
Displays the bank transfer amount including the bank charges amount in local currency, foreign currency, and system currency.
The values are calculated according to the exchange rate of the payment run date.
Generating the Payment Orders Report
Context
Creating a payment order in the payment wizard is the first step in generating a request to the bank to create an outgoing or
incoming payment for specific business partners and documents. The payment order amount is the sum of all documents that are
included in a payment order row of a payment order run. You can generate bank files for payment orders without creating
payments in SAP Business One. You send the bank files to the bank, and the request process is completed.
 Note
Before generating electronic outbound bank files, you need to install and start the Payment add-on. The bank files are the same
as those generated for payment runs except for the following situation: when the bank file includes payment document number,
as the payment documents are not created in SAP Business One yet, the payment document number will be replaced by a
payment order number.
You use the Payment Orders Report by Business Partner - Selection Criteria window or the Payment Orders Report by Payment
Run - Selection Criteria window to display detailed information for one or more payment orders.
Procedure
1. From the SAP Business One Main Menu, choose Banking Banking Reports Payment Orders Report by Business
Partner or Payment Orders Report by Payment Run .
2. In the Payment Orders Report by Business Partner - Selection Criteria window or in the Payment Orders Report by
Payment Run - Selection Criteria window, specify a range for each field to define the information to be included in the
report.
3. When you have finished, choose the OK button.
Results
The Payment Orders Report by Business Partner window or the Payment Orders Report by Payment Run window appears,
displaying detailed information for the payment order runs that match your selection criteria.
Paying Negative Totals Using the Payment Wizard
Prerequisites
To use the payment wizard, make sure you have set up the following:
This is custom documentation. For more information, please visit SAP Help Portal. 91

6/8/26, 6:08 AM
1. Banks
2. House Bank Accounts
3. Payment Methods
4. Payment methods on Business Partner Master Data: Payment Run Tab
Context
To generate payments of negative totals in the payment wizard, follow the procedure below.
Procedure
1. On the General tab of the Document Settings window, select the Enable Negative Payment for Payment Wizard checkbox.
For more information, see Document Settings: General Tab.
2. In the Payment Methods - Setup window, define a negative payment method for the payment method that you want to use
in the payment wizard. For more information, see Payment Methods - Setup.
If the payment method that you want to use in the payment wizard is included for a business partner, the negative payment
method you defined will be automatically included for the business partner.
3. On the Payment Run tab of the Business Partner Master Data window, ensure that both payment methods are included.
The two payment methods are the payment method that you want to use in the payment wizard and its negative payment
method. For more information, see Business Partner Master Data: Payment Run Tab.
4. From the SAP Business One Main Menu, choose Banking Payment Wizard .
The first window provides a brief introduction to the payment wizard. Choose Next to start the payment wizard.
5. Make the required choices in each step. For more information, see Working with the Payment Wizard.
6. In step 6, for payments with negative totals, a yellow icon appears in the Status column for each payment. This indicates
that the payment method you selected in step 5 is updated to its negative payment method. Choose the Next button to
create an opposite payment for the business partner, that is, an incoming payment will be created for a vendor, or an
outgoing payment will be created for a customer.
For more information about the Status column, see Payment Wizard: Step 6 - Recommendation Report.
 Note
If the validation of the negative payment method does not pass, a red icon appears in the Status column. To see the
specific reason why the validation failed, hover your mouse over the icon for the tooltip. For more information about the
payment method validation, see Payment Methods - Setup.
You cannot continue creating a payment when a red icon appears in the Status column.
Results
Once the payment run is executed, an opposite payment is generated for the business partner, using the negative payment
method. This means that an incoming payment is created for a vendor, or an outgoing payment is created for a customer.
Combined Cash Flow Assignment Window
Use this window to assign the active cash flow line items, and their corresponding amounts, to a cash relevant transaction,
enabling you to generate the Cash Flow report.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 92

6/8/26, 6:08 AM
The cash flow line items must be defined during initial configuration.
To access this window:
1. Choose Banking Incoming/Outgoing Payments Incoming/Outgoing Payments , and choose .
2. In the displayed Payment Means window, click the Primary Form Item field, and choose Define new assignment.
Combined Cash Flow Assignment Window
G/L Account
The cash flow-relevant G/L account is automatically defined from the previous transaction and is not editable.
Total
This value is automatically defined from the previous transaction and is not editable.
Primary Form Item
Specify the relevant cash flow line item from those previously defined in the Cash Flow Line Items - Setup window.
 Note
You can change the cash flow line item:
After the payment is executed, unless the payment is a credit card partial or split payment
At a later stage, in the corresponding journal entry or original transaction, unless the transaction has been cancelled
Amount(LC)
Automatically calculates and displays the remaining amount in Total, unless the field already contains a value. You can change this
field manually.
Amount(FC)
Automatically calculates and displays the remaining amount in Total, unless the field already contains a value. You can change this
field manually.
If the amount is not in local currency, it is automatically calculated in local currency, according to the appropriate exchange rate.
 Note
This column is not displayed if the amount is already in local currency.
Subtotal Amount
Automatically calculates and displays the current total value as each amount is inserted.
The Update button is disabled until the Subtotal amount is equal to the Total amount at the top of the window.
More Information
Cash Flow Line Items - Setup
Cash Flow Report Window
This is custom documentation. For more information, please visit SAP Help Portal. 93

6/8/26, 6:08 AM
Working with Bank Statement Processing
The bank statement processing function lets you generate incoming and outgoing payments, and perform internal, and external,
reconciliation. By entering bank statement details, either automatically or manually, you can create transactions that have not yet
been posted, such as incoming payments from a customer or notifications of clearance of payments to a vendor.
Bank statement processing supports the following scenarios:
Creating, posting, and internal reconciliation of those business partner incoming and outgoing payments made by direct
debit or bank transfer and not already entered in SAP Business One
Posting and internal reconciliation of interim accounts used in payments with the payment means of bank transfer (via
either the payment wizard or manual payment)
Posting and external reconciliation of bank debits and credits, for example, bank handling charges and interest payments
External reconciliation of transactions already posted in SAP Business One, for example, by manual payments or the
payment wizard
Prerequisites
Bank statement processing is activated for your company
File formats have been uploaded for imported bank statements from given banks
The following are set up in SAP Business One to support bank statement processing for your company:
Banks
House bank accounts
Internal bank operation codes
External bank operation codes
Matching criteria
Related Information
Setting Up Bank Statement Processing
Using Bank Statement Processing
Bank Statement Processing Windows
Bank Statement Processing Business Scenarios
Using Bank Statement Processing
Prerequisites
Your company superuser has activated bank statement processing.
Context
The interactive graphics below help you navigate through this section. Choose the highlighted areas for more information.
This is custom documentation. For more information, please visit SAP Help Portal. 94

6/8/26, 6:08 AM
Please note that image maps are not interactive in PDF outputs.
Related Information
Working with Bank Statement Processing
Entering Bank Statements
You can add bank statement information to SAP Business One using bank statement processing as follows:
Manually import bank statements
For more information, see: Adding Bank Statements Manually.
Automatically import bank statements
For more information, see: Importing Bank Statements Automatically.
Importing Bank Statements Automatically
Prerequisites
You have assigned a bank statement format (BFP) to the house bank account specified in the header area. For more
information, see Assigning Bank Statement Formats to House Bank Accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 95

6/8/26, 6:08 AM
In the House Bank Accounts – Setup window, you have selected the Imported Bank Statement checkbox of the house
bank account specified in the header area.
The bank file containing the required bank statement is located on an accessible server or PC client.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statement and External Reconciliation Bank
Statement Processing .
2. In the Bank Statement Summary window, specify information in the general area fields, and then choose the Import from
File button.
3. In the folder list, locate and open the folder containing the required bank file.
4. Select the bank file and then choose the Open button to start importing the bank file automatically.
Results
The bank statement information appears in the Bank Statement Details window. You can now perform internal and external
reconciliation and create a draft bank statement.
Adding Bank Statements Manually
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statement and External Reconciliation Bank
Statement Processing .
2. In the Bank Statement Summary window, specify, in the appropriate general area fields, the information appearing in the
bank statement header, and then choose the Create New button.
3. In the Bank Statement Details window, enter the data appearing in each bank statement transaction row.
Results
You can now perform internal and external reconciliation and create a draft bank statement.
Accessing Bank Statements
Context
You can access bank statements in the Bank Statement Summary window, which contains a list of all bank statements for the
bank account specified in the general area:
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statement and External Reconciliation Bank
Statement Processing .
2. In the general area in the Bank Statement Summary window, specify the required information.
Results
This is custom documentation. For more information, please visit SAP Help Portal. 96

6/8/26, 6:08 AM
A list of all bank statements is displayed in the table of the Bank Statement Summary window, according to the bank account
information you have specified in the general area.
Creating a Draft Bank Statement
Saving as a draft allows you to access and finalize the bank statement at a later time or date. For example, if you need to check
information or wait for an approval before finalizing, you can save the bank statement as a draft and then call it up later and
subsequently finalize it.
Procedure
Define at least one transaction row in the Bank Statement Details window and choose the Save Draft button.
Result
A draft bank statement is added to SAP Business One and can be accessed through the Bank Statement Summary window, and
viewed by running the Bank Statement Information report.
Validating Posting Proposals
Posting proposals are references to existing transactions proposed for linking with transactions associated with or generated from
bank statement rows.
After you enter all required transaction rows in the Bank Statement Details window, you can begin to reconcile the bank
statement. When you choose the Posting Proposal for Uncleared Rows button, SAP Business One prepares posting proposals for
the transaction rows in the bank statement based on the matching criteria predefined during setup.
Prerequisites
At least 1 transaction row is defined in the Bank Statement Details window under Banking Bank Statement and External
Reconciliation Bank Statement Processing Bank Statement Summary .
Procedure
1. In the Bank Statement Details window, choose the Posting Proposal for Uncleared Rows button. SAP Business One
retrieves documents and journal entries based on the predefined matching criteria as candidates for the posting proposal.
2. Optionally, select Expand All mode to view details of the retrieved documents and journal entries for each transaction row.
3. Optionally, review the posting proposals for every transaction row. The objective is to clear all bank statement rows.
To clear the posting proposal for a transaction row, select the Cleared/Selected checkbox.
When you choose the Add Draft button, all rows that have been cleared are deleted.
To reject the posting proposal for a transaction row, deselect the Cleared/Selected checkbox.
You can change some values (such as discount percentage, discount value, value for partial payment, and more) on marketing
document rows.
You can add rows to the table by right-clicking any row in a table row and choosing Add Row. Only rows marked as Cleared are
saved.
This is custom documentation. For more information, please visit SAP Help Portal. 97

6/8/26, 6:08 AM
Example
Internal Bank Operation Code Posting Method Posting Proposal
BP BT Acc BP from/to Bank Account Existing marketing documents (invoices,
credit memos, down payment requests)
and business partner related journal entries
BP G/L Acc G/L Account from/to Bank Proposed journal entries
BP BT Interim Interim Account from/to Bank Accountt Existing journal entries
BP BT External External Reconciliation Existing journal entries
Performing Manual Reconciliation
Prerequisites
At least 1 posting proposal has been defined in the Bank Statement Details window under Banking Bank Statement and
External Reconciliation Bank Statement Processing Bank Statement Summary .
Context
When you generate a posting proposal, it is likely that some of the bank statement rows will not be automatically matched. For
example, if you cannot identify which business partner an unmatched payment relates to, you will not be able to assign a business
partner code. You cannot finalize a bank statement until every bank statement row is cleared.
Bank statement rows are only automatically matched if the posting proposal returns an unambiguous result. To reconcile any
unmatched or inadequately matched rows, you need to perform manual reconciliation.
 Note
Manual reconciliation is not available for payments to account, but you can still enter or change payment accounts in the Bank
Statement Row - Details Expanded window.
Procedure
1. In the Bank Statement Details window, double-click the row number of a bank statement row. The Bank Statement Row -
Details Expanded window appears.
2. In the general area and in the table area, specify the required information. You can add further documents or transactions
as possible matches for reconciliation as follows:
To access a list of open sales and purchasing documents, choose the Add Open Documents button. The Add Open
Documents window appears.
To access a list of open journal entry transactions by business partner, choose the Add Open BP JEs button. The
Add Open BP JEs window appears.
To access a list of open transactions, choose the Add Open Transactions button. The Add Open Transactions
window appears.
3. Select a document or journal entry row and choose the OK button.
4. In the Bank Statement Row - Details Expanded window, select document or journal entry rows as required. To prevent
unselected rows appearing in the Bank Statement Details window, select the Discard Unselected Rows checkbox.
This is custom documentation. For more information, please visit SAP Help Portal. 98

6/8/26, 6:08 AM
5. Choose the Update button.
Results
The selected document or journal entry is matched to the relevant bank statement transaction row in the Bank Statement Details
window.
Setting Matching Criteria for Manual Reconciliation of Business
Partner Payments
Context
After accessing the expanded details of a posting proposal in the Bank Statement Row Details - Expanded window, you can
further refine manual reconciliation of business partner payments by setting matching criteria. You can define up to 3 matching
rules.
SAP Business One uses these matching criteria based on the posting methods specified in the Posting Method column in the
Internal Bank Operation Codes window under Administration Setup Banking Bank Statement Processing , or in the
bank statement row.
Documents - rules for when the specified posting method is Business Partner from/to Bank Account for reconciling the
following:
Sales – A/R documents, such as invoices issued to customers and the related incoming payments
Purchasing – A/P documents, such as invoices received from vendors and the related outgoing payments
BP Journal Entries - rules for when the specified posting method is Business Partner from/to Bank Account.
Since journal entries have different matching parameters from those of sales and purchasing documents, there is a
separate set of matching criteria for journal entries.
Transactions - rules for when the specified posting method is Interim Account from/to Bank Account or External
Reconciliation.
Processing Multiple Payments
Prerequisites
In the Bank Statement Details window, you have specified the G/L Account/Doc. Identification No. field, which is required in the
processing of multiple payments.
Context
Bank statement processing supports multiple payments for a particular bank statement row. Some banks are able to deliver more
than one identification number for paid documents linked to the payment. These identification numbers are stored on the
particular bank statement row or in a separate file.
To process multiple payments with automatic matching, you need to save one or more identification numbers on the rows of the
bank statement in the Bank Statement Details window. When the button in the Identification No. field is chosen, SAP Business
One allows entry of new numbers or shows a list of existing numbers. If relevant, you can add additional new rows into the list. You
can also add amounts to each row if there are partial payments included.
This is custom documentation. For more information, please visit SAP Help Portal. 99

6/8/26, 6:08 AM
Based on the predefined matching criteria and the identification numbers, when you choose the Posting Proposal for Uncleared
Rows button, SAP Business One generates a posting proposal listing all marketing documents found. A posting proposal is only
accepted for posting if all matched documents belong to the same business partner.
Procedure
1. In the Bank Statement Details window, place your cursor within the G/L Account/Doc. Identification No. field.
2. Press TAB , or choose the button, or right-click and choose Multiple Payments.
3. In the Multiple Payments window, specify the required information.
Finalizing a Bank Statement
Prerequisites
At least 1 posting proposal has been defined in the Bank Statement Details window under Banking Bank Statement and
External Reconciliation Bank Statement Processing Bank Statement Summary .
Context
Finalizing a bank statement can only take place if the difference between the values shown in the Starting Balance and Ending
Balance fields in the Bank Statement Details window equals zero.
 Note
To finalize the bank statement, even if the difference does not equal zero, select the No Validation for Starting/Ending Balance
checkbox in the House Bank Accounts - Setup window.
Procedure
1. In the Bank Statement Details window, choose the Finalize button.
2. If you cannot finalize your bank statement, that is, if the Difference field does not equal zero, then review the posting
proposals for every transaction row. The objective is to clear all bank statement rows.
3. When you have finished reviewing the list of posting proposals, choose the Finalize button.
Results
All deselected rows are deleted, and the cleared bank statement rows are saved in the SAP Business One database and in the
Accounting module.
Finalized bank statements are saved in SAP Business One and can be accessed through the Bank Statement Summary window,
and viewed by running the Bank Statement Information report.
Example
Starting Balance EUR -93,041.01
Ending Balance EUR -93,141.01
Difference EUR - 100.00
This is custom documentation. For more information, please visit SAP Help Portal. 100

6/8/26, 6:08 AM
The document cannot be finalized.
Starting Balance EUR -93,041.01
Ending Balance EUR -93,041.01
Difference EUR 0.00
The document can be finalized.
Generating the Bank Statement Information Report
Context
You use the Bank Statement Information - Selection Criteria window to display detailed information for one or more bank
statements.
For finalized bank statements, the report shows incoming payments, outgoing payments, and journal entries that have already
been posted.
For draft bank statements, the report shows posting proposals for all rows based on the expanded rows – simulation report.
Procedure
1. From the SAP Business One Main Menu, choose Banking Banking Reports Bank Statement Information .
2. In the Bank Statement Information – Selection Criteria window, specify a range for each field to define the information to
be included in the report.
3. When you have finished, choose the OK button.
Results
The Bank Statement Information window appears, displaying detailed information for the bank statements that you have
selected.
Bank Statement Processing Windows
Use the following windows to work with bank statement processing:
Bank Statement Details Window
Bank Statement Row - Details Expanded Window
Bank Statement Summary
Add Open Documents Window
Add Open BP Journal Entries Window
Add Open Transactions Window
Multiple Payments Window
Bank Statement Information - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 101

6/8/26, 6:08 AM
Add Open BP Journal Entries Window
Use this window to specify matching criteria for reconciling manual journal entries posted to business partners. You can set a
combination of up to three rules. Each rule can consider one of the parameters described below.
 Note
Each parameter can be used for only one rule. Once you assign a parameter to a rule, it is removed from the dropdown lists of
the other rules.
 Note
SAP Business One adds BP journal entries with posting dates that are earlier than or the same as the posting date of the bank
statement row in the Bank Statement Details window. If the Posting Date field of the bank statement row is empty, SAP
Business One adds BP journal entries with posting dates that are earlier than or the same as the current system date.
To open this window:
1. From the SAP Business One Main Menu, choose Banking Setup Banking Bank Statements and External
Reconciliations Bank Statement Processing Bank Statement Summary Bank Statement Details .
2. Double-click a row number whose posting method is Business Partner from/to Bank Account.
3. Choose Add Open BP JEs.
Add Open BP Journal Entries Window Fields
Posting Date
Select this parameter to assign documents for reconciliation while considering the posting date assigned to them.
Displays the Variation in Days field, in which you specify the number of days to be considered as a legitimate difference within
which transactions are selected for reconciliation. When this field is left blank, SAP Business One treats the value as zero.
 Example
Variation in Days is defined as 3. The posting date of a specific invoice is 01.05.2007, and there is a payment for the exact
amount with a posting date of 06.05.2007. Because the difference is 5 days, the invoice is not selected for reconciliation.
Due Date
Select this parameter to assign documents for reconciliation while considering the due date assigned to them.
Displays the Variation in Days field, in which you specify the number of days to be considered as a valid difference within which
transactions are selected for reconciliation. When this field is left blank, SAP Business One treats the value as zero.
 Example
Variation in Days is defined as 3. The due date of a specific invoice is 01.05.2007, and there is a payment for the exact amount
with a due date of 03.05.2007. Because the difference is 2 days, the invoice is selected for reconciliation.
Balance Amount
Select this parameter to assign documents for reconciliation according to their total amounts.
This is custom documentation. For more information, please visit SAP Help Portal. 102

6/8/26, 6:08 AM
Displays the Matching Difference field, in which you specify the maximum variance in amounts (in local currency) that should be
tolerated by SAP Business One.
If the variance between amounts is greater than the value specified, these amounts are not selected for reconciliation. To increase
the degree of accuracy of the reconciliation, define a low value in this field.
 Example
You specified 0.5 in the Matching Difference field. SAP Business One scans the manual journal entries posted to a specific
business partner, looking for a transaction to be reconciled with a 100.08 debit amount. A credit transaction of 100.7 is found,
that is, a difference of 0.62. In addition, a credit transaction of 99.85, that is, a difference of 0.23, is also found. Although both
transactions are proposed for internal reconciliation, as neither transaction directly matches the bank statement row amount,
neither is automatically selected for internal reconciliation.
Ref. 1, Ref. 2, Ref. 3
Select one of the references, 1 to 3, to reconcile journal entries posted to business partners, while using the value defined in the
Ref. 1, Ref. 2, or Ref. 3 field in the Journal Entry window as a matching criterion.
Displays the Relate to XXX First Chars. field, in which you specify a number higher than 0 to define the level of accuracy of this
parameter. The lower the number, the lower the level of accuracy, and vice versa. SAP Business One checks the defined number of
characters starting from the left.
 Note
You can use only one reference as a rule in the matching criteria.
You selected Ref. 1 for Rule 1. In the Relate to XXX First Chars. field you specified the value 3. When you continue to Rule 2, the
options Ref. 2 and Ref. 3 do not appear in the dropdown list. SAP Business One scans the manual journal entries created for a
business partner, looking for a match to a transaction with a reference number of 96785. When it finds a journal entry with the
value of 9674785, it considers it a match since the first 3 characters are identical.
Add Open Documents Window
Use this window to specify matching criteria for selecting sales and purchasing documents for manual reconciliation with their
respective payments. You can set a combination of up to three rules. Each rule can consider one of the parameters described
below.
 Note
Each parameter can be used for only one rule. Once you assign a parameter to a rule, it is removed from the dropdown lists of
the other rules.
 Note
SAP Business One adds open documents with posting dates that are earlier than or the same as the posting date of the bank
statement row in the Bank Statement Details window. If the Posting Date field of the bank statement row is empty, SAP
Business One adds open documents with posting dates that are earlier than or the same as the current system date.
To open this window:
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Bank
Statement Processing Bank Statement Summary Bank Statement Details .
2. Double-click a row number whose posting method is Business Partner from/to Bank Account.
This is custom documentation. For more information, please visit SAP Help Portal. 103

6/8/26, 6:08 AM
3. Choose Add Open Documents.
Add Open Documents Window Fields
Doc Type
Select a document type from the dropdown list:
All
A/R Down Payments
A/R Invoices
A/R Credit Memos
Sales Orders
A/P Down Payments
A/P Invoices
A/P Credit Memos
Purchase Orders
 Note
The options Sales Orders and Purchase Orders are available only when you have selected values in the Create Down Payment
in Bank Statement Processing dropdown list on the Per Document tab of the Document Settings window.
Posting Date
Selects a document if its due date is within a specified number of days of the bank statement row.
Displays the Variation in Days field, in which you specify the number of days to be considered as a legitimate difference within
which transactions are selected for reconciliation. If Posting Date is blank, the Variation in Days field is set to zero.
 Example
Variation in Days is defined as 3. The posting date of a specific invoice is 01.05.2007. There is a payment for the exact amount
with a posting date of 06.05.2007. Because the difference is 5 days, the invoice is not selected for reconciliation.
Due Date
Selects a document if its due date is within a specified number of days of the bank statement row.
Displays the Variation in Days field, in which you specify the number of days to be considered as a legitimate difference within
which transactions are selected for reconciliation. If Due Date is blank, the Variation in Days field is set to zero.
 Example
Variation in Days is defined as 3. The due date of a specific invoice is 01.05.2007. There is a payment for the exact amount with
a due date of 03.05.2007. Because the difference is 2 days, the invoice is selected for reconciliation.
Balance Amount
Select this parameter to assign documents for reconciliation according to their total amounts.
Displays the Matching Difference field, in which you specify the maximum variance in amounts (local currency) that should be
tolerated by SAP Business One.
This is custom documentation. For more information, please visit SAP Help Portal. 104

6/8/26, 6:08 AM
If the variance between amounts is greater than the value specified, these amounts are not selected for reconciliation.
To increase the degree of accuracy of the reconciliation, define a low value. Amount matching is always against the amount
specified in the bank statement row and never against the amounts specified in the Multiple Payments window.
Document Number
Select this parameter to assign documents for reconciliation with payments with identical document numbers.
Customer/Vendor Name
Select this parameter to assign documents for reconciliation while comparing the value set in the Name field in sales or
purchasing documents with the value set in the bank statement row in the BP Name field.
Displays the Relate to XXX First Chars field, in which you specify a number to define the level of accuracy of this parameter. The
lower the number, the lower the level of accuracy, and vice versa. SAP Business One checks the defined number of characters
starting from the left.
 Note
If you leave this field blank, SAP Business One looks for a complete match of the customer or vendor name.
BP Bank Code + Account
SAP Business One uses the values defined in the Bank Code and Account No. fields in the Business Partner Bank Accounts –
Setup window.
To view the window, from the SAP Business One Main Menu, choose Business Partners Business Partner Master Data
Payment Terms tab, and click next to the Bank Country/Region field.
 Note
This match only works if both the Bank Code and Account No. fields in the Business Partner Bank Accounts – Setup are
populated.
IBAN
SAP Business One selects documents for reconciliation to bank statement rows according to:
Value set in the BP IBAN column under the Business Partner Details section in the Bank Statement Details window
Matching value set in the IBAN field on the Payment Terms tab of the Business Partner Master Data window. This applies
to documents posted to business partners.
Displays the Relate to XXX First Chars. field, in which you specify a number to define the level of accuracy of this parameter. The
lower the number, the lower the level of accuracy, and vice versa. SAP Business One checks the defined number of characters
starting from the left.
Discounted Balance Amount
Select this parameter to assign documents for reconciliation according to their discount amounts.
Displays the Matching Difference field, in which you specify the maximum variance in amounts (local currency) that should be
tolerated by SAP Business One.
If the variance between amounts is greater than the value specified, these amounts are not selected for reconciliation.
To increase the degree of accuracy of the reconciliation, define a low value.
BP Reference No.
This is custom documentation. For more information, please visit SAP Help Portal. 105

6/8/26, 6:08 AM
Lets you assign documents for reconciliation while comparing the value set in the Customer Ref. No. or Vendor Ref. No. field in
sales and purchasing documents with the value set in the Reference field in payment documents.
Displays the Relate to XXX First Chars. field, in which you specify a number to define the level of accuracy of this parameter. The
lower the number, the lower the level of accuracy, and vice versa. SAP Business One checks the defined number of characters
starting from the left.
If the field is left blank, SAP Business One looks for a complete match of business partner reference numbers.
 Example
The Customer Ref. No. in A/R Invoice No. 100 is CR123456. The value set in Relate to XXX First Chars. is 1. SAP Business One
looks for incoming payments with reference numbers that begin with the character C. There may be many incoming payments
that comply with this criterion. If the value set in Relate to XXX First Chars. is 3, SAP Business One searches for all incoming
payments with a reference number that begins with CR1. The quantity of incoming payments that begin with CR1 is much
smaller than the quantity of incoming payments that begin with C. This is why the higher the value set in this field, the greater
the accuracy of this criterion.
Add Open Transactions Window
Use this window to specify matching criteria for selecting open transactions for manual reconciliation with their respective
payments. You can set a combination of up to three rules. Each rule can consider one of the parameters described below.
 Note
Each parameter can be used for only one rule. Once you assign a parameter to a rule, it is removed from the dropdown lists of
the other rules.
 Note
SAP Business One adds open transactions with posting dates that are earlier than or the same as the posting date of the bank
statement row in the Bank Statement Details window. If the Posting Date field of the bank statement row is empty, SAP
Business One adds open transactions with posting dates that are earlier than or the same as the current system date.
To open this window:
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Bank
Statement Processing Bank Statement Summary Bank Statement Details .
2. Double-click a row number whose posting method is Bank Interim Account from/to Bank Account or External
Reconciliation.
3. Choose Add Open Transactions. Alternatively, choose Alt + A .
After you choose the OK button in the Add Open Transactions window, a message appears telling you how many open
transactions have been found.
Add Open Transactions Window Fields
Posting Date
Select this parameter to assign documents for reconciliation while considering the posting date assigned to them.
Displays the Variation in Days field, in which you specify the number of days to be considered as a legitimate difference within
which transactions are selected for reconciliation. When this field is left blank, SAP Business One treats the value as zero.
This is custom documentation. For more information, please visit SAP Help Portal. 106

6/8/26, 6:08 AM
 Example
Variation in Days is defined as 3. The posting date of a specific invoice is 01.05.2007, and there is a payment for the exact
amount with a posting date of 06.05.2007. Because the difference is 5 days, the invoice is not selected for reconciliation.
Due Date
Select this parameter to assign documents for reconciliation while considering the due date assigned to them.
Displays the Variation in Days field, in which you specify the number of days to be considered as a valid difference within which
transactions are selected for reconciliation. When this field is left blank, SAP Business One treats the value as zero.
 Example
Variation in Days is defined as 3. The due date of a specific invoice is 01.05.2007, and there is a payment for the exact amount
with a due date of 03.05.2007. Because the difference is 2 days, the invoice is selected for reconciliation.
Balance Amount
Select this parameter to assign documents for reconciliation according to their total amounts.
Displays the Matching Difference field, in which you specify the maximum variance in amounts (in local currency) that should be
tolerated by SAP Business One.
If the variance between amounts is greater than the value specified, these amounts are not selected for reconciliation. To increase
the degree of accuracy of the reconciliation, define a low value in this field.
 Example
You specified 0.5 in the Matching Difference field. SAP Business One scans the manual journal entries posted to a specific
business partner, looking for a transaction to be reconciled with a 100.08 debit amount. A credit transaction of 100.7 is found,
that is, a difference of 0.62. In addition, a credit transaction of 99.85, that is, a difference of 0.23, is also found. Although both
transactions are proposed for internal reconciliation, as neither transaction directly matches the bank statement row amount,
neither is automatically selected for internal reconciliation.
Ref. 1, Ref. 2, Ref. 3
Select one of the references, 1 to 3, to reconcile journal entries posted to business partners, while using the value defined in the
Ref. 1, Ref. 2, or Ref. 3 field in the Journal Entry window as a matching criterion.
Displays the Relate to XXX First Chars. field, in which you specify a number higher than 0 to define the level of accuracy of this
parameter. The lower the number, the lower the level of accuracy, and vice versa. SAP Business One checks the defined number of
characters starting from the left.
 Note
You can use only one reference as a rule in the matching criteria.
You selected Ref. 1 for Rule 1. In the Relate to XXX First Chars. field you specified the value 3. When you continue to Rule 2, the
options Ref. 2 and Ref. 3 do not appear in the dropdown list. SAP Business One scans the manual journal entries created for a
business partner, looking for a match to a transaction with a reference number of 96785. When it finds a journal entry with the
value of 9674785, it considers it a match since the first 3 characters are identical.
Bank Statement Details Window
Use this window to record your bank statement. You automatically import or manually enter the transactions listed by your bank so
that you can perform internal and external reconciliation.
This is custom documentation. For more information, please visit SAP Help Portal. 107

6/8/26, 6:08 AM
You can vary the fields and columns displayed in the Bank Statement Details window according to your company’s needs and
local business rules.
The fields that appear in the Bank Statement Details window are described below.
To open the window, from the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations
Bank Statement Processing . In the Bank Statement Summary window, specify in the required fields the information
appearing in the bank statement header, and then choose either the Create New button for manual processing or the Import from
File button for automatic processing.
 Note
When you right-click a bank statement row and choose Posting Proposal for Row, the row appears as the first row in the
window.
 Note
When you choose the Posting Proposal for Uncleared Rows button or the Posting Proposal for Row option after right-clicking
a bank statement row, SAP Business One proposes transactions with posting dates that are earlier than or the same as the
posting date of the bank statement row. If the Posting Date field of the bank statement row is empty, SAP Business One
proposes transactions with posting dates that are earlier than or the same as the current system date.
General Area
Bank Statement No.
The bank statement number optionally entered from the bank statement received.
 Note
After the bank statement is finalized, you can still change the bank statement number.
Bank Name
The value appearing in the Bank field in the Bank Statement Summary window is automatically copied to this field.
Bank Account
The bank account to which the bank statement is linked. The value appearing in the Account field in the Bank Statement
Summary window is automatically copied to this field. To open the House Bank Accounts – Setup window and to view the linked
bank account, choose .
Series
This field appears only if the Permit More than One Document Type per Series checkbox is selected in Administration System
Initialization Company Details Basic Initialization tab.
This value is copied from the Series column in the Bank Statement Summary window and specifies the numbering series to be
used for journal entries, as well as incoming and outgoing payments created through bank statement processing.
IBAN, BIC/SWIFT Code
Display the IBAN and BIC/SWIFT code of the selected house bank account.
G/L Account
G/L account to which the selected bank account is linked. SAP Business One populates this field according to the information
defined in the G/L Account field in Administration Setup Banking House Bank Accounts .
This is custom documentation. For more information, please visit SAP Help Portal. 108

6/8/26, 6:08 AM
No.
Displays the automatically-populated sequential row number in the Bank Statement Summary window.
Statement Date
Specify the date on which the received bank statement was generated by the bank and displayed on the bank statement. The
default is the current date.
 Note
After the bank statement is finalized, you can still change the statement date. This change does not affect the statement row
date, statement due date, posting date, due date, and document date in the Bank Statement Details window. This change does
not affect the period name or the sequential number in the Bank Statement Summary window.
Starting Balance
Specify the balance of the bank account before any of the transactions on the bank statement have been taken into consideration.
Enter the value as displayed on the bank statement received. The value must match the corresponding field in the Bank Statement
Summary window.
The default is the ending balance from the previous statement (draft or finalized).
 Note
When you have selected the No Validation for Starting/Ending Balance checkbox in the House Bank Accounts - Setup
window, the starting balance of your current bank statement can be different to the ending balance of the previous one.
Ending Balance
Specify the balance of the bank account after all the transactions on the bank statement have been taken into consideration. Enter
the value as displayed on the received bank statement. The value must match the corresponding field in the Bank Statement
Summary window.
Difference
Displays the difference between the cleared balance and the ending balance on the bank statement for the selected transactions.
G/L Account Currency
Shows the currency information taken from the G/L account’s definition in the Chart of Accounts window. The ## symbol
indicates that the G/L account is multicurrency.
Interim Account
Displays the offsetting G/L interim account to use for transaction posting defined in the House Bank Account – Setup window.
This field is shown only when the posting method is Bank Interim Account from/to Bank Account.
Row Details
Cleared/Selected
Select this checkbox to clear a bank transaction row or to select a posting proposal line. You can define a transaction row as
cleared only if the applied amount as matched in local currency or foreign currency is zero in the case of G/L account postings.
In the case of a business partner posting, the difference is posted to the business partner without the payment being based on an
existing marketing document.
Operation Code
This is custom documentation. For more information, please visit SAP Help Portal. 109

6/8/26, 6:08 AM
External Code
Specify the code for the transaction type according to the set of external codes in the External Bank Operation Codes window
that are associated with this bank account. This value may have been assigned during setup to an internal bank operation code
and may be displayed on the received bank statement.
Internal Code
Specify the code for the transaction type according to the Internal Code field in the Internal Bank Operation Codes window. This
value may have been assigned during setup to an external bank operation code, in which case it will be automatically populated if
the external code was selected.
 Note
When the bank file is imported automatically, the bank statement details usually contain only the external bank operation code.
If the bank operation code list has not been defined, choose an internal code manually for every bank statement row.
Posting Method
Specify the posting method to be used to create transactions for the bank statement rows associated with the internal operation
code on finalizing the bank statement, according to the Posting Method field in the Internal Bank Operation Codes window. The
available options are:
G/L Account from/to Bank Account – indicates the following:
A journal entry between the bank account and specific G/L accounts is created.
External reconciliation takes place between the bank statement row and the bank G/L account posting.
Business Partner from/to Bank Account – indicates the following:
An incoming or outgoing payment from or to the business partner is created.
Internal reconciliation takes place on the business partner side (if matching rules have been activated and matched
records have been selected for reconciliation).
External reconciliation takes place between the bank statement row and the bank G/L account posting.
Bank Interim Account from/to Bank Account - creates a journal entry that may be internally reconciled on the interim
bank account side (subject to matching criteria settings), and externally reconciled on the bank account side.
External Reconciliation – indicates that only external reconciliation is to be performed on the bank account side, but that
no transaction is posted.
Ignore – does not process any of the automatic actions described above – if associated with a bank statement row, that
row is recorded as being part of the bank statement. It effectively acts as a text line.
Dates from the Bank Statement
Row Date
The posting date of each transaction assigned to the respective row in the bank statement.
For a new bank statement row, the default statement row date is the value in the Statement Date field in the general area.
Due Date
The posting date of all the transactions created for the bank statement is the posting date assigned to that bank statement.
For a new bank statement row, the default statement due date is the value in the Statement Date field in the general area.
This is custom documentation. For more information, please visit SAP Help Portal. 110

6/8/26, 6:08 AM
Currency Details
Payment Currency
Specify the currency if a statement transaction is recorded as being in a different currency from the default currency. By default
the currency is the bank G/L account currency or the local currency if the bank G/L account is an all currency account.
Exchange Rate
Specify the exchange rate to apply for foreign currency conversion to local currency, as per the bank statement.
G/L Account/ Doc. Identification No.
The matching field for bank statement rows. If the row is a bank statement row, enter a document number or reference, as it
appears in the statement. If the row is a posting proposal row, SAP Business One populates this field with the document numbers
of proposed documents or the code and name of proposed G/L account postings.
When you have imported a bank statement with multiple reference numbers, that is, multiple numbers with commas in between in
the <Ustrd> field of the bank file, those numbers will be separated according to the commas as multiple rows in the Multiple
Payments window. To open the Multiple Payments window, choose the Choose from List button in the G/L Account/Doc.
Identification No. field.
Payment Currency Amounts
Incoming Amt
Specify the financial value for a particular transaction row in the case of an incoming payment.
Outgoing Amt
Specify the financial value for a particular transaction row in the case of an outgoing payment.
Discount Amount
Specify the financial value of the reduction on a particular transaction (row).
VAT Amount
Specify the amount of VAT included in the particular transaction (row).
Applied Amount
Enter the actual amount that was applied for the particular proposal (row) after the discount amount and VAT amount were taken
into consideration.
 Note
For one or more proposals within one uncleared bank statement row, you can choose Ctrl + B to display the following:
When the balance due of the bank statement row is larger than the balance due of the proposed transaction minus the
discount amount, this field displays the balance due of the proposed transaction minus the discount amount.
When the balance due of the bank statement row is smaller than the balance due of the proposed transaction minus the
discount amount, this field displays the balance due of the bank statement row.
This works also in All currency situations.
Default Discount %
Default percentage of discount value specified for the business partner.
This is custom documentation. For more information, please visit SAP Help Portal. 111

6/8/26, 6:08 AM
Additional Details
Reference
8-character additional information from the bank statement. The value is stored in the Ref. 3 field in the journal entry.
Details and Details 2
Additional information from the bank statement (254-character limit).
Business Partner Details
BP Name
Specify the business partner name corresponding to the specified business partner code.
BP Code
Specify the code of the business partner whose transactions you want to reconcile.
Control Account
For bank statement rows whose posting method is Business Partner from/to Bank Account, and for which you haven’t selected
any document, that is, the case of payment on account, define the control account. It will be taken to the payments created upon
finalizing the bank statement.
BP Bank Code, BP Bank Account, BP IBAN
Bank details of the business partner whose transactions you want to reconcile.
For a bank statement row with the posting method of Business Partner from/to Bank Account, after it is finalized with the
business partner bank code and bank account, if this bank code and bank account combination has not been assigned to this
business partner before, the combination will appear in the Business Partner Bank Account - Setup window for this business
partner.
To open this window, from the SAP Business One Main Menu, choose Business Partners Business Partner Master Data
Payment Terms tab, and choose the button next to the Bank Country/Region field. The next time this bank code and bank
account combination is entered or imported, if this combination is unique to the business partner, this business partner code will
be automatically identified in the BP Code field.
BP BIC/SWIFT Code
The BIC/SWIFT code of the business partner bank account, as defined in the Business Partner Bank Accounts – Setup window.
Interim Account
Enter the offsetting G/L interim account to use for transaction posting for the specified business partner.
Fee
Amount
Specify the fee charged by the bank for the particular transaction (row).
 Note
This is relevant only for a single bank statement row containing both a transaction amount and a bank fee. If bank fees are
presented as separate bank statement rows then this field should not be filled.
Account
Specify the account to which any fee amount charged for a transaction is posted.
This is custom documentation. For more information, please visit SAP Help Portal. 112

6/8/26, 6:08 AM
 Note
This is relevant only for a single bank statement row containing both a transaction amount and a bank fee. If bank fees are
presented as separate bank statement rows, then this field should not be filled.
Distr. Rule
Specify a distribution rule.
Project
Specify a project.
Dates for Posting Creation
Posting Date
The posting date to be assigned to the transaction. By default, this column is populated according to the definition for the
particular bank in Banks – Setup window.
Due Date
The due date to be assigned to the transaction. By default, this column is populated according to the definition for the particular
bank in Banks – Setup window.
Document Date
Enter the date on which the bank statement was generated. By default, this column is populated according to the definition for the
particular bank in the Banks - Setup window. If you enter the date manually, it is retained.
Journal Entry
The journal entry number after posting.
External Recon.
The number of the external reconciliation.
Log
SAP Business One displays information relating to automatic matching and processing errors.
Source
Displays the status of each bank statement row:
Imported - the bank statement row was imported from a bank file with no adjustments, except for possible value changes
in the Cleared/Selected or the BP Code field.
Imported and Amended - the bank statement row was imported from a bank file and values were manually adjusted in
fields other than the Cleared/Selected and the BP Code fields.
Manually Entered - the bank statement row was not imported but manually entered.
 Note
The field is not visible by default. You can set it to visible through the Form Settings window.
Bank Statement Information - Selection Criteria
This is custom documentation. For more information, please visit SAP Help Portal. 113

6/8/26, 6:08 AM
Use this window to display detailed information for one or more bank statements. To open this window, choose Banking
Banking Reports Bank Statement Information .
Key to Fields
G/L Account
Specify the range of account codes to be included in this report.
Bank Statement Date
Specify the range of dates generated by the bank of bank statements to be included in this report.
Bank Statement Number
Specify the range of bank statement numbers generated by the bank to be included in this report.
Internal Bank Operation Code
Specify the range of internal bank operation codes to be included in this report.
Business Partner Code
Specify the range of business partner codes to be included in this report.
Journal Entry
Specify the range of journal entry numbers to be included in this report.
Incoming Payment Number
Specify the range of incoming payment numbers to be included in this report.
Outgoing Payment Number
Specify the range of outgoing payment numbers to be included in this report.
More Information
Bank Statement Information Window
Bank Statement Information Window
This window displays the Bank Statement Information report according to your defined selection criteria.
To generate the report, from the SAP Business One Main Menu, choose Banking Banking Reports Bank Statement
Information , specify the required selection criteria, and choose the OK button.
 Note
This topic includes explanations of some of the fields in this window.
Key to Fields
G/L Account
Displays the code of the general ledger account to which the selected bank account is linked. SAP Business One populates this
field according to the information defined in the G/L Account field in Administration Setup Banking House Bank Accounts
This is custom documentation. For more information, please visit SAP Help Portal. 114

6/8/26, 6:08 AM
.
BS Date
Displays the date on which the received bank statement was generated by the bank and displayed on the bank statement.
No.
Row number in the Bank Statement Summary window.
BS No.
Displays the bank statement number optionally entered in the Bank Statement Details window from the bank statement received.
BP Code
Displays the code of the business partner related to the statement row as entered in the Bank Statement Details window.
Statement Row
Displays the number of the row in the bank statement received as entered in the Bank Statement Details window.
Credit, Debit
Displays the credit or debit amount of the bank statement row as entered in the Bank Statement Details window.
Payment
Displays the incoming or outgoing payment number.
Journal Entry
Displays the journal entry number after posting.
Bank Statement Row - Details Expanded Window
Use this window to perform manual reconciliation on a selected bank statement row. The fields displayed vary according to the
following types of posting methods:
Business Partner from/to Bank Account
G/L Account from/to Bank Account
Bank Interim Account from/to Bank Account or External Reconciliation
To open this window, from the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations
Bank Statement Processing Bank Statement Summary Bank Statement Details . In the table in the Bank Statement
Details window, double-click a row number. SAP Business One automatically proposes transactions in this window.
For bank statement row whose posting method is Business Partner from/to Bank Account, to add open marketing documents to
this window, choose the Add Open Documents button. For more information, see Add Open Documents Window.
For bank statement row whose posting method is Business Partner from/to Bank Account, to add open journal entries that are
business partner related to this window, choose the Add Open BP JEs button. For more information, see Add Open BP Journal
Entries Window.
For bank statement row whose posting method is Business Partner from/to Bank Account, to create journal entries for manual
reconciliation, choose the Create New JEs button. After you enter and post the new journal entry, the new data is copied to this
window. For more information, see Journal Entry Window.
This is custom documentation. For more information, please visit SAP Help Portal. 115

6/8/26, 6:08 AM
 Note
If you create a journal entry with a posting date later than the posting date of the bank statement row in the Bank Statement
Details window, this journal entry will not appear in the Bank Statement Row Details - Expanded window. To display the journal
entry, make sure that its posting date is earlier than or the same as the posting date of the bank statement row. If the Posting
Date field of the bank statement row is empty, make sure that the posting date of the journal entry is earlier than or the same
as the current system date.
For a bank statement row with a posting method of Bank Interim Account from/to Bank Account or External Reconciliation, to
add open transactions, choose the Add Open Transactions button. For more information, see Add Open Transactions Window.
General Area
Bank Row Amt
Amount for the specific bank statement transaction row.
Applied Amt
Amount of the specific document or transaction proposed for posting.
Balance
Calculated difference between the Bank Row Amt and Applied Amt fields for the payment currency and for the local currency.
This field is updated every time the value in the Applied Amt field is changed.
Details
Displays the same details as the Details field in the Bank Statement Details window.
Details2
Displays the same details as the Details2 field in the Bank Statement Details window.
Ref.
Displays the same details as the Reference field in the Bank Statement Details window.
Operation Code
Displays the same details as the Internal Code field in the Bank Statement Details window.
Rate
Displays the same details as the Exchange Rate field in the Bank Statement Details window.
Row Date
Displays the same details as the Row Date field in the Bank Statement Details window.
BP Code
Displays the same details as the BP Code field in the Bank Statement Details window.
BP Name
Displays the same details as the BP Name field in the Bank Statement Details window.
Row Details
Selected
This is custom documentation. For more information, please visit SAP Help Portal. 116

6/8/26, 6:08 AM
Indicates whether the specific document or transaction is proposed for posting.
BP Code
Code of the business partner for the specific document or transaction.
BP Name
Name of the business partner corresponding to specified business partner code. Value of the Name field in the original document
header.
Distr. Rule
For bank statement rows whose posting method is Business Partner from/to Bank Account or G/L Account from/to Bank
Account, define the distribution rules. They will be taken to the payments created upon finalizing the bank statement.
 Note
For sales or purchase orders, you cannot edit their distribution rules.
Default Cash Discount %
The percentage of discount in the Discount % field in the original document or transaction.
Original Amt - Payment Currency
Value of the Total Before Discount field in the original document or transaction in the payment currency.
Balance Due - Payment Currency
Value of the Balance Due field in the original document or transaction in the payment currency.
Discount Amt - Payment Currency
The amount shown in the field on the right in the Discount % field in the original document/transaction in the payment currency.
Applied Amt - Payment Currency
Value in the Total field in the original document/transaction in the payment currency.
 Note
For sales or purchase orders, you cannot edit this field.
 Note
For one or more proposals within one uncleared bank statement row, you can choose Ctrl + B to display the following:
When the balance due of the bank statement row is larger than the balance due of the proposed transaction minus the
discount amount, this field displays the balance due of the proposed transaction minus the discount amount.
When the balance due of the bank statement row is smaller than the balance due of the proposed transaction minus the
discount amount, this field displays the balance due of the bank statement row.
This works also in All currency situations.
Original Amt - Local Currency
Value of the Total Before Discount field in the original document/transaction in the local currency.
Balance Due – Local Currency
Value of the Balance Due field in the original document/transaction in the local currency.
This is custom documentation. For more information, please visit SAP Help Portal. 117

6/8/26, 6:08 AM
Discount Amt – Local Currency
The amount shown in the field on the right in the Discount % field in the original document/transaction in the local currency.
Applied Amt – Local Currency
Value of the Total field in the original document/transaction in the local currency.
Ref. 1
Value in the Ref 1 field of the journal entry associated with the proposed transaction.
Ref. 2
Value in the Ref 2 field of the journal entry associated with the proposed transaction.
Ref. 3
Value in the Ref 3 field of the journal entry associated with the proposed transaction.
BP Reference No.
Value in the BP Reference No. field in the original document as follows:
A/R Documents (except payments): Customer Reference No. field
A/P Documents (except payments): Vendor Reference No. field
A/R and A/P Incoming/Outgoing Payments: Reference field (from payment header
Posting Date
Value in the Posting Date field of the journal entry associated with the proposed transaction.
Due Date
Value in the Due Date field of the journal entry associated with the proposed transaction.
Document Date
Value in the Document Date field of the journal entry associated with the proposed transaction.
Bank Statement Summary
Use this window to access a list of all bank statements for the bank account specified in the general area.
By default, the bank statements are sorted first by the period name, and then by the sequential number in the No. column within
the same posting period.
To open this window, choose Banking Bank Statement and External Reconciliations Bank Statement Processing .
General Area
Country/Region
Choose the name of the country/region in which the required bank is located.
Bank
Choose the name of the required bank. The application automatically populates the Account and G/L Account fields according to
the information defined in Administration Setup Banking House Bank Accounts .
This is custom documentation. For more information, please visit SAP Help Portal. 118

6/8/26, 6:08 AM
Account
Bank account number to which the bank statement should be linked. The application automatically populates this field according
to the information defined in the Account No. field in Administration Setup Banking House Bank Accounts .
IBAN, BIC/SWIFT Code
Display the IBAN and BIC/SWIFT code of the selected house bank account.
G/L Account
G/L account to which the selected bank account is linked. The application automatically populates this field according to the
information defined in the G/L Account field in Administration Setup Banking House Bank Accounts .
G/L Account Balance
Current balance of the G/L account. The application automatically populates this field. The current balance is shown for
information only and is not saved in the header of the bank statement.
G/L Account Currency
Shows the currency information taken from the G/L account’s definition in the chart of accounts. The ## symbol indicates that the
G/L account is multicurrency.
Series
Specify the numbering series to be used for journal entries, as well as incoming and outgoing payments that are created through
bank statement processing.
This column appears only if the Permit More than One Document Type per Series checkbox is selected in Administration
System Initialization Company Details Basic Initialization tab.
Import from File
Choose the Import from File button to automatically import bank statements into SAP Business One without entering bank
statements manually. This button is activated only when you have assigned a bank statement format (BFP) to the house bank
account specified in the header area.
For more information, see Importing Bank Statements Automatically.
Create New
The Create New button opens the Bank Statement Details window and lets you create bank statements manually.
For more information, see Adding Bank Statements Manually.
Row Details
No.
The system-generated row number in the Bank Statement Summary window.
Period Name
Displays the name of the posting period that covers the statement date in the Bank Statement Details window when the bank
statement was entered as a draft or first finalized.
To see the details of posting periods, from the SAP Business One Main Menu, choose Administration System Initialization
Posting Periods .
Bank Statement No.
This is custom documentation. For more information, please visit SAP Help Portal. 119

6/8/26, 6:08 AM
Shows the bank statement number optionally entered from the bank statement. This is header information for the specified bank
statement.
Status
Shows the progress of bank statement processing. This is header information for the specified bank statement. The following
statuses are possible:
Draft – in progress
Finalized – the bank statement has been accepted
Old – statement created before bank statement processing was introduced to SAP Business One
Statement Date
Date on which the bank statement received from the bank was generated; appears in header of specified bank statement.
Starting Balance
Specify the balance of the bank account before any of the transactions on the bank statement have been taken into account. Enter
the value as displayed on the bank statement received.
Ending Balance
Ending balance of bank account after all transactions on the bank statement have been taken into account. This is the financial
value taken from the received bank statement.
Multiple Payments Window
Use this window to process multiple payments with automatic matching.
To open this window:
In the Bank Statement Details window, place your cursor in the G/L Account/Doc. Identification No. field. Either press the TAB
key, or right-click and choose Multiple Payments.
Key to Fields
Statement Row Amt
Amount appearing in the bank statement transaction row.
Multiple Payment Total
Total of the payment amounts in the proposed documents.
Document Identification
Identification number of the proposed document.
 Note
This field is used for matching.
Incoming Amt
Incoming amount appearing in the proposed document.
This is custom documentation. For more information, please visit SAP Help Portal. 120

6/8/26, 6:08 AM
 Note
This field is not used for matching.
Outgoing Amt
Outgoing amount appearing in the proposed document.
 Note
This field is not used for matching.
Bank Statement Processing Business Scenarios
This help topic contains links to common scenarios for bank statement transaction row entry and handling.
Incoming Payment from Customer
Incoming Payment from Customer With Cash Discount
Outgoing Payment Through Bank Transfer Using the Payment Wizard
Outgoing Payment and Exchange Rate Difference
Payment to Account: Salaries
Payment to Account: Sundry Expenses with Tax - Gas Expenses
Cash Deposit to a Bank Interim Account - Retail Business
External Reconciliation
More Information
Bank Statement Details Window
Incoming Payment from Customer
You create an A/R invoice for a customer in SAP Business One. You receive the bank statement which shows an incoming payment
from the customer made by direct bank transfer. You enter this payment manually into the Bank Statement Details window
together with the appropriate internal bank operation code, BP to/from bank acct. SAP Business One matches details
entered with the BP reference number specified in the G/L Account/Doc. Identification No. column and the transaction is
selected, cleared, and reconciled.
 Note
Only relevant fields are shown.
Bank Statement Details
Operation Code Currency Details G/L Payment Local Currency Business Dates for
- Internal Code - Payment Account/Doc. Currency Amounts - Partner Details - Posting Creation
Currency Identification Amounts - Incoming Amt BP Bank Code - Posting Date
No. Incoming Amt
This is custom documentation. For more information, please visit SAP Help Portal. 121

6/8/26, 6:08 AM
Operation Code Currency Details G/L Payment Local Currency Business Dates for
- Internal Code - Payment Account/Doc. Currency Amounts - Partner Details - Posting Creation
Currency Identification Amounts - Incoming Amt BP Bank Code - Posting Date
|                 |     | No.       |     | Incoming Amt |     |     |      |         |
| --------------- | --- | --------- | --- | ------------ | --- | --- | ---- | ------- |
| BP to/from bank | USD | 123456789 |     | 100          | 100 |     | 1234 | 4/15/09 |
acct
G/L Account Postings
| Business Partner |     | Bank         |     |     |     |     |     |     |
| ---------------- | --- | ------------ | --- | --- | --- | --- | --- | --- |
| Debit Credit     |     | Debit Credit |     |     |     |     |     |     |
| (1)100 (2)100    |     | (2)100       |     |     |     |     |     |     |
(1) Invoice 123456789
(2) Payment
Incoming Payment from Customer With Cash Discount
You issue an A/R invoice containing the payment amount due. The customer is eligible for a 10% discount, provided that payment
is made before the invoice due date. You receive the bank statement which contains a transaction row showing that a payment was
made within the discount period. SAP Business One matches the BP reference code entered for the incoming payment in the G/L
Account/Doc. Identification No. column in the Bank Statement Details window.
  Note
Only relevant fields are shown.
Bank Statement Details
Operation Currency Currency G/L Payment Local Discount Dates for
Code - Details - Details – Account/Doc. Currency Currency Amount Posting
Internal Code Payment Exchange Identification Amounts - Amounts - Creation -
|            | Currency | Rate | No.      |     | Incoming Amt | Incoming Amt |     | Posting Date |
| ---------- | -------- | ---- | -------- | --- | ------------ | ------------ | --- | ------------ |
| BP to/from | USD      | 1    | ABCD1234 |     | 100          | 100          | 10  | 4/15/09      |
bank acct
G/L Account Postings
| Business Partner |     | Bank  |        |     | Customer Discount |        |     |     |
| ---------------- | --- | ----- | ------ | --- | ----------------- | ------ | --- | --- |
| Debit Credit     |     | Debit | Credit |     | Debit             | Credit |     |     |
| (1)100 (2)100    |     | (2)90 |        |     | 10                |        |     |     |
(1) Invoice
(2) Payment
This is custom documentation. For more information, please visit SAP Help Portal. 122

6/8/26, 6:08 AM
Outgoing Payment Through Bank Transfer Using the Payment
Wizard
You use the payment wizard to create a bank file containing an instruction to make an outgoing payment to a vendor. When SAP
Business One generates the bank file, the bank posting is posted to a bank interim account prior to clearance on the bank
statement. You receive the bank statement which shows that the outgoing payment has been cleared. You enter the relevant
transaction row in the Bank Statement Details window and SAP Business One matches it to the outgoing payment amount. When
the bank statement is finalized, the interim bank posting is then cleared and transferred to the bank G/L account.
 Note
Only relevant fields are shown.
Bank Statement Details
Operation Code Dates from the Dates from the Currency Details Currency Payment Local Currency
- Internal Code Bank Statement Bank Statement - Payment Details - Currency Amounts -
- Row Date - Due Date Currency Exchange Rate Amounts - Outgoing Amt
Outgoing Amt
BP to/from bank 4/13/2009 4/13/2009 EUR 1 100 100
acct
G/L Account Postings
Business Partner Interim Bank Acct Bank
Debit Credit Debit Credit Debit Credit
(1)100 (1)100 (2)100 (1)100
(1) Payment
(2) Clearance
Outgoing Payment and Exchange Rate Difference
The company receives an invoice in US dollars from a multicurrency vendor and posts it in SAP Business One at an exchange rate
of 1.5 US dollars to 1 euro, the company’s local currency. The vendor pays the invoice in euros, at an exchange rate of 1 euro to 2 US
dollars. The bank statement is received and shows that the outgoing payment has been cleared. You enter the relevant transaction
row in the Bank Statement Details window and match it to the payment amount. When the bank statement is finalized, the posting
is transferred to the bank G/L account and the exchange rate difference posted to a separate G/L account.
 Note
Only relevant fields are shown.
Bank Statement Details
Operation Code - Currency Details - Currency Details - Payment Currency Local Currency Amounts
Internal Code Payment Currency Exchange Rate Amounts - Outgoing - Outgoing Amt
Amt
Bank Transfer EUR 2 USD 300 EUR 150
This is custom documentation. For more information, please visit SAP Help Portal. 123

6/8/26, 6:08 AM
G/L Account Postings
| Business Partner |     | Bank         |   Exchange Rate Gain |        |     |
| ---------------- | --- | ------------ | -------------------- | ------ | --- |
| Debit Credit     |     | Debit Credit |   Debit              | Credit |     |
| (2) (1)          |     |   (1)        |                      | (1)    |     |
| USD 300 USD 300  |     | USD 300      |                      | EUR 50 |     |
| EUR 200 EUR 200  |     | EUR 200      |                      | USD 0  |     |
(1) Invoice
(2) Payment
Payment to Account: Salaries
The company pays monthly salaries to its employees via a payroll system that gives the bank payment instructions. In this
simplified scenario, no employee benefits, such as health and life insurance, savings plans, and Social Security are involved, and no
tax is applied. Upon receipt of the bank statement the employee payments are recorded as cleared and need to be posted as G/L
transactions.
The Outgoing Payments window is used to issue an outgoing payment to the relevant salary and wages G/L account.
You enter the relevant transaction row in the Bank Statement Details window, with the internal bank operation code indicating
that the posting method is G/L Account From/To Bank Account. The transaction is matched against the relevant amount
and the relevant salary and wages G/L account. When the bank statement is finalized, the posting amount is transferred from the
bank G/L account to the salary and wages G/L account.
  Note
1. This scenario resembles bank fee handling.
2. Only relevant fields are shown.
Bank Statement Details
Operation Code Currency Details Payment Payment Local Currency Dates for Dates for
- Internal Code - Payment Currency Currency Amounts - Posting Creation Posting Creation
Currency Amounts - Amounts - Incoming Amt - Posting Date - Document
|     |     | Outgoing Amt | Applied Amt |     | Date |
| --- | --- | ------------ | ----------- | --- | ---- |
GLToFr USD 100,000.00 (100,000.00) 100,000.00 4/13/2009 4/13/2009
G/L Account Postings
| Bank         |   Salaries & Wages |        |     |     |     |
| ------------ | ------------------ | ------ | --- | --- | --- |
| Debit Credit |   Debit            | Credit |     |     |     |
|   100000     |   100000           |        |     |     |     |
Payment to Account: Sundry Expenses with Tax - Gas Expenses
This is custom documentation. For more information, please visit SAP Help Portal. 124

6/8/26, 6:08 AM
A company employee fills up her car with gasoline and gives the sales receipt to her company for reimbursement. The company
wants to log the purchase transaction and the associated VAT without opening a business partner master data record for the gas
station involved. The Outgoing Payments window is used to issue an outgoing payment to the relevant sundry expenses G/L
account. When the bank statement is received, it shows that the outgoing payment has been cleared.
The relevant transaction row is entered in the Bank Statement Details window, with the internal bank operation code indicating
that the posting method is G/L account from/to bank account. The transaction is matched against the relevant purchase
transaction and VAT amounts. When the bank statement is finalized, the posting amount is transferred from the bank G/L account
and divided between the expense G/L account and the sales tax G/L account.
 Note
Only relevant fields are shown.
Bank Statement Details
Operation Dates from Dates from Payment VAT Amt Payment Local Dates for Dates for
Code - the Bank the Bank Currency Currency Currency Posting Posting
Internal Statement - Statement - Amounts - Amounts - Amounts - Creation - Creation -
Code Row Date Due Date Outgoing Applied Amt Outgoing Posting Document
Amt Amt Date Date
GLToFr 4/13/2009 4/13/2009 100.00 10 (100.00) 100.00 4/13/2009 4/13/2009
G/L Account Postings
Bank Sundry Expenses - Gasoline VAT
Debit Credit Debit Credit Debit Credit
100 90 100
Cash Deposit to a Bank Interim Account - Retail Business
A retail company has a cash register and deposits a single day’s takings in the bank. In SAP Business One, a cash deposit was
made transferring the cash asset recorded from the sales posting to an interim account. A bank statement is received and a
transaction row shows that the cash amount was cleared.
The relevant transaction row is entered in the Bank Statement Details window, with the internal bank operation code indicating
that the posting method is Bank Interim Account from/to Bank Account. The transaction is matched against the cash
deposit transaction to the interim account. When the bank statement is finalized, the posting amount is transferred from the G/L
bank interim account to the G/L bank account.
 Note
Only relevant fields are shown.
Bank Statement Details
Operation G/L Payment Payment Local Interim Dates for Dates for Journal
Code - Account/Doc. Currency Currency Currency Account Posting Posting Entry
Internal Identification Amounts - Amounts - Amounts - Creation - Creation -
Code No. Incoming Applied Incoming Posting Document
Amt Amt Amt Date Date
This is custom documentation. For more information, please visit SAP Help Portal. 125

6/8/26, 6:08 AM
Operation G/L Payment Payment Local Interim Dates for Dates for Journal
Code - Account/Doc. Currency Currency Currency Account Posting Posting Entry
Internal Identification Amounts - Amounts - Amounts - Creation - Creation -
| Code       | No.           | Incoming | Applied | Incoming |        | Posting   | Document  |     |
| ---------- | ------------- | -------- | ------- | -------- | ------ | --------- | --------- | --- |
|            |               | Amt      | Amt     | Amt      |        | Date      | Date      |     |
| interimdep |               | 1000     | 1000    | 1000     | 161011 | 4/13/2009 | 4/13/2009 | 382 |
|            | JE 381/1 - DP | 1000     | 1000    | 1000     | 161011 |           |           | 381 |
3
G/L Account Postings
| Bank Interim |           | Bank    |        |     |     |     |     |     |
| ------------ | --------- | ------- | ------ | --- | --- | --- | --- | --- |
| Debit        | Credit    | Debit   | Credit |     |     |     |     |     |
| (1)1000      | (2)1000   | (2)1000 |        |     |     |     |     |     |
(1) Deposit
(2) Clearance
External Reconciliation
The company wants to verify the transactions recorded in SAP Business One against the bank statement and to create
adjustments, if required. In the following example, the bank statement shows an outgoing payment.
The relevant transaction row is entered in the Bank Statement Details window, with the internal bank operation code indicating
that the posting method is External Reconciliation. The transaction is matched to the outgoing payment amount and the relevant
journal entry displayed in the Bank Statement Details window. When the bank statement is finalized, no posting is made but an
external reconciliation is made connecting the bank statement row with the outgoing payment.
  Note
Only relevant fields are shown.
Bank Statement Details
Operation G/L Payment Payment Local Business Business Interim Dates for
Code - Account/Doc. Currency Currency Currency Partner Partner Account Posting
Internal Identification Amounts - Amounts - Amounts - Details - BP Details - BP Creation -
| Code     | No. | Outgoing   | Applied | Outgoing   | Name | Code |        | Posting    |
| -------- | --- | ---------- | ------- | ---------- | ---- | ---- | ------ | ---------- |
|          |     | Amt        | Amt     | Amt        |      |      |        | Date       |
| External |     | USD 100.00 | (USD    | USD 100.00 |      |      | 161010 | 12/12/2009 |
100.00)
  JE 384/0 - PS USD 100.00 (USD USD 100.00 AVendor AVendor 161010
|     | 23  |     | 100.00) |     |     |     |     |     |
| --- | --- | --- | ------- | --- | --- | --- | --- | --- |
External Reconciliation
This is custom documentation. For more information, please visit SAP Help Portal. 126

6/8/26, 6:08 AM
External reconciliation is the comparison of open transactions within SAP Business One with an external account statement. Most
commonly this is a bank statement. However, it could be a business partner’s account statement containing a list of transactions
that your customer sends to you as its vendor, for example.
For external bank statement reconciliations, SAP Business One supports two different processes:
Recording transactions from bank statements and then reconciling the transactions using the reconciliation function.
Recording and reconciling bank statements using the bank statement processing function (see Setting Up Bank Statement
Processing and Working with Bank Statement Processing).
In addition to performing reconciliations, you can also do the following:
View, cancel, re-create, and print previous external reconciliations
Print reconciliations when you manually or automatically perform external reconciliations
The interactive graphics below help you navigate through this section. Choose the highlighted areas for more information.
Please note that image maps are not interactive in PDF outputs.
Recording Transactions from External Statements
Context
To record transactions from external bank or business partner statements, you can enter information manually or automatically.
Later, to reconcile these transactions with the transactions recorded in the books, use the reconciliation function.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Process
External Bank Statement .
 Note
In few localizations the menu entry Process External Bank Statement is invisible by default. To display this feature click
the icon, and select the Process External Bank Statement option.
The Process External Bank Statement window appears.
2. From the G/L Account dropdown list, select G/L Account if you want to record transactions from your bank statements, or
select BP if you want to record transactions from your business partner’s statements. Specify the code of the G/L account
or business partner for which you want to record the transactions.
The Page Currency field automatically displays the currency defined for the G/L account or the business partner you
specified. This is the currency in which the amounts posted to this page are calculated.
This is custom documentation. For more information, please visit SAP Help Portal. 127

6/8/26, 6:08 AM
 Note
If All Currencies is defined for the specified G/L account or the business partner, the currency displayed is the local
currency; reconciliations and transactions of All Currencies entities are performed and calculated in the local currency.
3. Move the cursor to the first empty row and specify the information as it appears in the statement you received from the
bank or the business partner.
4. If you record transactions from your bank statements, to create an automatic incoming payment linked to an existing
invoice, in the table area select the Create Payment checkbox and specify the customer code and the existing invoice
number. For more information, see Automatically Creating Incoming Payments to Reconcile Bank State.
5. To save the information, choose Update.
Results
SAP Business One updates the list of external transactions and the expected current balance of the G/L account or the business
partner according to the statement. You can later reconcile those transactions.
Related Information
Performing External Reconciliations
Process External Bank Statement Window
Automatically Creating Incoming Payments to Reconcile Bank
Statements
Context
In the Process External Bank Statement window, if the amount recorded in a row is a credit amount and represents an incoming
payment from a customer using a bank transfer, SAP Business One can create the relevant incoming payment document
automatically.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Process
External Bank Statement .
2. From the G/L Account dropdown list, select G/L Account and specify the code of the G/L account for which you want to
record the incoming payment.
3. Move the cursor to the first empty row and specify the details as they appear on the statement you received from the bank.
For more information, see Recording Transactions from External Statements.
4. To create an automatic incoming payment, select the Create Payment checkbox and specify the remaining information
5. To save the information, choose the Update button.
Results
SAP Business One creates an incoming payment using a bank transfer. Then SAP Business One creates two reconciliations:
Internal reconciliation for the incoming payment with the invoice of the customer. The reconciliation type set for this
reconciliation is Payment.
External reconciliation for the incoming payment with the transaction from the bank statement. The reconciliation type set
for this reconciliation is Manual.
This is custom documentation. For more information, please visit SAP Help Portal. 128

6/8/26, 6:08 AM
Related Information
Process External Bank Statement Window
Process External Bank Statement Window
Use this window to record transactions from your external bank or business partner statements.
To open this window, choose Banking Bank Statements and External Reconciliations Process External Bank Statement .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Process External Bank Statement Window Fields
G/L Account
From the dropdown list, select G/L Account if you want to record transactions from your bank statements, or select BP if you want
to record transactions from your business partner’s statements.
Code
Specify the code of the G/L account or business partner for which you want to record the transactions.
Page Currency
Automatically displays the currency defined for the G/L account or the business partner you specified. This is the currency in
which the amounts posted to this page are calculated 9.
 Note
If All Currencies is defined for the specified G/L account or the business partner, the currency displayed is the local currency;
reconciliations and transactions of All Currencies entities are performed and calculated in the local currency.
Reconciled
Reconciliation number of the transactions for which you performed external reconciliations. For unreconciled transactions, this
field is blank.
Date
Specify the date that appears in the statement received from the external account.
Reference, Details, Details 2
Specify the reference and relevant details as they appear in the statement received from the external account; for example, fee or
deposit.
Debit Amount, Credit Amount
Specify the respective debit or credit amount from the external account statement.
Current Balance
Displays the expected current balance of the G/L account or the business partner calculated automatically by SAP Business One
for each row based on the information you specified from the statement. Negative balances are indicated by a minus sign.
Recalculate
This is custom documentation. For more information, please visit SAP Help Portal. 129

6/8/26, 6:08 AM
Refreshes and updates the expected current balance in the external account statement.
End of Page
Moves the cursor to the first empty row at the end of the table. This can be useful when you have many transactions in the table,
and you want to go instantly to the first empty row.
Additional Fields When You Choose G/L Account in the G/L Account Dropdown List
Create Payment
Enables the creation of an automatic incoming payment linked to an existing invoice.
Transact. Type
D - Doc Num - represents that document number of the invoice.
More Information
Recording Transactions from External Statements
Automatically Creating Incoming Payments to Reconcile Bank State
Performing External Reconciliations
You can perform external reconciliations manually, automatically, or semiautomatically (manually based on recommendations
from SAP Business One) for bank and business partner accounts.
 Recommendation
Use a reconciliation type that meets your business needs, as follows:
Manual reconciliation is appropriate for a small number of transactions, cases where partial reconciliations are required,
or when transactions are posted to more than one business partner or G/L account.
Automatic reconciliation is appropriate for a large number of transactions or a range of business partners or G/L
accounts, based on user-defined parameters and priorities.
Semiautomatic reconciliation is appropriate when you want to process transactions manually based on
recommendations provided by SAP Business One.
More Information
Recording Transactions from External Statements
Automatically Performing External Reconciliations
Semiautomatically Performing External Reconciliations
Automatically Performing External Reconciliations
You can perform automatic reconciliations when you need to reconcile a large number of transactions, or when you need to
reconcile a range of business partners or G/L accounts. The process for automatically reconciling business partner transactions or
This is custom documentation. For more information, please visit SAP Help Portal. 130

6/8/26, 6:08 AM
G/L accounts is similar.
SAP Business One performs automatic reconciliations for pairs of transactions, and the reconciliation is done separately for each
business partner or G/L account successively. If you allow automatic reconciliations with differences, SAP Business One posts any
differences found to the automatic reconciliation difference account.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
Prerequisites
To perform automatic reconciliations with reconciliation differences, you have to define an automatic reconciliation difference
account. For more information, see Defining an Automatic Reconciliation Difference Account.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations
Reconciliation .
The External Reconciliation - Selection Criteria window appears.
2. To specify whether to reconcile transactions of business partners or G/L accounts, from the Select Source dropdown list
select Business Partner or G/L Account.
3. Select the Automatic radio button and specify the selection criteria.
4. Choose the Reconcile button.
Result
SAP Business One reconciles the transactions according to the parameters you defined and then displays the External
Reconciliation window.
The transactions displayed in the upper tables are the ones created for the selected G/L accounts or business partners but could
not be reconciled according to the parameters you defined in the selection criteria window.
More Information
External Reconciliation - Selection Criteria Window
External Reconciliation Window
Defining an Automatic Reconciliation Difference Account
Context
You can perform automatic internal and external reconciliations of transactions with nonidentical amounts. To allow automatic
reconciliations with differences, you must first define the automatic reconciliation difference account. Then, when you perform the
This is custom documentation. For more information, please visit SAP Help Portal. 131

6/8/26, 6:08 AM
automatic reconciliation, you specify the maximum amount of the difference that should be allowed.
During automatic reconciliation, SAP Business One fully reconciles pairs of transactions. If a difference is found, and it is less than
or equal to the maximum difference amount you specified, it is posted to the automatic reconciliation difference account.
Procedure
1. From the SAP Business One Main Menu, choose Administration Setup Financials G/L Account Determination
General tab.
2. In the Automatic Reconciliation Diff. field, specify an existing G/L account or define a new account.
3. To save your changes, choose the Update button.
Related Information
Automatically Performing External Reconciliations
Semiautomatically Performing External Reconciliations
You can perform semiautomatic external reconciliations for business partner transactions and for G/L accounts. The reconciliation
is done manually, based on recommendations provided by SAP Business One. The process for semiautomatically reconciling
business partner transactions and semiautomatically reconciling G/L accounts is similar.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations
Reconciliation .
The External Reconciliation – Selection Criteria window appears.
2. To specify whether to reconcile transactions of a business partner or a G/L account, from the Select Source dropdown list
select Business Partner or G/L Account.
3. Choose the Semi-Automatic radio button and specify the selection criteria.
4. To generate the reconciliation recommendations, choose the Reconcile button.
The Reconciliation window appears. In the Open Transactions in Books and the Open Transactions in External Statement
tables, SAP Business One displays the list of transactions with unreconciled amounts greater than zero.
5. View the displayed information for each transaction.
 Note
To perform manual reconciliations not based on the recommendations, choose the Manual button. The External
Reconciliation window appears.
6. To see a list of recommended reconciliations, double-click a transaction row.
This is custom documentation. For more information, please visit SAP Help Portal. 132

6/8/26, 6:08 AM
The Reconciliation Recommendations window appears.
SAP Business One displays the selected transaction and below it a separate list of reconciliation recommendations for the
selected transaction, sorted in order of rank starting from the highest rank. The rank reflects the level of matching between
the selected transaction and the proposed transactions. It is calculated according to the parameters and the priority
weighting you specified in the External Reconciliation - Selection Criteria window. For more information, see Calculation of
Ranking for Reconciliation Recommendations.
7. To select a recommendation from the list of reconciliation recommendations, click once in the row of the desired
recommendation.
To perform the reconciliation, choose the Reconcile button.
 Note
If you choose to reconcile transactions with an amount difference (based on the recommendations), the Journal Entry
window appears. You must create the respective balancing transaction to complete the reconciliation.
If you decide not to reconcile the transaction that appears at the top of the window and instead want to display the next
transaction in the Reconciliation window, choose the Skip button. SAP Business One then displays the next transaction in
the first row of the window.
Result
SAP Business One reconciles the selected transactions.
More Information
External Reconciliation - Selection Criteria Window
Reconciliation Recommendations Window
Reconciliation Window
Journal Entry Window
Example: Semiautomatic External or Internal Reconciliation
Calculation of Ranking for Reconciliation Recommendations
When you perform semiautomatic external reconciliation, SAP Business One provides you with ranked recommendations for
reconciliations, which you then perform manually. The ranking calculation for each recommendation is comprised of the summary
of the ranking for the three parameters: the amount, the date, and the reference.
The priority weighting and the maximum deviation you specify for each parameter in the selection criteria for the external
reconciliation determine how the ranking is calculated.
Specifying the priority determines the maximum rank for a parameter.
Priority Weighting Value
High 45
Medium 35
This is custom documentation. For more information, please visit SAP Help Portal. 133

6/8/26, 6:08 AM
| Priority Weighting | Value |     |     |     |
| ------------------ | ----- | --- | --- | --- |
| Low                | 20    |     |     |     |
| Skip               | 0     |     |     |     |
The rank for each parameter is calculated using the following formula:
| Parameter |     | Formula |     | Comment |
| --------- | --- | ------- | --- | ------- |
Amount Priority Weighting – (absolute amount If Max. Deviation is zero, the parameter
difference / Max. Deviation) X Priority rank is the Priority Weighting value if both
|     |     | Weighting |     | transactions have the same amounts; |
| --- | --- | --------- | --- | ----------------------------------- |
otherwise it is zero
Date Priority Weighting – (absolute date If Max. Deviation is zero, the parameter
difference in days / Max. Deviation) X rank is the Priority Weighting value if both
Priority Weighting transactions have the same date; otherwise
it is zero
Reference Priority Weighting Rank is zero if the transactions do not have
the same reference number.
  Note
The result of [amount/date difference / Max. Deviation X Priority Weighting] is rounded down to the nearest whole
number.
If SAP Business One recommends reconciling a few transactions together, the calculation of the amount rank is based
on the summary of the amounts of those transactions. The calculation of the date rank is based on the summary of the
transactions’ date rank.
The total ranking for a recommended reconciliation is calculated as follows: rank = amount rank + date rank + reference rank
Example
You prioritized the parameters as follows:
| Parameter    | Priority Weighting | Max. Deviation |     |     |
| ------------ | ------------------ | -------------- | --- | --- |
| Amount       | High               | 50             |     |     |
| Posting date | Medium             | 30             |     |     |
| Reference 1  | Skip               | Not applicable |     |     |
You want to reconcile the following transaction:
| Transaction Number | Posting Date   | Reference 1 | Balance Due |     |
| ------------------ | -------------- | ----------- | ----------- | --- |
| 100                | October 5 2009 | 54          | 50          |     |
SAP Business One displays the following ranked recommendations:
This is custom documentation. For more information, please visit SAP Help Portal. 134

6/8/26, 6:08 AM
| Rank | Transaction Number | Posting Date     | Reference 1 | Balance Due |
| ---- | ------------------ | ---------------- | ----------- | ----------- |
| 72   | 304                | October 15, 2009 | 10          | 20          |
|      | 305                | October 29, 2009 | 22          | 35          |
| 55   | 306                | November 1, 2009 | 9           | 50          |
|      | 304                | October 15, 2009 | 10          | 20          |
| 49   | 306                | November 1, 2009 | 9           | 50          |
| 42   | 304                | October 15, 2009 | 10          | 20          |
| 39   | 305                | October 29, 2009 | 22          | 35          |
The following table details the calculations for the rank of each of the recommendations:
| Transaction Number | Amount Rank |     | Date Rank | Rank |
| ------------------ | ----------- | --- | --------- | ---- |
304 45 – |20 – 50| / 50 X 45 = 45 – 35 – 10 / 30 X 35 = 35 – 11 = 24 18 + 24 = 42
27 = 18
305 45 – |35 – 50| / 50 X 45 = 45 – 35 – 24 / 30 X 35 = 35 – 28 = 7 32 + 7 = 39
13 = 32
306 45 – |50 – 50| / 50 X 45 = 45 – 35 – 27 / 30 X 35 = 35 – 31 = 4 45 + 4 = 49
0 = 45
304, 305 45 – |20+35 – 50| / 50 X 45 = 24 + 7 = 31 41 + 31 = 72
45 – 4 = 41
304, 306 45 – |50+20 – 50| / 50 X 45 = 24 + 4 = 28 27 + 28 = 55
45 – 18 = 27
  Note
The combination of transactions 305 and 306 is not included in the recommendations since their balance due, which is 85,
deviates from the balance due of transaction 100 by more than 30, which is the value of the maximum deviation.
More Information
Semiautomatically Performing External Reconciliations
Example: Semiautomatic External or Internal Reconciliation
Reconciliation Recommendations Window
Example: Semiautomatic External or Internal Reconciliation
This example is relevant for both semiautomatic external and internal reconciliations.
The following open documents exist for a customer:
This is custom documentation. For more information, please visit SAP Help Portal. 135

6/8/26, 6:08 AM
| Document | Transaction Number | Posting Date       | Balance Due Amount |
| -------- | ------------------ | ------------------ | ------------------ |
| Invoice  | 905                | September 1, 2009  | 100                |
| Payment  | 906                | September 1, 2009  | 100                |
| Payment  | 907                | September 15, 2009 | 50                 |
| Payment  | 908                | October 5, 2009    | 50                 |
| Payment  | 909                | October 10, 2009   | 100                |
  Note
If the payments were recorded as incoming payments, you need to perform semiautomatic internal reconciliation. If the
payments were recorded as transactions on external statements (statements from a bank or business partner), you need to
perform semiautomatic external reconciliation.
To perform semiautomatic reconciliation, you prioritize the following parameters to be considered when SAP Business One
generates reconciliation recommendations for the reconciliation:
| Parameter    | Priority Weighting | Max. Deviation |     |
| ------------ | ------------------ | -------------- | --- |
| Amount       | High               | 50             |     |
| Posting date | High               | 30             |     |
| Reference 1  | Skip               | —              |     |
The Reconciliation Recommendations window displays the recommendations for the invoice:
For the three recommendations displayed, the payment with transaction number 906 is recommended as the best match. Its
balance due does not deviate from the invoice balance due, and its posting date does not deviate as well.
  Note
Payments with transaction number 908 and 909 do not appear in the recommendations since their posting date deviates by
more than 30 days from the posting date of the invoice.
More Information
Calculation of Ranking for Reconciliation Recommendations
Semiautomatically Performing External Reconciliations
Windows for Performing External Reconciliations
Use the following windows for performing external reconciliations:
External Reconciliation - Selection Criteria Window
External Reconciliation Window
Reconciliation Recommendations Window
This is custom documentation. For more information, please visit SAP Help Portal. 136

6/8/26, 6:08 AM
Reconciliation Window
External Reconciliation - Selection Criteria Window
Use this window to define the criteria for selecting transactions for external reconciliations.
To open the window, choose Banking Bank Statements and External Reconciliations External Reconciliation .
General/Manual
Select Source
To specify whether to reconcile transactions of a business partner or G/L account, from the dropdown list, select Business Partner
or G/L Account.
From... To...
In the From field, specify one business partner or one G/L account code you want to reconcile. This field is mandatory.
Due Date To
Displays by default the current date; specify a different date if required. Transactions with a due date earlier or equal to the
displayed date are reconciled.
Reconcile
Choose to start the reconciliation.
Automatic
Reconcile by Totals Only
Selecting this radio button:
Enables the reconciliation of transactions with matched amounts.
Displays the Variation in Days checkbox.
If you want SAP Business One to tolerate due-date differences between transactions with matching amounts, select the
Variation in Days checkbox. Then specify the number of days SAP Business One uses to consider whether reconciliation
takes place; the difference must be equal to or below the value you specify here. When left empty, this field is considered to
have a zero value.
 Example
You selected Due Date as a matching rule and specified the Variation in Days as 3. The due date of an invoice is October
1, 2009, and there is a payment for the exact amount with the posting date of October 6, 2009. The difference is five
days. In this case reconciliation does not take place.
Totals with Restrictions
Selecting this radio button:
Enables the reconciliation of transactions with matching amounts that also comply with additional conditions based on
reference and date.
Displays the Reference checkbox. If you select this checkbox:
This is custom documentation. For more information, please visit SAP Help Portal. 137

6/8/26, 6:08 AM
You can define additional conditions based on one of the references. From the dropdown list, select Ref. 1, Ref. 2, and Ref. 3,
which are fields in the Journal Entry window.
The Relate to .... Last Characters appears. Specify a number to indicate how many alphanumeric characters of the
selected reference are to be used an additional condition for matching during automatic reconciliation. The alphanumeric
characters are counted from right to left, and 0 (zero) is considered in the same way as other digits. For example, if the
reference is AZ2010ETL and the Relate to…Last Characters field is set to 4, then 0ETL is used for matching.
Displays the Date checkbox. Selecting this checkbox applies the posting date or due date as a condition for automatic
reconciliation.
Hide Reconciliation Process
Select this checkbox to hide the following for optimized performance:
The reconciliation process
The open transactions, both in books and in the external statement, in the External Reconciliation window after
reconciliation is finished
When this checkbox is selected, and after the reconciliation process is finished, the External Reconciliation window appears,
letting you define the print settings and print data.
 Note
When this checkbox is selected, the New Reconciliations Only radio button is not available in the External Reconciliation
Printing Preferences window. To print such reconciliations, find out the reconciliation number using the Manage Previous
External Reconciliations window, and enter the number in the Recon. From To fields of the External Reconciliation Printing
Preferences window when the New and Old Reconciliations radio button is selected.
 Note
This function is available only if you are using SAP Business One, version for SAP HANA.
Reconciliation Difference
 Note
The field is active only when you have defined the automatic reconciliation difference account.
Enables reconciliation of transactions with nonidentical amounts. In this field, specify the difference amount that should be
considered when automatic reconciliation is performed. Differences found during reconciliation are posted to the automatic
reconciliation difference account. For more information, see Defining an Automatic Reconciliation Difference Account.
Semiautomatic
Parameters
SAP Business One can take into account certain parameters when preparing the recommendation for reconciliation. You can
define the following parameters:
Amount – Enables SAP Business One to include transactions with different amounts in the reconciliation
recommendations. Enter the amount in the Max. Deviation column.
 Note
This is custom documentation. For more information, please visit SAP Help Portal. 138

6/8/26, 6:08 AM
This parameter influences the recommendation results only. If you choose to reconcile transactions with an amount
difference (based on the recommendations), you must create the corresponding balancing transaction to complete the
reconciliation.
Date – Select the date on which reconciliation recommendations should be based: either the due date or the posting date.
See also the Max. Deviation field.
Reference – Select the reference according to which you want the reconciliation recommendations to be made.
Priority Weighting
Determines the priority order in which each parameter is used by SAP Business One when ranking the generated
recommendations. Specify the weighting for each parameter: high, medium, low, or skip.
If you choose Skip, SAP Business One ignores the parameter when it is generating the reconciliation recommendations. For more
information, see Calculation of Ranking for Reconciliation Recommendations.
 Note
Skip is not available for the Amount parameter.
Max. Deviation
Specify the maximum deviation SAP Business One should consider when generating the reconciliation recommendations for the
following parameters:
Amount
Specify the maximum difference between transaction amounts above which SAP Business One does not recommend
reconciliation. If you do not specify an amount, SAP Business One includes transactions with no amount differences in the
reconciliation recommendations.
Date
Specify the difference in number of days between the dates assigned to the transactions above which SAP Business One
does not recommend reconciliation. If you choose to consider this parameter and you do not specify any value, SAP
Business One includes transactions with no date differences in the reconciliation recommendations.
Related Information
Automatically Performing External Reconciliations
Semiautomatically Performing External Reconciliations
External Reconciliation Window
Use this window to perform external reconciliations either manually or automatically.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
The window is divided into four identical tables:
This is custom documentation. For more information, please visit SAP Help Portal. 139

6/8/26, 6:08 AM
The tables on the left display the open transactions in books; the tables on the right display the open transactions in
external statements.
The upper tables display the open transactions on both sides (books and bank) that meet the selection criteria in the
External Reconciliation – Selection Criteria window. The lower tables display the transactions that you selected for
reconciliation.
To open the window, choose Banking Bank Statements and External Reconciliations Reconciliation . In the External
Reconciliation – Selection Criteria window, select either the Manual or Automatic radio button, specify the selection criteria, and
choose the Reconcile button.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
General Area
G/L Account/BP
Displays the G/L account or business partner code for which the reconciliation is performed. You can choose a different G/L
account or business partner.
Reconciliation Currency
Displays the currency of the reconciliation. This depends on the currency defined for the selected G/L account or business partner.
If the currency assigned to the selected G/L account or business partner is All Currencies, the local currency is displayed. The
reconciliation is performed in the local currency.
Print Settings
Opens the External Reconciliation Printing Preference window, in which you can define your preferences for printing
reconciliations.
Reconcile
Choose to reconcile the transactions displayed in the lower tables in the window.
Table Area
Transaction No. or Row
In the left-side tables: displays the journal entry transaction number.
In the right-side tables: displays the transaction row number in the Process External Bank Statement window.
Ref. 1, Ref. 2, Ref. 3
In the left-side tables: displays the reference number as it appears in the Ref. 1, Ref. 2 and Ref. 3 fields for the transaction in the
Journal Entry window. For more information about the sources of the information, see the explanations of Ref. 1, Ref. 2 and Ref. 3
in Journal Entry Window.
In the right-side tables: displays the reference number as it appears in the Reference field for the transaction in the Process
External Bank Statement window.
Amount
Original amount posted in the specific row of the transaction.
Details
This is custom documentation. For more information, please visit SAP Help Portal. 140

6/8/26, 6:08 AM
In the left-side tables: displays remarks as they appear in the Remarks field for the transaction in the Journal Entry window.
In the right-side tables: displays details as they appear in the Details field for the transaction in the Process External Bank
Statement window.
More Information
External Reconciliation - Selection Criteria Window
Automatically Performing External Reconciliations
Reconciliation Recommendations Window
 Note
This window is for semiautomatic external reconciliations only.
This window displays reconciliation recommendations generated according to the selection criteria and parameters defined in the
External Reconciliation – Selection Criteria window for semiautomatic reconciliations.
To open the window, choose Banking Bank Statements and External Reconciliations Reconciliation . In the External
Reconciliation – Selection Criteria window, select the Semi-Automatic radio button, specify the relevant information, and choose
the Reconcile button. In the Reconciliation window, double-click a transaction row.
 Note
This topic includes explanations of some of the fields and other elements in this window.
General Area and Table Columns
Rank
Recommendations are sorted in order of rank starting from the highest rank. The rank reflects the level of matching between the
selected transaction and the proposed transactions. It is calculated according to the parameters and the priority weighting you
specified in the External Reconciliation — Selection Criteria window.
Row
Displays the transaction row number in the Process External Bank Statement window.
Trans. No.
The journal entry number as it appears in the Trans. No. field in the Journal Entry window.
Posting Date/Due Date
The posting date or due date of this transaction row, depending on which value you specified in the External Reconciliation —
Selection Criteria window.
Ref 1, Ref 2, Ref 3
Reference 1, 2, or 3, of the transaction row displayed, depending on the reference specified in the External Reconciliation —
Selection Criteria window.
Amount
Displays the original amount posted in the specific row of the transaction.
This is custom documentation. For more information, please visit SAP Help Portal. 141

6/8/26, 6:08 AM
Details
For transaction in books, displays remarks as they appear in the Remarks field for the transaction in the Journal Entry window.
For transactions in external statements, displays details as they appear in the Details field for the transaction in the Process
External Bank Statement window.
More Information
External Reconciliation - Selection Criteria Window
Reconciliation Window for semiautomatic external reconciliations
Semiautomatically Performing External Reconciliations
Reconciliation Window
 Note
This window is for semiautomatic external reconciliations only.
The window displays transactions with unreconciled amounts greater than zero.
To open the window, choose Banking Bank Statements and External Reconciliations Reconciliation . In the External
Reconciliation – Selection Criteria window, select the Semi-Automatic radio button, specify the selection criteria, and choose the
Reconcile button.
 Note
This topic includes explanations of some of the fields and other elements in this window.
General Area
BP / G/L Account
Displays the G/L account or business partner code for which the reconciliation is performed.
Reconciliation Currency
Currency of the reconciliation. This depends on the currency defined for the selected G/L account or business partner. If the
currency assigned to the selected G/L account or business partner is All Currencies, the local currency is displayed, and the
reconciliation is performed in the local currency.
Ignore Negative Amounts
Select this checkbox to prevent the display of recommendations for transactions with negative amounts.
Manual
Choose to not use the recommendations and manually reconcile the transactions of the selected business partner or G/L account
by using the External Reconciliation window.
Table Areas
Open Transactions in Books
List of transactions with unreconciled amounts greater than zero in the books.
This is custom documentation. For more information, please visit SAP Help Portal. 142

6/8/26, 6:08 AM
Open Transactions in External Statement
List of transactions with unreconciled amounts greater than zero in the bank statement.
Trans. No.
The journal entry number as it appears in the Trans. No. field in the Journal Entry window.
Row
Transaction row number in the Process External Bank Statement window.
Posting Date/Due Date
The posting date or due date of this transaction row, depending on which value you specified in the External Reconciliation –
Selection Criteria window
Ref. 1/Ref. 2/Ref. 3
For Open Transactions in Books, displays reference 1, 2, or 3, of the transaction row, depending on the reference specified in the
External Reconciliation – Selection Criteria window. For more information about the sources of the information, see the
explanations of Ref. 1, Ref. 2 and Ref. 3 in Journal Entry Window.
For Open Transactions in External Statements, displays the reference number as it appears in the Reference field for the
transaction in the Process External Bank Statement window.
Amount
Amount posted in the specific row of the transaction.
More Information
External Reconciliation - Selection Criteria Window
Semiautomatically Performing External Reconciliations
Managing Previous External Reconciliations
You can view the history of all external reconciliations performed for a specified range of business partners or G/L accounts. You
can cancel and re-create external reconciliations created for business partners or G/L accounts as well as cancel incorrect external
reconciliations. For specific localizations, you can run a report on external reconciliations.
 Note
If bank statement processing is activated in SAP Business One, bank transactions recorded in bank statement processing are
not displayed in the Manage Previous External Reconciliations window. For more information, see the online help for SAP
Business One and How to Use Bank Statement Processing in Release 2007 at SAP Help Portal.
More Information
Viewing Previous External Reconciliations
Canceling Previous External Reconciliations
Re-Creating Previous External Reconciliations
Checking and Restoring Previous External Reconciliations
This is custom documentation. For more information, please visit SAP Help Portal. 143

6/8/26, 6:08 AM
Viewing Previous External Reconciliations
Context
Use this procedure to view external reconciliations that had been initiated previously by you or other users, whether manually,
automatically, or semiautomatically.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manage
Previous External Reconciliations .
The Manage Previous External Reconciliations - Selection Criteria window appears.
2. From the Previous Reconciliation for dropdown list, select to display previous reconciliations for business partners or for
G/L accounts and specify the selection criteria.
3. Choose the OK button.
The Manage Previous External Reconciliations window appears. It lists the previous external reconciliations that match
the selection criteria you specified in the Manage Previous External Reconciliations - Selection Criteria window.
This window contains three tables:
The upper table contains previous reconciliations.
The left-lower table lists the transactions in books associated with the reconciliation selected in the upper table.
The lower-right table lists the external statements associated with the reconciliation selected in the upper table.
 Note
In the lower tables, a row marked as bold indicates a balancing transaction.
4. From the Display Data for dropdown list, select whether to display all the reconciliations in the defined range or
reconciliations performed for a specific G/L account or business partner only.
5. To select a reconciliation in the upper table, click the relevant row.
The transactions associated with the selected reconciliation are displayed in the lower tables.
Related Information
Manage Previous External Reconciliations - Selection Criteria Window
Manage Previous External Reconciliations Window
Canceling Previous External Reconciliations
Context
Use this procedure to cancel external reconciliations that had been initiated previously by users, whether manually, automatically,
or semiautomatically.
Procedure
This is custom documentation. For more information, please visit SAP Help Portal. 144

6/8/26, 6:08 AM
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manage
Previous External Reconciliations .
2. In the Manage Previous External Reconciliations - Selection Criteria window, select to display previous reconciliations for
business partners or for G/L accounts. Specify the selection criteria and choose the OK button.
3. In the upper table in the Manage Previous External Reconciliations window, select one or more reconciliations to cancel
and choose the Cancel Reconciliation button.
Results
As a result of the cancellation:
Only the reconciliation serving as the link between the relevant transactions is opened.
The status of the involved documents (if there are any) is not changed from Closed to Open.
The Balance Due field is not updated.
If balancing transactions or automatic exchange-rate transactions are involved in the canceled reconciliation, they are not
reversed.
Related Information
Manage Previous External Reconciliations - Selection Criteria Window
Manage Previous External Reconciliations Window
Re-Creating Previous External Reconciliations
Context
After you have performed manual or semiautomatic external reconciliations, and even after automatic external reconciliations, you
may discover that there is an incorrect match between transactions. To address this situation, you can re-create previous external
reconciliations.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Manage
Previous External Reconciliations .
2. In the Manage Previous External Reconciliations - Selection Criteria window, select to display previous reconciliations for
business partners or for G/L accounts. Specify the selection criteria and choose the OK button.
3. In the upper table in the Manage Previous External Reconciliations window, select the relevant reconciliation you want to
re-create and choose the Redo button.
4. In the system message, click Continue.
Results
SAP Business One cancels the selected the reconciliation, opens the External Reconciliation window, and displays the relevant
transactions to be reconciled again. You can then make the necessary changes and reconcile the transaction.
Related Information
Manage Previous External Reconciliations - Selection Criteria Window
Manage Previous External Reconciliations Window
This is custom documentation. For more information, please visit SAP Help Portal. 145

6/8/26, 6:08 AM
Checking and Restoring Previous External Reconciliations
Incorrect external reconciliations are rare cases of reconciliations where the amounts on the debit and on the credit side do not
match.
You can display and cancel only incorrect external reconciliations or all the external reconciliations initiated by users and by SAP
Business One for a specific G/L account or business partner.
 Note
If bank statement processing is activated in SAP Business One, you must perform external reconciliations directly within the
bank statement processing functionality. Do not use this function to reconcile transactions from your bank statements. For
more information, see Setting Up Bank Statement Processing and Working with Bank Statement Processing in the general
online help file provided with SAP Business One.
 Note
If bank statement processing is activated in SAP Business One, bank transactions recorded in bank statement processing are
not displayed in the Check and Restore Previous External Reconciliations window.
Procedure
 Note
This action cannot be reversed.
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliations Check and
Restore Previous External Reconciliations .
2. In the Check and Restore Previous External Reconciliations window, specify the selection criteria and choose the Execute
button.
Reconciliations for the selected account or partner are displayed in the table.
3. Do one of the following:
To cancel all reconciliations displayed in the table, choose the Open All button.
To cancel only incorrect reconciliations, choose the Open Incorrect Only button.
 Caution
Once you choose the Open All button or the Open Incorrect Only button, you cannot undo the cancellation.
More Information
Check and Restore Previous External Reconciliations Window
Windows for Managing Previous External Reconciliations
Use the following windows for managing and reporting on previous external reconciliations:
Manage Previous External Reconciliations - Selection Criteria Wi
This is custom documentation. For more information, please visit SAP Help Portal. 146

6/8/26, 6:08 AM
Manage Previous External Reconciliations Window
Check and Restore Previous External Reconciliations Window
Manage Previous External Reconciliations - Selection Criteria
Window
Use this window to define the selection criteria for viewing, canceling, or re-creating previous external reconciliations created for
business partners or G/L accounts.
To open the window, choose Banking Bank Statements and External Reconciliations Manage Previous External
Reconciliations .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Previous Reconciliation for
From the dropdown list, select whether to display previous reconciliations for business partners or for G/L accounts.
G/L Acct/BP Code From…To…
Specify a range of business partners or G/L accounts, depending on your selection in the Previous Reconciliation for field.
Date From... To...
Specify a date range. The application displays reconciliations performed within this range.
Reconciliation No. From... To...
Specify a range of numbers representing the reconciliations the application should display.
More Information
Viewing Previous External Reconciliations
Canceling Previous External Reconciliations
Re-Creating Previous External Reconciliations
Manage Previous External Reconciliations Window
This window lists the external reconciliations that match the selection criteria you specified in the Manage Previous External
Reconciliations - Selection Criteria window.
To open the window, choose Banking Bank Statements and External Reconciliations Manage Previous External
Reconciliations .
This window contains three tables:
This is custom documentation. For more information, please visit SAP Help Portal. 147

6/8/26, 6:08 AM
The upper table contains previous reconciliations.
The left-lower table lists the transactions in books associated with the reconciliation selected in the upper table.
The lower-right table lists the external statements associated with the reconciliation selected in the upper table.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Upper Table Fields
G/L Acc./BP Code
Displays the code of the G/L account or business partner for which the reconciliation was performed.
Recon. No.
Sequential reconciliation number assigned to the external reconciliation by SAP Business One when the reconciliation took place.
Each business partner or G/L account has the same sequence of reconciliation numbers, starting from 1.
Recon. Amount
Total amount of the reconciliation.
Recon. Type
Type of reconciliation:
Manual
Reconciliation was performed in one of four ways: performed manually, performed in the Reconciliation Bank Statement
window, performed in the Process External Bank Statement window (see Automatically Creating Incoming Payments to
Reconcile Bank State), or performed by selecting the Manual radio button in the External Reconciliation - Selection
Criteria window.
By Total
Reconciliation was performed in one of two ways: by selecting the Automatic radio button in the External Reconciliation -
Selection Criteria window without considering any other factors or by selecting the Semi-Automatic radio button in the
External Reconciliation - Selection Criteria window and considering only the Amount parameter.
Due Date, Posting Date
Reconciliation was performed by selecting either the Automatic or the Semi-Automatic radio button in the External
Reconciliation - Selection Criteria window and considering either the due date or the posting date of the transactions.
Ref. 1, Ref. 2, Ref. 3
Reconciliation was performed by selecting either the Automatic or the Semi-Automatic radio button in the External
Reconciliation - Selection Criteria window and considering reference 1, 2, or 3 of the transactions.
In addition, the value in the Recon. Type field can be a combination of the due date or posting date and the reference number.
 Example
If you decide to consider Due Date and Ref. 3 in the selection criteria for the reconciliation, the value in the Recon. Type field is
Ref. 3 + Due Date.
Reconciliation Date
This is custom documentation. For more information, please visit SAP Help Portal. 148

6/8/26, 6:08 AM
Date on which the reconciliation was performed. However, if you perform external reconciliation using bank statement processing,
the field displays the due date from the bank statement line.
Creation Date
Date on which the reconciliation was performed.
Lower Table Fields
Display Data for G/L Account/BP
Specify whether to display all the reconciliations in the defined range, or reconciliations performed for a specific G/L account or
business partner.
Trans. No or Row
In the lower-left table: displays the journal entry number of the transaction involved in the selected reconciliation.
In the lower-right table: displays the row number of the transaction involved in the selected reconciliation in the Process External
Bank Statement window.
Due Date
Due date of the transaction involved in the selected reconciliation.
Ref. 1, Ref. 2, Ref. 3
In the lower-left table: displays the reference number as it appears in the Ref. 1, Ref. 2 and Ref. 3 fields for the transaction in the
Journal Entry window. For more information about the sources of the information, see the explanations of Ref. 1, Ref. 2 and Ref. 3
in Journal Entry Window.
In the lower-right table: displays the reference number as it appears in the Reference field for the transaction in the Process
External Bank Statement window.
Amount
Original amount posted in the specific row of the transaction involved in the selected reconciliation.
More Information
Manage Previous External Reconciliations - Selection Criteria Wi
Viewing Previous External Reconciliations
Canceling Previous External Reconciliations
Re-Creating Previous External Reconciliations
Check and Restore Previous External Reconciliations Window
Use this window to display and cancel only incorrect external reconciliations or all the external reconciliations initiated by users
and by SAP Business One for a specific G/L account or business partner.
 Note
Once you reverse external reconciliations, you cannot reverse this action.
This is custom documentation. For more information, please visit SAP Help Portal. 149

6/8/26, 6:08 AM
If bank statement processing is activated in SAP Business One, bank transactions recorded in bank statement processing are
not displayed in the Check and Restore Previous External Reconciliations window. For more information about external
reconciliations in bank statement processing, see Setting Up Bank Statement Processing and Working with Bank Statement
Processing.
To open the window, choose Banking Bank Statement and Reconciliations Check and Restore Previous External
Reconciliations .
 Note
This topic includes explanations of some of the fields and other elements in this window.
General Area
G/L Account/BP
Select whether to display reconciliations created for G/L accounts or for business partners.
G/L Acct/BP Code
Specify the code of the required G/L account or business partner for which you want to display former reconciliations.
Recon. From... To...
Specify a range of reconciliation numbers for displaying reconciliations. The default range is -999999 to 999999. The
reconciliations initiated by SAP Business One are assigned negative numbers. Positive numbers are assigned to reconciliations
initiated by the users.
Display Incorrect Reconciliations Only
Select to display only incorrect reconciliations. In general, incorrect reconciliations are displayed in red.
Display Incorrect Entries Starting From
To display incorrect entries whose difference is higher than a specific value, enter that value here.
Open All
Choose to open all reconciliations displayed in the table.
 Caution
Once you choose this button, you cannot undo the cancellation.
Open Incorrect Only
Choose to cancel only incorrect reconciliations.
 Caution
Once you choose this button, you cannot undo the cancellation.
Table Area
Recon.
Displays the reconciliation number.
Trans. No.
Displays the transaction number of the reconciled transactions.
This is custom documentation. For more information, please visit SAP Help Portal. 150

6/8/26, 6:08 AM
Row
Displays the row number of each transaction in the reconciliation.
Amount in Books
Displays the reconciled amount for each transaction as it appears on the books side.
Credit/Debit Acct
Displays the side of each transaction in the reconciliation. C stands for credit and D for debit.
Row in Bank
Displays the row number of the transaction in the bank statement.
Amount in Bank
Displays the reconciled amount in the bank statement.
Bank Credit/Debit
Displays the side of each transaction from the bank statement in the reconciliation. C stands for credit and D for debit. This column
appears only when displaying external reconciliations for G/L accounts.
Ref. 1
Displays the first reference of the reconciled transactions.
Posting Date, Due Date
Displays the posting date and due date of the reconciled transactions.
More Information
Checking and Restoring Previous External Reconciliations
Printing External Reconciliations
You can print both reconciled and unreconciled transactions for selected business partners or for G/L accounts, or print selected
previous external reconciliations.
More Information
Printing Reconciled and Unreconciled Transactions
Printing Previous External Reconciliations
Printing in SAP Business One
Printing Reconciled and Unreconciled Transactions
Context
Use this procedure to print reconciled and unreconciled transactions when you are manually or automatically reconciling
transactions for specific business partners or for G/L accounts.
This is custom documentation. For more information, please visit SAP Help Portal. 151

6/8/26, 6:08 AM
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliation
Reconciliation .
2. In the External Reconciliation - Selection Criteria window, from the Select Source dropdown list select Business Partner
or G/L Account, select the Manual or Automatic radio button, and specify the selection criteria. Then choose the
Reconcile button. For more information, see Semiautomatically Performing External Reconciliations and Automatically
Performing External Reconciliations.
3. In the External Reconciliation window, choose the Print Settings button.
The External Reconciliation Printing Preferences window appears
4. Specify your preferences and choose the Update button.
5. From the Tools menu, choose Layout Designer....
6. Select the preferred printing template.
7. Print the document.
 Note
You can edit the default templates or create new ones by using Print Layout Designer (PLD). For more information, see
How to Customize Printing Templates with Print Layout Designer at the SAP Help Portal.
Related Information
External Reconciliation Printing Preferences Window
Printing in SAP Business One
External Reconciliation Printing Preferences Window
Use this window to define your preferences for printing external reconciliations.
To open the window, choose Banking Bank Statements and External Reconciliations Reconciliation . In the External
Reconciliation - Selection Criteria window, from the Select Source dropdown list select Business Partner or G/L Account and
select either the Manual or Automatic radio button. Specify the selection criteria and choose the Reconcile button. In the External
Reconciliation window, choose the Print Settings button.
External Reconciliation Printing Preferences Window Fields
Print Reconciliations
When you select this option to print reconciliations, the following radio buttons appear:
New Reconciliations Only
Prints only the reconciliations that SAP Business One is about to perform.
New and Old Reconciliations
Prints reconciliations that were created in the past as well as the ones SAP Business One is about to perform. When you
select this option, additional fields appear that enable you to specify the reconciliation number range.
Unreconciled Transactions
When you select this checkbox, the Sorting 1 and Sorting 2 fields appear. Use these fields to define the sorting order of the
unreconciled transactions for the purpose of printing. You can sort by Transaction No., by Due Date, or by Ref 1.
Detailed Totals for External Reconciliations
This is custom documentation. For more information, please visit SAP Help Portal. 152

6/8/26, 6:08 AM
Select to include detailed totals related to the external bank reconciliations in the printed information.
More Information
External Reconciliation - Selection Criteria Window
External Reconciliation Window
Printing Reconciled and Unreconciled Transactions
Printing Previous External Reconciliations
Context
Use this procedure to print external reconciliations created by you, by other users, or by SAP Business One.
Procedure
1. From the SAP Business One Main Menu, choose Banking Bank Statements and External Reconciliation Manage
Previous External Reconciliations .
2. In the Manage Previous External Reconciliations - Selection Criteria window, from the Select Source dropdown list select
Business Partner or G/L Account, specify the selection criteria, and choose OK.
3. In the upper table of the Manage Previous External Reconciliations window, select the reconciliations you want to print.
4. From the Tools menu, choose Layout Designer....
5. Select the preferred printing template.
6. Print the document.
 Note
You can edit the default templates or create new ones by using Print Layout Designer (PLD). For more information, see
How to Customize Printing Templates with Print Layout Designer at SAP Help Portal.
Related Information
Printing in SAP Business One
Managing Previous External Reconciliations
Check Number Confirmation
This function enables you to verify that checks were printed properly, and that the numbers assigned to the checks by SAP
Business One match the numbers on the printed checks.
To confirm check numbers, choose Banking Check Number Confirmation .
More Information
Check Number Confirmation − Selection Criteria
Check Number Confirmation Window
This is custom documentation. For more information, please visit SAP Help Portal. 153

6/8/26, 6:08 AM
Confirming Printed Check Numbers
Prerequisites
You have made the following definitions:
The required parameters in Administration System Initialization Print Preferences Per Document tab with
Checks for Payment as the document type
The print-related parameters for each house bank account in Administration Setup Banking House Bank
Accounts
Context
The following procedure explains how to confirm a match between the numbers on printed checks and the numbers assigned to
these checks by SAP Business One.
Procedure
1. Choose Banking Check Number Confirmation .
The Check Number Confirmation – Selection Criteria window appears.
2. Enter the details of the bank account from which the checks are issued. You can also define a relevant posting date range
and internal number range.
3. Choose OK.
The Check Number Confirmation window appears. It displays checks that meet the defined selection criteria. By default,
SAP Business One assigns the status Confirmed to all checks in this window.
This window displays only checks that were printed but not confirmed at the time of printing.
4. Examine the printed checks and verify that their numbers match the numbers assigned to them by SAP Business One.
5. If required, change the status of the checks in the Check Number Confirmation window:
If you do not want to confirm or void a check, select Unconfirmed.
If you want to void the check, select Void.
6. To assign the statuses you have selected to the checks in this window, choose Update.
Results
The results depend on the status assigned to the check:
Confirmed checks
These checks are marked as printed and confirmed. They are not displayed in this window again. If you try to reprint a
confirmed check, SAP Business One notifies you that the check has been printed before.
Unconfirmed checks
These checks are marked as printed but not as confirmed. They reappear in the Check Number Confirmation window until
you confirm or void them. If you try to reprint an unconfirmed check, SAP Business One notifies you that the check has
been printed before but that the number has not been confirmed.
This is custom documentation. For more information, please visit SAP Help Portal. 154

6/8/26, 6:08 AM
Voided checks
These checks are marked as printed and voided. They do not reappear in the Check Number Confirmation window. If you
try to reprint a voided check, SAP Business One instructs you to ensure that the printer is loaded with the correct paper.
Related Information
Check Number Confirmation
Check Number Confirmation - Selection Criteria
Use this window to specify selection criteria for producing a list of checks whose accuracy you need to verify.
To open the window, choose Banking Check Number Confirmation .
After defining the criteria, choose OK to open the Check Number Confirmation window and proceed with the verification process.
Selection Criteria
Bank Account
Click to select a bank account or click for the following fields to make a selection:
Country/Region – select the country/region in which the bank is located.
Bank – select the bank in which the account is managed.
Account – select the required account.
Branch – if the branch of the selected bank account is defined in House Bank Accounts – Definitions window, it is
displayed here.
Posting Date From... To...
Define a range of posting dates to display checks created within this range.
Internal ID From... To...
Only checks whose internal key numbers fall within the specified range are displayed.
Vendor Code From... To...
Specify a range of vendor codes to display only checks that fall within this range.
Due Date From...To...
Specify a date range to display only checks with dates within the range.
More Information
Check Number Confirmation
Check Number Confirmation Window
This window displays details of the checks defined in the Check Number Information – Selection Criteria window. Use this window
to:
This is custom documentation. For more information, please visit SAP Help Portal. 155

6/8/26, 6:08 AM
Compare the accuracy of the information displayed here to the corresponding physical checks
Assign a print status to each check
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Check Number Confirmation Window
Print Status
Assign one of the following statuses to the displayed checks:
Unconfirmed – Assigned by default
Assign this status to checks that are neither confirmed as having been printed properly, nor verified as damaged.
 Note
The check number of an unconfirmed check can no longer be used unless you reset the print status to Not Printed.
Confirmed – Indicates the check was printed properly.
Damaged – Indicates a damaged check.
Assign this status to checks that were damaged during printing.
Not Printed – Assign this status to checks that have not yet been printed.
 Note
Changing the status of a check to Not Printed enables you to reuse the number assigned in the Check No. field.
A check that has never been printed and which is set to Not Printed reappears when you run check printing for checks
with a print status of To Be Printed.
 Note
If you change the status of a Not Printed check to Confirmed, Damaged, or Unconfirmed, then the next check number is
automatically assigned to it by default.
Internal ID
Displays the internal number assigned to the check and provides a link to it.
Country/Region, Bank, Account
Displays the details of the bank account from which the check is issued.
Due Date
Displays the due date of the check.
Total, Total (LC)
Displays the amount of the check in the check currency and in the local currency.
More Information
This is custom documentation. For more information, please visit SAP Help Portal. 156

6/8/26, 6:08 AM
Check Number Confirmation
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
This is custom documentation. For more information, please visit SAP Help Portal. 157

6/8/26, 6:08 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 158

6/8/26, 6:08 AM
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
This is custom documentation. For more information, please visit SAP Help Portal. 159

6/8/26, 6:08 AM
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
Related Information
Document Printing - Selection Criteria: Checks for Payment
Document Printing
Printing Documents Automatically
Context
You can set SAP Business One in such a way that certain document types, such as orders, are printed automatically when they are
created.
Procedure
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
This is custom documentation. For more information, please visit SAP Help Portal. 160

6/8/26, 6:08 AM
Printing Checks for Payment
Prerequisites
You have selected the Checks for Payment option and set other required parameters on the Per Document tab in
Administration System Initialization Print Preferences .
You have set the print-related parameters for each house bank account in Administration Setup Banking House
Bank Accounts .
Context
The following procedure explains how to print batches of checks for payment.
Procedure
1. From the SAP Business One Main Menu, choose Banking Document Printing .
The Document Printing – Selection Criteria window appears.
a. In the Document Type field, select Checks for Payment.
b. Specify all other required parameters and choose OK.
2. In the Print Checks for Payment window:
a. Deselect the checks that you do not want to print.
b. Verify that the Next Check No. value is correct; change, if necessary.
3. Load the printer with the correct check pages or blank paper and choose Print.
The Check Number Confirmation window appears.
4. Collect the printed checks from the printer and compare them to the checks displayed in the window.
5. If the numbers assigned by SAP Business One do not match the printed checks, you can change them. Correct the number
of the first check and press TAB . The subsequent check numbers are updated accordingly.
 Note
Only checks with successive numbers issued by the same account are updated accordingly. For example, if you change a
check number from 999 to 2000, check numbers 1000, 1001, 1002 and so on are updated to 2001, 2002 and 2003.
If the check numbers are not successive, you must correct each one manually.
6. By default, the print status of all checks in the window is Unconfirmed; change, if necessary.
7. Choose Update or OK.
Results
The numbers assigned to confirmed checks are marked as used.
The Next Check No. field in the House Bank Accounts – Setup window is updated.
Check numbers used for overflow printing are marked as voided.
The numbers assigned to checks with a print status of Unconfirmed cannot be reused, unless you reset the status to Not
Printed.
This is custom documentation. For more information, please visit SAP Help Portal. 161

6/8/26, 6:08 AM
Related Information
Checks for Payment
Document Printing - Selection Criteria: Checks for Payment
Use this window to specify selection criteria for printing checks.
To open the window, choose Banking Document Printing .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria: Checks for Payment
Document Type
Select Checks for Payment.
Print Checks
Select one of the following:
To Be Printed - lists the checks that are not yet printed.
For Reissuing - lists the checks that are already printed but should be printed again, together with their existing check
numbers.
Check Details Only - lists the checks that are already printed, whose details you need to reprint, together with their existing
check numbers.
Bank Account
Choose to open the Choose Bank window and choose the bank account for which the checks were created. The details of the
selected bank account are automatically displayed in the respective fields.
You can also specify the bank details one field at a time.
If you leave the fields empty, all house bank accounts defined in SAP Business One will be included.
Posting Date From...To...
Specify a posting date range to display only checks within this range.
Internal ID From...To...
Specify a range of internal key numbers to display only checks for payment within this range.
Vendor Code From...To...
Specify a range of vendors to display only checks issued for these vendors.
Due Date From...To...
Specify a date range to display only checks with dates within the range.
No. of Copies
Specify how many copies to print of each check.
This is custom documentation. For more information, please visit SAP Help Portal. 162

6/8/26, 6:08 AM
More Information
Printing Checks for Payment
Print Document Window
This window displays a list of documents to be printed. The list is based on the criteria you enter in the Document Printing -
Selection Criteria window. Select documents from the list using the table selection options for rows in SAP Business One. To
display each document, click .
To print the selected documents, choose Print.
Print Document Window
Document No., Posting Date, Due Date, BP Code, Total (LC)
These fields display relevant details about the documents to be printed.
More Information
Document Printing
Print Checks for Payment - To Be Printed
The following table describes the fields that appear in the Print Checks for Payment window.
To open the window, choose Banking Document Printing . In the Document Printing – Selection Criteria window, select
Check for Payment in the Document Type field. Enter the other parameters and choose OK.
 Note
The window is also accessible through the payment wizard.
Print Checks for Payment - To Be Printed
Bank
Displays the bank code from which the check originated.
Next Check No.
The number to be assigned to the next check to be printed, which is issued from the specified bank account. This number is taken
from the field Next Check No. in Administration Setup Banking House Bank Accounts - Setup window. You can change
the check number if required, but only to a greater number as smaller numbers are already assigned to checks that are already
printed.
Selection Column
All items are selected by default in this column. Deselect the checks for payment you do not want to print. To deselect or select all
items, double-click the column header.
If you deselect an account, all the checks originated by this account are also deselected.
Internal ID
This is custom documentation. For more information, please visit SAP Help Portal. 163

6/8/26, 6:08 AM
The internal alphanumeric key assigned automatically to the check by SAP Business One. This number is not printed on the check.
Click to display the check for payment.
Post. Date
The posting date of the check.
Vendor Code
Displays the code of the vendor for which the check is created.
Total, Total (LC)
Display the amount of the check in the original and local currency.
More Information
Printing Checks for Payment
Banking Reports
Use the reports under this menu entry to analyze and generate overviews of:
Checks for payment issued to vendors and other entities
Drafts created for banking related documents
External reconciliations related data (only if the checkbox Install Bank Statement Processing on the Basic Initialization
tab of the Company Details window is selected).
Check Register Report
This report gives an overview of the checks for payment created in SAP Business One. According to the selection criteria you
define, the report lists checks for payment, grouped by the originating accounts, and provides information such as whether a
check was printed, its amount, the confirmation status, and more.
Check Register Report - Selection Criteria
Use this window to specify selection criteria for the Check Register Report.
To open the window, choose Banking Banking Reports Check Register Report .
After defining the report, you can view it in the Check Register Report Window.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Selection Criteria
Due Date From...To...
This is custom documentation. For more information, please visit SAP Help Portal. 164

6/8/26, 6:08 AM
Specify a date range to display only checks with dates within the range.
Check No. From...To...
Specify a check number range to display only checks with numbers within the range.
 Note
Only relevant for printed checks.
Vendor Code From...To...
Specify a range of vendors to display only checks issued for these vendors.
Payment No. From...To...
Specify a range of Outgoing Payment numbers to display checks generated through these documents.
Checking Acct From...To...
Specify a range of house bank accounts to display in the report only checks issued by these accounts.
Display
Specify one of the following:
Voided checks only
Exclude voided checks
Printed checks only
Unprinted checks only
All checks
Display Results as List
When selected, a list of checks is displayed. When deselected, the checks are displayed grouped by credited bank account (the
account number appearing on the printed check).
Check Register Report Window
This window displays the Check Register Report according to the defined selection criteria.
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
Check Register Report Window
Account
Displays the house bank account issued the checks. Click the icon to display all the checks issued by that account.
Check No.
Displays the check number for printed checks. If the check is not printed yet this field displays 0 (=zero).
This is custom documentation. For more information, please visit SAP Help Portal. 165

6/8/26, 6:08 AM
G/L Acct/BP Code, G/L Acct/BP Name
Displays the code and name of the vendor or account for which the check was created.
Internal ID
Displays the internal alphanumeric key of the Checks for Payment document linked to the check.
Pmt No.
Displays the number of the Outgoing Payment document through which the check was created, and provides a link to it. If the
check was not created by an Outgoing Payment document this field displays 0 (=zero)
Payment Amt.
Displays the amount paid by the check.
Trans. No
Displays the number of the journal entry that reflects the check and provides a link to the journal entry window.
Status
Displays the current status of the check. The possible statuses are:
Confirmed – the check has been printed and confirmed.
Unconfirmed – the check has been printed but the number is not yet confirmed.
Void – the check has been voided in the Void Checks for Payment window.
Reissued – the check has been voided and then reissued.
Not Printed – the check has not been printed.
Overflow – the check information has overflowed the preprinted check paper in the printer, and has been printed on the
next check.
Printed
Indicates whether the check was printed or not.
Printed By
Displays the name of the user who printed the check.
Remarks
Displays remarks related to the check.
Payment Drafts Report
Use this function to display and process drafts of incoming and outgoing payment documents.
To create the report, choose Banking Banking Reports Payment Drafts Report .
Deleting Drafts
Context
This is custom documentation. For more information, please visit SAP Help Portal. 166

6/8/26, 6:08 AM
Follow this procedure to delete incoming and outgoing payments that were saved as drafts.
Procedure
1. Choose Banking Incoming Payments or Outgoing Payments Payment Drafts Report .
2. Specify the required parameters to display the drafts you want to delete.
3. Right-click the draft to be deleted and choose Remove.
 Note
You can only delete one draft at a time in the SAP Business One client.
To remove multiple drafts at the same time, please use SAP Business One, Web client. For more information, see the
topic Managing Drafts in the User Guide for the Web client.
Creating Regular Documents from Drafts
Procedure
1. Depending on the type of document you want to create, proceed as follows:
Sales documents
Choose Sales – A/R Sales Reports Document Drafts Report . In the Document Drafts – Selection Criteria
window, specify the required parameters and choose OK.
Purchasing documents
Choose Purchasing – A/P Purchasing Reports Document Drafts Report . In the Document Drafts –
Selection Criteria window, specify the required parameters and choose OK.
Incoming payment documents
Choose Banking Banking Reports Payment Drafts Report .
Outgoing payment documents
Choose Banking Banking Reports Payment Drafts Report or Banking Outgoing Payments Checks for
Payment Drafts .
Inventory documents
Choose Inventory Inventory Reports Document Drafts Report . In the Document Drafts – Selection Criteria
window, specify the required parameters and choose OK.
2. Double-click the required draft.
The document window appears in the Add mode.
3. Make any necessary changes and choose Add.
 Note
Since the number assigned to the regular document created from a draft is the one that currently appears in a new
document, it might be different than the one originally assigned to the draft.
Results
This is custom documentation. For more information, please visit SAP Help Portal. 167

6/8/26, 6:08 AM
The status of the draft is Closed.
Saving Documents as Drafts
Context
In SAP Business One, you can save sales and purchasing documents, payments, checks for payments and inventory documents as
drafts. This allows you to process them at a later point in time.
Procedure
1. Select the document you want to save as a draft.
2. Specify all required data.
3. To save the document draft, use one of the following options:
In the menu bar, choose File Save as Draft or right-click in the document window and choose Save as Draft.
Sale and purchasing documents:
Choose the Add Draft & New option in the document window. This option saves the document draft and
opens a new document in Add mode.
Using the dropdown, choose the Add Draft & View option in the document window. This option saves the
document draft and opens the draft in View mode.
Example
A customer phones to order certain items. During the conversation, you enter the sales order in SAP Business One. If, however, the
customer does not reach a final decision on whether to issue the order, you cannot add it. You save the order as a draft and process
it when the customer has decided to purchase the items.
You create a quotation for a customer. Since this is a large project, you work together with some colleagues to prepare the
quotation. Each of you is responsible for a different area of the quotation. You want to define the quotation data at an early stage to
ensure that you and your colleagues can access the current quotation when required. You save the quotation as a draft to ensure
that you can work on it until all the different areas have been completed.
 Note
This function is not the same as a release procedure. You can also define a release procedure for sales documents in the system
so that they are not posted in the system and subsequent activities are not carried out until the documents have been released.
Payment Drafts Report Window
This window displays the Payment Drafts Report.
To open the window, choose Banking Banking Reports Payment Drafts Report .
 Note
This topic documents fields and other elements in this window that either are not self-explanatory or require additional
information.
This is custom documentation. For more information, please visit SAP Help Portal. 168

6/8/26, 6:08 AM
Payment Drafts Report Window
User
To display drafts created by a particular user, specify this user. Super users can view drafts created by all users, while regular users
can view only those drafts that they have created.
 Note
Regular users, if given the following two authorizations, can view incoming or outgoing payment drafts created by other users
respectively. To define the authorizations View Incoming Payment Drafts Created by Other Users and View Outgoing
Payment Drafts Created by Other Users, go to Administration System Initialization Authorizations General
Authorizations Banking Outgoing Payments Payment Drafts Report .
Open Only
Displays only the drafts that were not added as regular payment documents.
Incoming Payments
Displays drafts created for incoming payments.
Outgoing Payments
Displays drafts created for outgoing payments.
Document
Type of document: incoming or outgoing payment.
Posting Date
Posting date of the payment document.
Document Total
Total payment amount.
Document Remarks
Remarks specified in the Remarks fields of the payment document.
Closed
Indicates whether or not the status of the draft is closed. After the draft is added and becomes a regular document, its status
changes to closed.
Payment Wizard Reports
Use payment wizard reports to view detailed information about different aspects of payment wizard runs.
Prerequisites
In the eighth step of the payment wizard: Payment Run Summary and Printing, you have chosen the button to display one of
the following reports:
Non-Included Trans. Report
Country/Region Summary Report
This is custom documentation. For more information, please visit SAP Help Portal. 169

6/8/26, 6:08 AM
Currency Summary Report
BP Summary Report
Payment Method Summary Report
Bank Account Summary Report
Payment Summary Report
Shortcut Keys in Payment Documents
Use the following shortcut keys in incoming and outgoing payments.
Shortcut Keys in Payment Documents
Function Menu Command Shortcut Key
Display the Payment Means window Go To Payment Means... Ctrl + Y
Generate the Transaction Journal report Go To Transaction Journal... Ctrl + J
Position the cursor in the Business Partner Go To Business Partner Code Ctrl + U
Code field
Move to the first row in the table Go To First Row Ctrl + H
Move to the last row in the table Go To Last Row Ctrl + E
Proceed to the Remarks field Go To Remarks Ctrl + R
Copy the amount due to the Total or Right Click Copy Balance Due Ctrl + B in the Total or Amount field
Amount fields in the Payment Means
window
Move to the next active field after you have Ctrl + Shift + Tab
changed the business partner name or a
G/L account name in Checks for Payment
Shortcut Keys in Payment Documents
Function Menu Command Shortcut Key
Display the Payment Means window Go To Payment Means... Ctrl + Y
Generate the Transaction Journal report Go To Transaction Journal... Ctrl + J
Position the cursor in the Business Partner Go To Business Partner Code Ctrl + U
Code field
Move to the first row in the table Go To First Row Ctrl + H
Move to the last row in the table Go To Last Row Ctrl + E
Proceed to the Remarks field Go To Remarks Ctrl + R
Copy the amount due to the Total or Right Click Copy Balance Due Ctrl + B in the Total or Amount field
Amount fields in the Payment Means
window
This is custom documentation. For more information, please visit SAP Help Portal. 170

6/8/26, 6:08 AM
Function Menu Command Shortcut Key
Move to the next active field after you have Ctrl + Shift + Tab
changed the business partner name or a
G/L account name in Checks for Payment
More Information
About Shortcut Keys in SAP Business One
This is custom documentation. For more information, please visit SAP Help Portal. 171