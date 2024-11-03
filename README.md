# Perform-a-SQL-query

## Objective

This lab aims to provide hands-on experience in querying databases using SQL. By utilizing `SELECT`, `FROM`, and `ORDER BY` clauses, learners can effectively retrieve and organize relevant data from a database. This skill is essential for security analysts to investigate security incidents, analyze system logs, and identify potential threats.

## Project description

This project focuses on using SQL queries to retrieve and analyze data from a database. By employing `SELECT` and `FROM` clauses, users can extract specific information from tables. The `ORDER BY` clause is utilized to sort the retrieved data, enabling effective analysis and decision-making. This skill is crucial for security analysts who need to investigate security incidents, identify anomalies, and implement appropriate security measures.

## Skills Learned

* **Basic SQL Queries:** Constructing `SELECT` and `FROM` statements to retrieve specific data from a database.
* **Data Filtering:** Using `WHERE` clauses to filter data based on specific criteria.
* **Data Sorting:** Employing the `ORDER BY` clause to sort query results in ascending or descending order.
* **Database Querying:** Interacting with a database to extract relevant information.
* **Data Analysis:** Interpreting query results to identify potential security issues or anomalies.

By mastering these skills, effective analysis of large datasets, identification of trends, and informed decision-making to enhance security posture can be achieved.

## Tools Used

* **SQL Database:** A database management system used to store and manage structured data.
* **SQL Query Language:** Used to interact with the database and retrieve specific information.
* **MariaDB Shell:** A command-line interface for interacting with the MariaDB database. 

By utilizing these tools, users can effectively query and analyze database information to support various security and administrative tasks.

## Steps
1. Retrieve employee device data
* In this task, you need to obtain information on employee devices because your team needs to update them. The information you need is in the machines table in the organization database.
  * First, you need to retrieve all the information about the employee devices.
     * Run the following query to select all device information from the machines table:
     * ![sql query 1](https://github.com/user-attachments/assets/b8e10661-7fce-4968-8a4f-65d136918e3d)
  * Next, you want to focus on the email client running on various devices.
     * Run the following query to select only the device_id and email_client columns from the machines table. Replace X with device_id and Y with email_client:
     * ![sql query 2](https://github.com/user-attachments/assets/629a2a69-5589-44e0-9aec-7b2a9f3454e2)
  * Now, you need information on the operating systems used on various devices and their last patch date.
    * Complete the query to return only the device_id, operating_system, and OS_patch_date columns from the machines table. Replace X, Y, and Z with the columns that you need to return:
    * ![sql query 3](https://github.com/user-attachments/assets/8f599950-1429-4276-8b8d-b4b2fe2ad28b)
      
2. Investigate login activity
* In this task, you need to analyze the information from the log_in_attempts table to determine if any unusual activity has occurred.
  * First, you need to investigate the locations where login attempts were made to ensure that they’re in expected areas (the United States, Canada, or Mexico).
    * Write a SQL query to select the event_id and country columns from the log_in_attempts table.
    * ![sql query 4](https://github.com/user-attachments/assets/d1ecabcd-b686-4cbd-b06b-e201336af6a3)
  * Next, you need to check if login attempts were made outside of the organization's working hours.
    * Write a SQL query that selects the username, login_date, and login_time columns from the log_in_attempts table.
    * ![sql query 5](https://github.com/user-attachments/assets/82cfb78c-3996-4bb4-b1ff-0411243143a2)
  * Now, you need to get a complete picture of all login attempts.
    * Write a SQL query that selects all columns from the log_in_attempts table, using a single symbol after the SELECT keyword.
    * ![sql query 6](https://github.com/user-attachments/assets/7c5c4fd9-9073-4e7c-9321-b999a1315f19)

3. Order login attempts data
* In this task, you need to use the ORDER BY keyword. You'll sequence the data that your query returns according to the login date and time.
  * First, you need to sort the information by date.
    * Run the following query, which orders log_in_attempts data by login_date:
    * ![sql query 7](https://github.com/user-attachments/assets/0b2ebd31-bcbf-450f-872b-3ae0eb2c6127)
  * Now, you need to further organize the previous results by ordering them by login_time.
    * Modify the query from the previous step by adding the login time to the ORDER BY clause. You must replace X with the appropriate column name:
    * ![sql query 8](https://github.com/user-attachments/assets/c8468197-eeaa-4f14-9e76-c27dfdba25d9)

### Summary

This activity provided hands-on experience in executing fundamental SQL queries, including selecting specific columns and sorting results. By mastering these core concepts, users can effectively retrieve and analyze data from databases, a crucial skill for various data-driven tasks.
