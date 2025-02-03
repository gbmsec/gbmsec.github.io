
## Business requirement
BCS should have a system in place to reconcile cash transfers with different counterparties on a daily basis. 

Description on the field mapping:


* Task 1070 recon with EURCL file. 250



Transfer Report Reconciliation in Calypso is a customized solution based on a comparison of two sets of cash transfer parameters extracted from the database tables. One set is the result of downloading trades from external Transfer report (ccp, exchange or brokerage report, further in the text – Agent Report) to custom tables. The second set is the Transfer Report from the regular Calypso database structure. Trade Reconciliation is carried out for a certain date, called Recon Date. Recon Date is not a trade parameter. Recon Date corresponds to Report Date of Agent Report and from Calypso side Recon Date is mapped to Settle Date per unique ISIN.

As a result of reconciliation a set of data is formed in the custom table showing the results for each incoming and outcoming Trindicating the reconciliation status:


*  **MATCHED**  – transfer amount was found in Calypso corresponding to the trade in the Agent Report and the values of all compared trade parameters were matched;
*  **UNMATCHED**  – transfer amount was found in Calypso corresponding to the trade in the Agent Report and the value of at least one of the compared parameters was not match;
*  **ALLEGED**  – transfer amount was not found in Calypso corresponding to the trade in the Agent Report;
*  **MISSING**  – there is a Calypso transfer amount which is missing in the Agent Report.

The Recon report in Calypso allows users to view the results and record the Reconciliation Protocol.


## Schedule task description and logic
The Scheduled Task is running automatically and searching for the new statements for reconciliation (task starts at 12:00). In accordance with the logic provided task in looking into a folder for third parties statement. Additionally task can be Run by the user at any given time, please follow the process below.

The task names are as follows:


* BCSRU = ‘BCS_RECON_TRANSFER_EUROCLEAR’

User should go to Calypso ‘Shceduled Task’.

![](images/storage/image2021-7-22_10-32-41.png)

In the ‘Shceduled Task’ User should search for ‘BCS_RECON_TRANSFER_EUROCLEAR’ and double click on it to see the ‘Shceduled Task Definition’ window.

![](images/storage/image2021-7-22_10-33-21.png)


### Main task parameters

1. Path to files:where files from Agent Report should be saved for reconciliation purposes

![](images/storage/image2021-7-22_10-33-54.png)

After all action above are performed, User should run the Task and check the results.

![](images/storage/image2021-7-22_10-34-26.png)



The next step is to open the newly added tab in Calypso (see below) Reports -  **Recon Transfer Report** 

![](images/storage/image2021-7-22_10-35-3.png)



The next step is to choose GL Account Name, Currency and period for which the reconciliation logic will run.

![](images/storage/image2021-7-22_10-35-26.png)

Finally data will appear on the table and the user will be able to see if the transfer amount is reconciled.

![](images/storage/image2021-7-22_10-35-49.png)


## Transfer Report Reconciliation Stages
There are three main stages of Trade Reconciliation process:


* Preparation of data for reconciliation
* Reconciliation and recording of results to the database
* Analysis of results and recording of Reconciliation Protocol.


### Stage 1. Preparation of data for reconciliation
Agent Report delivery and transformationReports from different Agents are received by the Firm through various communication channels (e-mail, file exchange, message queue) in heterogeneous formats (txt, xml, csv, xls. pdf). The mechanism for loading data to reconcile trades in Calypso BCS_LoadReconReportEngine expects data in a single csv format in \\fs\Calypso.Prod.Import\TranferReport folder. Agent Report translation to a common format and location of resulting csv files with the transfer data in the Calypso folder \\fs\Calypso.Prod.Import\TradeReport is made by ESB adapters.  To do this the Agent Report being received from external source is fed to an appropriate ESB adapter's working folder \\fs\ESB.AgentStatements.Prod\<Agent>\ **TranferReport** .

Data from EURCL is received in pdf format and transformed into a csv

![](images/storage/image2021-7-22_10-39-27.png)



The csv results extracted from EURCL statement



| Statement Firm |  ACCOUNT NUMBER | STATEMENT DATE | ISIN | INCOMEPAYABLEREPORT | CURRENCY | RELATED MONEY AMOUNT - TO YOUR DEBIT + TO YOUR CREDIT | 
|  --- |  --- |  --- |  --- |  --- |  --- |  --- | 
| varchar(50) | varchar2(255) | datetime | varchar2(12) | varchar2(50) | Three-characterISO 4217Currency Code | number | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | CH0044328745 |  | USD | 14,818.08- | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | CH0044328745 |  | USD | 14,890.85 | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | CH0044328745 |  | USD | 14,890.85+ | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | IL0011745804 |  | USD | 87,204.00- | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | IL0011745804 |  | USD | 74,400.00 | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | IL0011745804 |  | USD | 74,400.00+ | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | DE000A1PHFF7 |  | - | - | 
| Euroclear Bank SA/NV 75681 | 75681 | 11.05.2021 | US900123CM05 | coupon | USD | 80,500.00+ | 


## Reconciliation logic for equity like instruments cash transfer to EURCL


Each individual instrument (ISIN) is going to be reconciled against EURCL Statements Of Transactions on a daily basis. The Debit and Credit amounts from EURCL will be mapped to the corresponding fields in Calypso filed ‘Real Cash Amount’. The third party (EURCL) file format is not available, so we will need access to the historic data for testing our parsing logic which is going to be used for generating reconciliation data in the appropriate format. 

![](images/storage/image2021-7-22_10-51-32.png)



The below screenshot is the coupon payments on different ISINs and for different value date


## ![](images/storage/image2021-7-22_10-52-58.png)

Coupon parsing logic


Please note that we were not provided with the EURCL pdf file format and we have the only one report sample. So we have to have access to the historical pdf file to test different scenarios on the coupon and equity like instruments cash transfers.



The logic of parsing Coupon payment is the following: In the first ‘PRINCIPAL AMOUNT OR NUMBER OF SHARES’ column we look for the word COUPON and record all of the provided ISINs and cash amounts. In case where in Calypso the amount is presented in one figure we will sum up the amount in EURCL and add this information to the ‘Recon.Detail’ field of the reconciliation table.


## Trade Report file name convention


<Trade Report file name> = <Agent>_<ProductType>_<Agent Report file name>

For example, as the result of Agent Report processing from the file 20190725-1676-C1676-TRX (L)-5994516823p.xml Calypso will receive two Trade Report files: ABN_EquityBond_20190725-1676-C1676-TRX (L)-5994516823p.csv and ABN_Future_20190725-1676-C1676-TRX (L)-5994516823p.csv.

EURCL_TransferReport_Statements Of Transactions - 75681 - 2021-05-11

‘Statements Of Transactions - 75681 - 2021-05-11’ initial file name


## Account mapping


| Calypso GL Account.Account Name | EURCL account name | Calypso field External Name | 
|  --- |  --- |  --- | 
| BCSUK_EURCL_PROP_ANY_75681 | 75681 | 75681 | 
| BCSUK_EURCL_PROP_ANY_21948 | 21948 | 21948 | 
| BCSUK_EURCL_PROP_ANY_25375 | 25375 | 25375 | 
| BCSUK_EURCL_PROP_ANY_75681-CREST |  |  **Please advise what corresponding account should be used?**  | 
| BCSUK_EURCL_PROP_ANY_75681-DTCUS |  |  **Please advise what corresponding account should be used?**  | 











*****

[[category.storage-team]] 
[[category.confluence]] 
