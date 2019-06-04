# Coding Takehome 

## Rules 
- The solution should be written in Python
- You may use any online non-human resource including stackoverflow, tutorials, documentation, open source libraries, etc
- However, you should not use any library or function that specializes in anomaly detection.

Note: You do not need to provide any frontend interface. We are expecting a purely backend / command line solution. 

## transactions.json
You have been provided a data file `transactions.json` which contains a list of transactions, each transaction containing 
- a date (format: `mm-dd-yyyy`), 
- a string description
- a transaction amount

The list of transactions are already sorted by date (earliest date first).

## Part 1: Finding Sequences of Transactions
Create a function which analyzes the transactions and identify groups of transactions that are part of a sequence. A set of Transactions is considered a *"sequence"* if the following conditions are met: 

1. The transaction descriptions are similar

2. The timing of the transactions occur in regular intervals. Small deviations in the timing of the transactions by 2-3 days should not break a sequence. 

3. There are at list 4 transactions in the set

4. No two transactions in the set are less than 4 days apart. 

*Note: that it is not necessary for a transaction to be part of a sequence.*


## Part 2: Save the transactions and sequence data in a data structure
The data structure can be of your choosing. A requirement of this data structure is that for any given transaction, the data structure should be able to quickly lookup the other transactions that are part of the same sequence, if any. 

Notes: 
- you do not need to provide any frontend interface
- you do not need to write any unit / integration tests

## Submitting your answer: 
To submit your answer, send the files or a link to the repository to jie@gourmetgrowth.com. 



