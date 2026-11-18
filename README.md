🏦 Banking Transaction Analysis Using MySQL
👨‍💻 Author

Vignesh

📌 Project Overview

This project focuses on analyzing banking customer accounts and transaction data using MySQL.

The project demonstrates practical SQL concepts such as INNER JOIN, LEFT JOIN, GROUP BY, HAVING, aggregate functions, and filtering conditions to solve real-world banking business problems.

The database contains three relational tables: customers, accounts, and transactions.

🗄️ Database Structure
1. customerr

Stores customer information.

Column Name	Data Type
customer_id	INT (Primary Key)
customer_name	VARCHAR(100)
age	INT
city	VARCHAR(50)
2. accountss

Stores customer account details.

Column Name	Data Type
account_id	INT (Primary Key)
customer_id	INT (Foreign Key)
account_type	VARCHAR(30)
balance	DECIMAL(12,2)
account_status	VARCHAR(20)
3. transactionss

Stores banking transaction details.

Column Name	Data Type
transaction_id	INT (Primary Key)
account_id	INT (Foreign Key)
transaction_date	DATETIME
amount	DECIMAL(12,2)
transaction_type	VARCHAR(30)
status	VARCHAR(20)
location	VARCHAR(50)
receiver_account	INT
🛠️ Technologies Used
MySQL
SQL
MySQL Workbench
📚 SQL Concepts Covered
INNER JOIN
LEFT JOIN
WHERE
GROUP BY
HAVING
ORDER BY
COUNT()
SUM()
Aggregate Functions
Primary Key
Foreign Key
NULL Handling
📊 SQL Queries and Business Problems

This project covers 14 SQL queries based on real-world banking scenarios.

1. Display Customer Name and Account Balance

Concept: INNER JOIN

Displays customer names along with their account balances.

2. Find Customers with Failed Transactions

Concept: INNER JOIN, WHERE

Identifies customers who have failed transactions.

3. Find Customers Who Made Transactions Above ₹1,00,000

Concept: INNER JOIN, WHERE

Displays customer name, account ID, transaction ID, and transaction amount.

4. Find Customers with More Than 5 Successful Transactions

Concept: COUNT(), GROUP BY, HAVING

Displays customer names and their total successful transaction counts.

5. Find Customers Whose Total Failed Transaction Amount Exceeds ₹30,000

Concept: SUM(), GROUP BY, HAVING

Identifies customers whose total failed transaction amount exceeds ₹30,000.

6. Find Accounts Where Successful Withdrawal Amount Exceeds ₹1,00,000

Concept: SUM(), GROUP BY, HAVING

Identifies accounts with total successful withdrawal amounts greater than ₹1,00,000.

7. Display Customers Whose Total Transaction Amount Exceeds ₹2,00,000

Concept: SUM(), COUNT(), GROUP BY, HAVING

Displays customer name, account type, total transaction amount, and transaction count.

8. Find Customers Who Do Not Have Any Accounts

Concept: LEFT JOIN, IS NULL

Identifies customers who do not have an account.

9. Find Accounts That Have Never Made Any Transactions

Concept: LEFT JOIN, IS NULL

Identifies accounts without any transaction records.

10. Find Customers Who Have Accounts but No Successful Transactions

Concept: INNER JOIN, LEFT JOIN, IS NULL

Identifies customers who have accounts but have never completed a successful transaction.

11. Display All Accounts and Their Transaction Counts

Concept: LEFT JOIN, COUNT(), GROUP BY

Displays all accounts, including accounts with zero transactions.

12. Find Customers Who Have Never Made a Failed Transaction

Concept: LEFT JOIN, IS NULL

Identifies customers who do not have any failed transactions.

13. Find Accounts That Have Made More Than 2 Transactions

Concept: GROUP BY, COUNT(), HAVING

Identifies accounts with more than two transactions.

14. Find Repeated Transfers to the Same Receiver

Concept: GROUP BY, HAVING, COUNT()

Identifies accounts that transferred the same amount to the same receiver more than once.

📁 Project Structure
text
Banking-Transaction-Analysis/
│
├── README.md
│
└── banking_analysis.sql

🚀 How to Run This Project
Install MySQL Server or MySQL Workbench.
Create a new SQL file.
Execute the CREATE TABLE statements.
Insert the customer, account, and transaction records.
Run the SQL queries one by one.
Analyze the query results.
🎯 Key Learning Outcomes

Through this project, I gained practical experience in:

Understanding relationships between multiple database tables.
Performing INNER JOIN and LEFT JOIN operations.
Analyzing successful and failed transactions.
Identifying high-value transactions.
Using aggregate functions such as SUM() and COUNT().
Filtering grouped data using HAVING.
Identifying customers without accounts.
Finding accounts without transactions.
Detecting repeated banking transactions.
Solving real-world business problems using SQL.
💡 Conclusion

This Banking Transaction Analysis project helped me strengthen my SQL skills through practical business scenarios.

I gained hands-on experience in joining multiple tables, analyzing transaction data, applying aggregate functions, and extracting meaningful insights from relational databases.

This project is part of my learning journey toward becoming a Data Analyst.

⭐ If you find this project useful, feel free to explore and share your feedback!

Created by Vignesh | MySQL Project# SQL
SQL Description
