**==> picture [596 x 420] intentionally omitted <==**

User Guide | PUBLIC Document Version: 1.0 – 2025-05-16 

## **How to Prepare for and Perform Data Archiving in SAP Business One** 

**==> picture [58 x 30] intentionally omitted <==**

## **Content** 

|**1**|**Document History. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3**|
|---|---|
|**2**|**Introduction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4**|
|2.1|Glossary. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5|
|**3**|**Patch Updates. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7**|
|**4**|**Background. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8**|
|4.1|What Is a Cluster?. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8|
|4.2|Which Clusters Are Archivable?. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .8|
|4.3|Data Archive Journal Entry. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9|
|4.4|Data Archive Inventory Transaction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .11|
|4.5|Data Archive External Bank Statement Line. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .12|
|**5**|**What Data is Archived?. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .16**|
|5.1|Financials. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .18|
|5.2|Sales Opportunities. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .18|
|5.3|Sales - A/R. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .18|
|5.4|Purchasing - A/P. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 20|
|5.5|Business Partners. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .21|
|5.6|Banking. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 21|
|5.7|Inventory. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .22|
|5.8|Production. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .22|
|5.9|Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23|
|5.10|Miscellaneous. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23|
|**6**|**How to Prepare for Data Archiving. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24**|
|**7**|**Simulating Data Archive Runs. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 28**|
|**8**|**Archiving Data. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 49**|
|**9**|**Loading Saved Data Archive runs. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 58**|
|**10**|**Restoring the Read-Only Company Database. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 60**|
|**11**|**Searching Transactions across Multiple Data Archive Runs. . . . . . . . . . . . . . . . . . . . . . . . . . . 62**|



How to Prepare for and Perform Data Archiving in SAP Business One 

**Content** 

**2** 

PUBLIC 

**1 Document History** 

|Version|Date|Change|Change|
|---|---|---|---|
|1.0|2025-05-16|•|Guide converted from PDF to HTML format for viewing on the SAP Help Portal.|
|||•|Guide updated with latest screenshots and features.|
|||•|Added a new sectionPatch Updates [page 7].|



How to Prepare for and Perform Data Archiving in SAP Business One **Document History** 

PUBLIC 

**3** 

## **2 Introduction** 

##  Note 

The data archive wizard is not supported in SAP Business One Browser Access, or SAP Business One, version for SAP HANA. 

Companies that have worked with SAP Business One for more than two years can use the data archive wizard to archive closed transactional data relating to previous financial periods that have been locked. Closed transactional data can be closed sales and purchasing documents, reconciled journal entries, and so on. 

##  Recommendation 

We recommend that you use the data archiving function regularly, for example, once a year. Otherwise, the archiving process can take days. 

With the data archive wizard, you can perform the following tasks: 

- Simulate a data archive wizard run 

The simulation gives you a preview of the expected results of the actual wizard run. It enables you to know: 

   - The data that will be removed 

   - The expected reduction in database size 

- Initiate a data archive wizard run 

When the run is complete, a certain amount of data is permanently removed from the database. This action is irreversible. 

##  Note 

SAP Business One automatically backs up the database before any data is removed. If needed, you can always restore the backup file, review the database, generate reports, and print documents. The database you restore is in read-only mode, so you cannot change or add any data to it. 

The amount of data removed depends on the length of the period included in the data archive wizard run and on the preparations made before the data archive wizard run starts. 

- Load a saved data archive wizard run 

   - All the data archive wizard runs are saved. If needed, you can view any data archive wizard run that was executed in the past, and check whether a specific document was archived in a specific run. 

- Search for documents or transactions across data archive runs 

This is relevant for companies that have performed more than one data archive run. If there is a need to locate a certain transaction or document that had been archived, you can search for it across multiple data archive runs. 

You can find more information about troubleshooting and localization specific information in SAP Note 3314881 . 

How to Prepare for and Perform Data Archiving in SAP Business One **Introduction** 

**4** PUBLIC 

## **2.1 Glossary** 

|Term|Description|
|---|---|
|Archived Period|The date range to which the data archive simulation or data archive wizard run is applied. The|
||start date is always the frst day of the company activity in SAP Business One, in other words, the|
||frst day of the earliest posting period defned in the company. The end date is the last day of the|
||posting period selected in the 5th step of the data archive wizard, and at least two years earlier|
||than the current system date.|
||Note|
||The data recorded during the last two years is required for the regular fnancial activity of the|
||business and, therefore, cannot be included in the archived period.|
|Data Archive Journal<br>Journal entry that is created during the data archive wizard run to refect the values of journal||
|Entry<br>entries and documents removed from the company database during the data archive wizard run.||
|Data Archive Inventory<br>Entry<br>Inventory entry that is created during the data archive wizard run to refect the values of inventory<br>transactions removed during the data archive wizard run. The removal of inventory transactions||
|and the creation of the data archive inventory entry is relevant only for companies that manage a||
|non-perpetual inventory system and do not use purchase accounting (the_Use Perpetual Inventory_||
|and_Use Purchase Accounts Posting System_checkboxes are not selected on the<br>_Administration_||
||_System Initialization_<br>_Company Details_<br>_Basic Initialization_<br>tab).|
||You can view the inventory entries in the following two places:|
||•<br>_Inventory_<br>_Inventory Reports_<br>_Inventory Posting List_<br>_Expanded Selection Criteria_|
||_Archived Inventory Journal_|
||•<br>_Inventory_<br>_Inventory Reports_<br>_Inventory Valuation Report_|
|Sub Period|The periods included in a defned posting period: days, months, quarters, or year (defned in|
||_Administration_<br>_System Initialization_<br>_Posting Periods_<br>_Posting Periods_<br>window).|
|Transaction|Any record in an SAP Business One company database that is included in the data archive wizard|
||run and considered as a potential candidate to be removed from the company database after the|
||data archive process is complete.|
||In the context of the data archive wizard, the term “transaction” represents documents (such|
||as sales quotations and service calls), journal entries, and other records (such as customer|
||equipment cards, service contracts, activities, and so on).|



How to Prepare for and Perform Data Archiving in SAP Business One **Introduction** 

PUBLIC **5** 

|Term|Description|
|---|---|
|Cluster|Group of transactions linked to each other by business logic connections. A cluster contains at|
||least one transaction.|
||Example|
||The following transactions are linked to each other by business logic connections and, there-|
||fore, all of them are included in a single cluster:|
||Sales quotation copied to a sales order, copied to a delivery, and then to an A/R invoice that|
||was paid by an incoming payment.|
|Removable/ Nonre-<br>movable Transaction|A transaction that complies with the conditions detailed inWhat Data is Archived? [page 16]. It<br>is considered by the data archive wizard as a transaction that can be archived and permanently|
||removed from the company database.|
||The following are considered nonremovable transactions:|
||•<br>A transaction that does not comply with the conditions listed inWhat Data is Archived? [page|
||16].|
||•<br>A transaction that is considered removable but is linked to a transaction that does not comply|
||with the conditions listed inWhat Data is Archived? [page 16].|
|Removable/ Nonre-<br>movable Cluster<br>A cluster that consists of removable transactions only (in other words, all the transactions in the<br>cluster are indicated as Removable Transactions) can be removed from the company database.||
|A cluster that includes at least one nonremovable transaction cannot be removed from the com-||
|pany database.||



How to Prepare for and Perform Data Archiving in SAP Business One 

**Introduction** 

**6** PUBLIC 

**3 Patch Updates** 

The latest patch of SAP Business One is needed to take full advantage of available data archiving functionality. The changes and enhancements related to data archiving, and provided in patches, are described below. See the individual SAP Notes about the patches for business scenarios and more information. 

## **Version 10.0 Feature Package 2305** 

As of SAP Business One 10.0 FP 2305, you can perform data archiving by documents. With this new archive method, you can determine which document types to archive. Closed or canceled documents can be archived regardless of their relationships to any base or target document that is still open. For more information, see SAP Note 3315306 . 

How to Prepare for and Perform Data Archiving in SAP Business One **Patch Updates** 

PUBLIC **7** 

## **4 Background** 

Companies that have worked with SAP Business One for a few years may have a large company database. This makes navigation between documents, journal entries, and other records more difficult, slows down the generation of reports, and requires more resources for regular maintenance activities (larger backup files require more space, upgrade process takes more time and requires more free space as well). 

The data archive wizard reduces the size of the company database by removing data that is no longer required for the regular course of work (older than two years), while reflecting the accounting and inventory values of the removed data by creating respective transactions. 

To ensure that the company database remains integral after the data archive process is done, the archiving method is cluster based. 

## **4.1 What Is a Cluster?** 

A cluster is a group of documents and/or transactions recorded in a SAP Business One company database that are linked to each other by business logic connections. 

##  Example 

Sales quotation no. 109 is copied into sales order no. 220. Sales order no. 225, which was created for the same customer, is fully copied together with sales order no. 220 into delivery no. 565. The delivery is fully copied into A/R invoice 320, which is partially paid by incoming payment no. 290 and partially copied into an A/R credit memo. All of these documents are considered as one cluster, as they are linked to each other by business logic connections. 

## **4.2 Which Clusters Are Archivable?** 

A cluster is archivable only if all the transactions included in it are defined as _Removable_ . The complete list of the transactions that can be removed and their specific conditions for being removable are provided in What Data is Archived? [page 16] 

If one of the transactions included in the archived period is found to be nonremovable, none of the transactions that are included in the same cluster can be archived. 

Since a single cluster may contain many transactions, and it is enough to have one nonremovable transaction in a cluster to mark the whole cluster as nonremovable, an appropriate preparation of the company database for the data archive wizard run can make a significant difference in the data archive results. 

You can find more information about cluster analysis in SAP Note 3358243 and this blog . 

How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

**8** PUBLIC 

## **4.3 Data Archive Journal Entry** 

To keep the correct balances of G/L accounts and business partners after the data archive wizard run takes place, SAP Business One automatically creates special journal entries to reflect the total values of the removed transactions. 

After SAP Business One identifies which transactions can be removed (for a complete list and criteria, see What Data is Archived? [page 16]), it aggregates the debit and credit amounts and composes the sums to data archive journal entries. 

The number of data archive journal entries created during the data archive wizard run depends on the length of the archived period, on the user settings, and on the amount of removable data. The available options are as follows: 

- One data archive journal entry per posting period 

##  Example 

The data archive wizard run is initiated for the period: 01.01.2002 – 31.12.2003. This date range includes two posting periods, 2002 and 2003. In this case, a maximum of two data archive journal entries are created. 

- One data archive journal entry per sub period 

##  Example 

The data archive wizard run is initiated for the period: 01.01.2002 – 31.12.2003. The sub periods defined in the company are quarters. This date range includes eight quarters. In this case, a maximum of eight data archive journal entries are created. 

- One data archive journal entry per month 

##  Example 

The data archive wizard run is initiated for the period: 01.01.2002 – 31.12.2003. The sub periods defined in the company are quarters, but the user chose to have one data archive journal entry for each month. This date range includes 24 months. In this case, a maximum of 24 data archive journal entries are created. 

Following is an example of a data archive journal entry: 

##  Example 

The company started working with SAP Business One on January 1st 2002. The company defined two sub periods in 2002. 

|Period Code|From|To|
|---|---|---|
|2002-1|01.01.02|01.07.02|
|2002-2|02.07.02|31.12.02|



How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

PUBLIC 

**9** 

The period to be archived is 1.1.2002 – 31.12.2002. Following are transactions existing in the company database: 

Transaction 1 - A/R invoice no. 99 

|Posting Date|G/L Acct/Business Partners|Debit|Credit|Balance Due|
|---|---|---|---|---|
|01.02.2002|Business Partner A|100||30|
|01.02.2002|Revenue Account||100|100|
|Transaction 2 – Partial payment for A/R invoice no. 99|||||
|Posting Date|G/L Acct/Business Partners|Debit|Credit|Balance Due|
|01.02.2002|Business Partner A||70|0|
|01.02.2002|Bank Account|70||70|
|Transaction 3 – A/R invoice no. 100|||||
|Posting Date|G/L Acct/Business Partners|Debit|Credit|Balance Due|
|01.02.2002|Business Partner A|90||0|
|01.02.2002|Revenue Account||90|90|
|Transaction 4 – Payment for A/R invoice no. 100|||||
|Posting Date|G/L Acct/Business Partners|Debit|Credit|Balance Due|
|02.07.2002|Business Partner A||90|0|
|02.07.2002|Revenue Account|90||90|



The user chooses to group the data archive transactions by period, which in this example is the year 2002. Transactions 3 and 4 comply with the data archive rules: 

- Both are within the date range of the archived period. 

- Both are fully reconciled. 

- Neither is linked to transactions with dates outside the date range of the archived period. 

Therefore, transactions 3 and 4 are removed from the database and the following data archive transaction is created to reflect their values: 

|Posting Date|G/L Acct/Business Partners|Debit|Credit|Balance Due|
|---|---|---|---|---|
|31.12.2002|Business Partner A||90|90|
|31.12.2002|Revenue Account|90||90|



##  Note 

Transactions 1 and 2 are considered nonremovable: 

- The business partner line in transaction 1 is not fully reconciled, and therefore transaction 1 is nonremovable. 

How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

**10** PUBLIC 

• Transaction 2 is linked to transaction 1. Since transactions that are linked to nonremovable transactions cannot be removed, transaction 2 is nonremovable as well. 

## **4.4 Data Archive Inventory Transaction** 

##  Note 

This section is relevant only for companies that manage a non-perpetual inventory system and do not use purchase accounting (the _Use Perpetual Inventory_ and _Use Purchase Accounts Posting System_ checkboxes are not selected on the _Administration System Initialization Company Details Basic Initialization_ tab). 

The data archive wizard removes all inventory transactions that comply with the data archive rules. SAP Business One then creates one data archive inventory transaction per item, per warehouse, that reflects the inventory value within the removed inventory transactions within the archived period. 

##  Note 

Only one data archive inventory transaction is created per item per warehouse for the archived period. Unlike data archive journal entries, the data archive inventory transactions cannot be grouped by subperiod or month. 

The inventory value in the data archive inventory transaction calculation is based on the source price selected by the user in the data archive wizard in step no. 5. 

##  Example 

A company has been working with SAP Business One since January 1st 2003. The company manages a non-perpetual inventory system. It has two warehouses and three items. The company performed a data archive for the years 2003 and 2004. 

The following inventory transactions have been recorded until 31.12.2004 and are considered removable: 

|Transaction|Item|Quantity|From Whse|To Whse|
|---|---|---|---|---|
|Goods receipt 1|Item_1|20||WH1|
|Goods receipt 1|Item_2|10||WH1|
|Delivery 100|Item_1|5|WH1||
|Goods receipt 2|Item_3|30||WH2|
|Goods receipt 2|Item_2|20||WH2|
|Delivery 101|Item_3|6|WH2||
|Inventory trans. 40|Item_3|3|WH2|WH1|



How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

PUBLIC **11** 

Following are the prices of the items in local currency in the purchasing price list that was specified by the user as the price source for inventory transactions: 

|Item Code|Price (Local Currency)|
|---|---|
|Item_1|25|
|Item_2|35|
|Item_3|45|



The following data archive inventory transactions are created to reflect the inventory values of the removable transactions: 

|Transaction|Item|Whse|Total Qty. in Whse|Inventory Value (LC)|
|---|---|---|---|---|
|Trans. 1|Item_1|WH1|20-5 = 15|15*25 = 375|
|Trans. 2|Item_2|WH1|10|10*35 = 350|
|Trans. 3|Item_2|WH2|20|20*35 = 700|
|Trans. 4|Item_3|WH1|3|3*45 = 135|
|Trans. 5|Item_3|WH2|30-6-3 = 21|21*45 = 945|



Additional Information: 

- The posting date of the data archive inventory transaction is the last day of the archived period. 

- If the source price for the data archive inventory transaction is defined in foreign currency, SAP Business One calculates the source price in local currency based on the exchange rate defined for the last day of the archived period. If an exchange rate is not available, an error message appears, and the _Exchange Rate and Indexes_ window opens, asking the user to specify the exchange rate for the last day of the archived period. 

- To view only the archived inventory journal entries in the inventory posting list, in the _Expanded Selection Criteria_ window by choosing _Expanded_ from the _Inventory Posting List - Selection Criteria_ window ( _Inventory Inventory Reports Inventory Posting List_ ), select the _Archived Inventory Journal_ checkbox. 

## **4.5 Data Archive External Bank Statement Line** 

The data archive wizard removes all the bank statement lines that were recorded within the date range of the archived period, and that are connected to removable clusters. Each sequence of removable lines is grouped into one line that represents the accumulated debit amounts and accumulated credit amounts. The sequences of removable lines are separated by nonremovable lines. 

How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

**12** PUBLIC 

##  Example 

Following table demonstrates how sequences of removable lines are defined: 

|Line No.|Removable/Nonremovable|Sequences|
|---|---|---|
|1|Removable|Sequence no. 1|
|2|Removable||
|3|Removable||
|4|Removable||
|5|Nonremovable||
|6|Removable|Sequence no. 2|
|7|Removable||
|8|Nonremovable||
|9|Removable|Sequence no. 3|
|10|Nonremovable||



##  Example 

The following example demonstrates how the data archive wizard handles different scenarios in external bank statements. 

The following table reflects the lines recorded in the _Process External Bank Statement_ window for G/L account code GL1000. On 30.06.2006, a data archive wizard run took place. The _Comments_ column indicates the data archive status for each line: 

|Seq. No.|Date|Rec. No.|Debit|Credit|Comments|
|---|---|---|---|---|---|
|1|1.6.06|7|100||Removable|
|2|1.6.06|8||50|Removable|
|3|5.6.06|11|70||Removable|
|4|7.6.06|9||80|Nonremovable. Connected to nonremovable clus-|
||||||ter|
|5|10.6.06|8|70||Removable|
|6|10.6.06|14||160|Removable|
|7|15.6.06|11||90|Removable|
|8|21.6.06|12|100||Removable|
|9|21.6.06|13||150|Nonremovable. Reconciliation includes lines out-|
||||||side of archived period (line 16)|
|10|25.6.06|14|700||Removable|
|11|26.6.06|18||500|Nonremovable. Reconciliation includes lines out-|
||||||side of archived period (line 14)|
|12|29.6.06|16|300||Removable|



How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

PUBLIC 

**13** 

|Seq. No.|Date|Rec. No.|Debit|Credit|Comments|
|---|---|---|---|---|---|
|13|30.6.06|19||400|Removable|
|14|2.7.06|18|100||Nonremovable. Outside archive period|
|15|5.7.06|20||100|Nonremovable. Outside archive period|
|16|5.7.06|13|60||Nonremovable. Outside archive period|



SAP Business One handles the removable lines in the bank statement above as follows (the nonremovable lines remain the same): 

Lines 1-3 are aggregated: 

|Seq. No.|Date|Rec. No.|Debit|Credit|Comments|
|---|---|---|---|---|---|
|1|1.6.06|7|100||Removable|
|2|1.6.06|8||50|Removable|
|3|5.6.06|11|70||Removable|



They are aggregated into one line: 

|Seq.|No.||Date||Debit||Credit||
|---|---|---|---|---|---|---|---|---|
|3|||5.6.06||170||50||
|Lines|5-8|are aggregated:|||||||
|Seq.|No.|Date||Rec. No.|Debit|Credit||Comments|
|5||10.6.06||8|70|||Removable|
|6||10.6.06||14||160||Removable|
|7||15.6.06||11||90||Removable|
|8||21.6.06||12|100|||Removable|



|They are aggregated into|They are aggregated into|one line:|||||
|---|---|---|---|---|---|---|
|Seq. No.||Date|Debit||Credit||
|8||21.6.06|170||250||
|Line 10 is removable:|||||||
|Seq. No.|Date|Rec. No.|Debit|Credit||Comments|
|10|25.6.06|14|700|||Removable|
|It is "converted" to a data||archive line:|||||
|Seq. No.||Date|Debit||Credit||
|10||25.6.06|700||||



How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

**14** PUBLIC 

||Lines 12-13 are aggregated:<br>Seq. No.<br>Date<br>Rec. No.<br>Debit<br>Credit<br>Comments<br>12<br>29.6.06<br>16<br>300<br>Removable<br>13<br>30.6.06<br>19<br>400<br>Removable<br>They are aggregated into one line:<br>Seq. No.<br>Date<br>Debit<br>Credit<br>13<br>30.6.06<br>300<br>400|
|---|---|



The data archive bank statement line is structured as follows: 

- Sequence number – determined by the sequence number of the last line in the group. For example, if lines 1 to 4 are grouped to one data archive line, the sequence number of the data archive line is 4. 

- Date – determined by the date of the last line in the group. For example, line 1 and line 2 are grouped. The date for Line 1 is May 22nd and for line 2 it is May 23rd. The date of the data archive line is set to May 23rd. 

- Reconciliation number – when the data archive line represents reconciled lines, the reconciliation number is set to zero, and the line is marked as reconciled (as such, it does not appear as a candidate for reconciliation in the _External Reconciliation_ window). 

##  Note 

By default, the data archive wizard handles only reconciled lines; however, the user can choose to archive unreconciled lines as well. 

How to Prepare for and Perform Data Archiving in SAP Business One **Background** 

PUBLIC **15** 

## **5 What Data is Archived?** 

To ensure a smooth and correct workflow in SAP Business One after the data archive process is complete, certain rules and guidelines are defined to determine which transactions can be removed and which cannot. 

The following table lists the database objects that can be removed (together with their sub objects) during the data archiving process. The table is followed by a detailed explanation about the removal guidelines for each transaction. 

|Object|Object Name|Object Type|
|---|---|---|
|OINV|A/R Invoice|13|
|ORIN|A/R Credit Memo|14|
|ODLN|Delivery|15|
|ORDN|Returns|16|
|ORDR|Sales Order|17|
|OPCH|A/P Invoice|18|
|ORPC|A/P Credit Memo|19|
|OPDN|Goods Receipt PO|20|
|ORPD|Goods Return|21|
|OPOR|Purchase Order|22|
|OQUT|Sales Quotations|23|
|ORCT|Incoming Payment|24|
|ODPS|Deposit|25|
|OBTD|Journal Vouchers List|29|
|OJDT|Journal Entry|30|
|OCLG|Activities|33|
|OBNK|External Bank Statement Received|42|
|OVPM|Outgoing Payments|46|
|OCHO|Checks for Payment|57|
|OIGN|Goods Receipt|59|
|OIGE|Goods Issue|60|
|OWTR|Inventory Transfer|67|
|OWKO|Production Instructions|68|
|OCRH|Credit Card Management|72|
|OCRV|Credit Payment|74|
|ODPT|Postdated Deposit|76|



How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

**16** PUBLIC 

|Object|Object Name|Object Type|
|---|---|---|
|OOPR|Sales Opportunity|97|
|ODRF|Drafts|112|
|OWDD|Documents for Confrmation|122|
|OCHD|Checks for Payment Drafts|123|
|OPDF|Payment Drafts|140|
|OPKL|Pick List|156|
|OPWZ|Payment Wizard|157|
|OMRV|Inventory Revaluation|162|
|OCPI|A/P Correction Invoice|163|
|OCPV|A/P Correction Invoice Reversal|164|
|OCSI|A/R Correction Invoice|165|
|OCSV|A/R Correction Invoice Reversal|166|
|OINS|Customer Equipment Card|176|
|OBOE|Bill of Exchange for Payment|181|
|OBOT|Bill of Exchange Transaction|182|
|OCTR|Service Contracts|190|
|OSCL|Service Calls|191|
|ODWZ|Dunning Wizard|197|
|OWOR|Production Order|202|
|ODPI|A/R Down Payment|203|
|ODPO|A/P Down Payment|204|
|OVRT|Tax Invoice Report|245|
|OSRT|Korean Summary Report|246|
|OMIN|A/R Monthly Invoice|270|
|OTSI|Sales Tax Invoice|280|
|OTPI|Purchase Tax Invoice|281|
|OJST|TDS Adjustment|10000079|
|OTPW|Tax Payment Wizard|140000008|
|OOEI|Outgoing Excise Invoice|140000009|
|OIEI|Incoming Excise Invoice|140000010|
|OMIV|A/P Monthly Invoice|140000014|
|OEJB|Wizard Run Details for ERV-JAb|350000004|



How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

PUBLIC **17** 

## **5.1 Financials** 

- Journal Entry – Manual journal entries with posting dates within the archived period can be removed, except for the following: 

   - Journal entries that include one or more business partner lines that are partially reconciled 

   - Journal entries that are reconciled against nonremovable transactions or against transactions with a posting date that deviates from the archived period 

   - Journal entries created through the _Period-End Closing_ utility 

   - Journal entries created by documents can be removed if the originating document is removable. If the originating document is not fully reconciled or is reconciled against a nonremovable transaction or is reconciled against a transaction that deviates from the archived period, the journal entry is nonremovable. 

- Journal Voucher – Journal vouchers with the status _Closed_ , and which include only journal voucher entries within the archived period, are removable. 

## **5.2 Sales Opportunities** 

Sales Opportunity – Sales opportunities created within the archived period, and having the status _Won_ or _Lost_ , are removable. 

## **5.3 Sales - A/R** 

- Sales Quotation – Sales quotations created within the archived period date range, and having the status _Closed_ or _Canceled_ , can be removed, unless they are connected to nonremovable documents. Sales quotations having the status _Closed_ or _Canceled_ that are connected to nonremovable documents, but have the _Archive Nonremovable Sales Quotation_ checkbox selected ( _Sales Quotation Accounting_ tab), can be removed as well. 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

**18** PUBLIC 

**==> picture [295 x 314] intentionally omitted <==**

- Sales Order – Sales orders that were created within the archived period date range and have the status _Closed_ or _Canceled_ can be removed, unless they are linked to nonremovable transactions. 

- Delivery and Return – If these documents were created within the archived period date range and have the status _Closed_ , they can be removed, unless they are linked to nonremovable documents. 

- A/R Down Payment Request – A/R down payment requests created within the archived period date range, having the status _Closed_ , that are linked to a final payment, and are not linked to a nonremovable incoming payment, can be removed. 

- A/R Down Payment Invoice – A/R down payment invoices having the status _Closed_ , that are linked to a final invoice, can be removed. 

- A/R Correction Invoice – A/R correction invoices created within the archived period and having the status _Closed_ (were fully copied to an A/R correction invoice reversal), can be removed. 

- A/R Correction Invoice Reversal – A/R correction invoice reversals that were created within the archived period and having the status _Closed_ can be removed. 

- A/R Credit Memo – A/R credit memos having the status _Closed_ can be removed, unless the journal entry created by the A/R credit memo is nonremovable. 

- A/R Invoice – A/R invoices having the status _Closed_ , that were created within the archived period can be removed, unless the journal entry created by the A/R invoice is nonremovable, or the A/R invoice is linked to an A/R correction invoice that cannot be removed. 

- A/R Reserve Invoice – A/R reserve invoices that were created within the archived period and having the status _Closed_ (fully reconciled and fully delivered) can be removed, unless the journal entry created by the A/R reserve invoice is nonremovable, or the A/R reserve invoice is linked to an A/R correction invoice that cannot be removed. 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

PUBLIC 

**19** 

- A/R Monthly Invoice - A/R monthly invoices that were created within the archived period, having the status _Closed_ , and with connected individuals within the archived period can be removed. 

- Dunning Wizard Run – Dunning wizard runs with the date of the dunning run within the archived period, and having the status _Saved Parameters_ or _Executed, Not Yet Printed Wizard_ or _Executed and Printed_ , can be either fully removed if all the linked documents are removable, or partially removed if some of the linked documents are removable. When all the linked documents are archived, the dunning run will be archived. You can archive a dunning wizard run when it meets both the following conditions: 

   - It has the status _Saved Parameters_ or _Executed, Not Yet Printed Wizard_ or _Executed and Printed_ . 

   - The date of the dunning run is more than two years ago. 

- A/R Tax Invoice – A/R tax invoices that were created within the archived period can be removed if all the documents that are linked to them are removable. 

## **5.4 Purchasing - A/P** 

- Purchase Order – Purchase orders created within the archived period and having the status _Closed_ or _Canceled_ can be removed, unless they are linked to nonremovable transactions. 

- Goods Receipt PO and Goods Return – If these documents were created within the archived period and have the status _Closed_ , they can be removed, unless they are linked to nonremovable transactions. 

- A/P Down Payment Request – A/P down payment requests that were created within the archived period, that have the status _Closed_ , and are linked to final payments can be removed. Exception: An A/P down payment request that is linked to a nonremovable outgoing payment cannot be removed. 

- A/P Down Payment Invoice – A/P down payment invoices that were created within the archived period, that have the status _Closed_ , and are linked to a final invoice, can be removed. 

- A/P Correction Invoice – A/P correction invoices that were created within the archived period and have the status _Closed_ (fully copied to A/P correction invoice reversal) can be removed. 

- A/P Correction Invoice Reversal – A/P correction invoice reversals that were created within the archived period and have the status _Closed_ can be removed. 

- A/P Credit Memo – A/P credit memos created within the archived period and having the status _Closed_ can be removed, unless the journal entry created by the A/P credit memo is nonremovable. 

- A/P Invoice – A/P invoices having the status _Closed_ can be removed, unless the journal entry created by the A/P invoice cannot be archived, or if the A/P invoice is linked to an A/P correction invoice that cannot be removed. 

- A/P Reserve Invoice – A/P reserve invoices that were created within the archived period and have the status _Closed_ (fully reconciled and fully delivered) can be removed, unless the journal entry created by the A/P reserve invoice cannot be archived, or if the A/P reserve invoice is linked to an A/P correction invoice that cannot be removed. 

- A/P Monthly Invoice – A/P monthly invoices that were created within the archived period, have the status _Closed_ , and whose connected individuals are all within the archived period, can be removed. 

- A/P Tax Invoice – A/P tax invoices that were created within the archived period can be removed if all the documents that are linked to them are removable. 

- Landed Costs – Landed costs documents can be removed when all the following are met: 

   - The company does not manage the purchase accounts posting system, that is, the _Use Purchase Accounts Posting System_ checkbox is not selected ( _Administration System Initialization Company Details Basic Initialization_ tab). 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

**20** PUBLIC 

- The latest landed cost in the business chain has the status _Closed_ . 

- Related goods receipt POs are archived. 

## **5.5 Business Partners** 

Activity – Activities with statuses _Closed_ and _Open_ , with start and end dates within the archived period, can be removed. 

## **5.6 Banking** 

- Incoming Payment – Incoming payments that were created within the archived period and having the status _Closed_ can be removed, unless: 

   - The journal entry created by the incoming payment is nonremovable. 

   - The payment means in the incoming payment are either undeposited checks or credit card vouchers. 

- Check – Checks received that are deposited as cash, canceled, or endorsed, and whose date is within the archived period, can be removed. 

- Credit Card Voucher – Credit card vouchers that were created within the archived period and deposited can be removed. In case of multiple payments, if the date of the latest credit card voucher deviates from the archived period, all the credit card vouchers in this payment are nonremovable. 

- Deposit – Deposits that were created within the archived period can be removed unless: 

   - The journal entry created by the deposit is nonremovable. 

   - The deposit includes a nonremovable check, credit card voucher, or bill of exchange. 

- Postdated Check Deposit – Postdated check deposits that were created within the archived period can be removed, unless they include nonremovable checks, or if the journal entry created by the postdated check deposit is nonremovable. 

- Postdated Credit Voucher Deposit – Postdated credit voucher deposits that were created within the archived period can be removed, unless they include nonremovable credit card vouchers, or if the journal entry created by the postdated credit voucher deposit is nonremovable. 

- Outgoing Payment – Outgoing payments created within the archived period that are fully reconciled can be removed, unless they include nonremovable bills of exchange. 

- Checks for Payment – Checks for payment that did not create journal entries (the _Create Journal Entry_ checkbox is not selected on the check) can be removed. Checks for payment that created journal entries (the _Create Journal Entry_ checkbox is selected) can be removed, unless the journal entry is nonremovable. 

- Bill of Exchange – Receivables 

- Bill of Exchange – Payables 

- Bill of Exchange Management – Bills of exchange management can be removed if all the bills of exchange that are linked to them are removable. 

- Payment Wizard Run – Payment wizard runs with a date within the archived period and with the status _Executed_ , _Saved_ , or _Canceled_ can be removed. Payment wizard runs with the status _Recommended_ cannot be removed. 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

PUBLIC **21** 

- Bank Statement Details – Bank statement details records (listed in the _Bank Statement Summary_ window) with _Statement Date_ within the archived period, and with the status _Finalized_ can be removed. 

- External Bank Statement – All the lines recorded for specific G/L accounts or business partners in the _Process External Bank Statement_ window that are connected to removable clusters, are considered removable as well. Lines that comply with one or more of the following categories cannot be archived: 

   - Lines that are connected to nonremovable clusters 

   - Lines that are partially reconciled 

   - Lines that are reconciled with transactions created outside the date range of the archived period 

## **5.7 Inventory** 

- Goods Receipt and Goods Issue – Goods receipts and goods issues created within the archived period can be removed. 

- Inventory Transfer – Inventory transfers created within the archived period, and that are based on removable document (if based) can be removed. 

- Inventory Revaluation – Inventory revaluation transactions within the archived period that do not include FIFO items can be removed. 

- Pick List – Pick lists can be either fully removed if the status is _Closed_ and all the linked sales orders are removable, or partially removed if the status is _Closed_ and some of the linked sales orders are removable. When a pick list can be partially removed, lines of the removable sales orders will be removed when the sales orders are archived. 

##  Note 

You can perform data archiving for documents included in closed pick lists, even though the closed pick lists include other open documents. 

After data archiving, information related to the archived documents no longer displays in the pick lists. 

- Bin Location – The transaction history of bin locations within the archived period can be removed. As a result, the bin location allocation is removed from all transactions within the period, even if the transactions themselves are not archived. 

## **5.8 Production** 

- Production Order – Production orders with the status _Closed_ can be removed. 

- Work Order – Work orders can be removed if they comply with the following conditions: 

   - The work orders have been upgraded to production orders, and those production orders were created based on the upgraded work orders and are removable. 

   - The work orders were set to the status _Closed_ , _Canceled_ , or _Completed_ (and therefore were not upgraded to production order), and their _Finish Date_ is within the archived period. 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

**22** PUBLIC 

If the _Finish Date_ field is empty, SAP Business One checks if the work order date is in the date range of the archive period, and if so, the work order is removable. 

## **5.9 Service** 

- Service Call – Service calls with the status _Closed_ and that have _Created On_ and _Closed On_ dates within the archived period can be removed. 

- Service Contract – Service contracts with _Termination Date_ within the archived period and service contracts with no termination date but with an _End Date_ within the archived period can be removed. 

- Customer Equipment Card – Customer equipment cards whose linked service calls, service contracts, deliveries, and invoices are removable, can be removed. 

## **5.10 Miscellaneous** 

- Draft – Drafts of sales, purchasing, banking, and inventory documents can be removed, unless they are part of an approval procedure and one of the following is true: 

   - The status of the approval is _Pending_ . 

   - The approval had been provided but the draft has not been added yet as a regular document. 

- Tax Payment Wizard – Tax payment wizard runs within the archived period can be removed. 

- User Defined Object – Only user-defined objects determined as document type and for which the _Data Archive_ ( _Requires Implementation DLL_ ) checkbox is selected (in _Tools Customization Tools Object Registration Wizard_ ) can be removed. 

- Document after Year Transfer – Documents that were “year transferred” are not linked to the journal entry created when were added originally. Such documents are removed from the company database if they comply with all the conditions described above, excluding the ones related to journal entries. 

- Request for Approval – Requests for approval with the status _Approved_ or _Rejected_ can be removed as long as the draft document connected to it was added. 

- Log File – Records in log files related to removed transactions are removed as well. 

- Financial XML File Generation Wizard – Financial XML file generation wizard runs with the status _Executed_ and which took place within the archived period can be removed. 

- Receipt Transaction with Uncompleted Serial Numbers or Batches – When an item is set to manage serial numbers or batches on release only, and some receipt transactions containing this item are still open for serial number or batch completion, such documents and related document clusters cannot be removed. For more information, see SAP Note 1762837 . 

How to Prepare for and Perform Data Archiving in SAP Business One **What Data is Archived?** 

PUBLIC **23** 

## **6 How to Prepare for Data Archiving** 

## **Context** 

SAP Business One enables you to perform data archiving for posting periods that ended more than two years ago, and that were assigned with the status _Locked_ or _Archived_ . 

To optimize the results of the data archive process, we strongly recommend that you make the following preparations: 

Since most of the transactions to be archived are documents with the status _Closed_ , generate the _Open Items_ 

_List_ report (choose _Reports Sales and Purchasing Open Items List_ ) and close, where possible, any document created within the period you intend to archive. This way you can increase the amount of data that will eventually be removed. 

##  Example 

You are about to archive the posting periods related to the year of 2012. Generate the open items list report and sort it according to the _Posting Date_ column: 

**==> picture [402 x 275] intentionally omitted <==**

Now, check which of the sales quotations that were created during 2012 can be closed. 

Generate a list of the different draft documents and check which of the drafts should and can be added as regular documents, and which are no longer relevant, and, therefore, can be removed. 

How to Prepare for and Perform Data Archiving in SAP Business One 

**How to Prepare for Data Archiving** 

**24** PUBLIC 

If your company manages a non-perpetual inventory system, the data archive wizard run handles inventory transactions as well. Although it is not mandatory, make sure to define prices for all of the items in the price list that will be used as the source price for the data archive inventory transaction. 

##  Note 

If the price list you are going to use as the source price for the data archive inventory transactions is in foreign currency, make sure that the exchange rate for the last day in the archived period exists in the _Exchange Rate and Indexes_ window. 

##  Note 

The data archive wizard does not handle inventory transactions in companies that manage a non-perpetual inventory system together with the purchase accounts posting system (on the _Administration System Initialization Company Details Basic Initialization_ tab, the _Use Perpetual Inventory_ checkbox is not selected and the _Use Purchase Accounts Posting System_ checkbox is selected). 

The data archive wizard run results in the creation of journal entries. To enable the creation of those journal entries, make sure that the default numbering series assigned to _Journal Entries_ has enough free numbers between the _Next Number_ and the _Last Number_ to be used by the data archive journal entries. 

##  Example 

The data archive wizard run is to be activated for the following period: calendar year 2006 and first half of 2007, a total of 18 months. The grouping of the data archive journal entries is set to be per month. It means that a maximum of 18 journal entries are expected to be added to the company database. Looking at the _Document Numbering – Setup_ window ( _Administration System Initialization Document Numbering_ ), the number of the next journal entry is 2589 and the last number in the series assigned to journal entries is 2600: 

**==> picture [400 x 247] intentionally omitted <==**

In this case, there might not be enough numbers available for creating all the data archive journal entries (only 12 numbers are available, while 18 journal entries may be created). Either adjust the last number of 

How to Prepare for and Perform Data Archiving in SAP Business One **How to Prepare for Data Archiving** 

PUBLIC 

**25** 

the series, or set another numbering series with enough numbers available, as the default series for journal entries. 

The data archive wizard applies only for posting periods with the status _Locked_ or _Archived_ . Make sure to complete the _Period-End Closing_ process for all of the posting periods you want to include in the data archive wizard run or in the data archive simulation, and set their status to _Locked_ . 

##  Note 

If the archived period includes posting periods with profit and loss accounts with a balance other than zero, and/or posting periods with a status other than _Locked_ or _Archived_ , the data archive wizard run or simulation fails. 

Back up your company database up to one hour before initiating the data archive wizard run. 

##  Note 

If you initiate the data archive wizard run and SAP Business One detects that no backup has taken place within the last hour, a warning message to that effect appears and the _Next_ button in the data archive wizard is disabled. 

If your company manages a perpetual inventory system, we highly recommend running the inventory valuation inconsistency check. This lets you determine in advance whether it will be necessary to run the inventory valuation utility for the period to be archived before beginning the data archive run. For more information about how to run the inventory valuation inconsistency check, see 1460925 . 

##  Note 

When you initiate the data archive wizard run, SAP Business One checks whether it is necessary to run the inventory valuation utility for the period to be archived. If this is the case, the data archive wizard run is disabled until the inventory valuation utility is run for the relevant period. It is not mandatory to accept the results of the inventory valuation utility to proceed with the data archive wizard run. However, we highly recommend you do so, since a certain amount of data is removed from the database during the data archive run and this may lead to incomplete results on subsequent runs of the inventory valuation utility. 

##  Note 

When you initiate a data archive simulation run, SAP Business One runs the same check. However, if it is required to run the inventory valuation utility for the relevant period and this has not been done, a warning message appears, but the data archive simulation run does not fail. 

Before initiating the data archive wizard run, make sure that no other users are connected to the SAP Business One company database, either by logging on to SAP Business One or by connecting directly through the SAP Business One database server. If additional connected users are detected, the data archive wizard run fails. 

A data archive simulation run can take place while other users are connected to the same SAP Business One company database; however, only one user can initiate the data archive simulation run at a time. Running data archive simulation in parallel on more than one instance of the SAP Business One application or from within a SAP Business One application client is impossible. 

Before initiating the data archive wizard run, make sure to close all open windows in the application. If application windows remain open, a relevant system message appears and the Next button in the data archive 

How to Prepare for and Perform Data Archiving in SAP Business One **How to Prepare for Data Archiving** 

**26** 

PUBLIC 

wizard is disabled. Any add-ons that are active on the SAP Business One client being used for running the data archive wizard run are automatically closed. 

How to Prepare for and Perform Data Archiving in SAP Business One **How to Prepare for Data Archiving** 

PUBLIC **27** 

## **7 Simulating Data Archive Runs** 

## **Prerequisites** 

You have prepared your company database according to the recommendations provided in the How to Prepare for Data Archiving [page 24] chapter. 

## **Context** 

The simulation provides you with a preview of the expected results of the actual data archive wizard run. It enables you to know: 

- The transactions that are expected to be removed 

- The expected reduction in database size 

##  Note 

The data archive wizard contains 14 steps for companies that manage a perpetual inventory system and 15 steps for companies that manage a non-perpetual inventory system and do not use purchase accounting. 

##  Note 

When running a simulation, the process ends at step 10 for companies that manage a perpetual inventory system, and at step 11 for companies that manage a non-perpetual inventory system and do not use purchase accounting. 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC 

**28** 

## **Procedure** 

1. From the SAP Business One _Main Menu_ , choose _Administration Utilities Data Archive Wizard_ . In the _Introduction to Data Archive Wizard_ window, choose the _Next_ button. 

**==> picture [438 x 331] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC 

**29** 

2. The following window provides you with further information about the essence of the data archive methodology. To continue, choose the _Next_ button. 

**==> picture [438 x 331] intentionally omitted <==**

3. In the _Archive Method_ window, you can choose to archive data by financial periods, business partners, or documents. For more information about archiving data by documents, see the patch update for version 10.0 feature package 2305 in Patch Updates [page 7]. Select _Data Archive by Financial Periods_ , and choose 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**30** PUBLIC 

**==> picture [23 x 8] intentionally omitted <==**

**----- Start of picture text -----**<br>
Next .<br>**----- End of picture text -----**<br>


**==> picture [438 x 332] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC 

**31** 

4. In the _Wizard Options_ window, select the _Run Data Archive Simulation_ radio button and choose the _Next_ button. 

**==> picture [438 x 331] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**32** PUBLIC 

5. The _Data Archive Parameters_ window appears. The parameters to be set in this window depend on the company configuration. 

**==> picture [438 x 331] intentionally omitted <==**

|Field|User Action/Description|User Action/Description|
|---|---|---|
|_Archive Period_|The period to be covered by the data archive simulation.||
||In the_To_feld, choose<br>. The_List of Posting Periods_window appears.||
|||Note|
|||You cannot type data into the_To_feld. Setting a period for archiving is possible only by|
|||choosing it from the_List of Posting Periods_window.|
|Only posting periods that are at least two years older than the current date are listed in the|||
|window. Choose the latest posting period to be included in the data archive simulation run.|||
|The date of the last day in the chosen posting period is displayed in the_To_feld.|||
|The “from” date of the archived period is always the frst day of the earliest posting period in|||
|the company database.|||



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **33** 

|Field|User Action/Description|
|---|---|
|_Price Source for_|This section appears only for companies that manage a non-perpetual inventory system and|
|_Inventory Entry_|do not use purchase accounting (the_Use Perpetual Inventory_and_Use Purchase Accounts_|
|_Grouping_|_Posting System_checkboxes are not selected on the<br>_Administration_<br>_System Initialization_|
||_Company Details_<br>_Basic Initialization_<br>tab).|
||In the_Price Source_feld, select the price list to be considered when inventory transactions are|
||grouped.|
||To group items for which price is not defned in the price list selected in the_Price Source_|
||feld, select the_Allow Grouping of Zero Price Items_checkbox. By default, this checkbox is not|
||selected.|
|_Bank Statement_|This section appears only for companies that do not use automatic bank statement processing|
|_Archiving_|(the_Install Bank Statement Processing_checkbox is not selected on the<br>_Administration_|
||_System Initialization_<br>_Company Details_<br>_Basic Initialization_<br>tab), and that have at least|
||one bank statement recorded (in<br>_Banking_<br>_Bank Statements and External Reconciliations_|
||_Process External Bank Statement_<br>).|
||In such companies, the data archive wizard handles automatically reconciled lines in the|
||external bank statements. To enable archiving unreconciled lines in bank statements as well,|
||select the_Allow Archiving of Unreconciled Bank Statement Records_checkbox.|
|_Inventory Valuation_|This section appears only for SAP Business One companies that manage a perpetual inventory|
|_Utility Parameters_|system (the_Use Perpetual Inventory_checkbox is selected on the<br>_Administration_<br>_System_|
||_Initialization_<br>_Company Details_<br>_Basic Initialization_<br>tab).|
||In the_Direct USD Rate_feld, specify the current exchange rate of one US dollar in the compa-|
||ny’s local currency. SAP Business One runs a few checks and validates the inventory value|
||accordingly. Based on the results of the checks, you are notifed if there is a need to run the|
||inventory valuation utility.|



##  Recommendation 

Since only posting periods with the period status _Locked_ or _Archived_ can be included in the data archiving simulation run, we recommend that you add the column _Period Status_ to the _List of Posting_ 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**34** PUBLIC 

_Periods_ window. This way you can tell which of the posting periods are archivable. To do so, perform the following steps: 

1. While the _List of Posting Periods_ window is open, choose in the toolbar. The _List of – Settings_ window appears: 

**==> picture [293 x 263] intentionally omitted <==**

2. The dropdown list of line 3 displays a list of all the columns that can be added to the _List of Posting Periods_ window. Select _Period Status_ and choose _Update_ . Then choose _OK_ . 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **35** 

**==> picture [293 x 305] intentionally omitted <==**

3. To apply the new settings, close the _List of Posting Periods_ window and open it again. 

**==> picture [401 x 223] intentionally omitted <==**

6. After specifying all the relevant details in the _Data Archive Parameters_ window, choose the _Next_ button. This process may take some time, depending on the size of your company database and the overall length of the period included in the data archive simulation run. 

7. If any errors are detected, the _Data Archive Error/Warning Log_ window appears, listing all the errors found and providing warnings and recommendations. The contents of this window can be printed, saved in PDF format, and exported to a Microsoft Excel file. Depending on the severity of the errors found, the _Next_ 

How to Prepare for and Perform Data Archiving in SAP Business One 

**Simulating Data Archive Runs** 

**36** PUBLIC 

button might be disabled. In such a case, you are required to first resolve the errors and then initiate the data archive simulation run again. 

##  Recommendation 

We recommend addressing as many as possible the issues listed in this window, even when only warnings are listed and the _Next_ button is available. 

**==> picture [422 x 320] intentionally omitted <==**

If no errors or warnings are found, the _Data Archive Recommendations_ window appears. 

8. The _Data Archive Recommendations_ window displays the results of the database analysis done by SAP Business One, providing detailed information regarding which transactions can be archived and which cannot. The information in the _Data Archive Recommendations_ window is provided in two levels of details: _Cluster View_ (the default display mode) and _Transactions View_ . After reviewing the recommendations, choose the _Next_ button. 

##  Note 

You can print or print preview the data archive recommendations. In case the list of recommendations is very long, these actions might take some time. If you choose to print the data archive recommendations, it may consume a large amount of paper. 

Following are screen captures and details related to the two display modes mentioned above: 

- Cluster View 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **37** 

**==> picture [421 x 318] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**38** PUBLIC 

|Field|User Action/Description|User Action/Description|
|---|---|---|
|_Group By_|Choose the display mode of the data removal recommendations:||
||•|_Document Cluster_– the default display mode. Each line in the table represents|
|||one cluster. To view the transactions included in a specifc cluster, double-click|
|||the line of the required cluster. The display mode changes to_Transaction View_|
|||and the number of the selected cluster appears in the title. To return to the|
|||_Cluster View_mode, choose the_Back to Cluster View_button.|
||•|_None_– every line in the table displays the details related to a single transaction|
|||or document included in the period defned for the data archive simulation run.|
|_Display_|You|can flter the clusters listed in the table by:|
||•|_All Clusters_– the default option. All the clusters included in the period defned|
|||for the data archive simulation run are listed in the table.|
||•|_Removable Clusters_– only clusters that can be removed are listed in the table.|
||•|_Nonremovable Clusters_– only clusters that cannot be removed from the com-|
|||pany database are listed in the table.|
|_Cluster Status_|Indicates whether a cluster is removable or not:||
|||- the cluster is removable|
|||- the cluster is not removable|
|_Cluster ID_|The number assigned to the cluster during the data archive simulation run. This ID is||
||unique for the specifc run only.||
|_No. of Transactions in_|Indicates how many transactions are included in each cluster. A cluster can include||
|_Cluster_|one|or multiple transactions.|



- Transaction View 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **39** 

**==> picture [421 x 250] intentionally omitted <==**

|Field|User Action/Description|
|---|---|
|_Display_|You can flter the transactions listed in the table by:|
||•<br>_All Transactions_– the default option. All the transactions included in the period de-|
||fned for the data archive simulation run are listed in the table.|
||•<br>_Removable Transactions_– only transactions that can be removed are listed in the|
||table.|
||•<br>_Nonremovable Transactions_– only transactions that cannot be removed from the|
||company database are listed in the table.|
|_Date From … To…_|Appear only when the value in the_Group By_feld is_None_. To display transactions within a|
||specifc date range, specify this range here. To apply the defned range, press TAB.|
|_Trans. Type_|By default, all the transactions included in the period defned for the data archive simula-|
||tion run are displayed. To display transactions of a specifc type only, select the required|
||type from the dropdown list.|
|_Doc. No. From… To…_|Appear only when a specifc transaction type is selected in the_Trans. Type_feld.|
||To display only documents within a specifc number range, specify this range in these|
||felds and press TAB.|



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**40** PUBLIC 

|Field|User Action/Description|
|---|---|
|_Close Transaction_|The column and the button appear only if the following conditions apply:|
|(the column in the|•<br>The value in the_Group By_feld is_None_or a specifc cluster.|
|table)|•<br>The value in the_Display_feld is_Nonremovable Transactions_.|
|_Close Transactions_|•<br>The value in_Trans. Type_is_Sales Quotations_,_Sales Orders_,_Purchase Orders_, or_Service_|
|(the button)|_Calls_.|
||Select the checkboxes for the transactions that you want to close.|
||To close the selected transactions, choose the_Close Transactions_button.|



**==> picture [331 x 244] intentionally omitted <==**

|_Status_|Indicates whether a transaction is removable or not:|
|---|---|
||- the transaction is removable|
||- the transaction is not removable|



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **41** 

|Field|User Action/Description|
|---|---|
|_Doc. No._,_Series_|The number of the document or journal entry and the numbering series used when the<br>document or journal entry was created. To view the document or journal entry, choose<br>.<br>Note<br>For payment wizard runs, both columns are empty.<br>Note<br>For customer equipment cards, the_Doc. No._column includes only the<br>icon that<br>opens the_Customer Equipment Card_window.<br>Note<br>For customer equipment cards, service contracts, sales opportunities, check register,<br>checks for payment, and activities, the_Series_column is empty.|
|_Transact. Type_|The type of the transaction in the line, such as_A/R invoice_,_Incoming Payment_, and so on.<br>Note<br>•<br>_Goods Receipt_represents both goods receipt documents (under<br>_Inventory_<br>_Inventory Transactions_<br>_Goods Receipt_<br>) and receipts from production docu-<br>ments (under<br>_Production_<br>_Receipt from Production_<br>). The_Remarks_column<br>indicates which line refers to goods receipt and which to receipt from production.<br>•<br>_Goods Issue_represents both goods issue documents (under<br>_Inventory_<br>_Inventory Transactions_<br>_Goods Issue_<br>) and issue for production documents<br>(under<br>_Production_<br>_Issue for Production_<br>). The_Remarks_column indicates<br>which line refers to goods issue and which to issue for production.|
|_Date_|Displays the date depending on the transaction type displayed in the line. Mostly it displays<br>the posting date assigned to documents, transactions, and wizard runs. Following are<br>exceptions:<br>Transaction Type<br>Date Displayed<br>_Sales Opportunities_,_Activities_,_Service_<br>_Contracts_<br>_Start Date_<br>_Deposits_<br>_Deposit Date_<br>_Bank Statements_<br>_Statement Date_<br>_Service Calls_<br>_Created On_<br>_Dunning Wizard_<br>_Date of the Dunning Run_<br>_Customer Equipment Cards_<br>N/A – column is empty|



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**42** PUBLIC 

|Field|User Action/Description|User Action/Description|
|---|---|---|
|_Total (LC)_|The total amount of the transaction or document in local currency.||
|||Note|
|||This column is empty for customer equipment cards, goods receipts that represent|
|||receipt from production, and production orders.|



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **43** 

|Field|User Action/Description|User Action/Description|User Action/Description|
|---|---|---|---|
|_Reason for error_|Relevant only for nonremovable transactions. Indicates why a transaction is nonremovable.|||
||The possible reasons for errors are:|||
||•|_Nonremovable Document_– the transaction or document in the line does not comply||
|||with the conditions required for archiving. For more information, see theWhat Data is||
|||Archived? [page 16]chapter.||
||||Example|
||||A sales quotation with the status_Open_is marked as_Nonremovable Document_,|
||||since only_Closed_or_Canceled_sales quotations can be archived.|
||•|_Connected to nonremovable document_– the transaction or document in the line is||
|||linked to at least one transaction or document that does not comply with the condi-||
|||tions required for archiving.||



##  Example 

A delivery with the status _Closed_ that is fully copied to an A/R invoice is nonremovable since the A/R invoice is only partially paid. 

- _Document and connected documents are not removable_ – the transaction or document in the line does not comply with the conditions required for archiving, and neither does at least one document or transaction that is linked to it. 

##  Example 

Sales order no. 2 is partially (and therefore still in status _Open_ and cannot be removed) copied to delivery no. 5, which has the status _Open_ (and therefore cannot be removed). 

To further investigate the reasons for a specific error, right-click the line of the required transaction, and choose _Connected Documents_ . 

The _Connected Documents_ window appears: 

**==> picture [331 x 191] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**44** PUBLIC 

|Field|User Action/Description|
|---|---|
||In the_Display_dropdown menu, select one of the following options:|
||•<br>_All Documents_– displays all the documents that are connected to the selected trans-|
||action.|
||•<br>_Within Archiving Date Range_– displays only the documents connected to the selected|
||transaction that are created within the date range of the archived period.|
||•<br>_Outside Archiving Date Range_- displays only the documents connected to the se-|
||lected transaction that are created outside the date range of the archived period.|
|_Cluster_|The cluster ID to which the transaction or document belongs. The cluster ID is unique for|
||the specifc run, so a specifc transaction may be included with a diferent ID in a cluster|
||when the data archive simulation run is on a diferent period.|
|_Remarks_|Displays the text entered in the_Journal Remark_feld in the document. Following are the|
||exceptions:|
||•<br>For payment wizard runs – displays the payment run name|
||•<br>For customer equipment cards – displays the serial number|



9. In the _Journal Entry Compression Rules_ window, set the parameters according to which SAP Business One creates the compressed journal entries that represent the data to be archived. Choose the _Next_ button. 

**==> picture [438 x 331] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **45** 

|Field|User Action/Description|User Action/Description|
|---|---|---|
|_Group by Period_|Defne whether to create one journal entry for every posting period, subperiod, or month.||
|_Length_|||
|_Group by Project_|Groups together journal entry lines that are assigned to the same project.||
|_Group by Proft Center_|Groups together journal entry lines that are assigned to the same proft center.||
|_Reference 1_,_Reference_|Defne the values to appear in the_Reference 1_and_Reference 2_felds in the data archive journal||
|_2_<br>entries.|||
|||Note|
|||Since the data archive simulation tool does not create any data archive journal entry, you|
|||can leave those felds empty while running the data archive simulation.|
|_Journal Remarks_|Enter remarks of up to 50 characters to be added to the data archive journal entries. If you||
||leave this feld empty, the following text is assigned by default:`Data Archive – <last`||
||`date of archived period>`.||
|||Example|
|||In the_Archive Period To_feld (in step no. 5) you have selected the posting period 2007-11.|
|||The default text in the_Journal Remarks_feld is:`Data Archive – 30.11.2007`.|



##  Note 

Step no. 10 is relevant only for companies that manage a non-perpetual inventory system and do not use purchase accounting (the _Use Perpetual Inventory_ and _Use Purchase Accounts Posting System_ checkboxes are not selected on the _Administration System Initialization Company Details Basic Initialization_ tab). 

10. The _Inventory Entry Compression Rules_ window appears. If none of the inventory transactions within the archived period is removable, the window is displayed in read-only mode, and a pertinent error message appears. You can continue by choosing the _Next_ button. Otherwise, specify the required parameters and choose the _Next_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**46** PUBLIC 

**==> picture [434 x 327] intentionally omitted <==**

|Field|User Action/Description|
|---|---|
|_Price Source_|Select the price list according to which the values of the data archive inventory|
|entries are calculated. The available pricelists are the ones defned by the user in||
||_Inventory_<br>_Price Lists_<br>_Price Lists_<br>window, and the_Last Evaluated Price_|
|price list.||
|_Allow Grouping of Zero Price Items_|Creates a data archive inventory entry for items for which a price is not defned in|
|the selected price list.||
|_Reference 1_,_Reference 2_|Specify references 1 and 2 to be recorded in the respective felds of the data|
||archive inventory entry. Each reference can contain up to 11 characters.|
|_Journal Remarks_|Enter remarks of up to 254 characters to be added to the data archive inventory|
||entries. If you leave this feld empty, the following text is assigned by default:`Data`|
||`Archive – <last date of archived period>`.|
||Example|
||In the_Archive Period To_feld (in step no. 5) you have selected the posting pe-|
||riod 2007-11. The default text in the_Journal Remarks_feld is:`Data Archive`|
||`– 30.11.2007`.|



How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

PUBLIC **47** 

11. The _Data Archive Expected Results_ window appears, providing you with details regarding the expected results of the data archive wizard run if you were to run it right after the data archive simulation run takes place, and with the same parameters selected. 

**==> picture [438 x 331] intentionally omitted <==**

|Field|User Action/Description|
|---|---|
|_Expected Reduction in Database_|The number of megabytes expected to be removed from your company database|
|_Size (MB)_|if you initiate the data archive wizard run with the same parameters as defned for|
||the data archive simulation run.|
|_Expected Reduction in Database_|The relative portion to be reduced from your company database size in percen-|
|_Size (%)_|tages, if you initiate the data archive wizard run with the same parameters as|
||defned for the data archive simulation run.|
|_Expected Number of Removed_|The number of transactions expected to be removed from your company database|
|_Transactions_|if you initiate the data archive wizard run with the same parameters as defned for|
||the data archive simulation run.|
|_Expected Reduction in Transaction_|The relative portion of the transactions to be removed from your company data-|
|_Size (%)_|base, in percentages, if you initiate the data archive wizard run with the same|
||parameters as defned for the data archive simulation run.|
|_Expected Reduction in Transaction_|The relative portion of the transactions to be removed from your company data-|
|_Size within Archived Range (%)_|base, within the archived period, in percentages, if you initiate the data archive|
||wizard run with the same parameters as defned for the data archive simulation|
||run.|



12. To conclude the data archive simulation run, choose the _Finish_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Simulating Data Archive Runs** 

**48** PUBLIC 

## **8 Archiving Data** 

## **Prerequisites** 

- You have made all the relevant preparations as detailed in the How to Prepare for Data Archiving [page 24] chapter. 

- There are no other users logged on to the company database. 

- You have run the data archive simulation for the period you intend to archive. 

## **Context** 

This chapter walks you through the data archive run. At the end of the process, a certain amount of data is permanently removed from the company database. 

## **Procedure** 

1. From the SAP Business One _Main Menu_ , choose _Administration Utilities Data Archive Wizard_ . In the _Introduction to Data Archive Wizard_ window, choose the _Next_ button. 

Another introductory window, providing an example of a document cluster, appears. Choose the _Next_ button. 

2. In the _Archive Method_ window, you can choose to archive data by financial periods, business partners, or documents. For more information about archiving data by documents, see the patch update for version 10.0 feature package 2305 in Patch Updates [page 7]. Select _Data Archive by Financial Periods_ , and choose _Next_ . 

3. In the _Wizard Options_ window, select the _Start New Data Archive Run_ radio button and choose the _Next_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

PUBLIC **49** 

**==> picture [438 x 332] intentionally omitted <==**

4. In the _Data Archive Parameters_ window, specify the period to be archived and additional details related to the data archive wizard run. 

##  Note 

Some of the sections appearing in this window are dependent on the company configuration and, therefore, may vary from one company to another. 

The table below provides descriptions only for the parameters that are exclusive to the data archive wizard run. For information about the rest of the parameters in this window, see step no. 5 in the Simulating Data Archive Runs [page 28] chapter. 

How to Prepare for and Perform Data Archiving in SAP Business One 

**Archiving Data** 

**50** PUBLIC 

**==> picture [438 x 332] intentionally omitted <==**

Field User Action/Description _Data Archive Run Name_ By default, SAP Business One assigns to each data archive wizard run a unique name based on the following formulation: `<data archive wizard run sequential no.>_<run date>` You can specify a different name if needed. It must be unique and can consist of up to 100 alphanumeric characters.  Example A company performed the data archive wizard run for the fourth time on December 1[st] 2009. SAP Business One assigned to it by default the following name: `4_20091201` . _Read Only DB Backup Path_ Displays the path to the directory where the backup file for the read-only database is stored. By default, this is the same directory that is used for the regular backups on the MS SQL server. 

5. If any errors are detected, the _Data Archive Error/Warning Log_ window appears, listing all the errors found and providing warnings and recommendations. The contents of this window can be printed, saved in PDF format, and exported to a Microsoft Excel file. Depending on the severity of the errors found, the _Next_ 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

PUBLIC **51** 

button might be disabled. In such a case, you are required to first resolve the errors and then initiate the data archive wizard run again. If no errors are found, the _Data Archive Recommendations_ window appears. 

6. The _Data Archive Recommendations_ window displays the results of the database analysis done by SAP Business One, providing detailed information regarding which data items can be archived and which cannot. The information in the _Data Archive Recommendations_ window is provided in two levels of details: _Cluster View_ (the default display mode) and _Transactions View_ . 

7. After reviewing the recommendations, decide whether you would like to fine tune and make some more adjustments (to optimize the results). To continue, choose the _Next_ button. 

##  Note 

If none of the transactions included in the data archive wizard run can be removed, the _Next_ button is disabled. 

8. In the _Journal Entry Compression Rules_ window, define the parameters according to which the data archive journal entries will be created. To continue, choose the _Next_ button. 

##  Note 

The next step is relevant only for companies that manage a non-perpetual inventory system and do not use purchase accounting (the _Use Perpetual Inventory_ and _Use Purchase Accounts Posting System_ checkboxes are not selected on the _Administration System Initialization Company Details Basic Initialization_ tab). 

9. The _Inventory Entry Compression Rules_ window appears. If none of the inventory transactions within the archived period is removable, the window is displayed in read-only mode, and a pertinent error message appears. You can continue by choosing the _Next_ button; otherwise, specify the required parameters and choose the _Next_ button. 

10. The _Data Archive Expected Results_ window provides you with an overview about the expected results of the data archive wizard run. If, based on the information provided in this window, you would like to make some more adjustments to your company database in order to optimize the potential results, choose the _Cancel_ button. To continue with the data archive wizard run, choose the _Next_ button. 

11. The _Progress Bar_ window appears, providing you with an overview about the upcoming process. To continue, choose the _Next_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

**52** PUBLIC 

**==> picture [438 x 331] intentionally omitted <==**

12. A progress bar appears indicating the progress made in the process and displaying icons indicating the current step of the process. 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

PUBLIC **53** 

**==> picture [438 x 331] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

**54** PUBLIC 

|Action|Description|Description|
|---|---|---|
|_1. Creating a read-only_|SAP Business One creates a read-only company database that is a snapshot of the||
|_backup database_|company database as it is right before any data item is removed from the database.||
||The read-only database backup is automatically saved into the backup path defned for||
||the regular backups of SAP Business One.||
||You can identify it according to its name:||
||`<Database Name>_<No. of Data Archive Wizard`||
||`Run>_ReadOnly.bak`||
|||Example|
|||The name of a company database is B1Company, and a data archive wizard run was|
|||performed on the company just once. The read-only database backup fle name is:|
|||`B1Company_1_ReadOnly`|



|||Note|
|---|---|---|
|||The read-only company database is for review purposes only. If, for some reason,|
|||it is required to roll back and work with the company database as it was before the|
|||data archive run was performed, restore the latest backup created before the data|
|||archive wizard run was initiated.|
|_2. Removing transactional_|SAP Business One removes from the company database all transactions that were||
|_data_|identifed as removable.||
|_3. Creating data archive_|SAP Business One creates new journal entries to refect the values of the removed||
|_entries_<br>transactions. The data archive journal entries are created according to the defnitions|||
|you made in the_Journal Entry Compression Rules_window.|||
|_4. Shrinking database_and_5._|The sizes of the database and the log fles are reduced as a result of the data removal.||
|_Shrinking database log fles_|||
|_6. Re-indexing database_|The database is re-indexed to improve performance.||



13. Once the process is completed, the _Data Archive Summary_ window appears, providing you with the details related to the actual database size reduction, and more. To complete the data archiving process, choose the _Close_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

PUBLIC **55** 

**==> picture [438 x 331] intentionally omitted <==**

##  Note 

Any errors detected during the data archive wizard run are listed in step number 14, which then becomes the last step in the wizard. 

## **Results** 

In addition to a reduction in database size and the creation of the data archive journal entries and inventory entries, the status of the posting periods that were included in the data archive wizard run is updated to _Archived_ . 

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

**56** PUBLIC 

**==> picture [455 x 360] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Archiving Data** 

PUBLIC **57** 

## **9 Loading Saved Data Archive runs** 

## **Context** 

If you need to track documents and to check whether and when they were archived, you can load each of the data archive wizard runs. 

The following procedure describes the data available in the saved data archive runs. 

## **Procedure** 

1. From the SAP Business One _Main Menu_ , choose _Administration Utilities Data Archive Wizard_ . In the _Introduction to Data Archive Wizard_ window, choose the _Next_ button. 

Another introductory window, providing an example of a document cluster, appears. Choose the _Next_ button. 

2. In the _Archive Method_ window, select one of the options, and choose _Next_ . 

3. In the _Wizard Options_ window, select the _Load Saved Data Archive Run_ radio button. A table listing all the data archive wizard runs that were executed appears. 

Select the row of the data archive wizard run you would like to load, and choose the _Next_ button. 

**==> picture [438 x 247] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Loading Saved Data Archive runs** 

**58** PUBLIC 

|Field|User Action/Description|
|---|---|
|_Data Archive Run Name_|Displays the names of the executed data archive runs. To browse to the read-only|
||company database created right before the transactions were removed from the|
||database, choose<br>in this column.|
||Note|
||Browsing through a read-only company database is possible only if the rele-|
||vant read-only backup fle is restored and placed on the SAP Business One|
||database server. For detailed information see theRestoring the Read-Only|
||Company Database [page 60]chapter.|
|_Run Date_|The date on which the data archive run took place.|
|_To Date_|The last day of the archived period in a particular data archive run.|
|_DB Reduc. (%)_|Displays the percentage of the removed data compared to the original size of the|
||database.|
|_DB Reduc. (MB)_|Displays the number of megabytes that were removed from the company data-|
||base within the data archive wizard run.|
|_Tran. Reduc (%)_|Displays the percentage of the transactions that were removed compared to the|
||number of transactions in the company database.|
|_Tran. Reduc._|The number of transactions that were removed from the database.|
|_Tran. Arc Red.(%)_|The percentage of removed transactions out of the total transactions in the ar-|
||chived period.|



4. The _Data Archive Parameters_ window appears in read-only mode, displaying the parameters specified for the selected data archive run. To continue, choose the _Next_ button. 

5. The _Data Archive Recommendations_ window appears listing all the clusters that were archived. You can switch between _Cluster View_ (the default display mode) and _Transactions View_ , and filter the transactions by posting date and transaction types. To continue, choose the _Next_ button. 

6. The _Journal Entry Compression Rules_ window appears in read-only mode. Here you can check the grouping defined for the data archive journal entries and the references and journal remarks. You cannot make any updates in this window. To continue, choose the _Next_ button. 

##  Note 

The next step is relevant only for companies that manage a non-perpetual inventory system and do not use purchase accounting (the _Use Perpetual Inventory_ and _Use Purchase Accounts Posting System_ checkboxes are not selected on the _Administration System Initialization Company Details Basic Initialization_ tab). 

7. The _Inventory Entry Compression Rules_ window appears in read-only mode. Here you can view the price list that was specified as the price source, as well as other parameters specified for the data archive inventory entry. To continue, choose the _Next_ button. 

8. The _Data Archive Summary_ window appears. It displays the results of the data archive run. The numbers provided here are the same numbers as those displayed in the _Wizard Options_ window after you have selected the _Load Saved Data Archive Run_ radio button. 

9. To conclude the review, choose the _Close_ button. 

How to Prepare for and Perform Data Archiving in SAP Business One **Loading Saved Data Archive runs** 

PUBLIC **59** 

## **10 Restoring the Read-Only Company Database** 

## **Context** 

Circumstances may require you to examine the original company database, right before the data removal of a specific data archive wizard run took place. You may need to: 

- Analyze historical transactions, such as sales analysis reports, profit and loss statements, and so on. 

- Locate historical invoices following a dispute with a customer regarding an old debt. 

- Locate a serial number transaction regarding the warranty of an item. 

- Supply tax officials with historical data, such as VAT declarations, transactional information, inventory value reports, and so on when the company is going through an audit. 

For the reasons listed above, SAP Business One automatically creates a backup of the company database during the data archive wizard run. 

The backup file reflects the status of the company database right before transactions are permanently removed. This backup file is assigned automatically with the following name: `<Database Name>_<No. of Data Archive Wizard Run>_ReadOnly.bak` . It is saved automatically in the backup directory defined for the regular database backups of SAP Business One. The path to the default backup directory is displayed in the _Data Archive Parameters_ window, in the _Read Only DB Backup Path_ field. 

##  Example 

A database name is: Evergreen_inc. Once the first data archive wizard run takes place, the read-only backup file created automatically by SAP Business One is: `Evergreen_inc_1_ReadOnly.bak` . 

Unlike with the backup files created on a regular basis for the company database, when you restore a backup file created by the data archive wizard run, the SAP Business One company that appears in the _Choose Company_ window is in a read-only mode. 

You can only generate reports, view documents, and print them. You cannot update or change the data itself. 

## **Procedure** 

The complete instructions for restoring a company database from a backup file are available in the _Administrator Guide_ , in the section: _Restoring Data When msdb Is Unavailable_ . 

## **Results** 

- The read-only company database is displayed in the _Choose Company_ window and can be accessed like any other company, but it cannot be updated or changed. 

How to Prepare for and Perform Data Archiving in SAP Business One **Restoring the Read-Only Company Database** 

**60** 

PUBLIC 

##  Note 

If you have upgraded SAP Business One and the read-only company database is an older version than the current one, you can upgrade the read-only company database according to the instructions provided in the _Upgrade Process_ chapter in the _Administrator Guide_ . 

- When you enter a read-only company, the phrase _Archived Database_ is added to all window titles. For example: 

**==> picture [233 x 402] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Restoring the Read-Only Company Database** 

PUBLIC **61** 

## **11 Searching Transactions across Multiple Data Archive Runs** 

## **Context** 

If you need to track a specific document that was archived, and the company has already performed multiple data archive wizard runs, you can search simultaneously for the required document across all the data archive wizard runs. 

## **Procedure** 

1. From the SAP Business One _Main Menu_ , choose _Administration Utilities Data Archive Wizard_ . In the _Introduction to Data Archive Wizard_ window, choose the _Next_ button. 

Another introductory window, providing an example of a document cluster, appears. Choose the _Next_ button. 

2. In the _Archive Method_ window, select _Data Archive by Financial Periods_ or _Data Archive by Business Partners_ , and choose _Next_ . 

3. In the _Wizard Options_ window, select the _Search Across Data Archive Runs_ radio button and choose the _Next_ button. 

**==> picture [438 x 271] intentionally omitted <==**

How to Prepare for and Perform Data Archiving in SAP Business One **Searching Transactions across Multiple Data Archive Runs** 

**62** PUBLIC 

The _Data Archive Recommendations_ window appears in read-only mode. It displays by default all the removable clusters from all the data archive wizard runs that were performed in the company database. 

**==> picture [438 x 331] intentionally omitted <==**

4. To search for a specific document, switch to _Transaction View_ , and filter the list according to the required transaction type, document number, and/or date range. The line (or lines) with the required document is displayed: 

How to Prepare for and Perform Data Archiving in SAP Business One **Searching Transactions across Multiple Data Archive Runs** 

PUBLIC **63** 

**==> picture [438 x 331] intentionally omitted <==**

To view the required document, choose either in the _Data Archive Run Name_ column or in the _Doc. No._ column. If the read-only database of the particular data archive wizard run has been restored and is located on the SAP Business One database server, another instance of the SAP Business One application is opened and connected to the read-only database, enabling you to browse through. If the read-only database is not available, an error message appears. 

How to Prepare for and Perform Data Archiving in SAP Business One **Searching Transactions across Multiple Data Archive Runs** 

**64** PUBLIC 

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

How to Prepare for and Perform Data Archiving in SAP Business One **Important Disclaimers and Legal Information** 

PUBLIC **65** 

www.sap.com/contactsap 

© 2026 SAP SE or an SAP affiliate company. All rights reserved. 

No part of this publication may be reproduced or transmitted in any form or for any purpose without the express permission of SAP SE or an SAP affiliate company. The information contained herein may be changed without prior notice. 

Some software products marketed by SAP SE and its distributors contain proprietary software components of other software vendors. National product specifications may vary. 

These materials are provided by SAP SE or an SAP affiliate company for informational purposes only, without representation or warranty of any kind, and SAP or its affiliated companies shall not be liable for errors or omissions with respect to the materials. The only warranties for SAP or SAP affiliate company products and services are those that are set forth in the express warranty statements accompanying such products and services, if any. Nothing herein should be construed as constituting an additional warranty. 

SAP and other SAP products and services mentioned herein as well as their respective logos are trademarks or registered trademarks of SAP SE (or an SAP affiliate company) in Germany and other countries. All other product and service names mentioned are the trademarks of their respective companies. 

Please see https://www.sap.com/about/legal/trademark.html for additional trademark information and notices. 

**==> picture [58 x 30] intentionally omitted <==**

