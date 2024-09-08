# Python Script for Loading CSV Data into MySQL

## Purpose:

This Python script is designed to load CSV data from a specified folder into a MySQL database. It automatically creates tables with appropriate data types based on the CSV data and inserts the data into the corresponding tables.

## Prerequisites:

-  Python 3.x
-  pandas
-  mysql-connector-python
-  MySQL database

## Usage:

### 1. Configure:

- Replace the values for host, user, password, and database in the mysql.connector.connect() call with your MySQL database credentials.
- Update the folder_path variable to point to the directory containing the CSV files.
- Modify the csv_files list to include the CSV files and their corresponding table names.


### 2. Run:

Execute the Python script.

## Features:

- Automatically creates tables with appropriate data types based on the CSV data.
- Handles NaN values by replacing them with None for SQL NULL.
- Cleans column names by replacing spaces, hyphens, and periods with underscores.
- Inserts data into the tables using prepared statements for security and efficiency.
- Provides a clear and concise structure for data loading.

## Additional Notes:

- For large datasets, consider using bulk insert methods or asynchronous processing to improve performance.
- Ensure that the CSV files have consistent headers and data types.
- If you encounter errors, check the MySQL logs for more information.
- Customize the script as needed to fit your specific requirements.
