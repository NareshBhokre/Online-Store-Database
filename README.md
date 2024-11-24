# Online-Store-Database Task-2
# Problem Statement: 
Develop a database for any entity you like i.e hospital ,library, school, movie rental, online store. This project involves more queries and database design. For example: For a e store database you can design tables for products, customers, orders, and payments.

1. CREATE TABLE customers (
    customer_id INT AUTO_INCREMENT PRIMARY KEY,
    first_name VARCHAR(255) NOT NULL,
    last_name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL UNIQUE,
    phone_number VARCHAR(20),
    address TEXT,
    city VARCHAR(100),
    state VARCHAR(100),
    postal_code VARCHAR(20),
    country VARCHAR(100)
  );
  
INSERT INTO customers (first_name, last_name, email, phone_number, address, city, state, postal_code, country)
  VALUES ('John', 'Doe', 'john.doe@example.com', '123-456-7890', '123 Main St', 'Springfield', 'IL', '62701', 'USA'),
    ('Jane', 'Smith', 'jane.smith@example.com', '987-654-3210', '456 Oak Rd', 'Chicago', 'IL', '60601', 'USA'),
    ('Alice', 'Johnson', 'alice.johnson@example.com', '555-123-4567', '789 Pine Ln', 'Los Angeles', 'CA', '90001', 'USA'),
    ('Bob', 'Brown', 'bob.brown@example.com', '555-987-6543', '101 Maple Ave', 'New York', 'NY', '10001', 'USA'),
    ('Charlie', 'Davis', 'charlie.davis@example.com', '555-555-5555', '202 Birch Blvd', 'Houston', 'TX', '77001', 'USA');

SELECT * FROM Customers;

2. CREATE TABLE products (
    product_id INT AUTO_INCREMENT PRIMARY KEY,
    product_name VARCHAR(255) NOT NULL,
    description TEXT,
    price DECIMAL(10, 2) NOT NULL,
    category VARCHAR(100),
    stock_quantity INT DEFAULT 0,
    supplier VARCHAR(255)
   );
INSERT INTO products (product_id, product_name, description, price, category, stock_quantity, supplier)
VALUES (1, 'Wireless Mouse', 'Ergonomic wireless mouse', 25.99, 'Electronics', 150, 'TechSupplies Inc.'),
       (2, 'Bluetooth Speaker', 'Portable Bluetooth speaker', 49.99, 'Electronics', 80, 'SoundCo'),
       (3, 'Stainless Steel Water Bottle', '500ml reusable bottle', 15.50, 'Home & Kitchen', 200, 'EcoGoods LLC'),
       (4, 'LED Desk Lamp', 'Adjustable LED desk lamp', 35.00, 'Home & Office', 120, 'BrightLight Ltd.'),
       (5, 'Yoga Mat', 'Non-slip yoga mat', 20.00, 'Fitness', 300, 'FitZone Retailers');

SELECT * FROM products;

3. 



# Write SQL queries to handle customer orders.
