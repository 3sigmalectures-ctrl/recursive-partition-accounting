Repository Contents

1. Closed-Flow Accounting Spreadsheet [single-table-double-entry-accounting_V10.xlsx]
– implementation of the transaction-matrix accounting framework described in the accompanying paper.

2. LAMBDA (Part 1: Concepts & Context) 
– introduction to spreadsheet functional programming and the theoretical foundations of LAMBDA functions.  

3. Practical LAMBDA Programming (Part 2: Applications & Practice) 
– practical guide to LET, LAMBDA, MAP, REDUCE, SCAN, recursion, and function-library design patterns used in the spreadsheet implementation.  

Together these materials document the computational architecture underlying the spreadsheet implementation of the closed-flow accounting framework.


Quick Start

This workbook demonstrates a multiperiod accounting system represented in a single transaction table. From the transaction history, the workbook automatically generates:

* Account Positions
* Income Statements
* Intra-Period Balance Sheets
* End-of-Period Balance Sheets

The workbook permits financial statements to be generated at any arbitrary transaction point rather than only at predefined reporting dates.

Getting Started

1. Open the DOUBLE-ENTRY-SYSTEM sheet.
2. Locate the Select Report column.
3. Select a reporting date (for example, m1.w2).
4. Review the automatically generated:
    * Account Positions
    * Income Statement
    * Balance Sheet (Intra-Period or End-of-Period)
5. Repeat for other reporting dates to observe how financial statements evolve through time.

⸻

Sheet Guide

ACC SYSTEM SPEC.

Describes the economic scenario used in the example.

CHART-OF-ACCOUNTS

Defines the account structure used throughout the workbook.

SINGLE-ENTRY-SYSTEM

Single-entry representation of the transaction matrix.

DOUBLE-ENTRY-SYSTEM

Double-entry representation of the transaction matrix.

JOURNAL

Traditional journal view of the double-entry transactions.

LEDGER

Traditional ledger view of the double-entry ledger of accounts.

⸻

Important Note

Reports may be generated at any transaction point. Intra-period reports generally display current-period income and expense balances, while end-of-period reports reflect the effects of the closing process.

Because closing entries transfer income and expense balances to the Capital account, the Income Statement associated with an end-of-period report will generally be zero. To view the Income Statement for a particular period, select the report immediately preceding the closing transaction.

This behavior is common to conventional accounting systems and is not unique to the framework presented in this workbook.

The workbook permits financial statements to be generated at any arbitrary transaction point rather than only at predefined reporting dates.

One small improvement: I would change “arbitrary transaction point” to “arbitrary transaction date or transaction number” if the report selector is actually tied to individual transactions. Readers tend to understand that wording more quickly.
