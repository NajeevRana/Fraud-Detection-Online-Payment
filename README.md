# Fraud-Detection-Online-Payment

We reside in a digital era characterized by an increasing embrace of contemporary technologies, which have significantly streamlined our daily tasks and demonstrated reliability.
In recent years, online payments have emerged as a prominent scenario. A mere click or tap simplifies and expedites our transactions. Despite the evident advantages of online payments, there exists a cohort of fraudulent individuals employing various tactics to exploit unsuspecting individuals and pilfer their funds.
The surge in online payment usage has corresponded with a noteworthy increase in online payment fraud. This surge in fraudulent activity poses a substantial concern, especially for individuals who lack familiarity with current technologies.

**Columns in dataset**
1) step: represents a unit of time where 1 step equals 1 hour
2) type: type of online transaction
3) Amount: the amount of the transaction
4) nameOrig: customer starting the transaction
5) oldbalanceOrg: balance before the transaction
6) newbalanceOrig: balance after the transaction
7) nameDest: recipient of the transaction
8) oldbalanceDest: initial balance of the recipient before the transaction
9) newbalanceDest: the new balance of the recipient after the transaction
10) isFraud: fraud transaction

**Analysis insights**
1. What is the fraud percentage that has happened in the overall transaction?
There have been a total of 8,213 fraudulent transactions, representing approximately 0.13% of the total transactions conducted.

2. At what amount range, fraud has happened?
The fraudulent transaction amounts vary between 1.3 and 3.6 lakh, with the majority falling within the range of 340,000 to 360,000 (3.4 to 3.6 lakh).

3. Were we able to mark the fraud transaction as isFlaggedFraud?
No, Out of a dataset consisting of 63,00,000 records, only 16 were identified as fraud, representing a very low percentage of approximately 0.195% of the total fraudulent transactions.

4. Under which type of transfer payment type fraud has occurred mostly.
Fraudulent activities have exclusively occurred within the cashout and transfer transaction types. Specifically, 0.183% of the total fraud incidents are associated with the cashout mode, while 0.769% are attributed to the transfer mode.

5. Were all the isFlaggedFraud records that are marked as fraud correct?
Yes. All of the 16 transactions that were flagged as fraud are confirmed to be genuine fraud transactions.

6. What is the percentage of incorrectly flagged fraud records?
We've identified approximately 8,197 records erroneously labeled as 0, making up 99.805% of the total flagged fraud records.

**Conclusion**
1. A substantial quantity of records has been incorrectly marked as 0.
2. If we fail to accurately handle this incorrect flagging, it could have significant repercussions in the future, potentially resulting in an increase in the reported percentage of online payment fraud. This concern is particularly pertinent as people increasingly rely on online payment methods nowadays.
3. Typically, fraudsters tend to target amounts within the range of 1-4 lakhs, which undeniably represents a substantial sum.
4. Fraudsters primarily concentrate their efforts on transactions involving cashout and transfer modes.
5. Interestingly, despite the growing prevalence of online payments, incidents of fraud during payment mode transfers are relatively uncommon.
6. It's worth noting that despite their strong positive correlation scores, we haven't extracted a substantial amount of information from the columns pertaining to oldbalanceOrg, newbalanceOrig, nameDest, oldbalanceDest, and newbalanceDest.
