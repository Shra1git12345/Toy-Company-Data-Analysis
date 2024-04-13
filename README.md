# Toy-Company-Data-Analysis
Suppose you are an analyst working in a company that sells toy replicas of branded vehicles such as cars, bikes, trucks, buses, etc.
First, you must understand the process and structure of the database. You need to work with the following three sections in this database:

Employee section
Customer section
Product section

1]Employee section: This section is divided into the following two tables:

employees: This table contains information about a company’s employees. Each entry in this table is identified uniquely by the ‘employeeNumber’, which is the primary key of this table.

offices: This contains information about the company’s offices located around the world. Each office is uniquely identified by the ‘officeCode’, which is the primary key of this table. Each employee must have only one office against their ID, in which they have to work.


2]Customer section: This section contains the following four tables: 

customers: This table contains information about the customers who buy the models in bulk from the company. They are retailers or shopkeepers who own firms or shops, not the final consumers. Each customer is uniquely identified by the ‘customerNumber’, which is the primary key of this table. A particular customer is either assigned an employee or not assigned any employee. The assigned employee is identified by the ‘salesRepEmployeeNumber’ column in this table. Multiple customers can be assigned to an employee.

orders: This table contains information about the orders placed by the customers. Each order is uniquely identified by its ‘orderNumber’, which is the primary key of this table. A particular customer can place multiple orders, but each order should have a unique ‘orderNumber’.

orderdetails: This table also contains the details of the orders placed by customers. However, both the ‘orderNumber’ and ‘productCode’ are part of the composite primary key here.

payments: This table contains information about the payments made by customers after placing the orders. Here, you will see a column named ‘checkNumber’, which refers to the unique number of the check through which the customer (customerNumber) has made the payment. Under this table, ‘checkNumber’ is the primary key.

 

Product Section: This section has the following two tables:

products: The products table contains information about the different products that are sold by the company. Each product is uniquely identified by the productCode, which is the primary key of this table.

productlines: This table is a broad categorisation of the type of toy models that are sold by the company, including vintage cars, motorcycles, trains, and ships. Each product in the ‘products’ table must have a single product line.


So, you will have the following eight tables:

employees
offices
customers
orders
orderdetails
payments
products
productlines

 
You need to prepare the entity relational diagram (ERD) for this case study after understanding the descriptions of the above-mentioned tables.

 

You have already been provided with the data set, so you do not have to create any table in the database. You are mainly required to write SQL queries to answer the graded questions.
