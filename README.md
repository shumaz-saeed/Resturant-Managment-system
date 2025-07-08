
# Restaurant Management System 

Welcome to the Restaurant Management System\! This Python application offers a seamless experience for both customers and administrators, handling everything from table reservations and order placement to staff management and detailed logging.

-----

## ✨ Features at a Glance

### For Our Valued Customers:

  * **Dine-in Experience**: Easily reserve tables and place your orders right from your seat.
  * **Takeaway Convenience**: Get your favorite meals to go with a quick and efficient ordering process.
  * **Intuitive Menu**: Browse our delicious offerings with clear item IDs and prices.
  * **Flexible Payments**: Pay with **cash** or **card**, ensuring a smooth checkout.
  * **Instant Receipts**: Receive a detailed receipt for every order, plus a comprehensive CSV record of all transactions.

### For Our Dedicated Admin Team:

  * **Worker Management**: **Add**, **view**, **update**, or **remove** staff details with ease.
  * **Table Oversight**: Keep track of all tables, their seating capacity, and reservation status.
  * **Effortless Reset**: **Unreserve all tables** with a single command, perfect for daily resets or special events.

### Behind the Scenes:

  * **Robust Database**: Powered by **SQLite**, ensuring all your data—workers, orders, and tables—is securely stored.
  * **Smart Logging**: Every significant action is **logged** in `restaurant.log`, giving you a clear history of operations.

-----

## 🚀 Get Started

1.  **Save the Code**: Copy the provided Python code and save it as `restaurant_system.py` (or any name you prefer) on your computer.

2.  **Run the Application**: Open your terminal or command prompt, navigate to where you saved the file, and simply run:

    ```bash
    python restaurant_system.py
    ```
OR FOR PIC :


![image](https://github.com/user-attachments/assets/c0afbcb7-80e8-49a6-8a31-8e22b97c4450)

-----

## 👨‍🍳 How to Use

Upon launching the application, you'll be greeted with a friendly welcome.

### Customer Journey:

1.  **Dine In**:

      * Choose from options to **view all tables**, **reserve a table** (specify the number of seats you need, and we'll find an exact match\!), or **proceed to the menu** if you already have a table number.
      * Once your table is set, browse our menu and select items by their ID. You can add as many as you like\!

2.  **Takeaway**:

      * Opt for takeaway, and we'll let you know the estimated preparation time.
      * From the takeaway menu, you can **view the full menu** or **place your order** directly.

3.  **Payment**:

      * After placing your order, select your preferred payment method: **Cash** or **Card**.
      * If paying by card, you'll be asked for your 11-digit account number for a secure transaction.

### Admin Access:

  * The **Admin Panel** is accessible from the "Takeaway" menu.
  * **Password**: The default admin password is `admin123`.
  * Once inside, you'll find options to manage workers and unreserve all tables.

-----

## 🗄️ Database Structure

Our system uses a simple yet effective SQLite database (`restaurant.db`) with three tables:

  * **`workers`**:

      * `id`: Unique identifier for each worker.
      * `name`: Worker's full name.
      * `role`: Worker's job role (e.g., "Waiter", "Chef").

  * **`orders`**:

      * `id`: Unique identifier for each order.
      * `table_number`: The table number for dine-in orders (0 for takeaway).
      * `items`: A list of all items ordered.
      * `total_price`: The total cost of the order.
      * `timestamp`: When the order was placed.

  * **`tables`**:

      * `number`: Unique table number.
      * `seats`: Number of seats available at the table.
      * `is_reserved`: Status of the table (0 = Free, 1 = Reserved).

-----

## 📜 Logs & Receipts

  * **`restaurant.log`**: A detailed log of all major activities, perfect for monitoring operations and troubleshooting.
  * **`receipt_table_[table_number].txt`**: Individual, human-readable receipts for each dine-in order.
  * **`receipts.csv`**: A comprehensive CSV file containing records of all orders, great for financial tracking and analysis.

-----

## ⚖️ License

This project is open-source and distributed under the **MIT License**.

-----
