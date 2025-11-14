
📘 Python MySQL Connection — Simple Explanation

This code demonstrates how to connect Python to a MySQL database using PyMySQL and retrieve data from a table.

# 📌 Python MySQL Database Connection — Explanation

This script shows how to connect Python to a MySQL database using the `pymysql` library and execute a simple `SELECT` query.

## 🔧 1. Import Library
```python
import pymysql


Imports pymysql, a library used to communicate with MySQL databases.

🔌 2. Create Database Connection
mydb = pymysql.connect(
    host="***", 
    user="***", 
    password="****", 
    port=***, 
    database="***" 
)


Connects to the MySQL server using the given credentials.

*** is used to hide sensitive information before uploading to GitHub.

⚡ 3. Connection Confirmation
print("Connection successful!")

🧭 4. Create Cursor
mycursor = mydb.cursor()


A cursor allows Python to execute SQL queries.

📥 5. Execute SQL Query
mycursor.execute("select * from table_name")


Runs a SQL query to fetch all records from the given table.

📤 6. Fetch & Display Results
for i in mycursor:
    print(i)


Iterates through each row returned by the query and prints it.
