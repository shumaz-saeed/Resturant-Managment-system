# Resturant-Managment-system

A simple Python-based Command-Line Restaurant Management System, implementing Object-Oriented Programming (OOP), SQLite3 database, and the logging module for storing orders, workers, and table reservations. Customer receipts are generated in .txt and .csv formats.


📂 Project Features
✅ Dine-In & Takeaway System
✅ Menu Management (pre-loaded items)
✅ Order Placement & Receipt Generation
✅ Table Reservation & Viewing
✅ Admin Panel (add/update/remove workers — password protected)
✅ SQLite3 Database for data persistence
✅ CSV Receipt Logs
✅ Activity Logging using Python's logging module

🔧 Technologies Used
Python 
SQLite3 (sqlite3)
Logging (logging)
CSV file handling (csv)

🔐 Admin Login
To access worker management functions:
Username: none required
Password: admin123

📊 Data Storage
Data Type	Storage
Workers	SQLite3 (workers table)
Orders	SQLite3 (orders table) + CSV Logs
Tables	SQLite3 (tables table)
Logs	restaurant.log
Receipts	receipts.csv + receipt_table_{num}.txt

📜 License

This project is licensed under the MIT License.



