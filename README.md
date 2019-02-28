# Coding Takehome 

## Rules 
- The solution should be written in Python
- You may use any online non-human resource including stackoverflow, tutorials, documentation, open source libraries, etc
- However, you should not use any library or function that specializes in anomaly detection

## transactions.json
You have been provided a data file `transactions.json` which contains a list of transactions, each transaction containing 
- a date (format: `mm-dd-yyyy`), 
- a string description
- an amount
The list of transactions are already sorted by date (earliest date first).

## Task 1: Finding Sequences of Transactions
Create a function which analyzes the transactions and identify groups of transactions that are part of a sequence. Transactions are part of a sequence if: 
1. The transaction descriptions are similar 

AND

2. The timing of the transactions occur in regular intervals. Small deviations in the timing of the transactions by 2-3 days should not break a sequence. 

3. There are at least 4 transactions in the sequence. 

Note that it is not necessary for a transaction to be part of a sequence. No transaction should be part of more than 1 sequence. 

## Task 2: Save the transactions and sequence data in a data structure
The data structure can be of your choosing. A requirement of this data structure is that for any given transaction, the data structure should be able to quickly lookup the other transactions that are part of the same sequence, if any.

## Task 3: Detect Anomalies (Bonus)
For each found sequence of transactions, attempt to detect "anomolies". 
An anomaly is a transaction in the sequence has an amount that is unusual given the amounts of the other transactions in the same sequence.
Note that not all sequences have an anomally. 

## Submitting your answer: 
To submit your answer, send the files or a link to the repository to jie@gourmetgrowth.com. 



