My SQL Pizza Sales Data Analysis Project
As someone building their skills, I've found that projects are absolutely crucial for showcasing what you can do. That's why I created this SQL Pizza Sales Data Analysis project. My aim here was to dive deep into a pizza sales dataset, tackling a wide range of SQL queries – from the straightforward basics right through to more advanced concepts. This project truly gave me hands-on experience, demonstrating how I approached setting up a database, importing data, writing complex queries, and interpreting the results to pull out valuable business insights.
🍕 My Project's Journey
My main objective with this project was to complete an end-to-end data analysis on a pizza sales dataset. I really enjoyed exploring different facets of the sales data, such as finding the total number of orders, calculating revenue, identifying popular pizza types and sizes, and spotting sales trends over time. A key part of the process was also learning how to prepare my analysis for presentation, which included creating a professional PDF report and then sharing it on platforms like GitHub and LinkedIn.
✨ Key Skills & Concepts I Explored
Through this project, I really got to grips with a comprehensive set of SQL concepts and functions, which include:
• Database Creation and Management: I started by setting up a new database, which I called 'pizzahut', and then importing my data into it.
• Table Creation: I manually defined table structures, carefully specifying column names, data types (like INTEGER, DATE, TIME, TEXT, DOUBLE), and constraints such as NOT NULL and PRIMARY KEY. This was particularly useful for handling larger datasets.
• Data Import: I learned how to import CSV files into MySQL Workbench. For smaller files, the Table Data Import Wizard was perfect, but for larger ones (over 20,000 rows, for example), I found it much more efficient to create the table structure first, then import the data into the existing table.
• SELECT Queries: Fundamental for retrieving specific data.
• WHERE Clause: Essential for filtering results based on specific conditions.
• Aggregate Functions: I extensively used COUNT(), SUM(), and AVG() to summarise data effectively.
• GROUP BY Clause: Vital for grouping rows when applying aggregate functions.
• ORDER BY Clause: Used this for sorting my query results in both ascending (ASC) and descending (DESC) order, especially when looking for top items.
• JOIN Operations: A huge part of this project involved combining data from multiple tables using INNER JOIN, based on common columns like pizza_id, order_id, and pizza_type_id. It definitely solidified my understanding of joins.
• ROUND() Function: Handy for rounding numerical values, particularly for presentation, such as sales figures to two decimal places or average quantities to zero decimal places.
• LIMIT Clause: Great for restricting the number of rows, especially when finding top N results.
• Subqueries: I delved into embedding one SQL query within another to perform more complex operations, particularly for calculating aggregated values that were then used in outer queries. This was a bit more challenging but really rewarding.
• Window Functions: I specifically used RANK() to assign a rank to each row within a partition, which was perfect for identifying top items within different pizza categories.
• Commenting in SQL: I made sure to use -- or /* ... */ to add comments to my SQL scripts for readability and documentation.
• Query Beautification: A simple but effective trick was using CTRL + B in MySQL Workbench to format my SQL queries, making them much easier to read.
📊 The Data I Worked With
I worked with a Pizza Sales dataset, which conveniently came as four CSV files. This dataset was sourced from a GitHub repository, with the link available in the video description.
The four data files I used were:
• orders.csv: This file held information about each order, including the order_id, order_date, and order_time.
• pizza_types.csv: This provided details about the different pizza types, such as id, name, category, and ingredients.
• pizzas.csv: This contained information about individual pizzas, including pizza_id, pizza_type_id, size (Small, Medium, Large, XL, XXL), and price.
• order_details.csv: This was crucial, containing specifics for each item in an order, like order_details_id, order_id (acting as a foreign key linking to orders), pizza_id (linking to pizzas), and quantity. I noticed the order_id often repeated here, indicating that multiple pizzas could be part of a single order.
🛠️ Tools & Technologies I Used
The main tools I leveraged for this analysis were:
• MySQL Workbench: This was my primary SQL client for managing the database, creating tables, importing data, and executing all my queries.
• SQL (Structured Query Language): The core language, of course, for all my database interactions and data analysis.
• CSV (Comma Separated Values): The format in which my raw dataset was provided.
• Canva: I found Canva really useful for creating a professional presentation (PDF) to effectively showcase my project's findings.
• GitHub: I used GitHub for version control, hosting my SQL scripts, and publishing the project presentation PDF, making it easy to share my work.
• LinkedIn: A great platform for sharing my project outcomes and insights with a broader professional network.
⚙️ How I Set Up & Executed This Project
To give you an idea of how I got this project up and running, here are the steps I followed:
1. Downloaded the Data: I first obtained the pizza_sales.zip file from the GitHub repository link mentioned in the video description.
2. Extracted the Data: I unzipped the file into a dedicated folder on my desktop, which I named "SQL Pizza Sales Project". This folder then contained the four necessary CSV data files.
3. Opened MySQL Workbench: I launched MySQL Workbench and made sure I was connected to my MySQL server.
4. Created the Database: I executed the SQL query CREATE DATABASE pizzahut; to set up a new database specifically for this project.
5. Selected the Database: I then double-clicked the newly created pizzahut database in the SCHEMAS panel of MySQL Workbench to make it the active database for all my subsequent operations.
6. Imported the Tables:
    ◦ Smaller Files (pizzas.csv, pizza_types.csv): For these, I used the Table Data Import Wizard. I right-clicked on "Tables" under my pizzahut database, selected "Table Data Import Wizard", browsed to my CSV file, chose "Create New Table", and confirmed the suggested data types before finishing the import.
    ◦ Larger Files (orders.csv, order_details.csv): For the larger datasets (like orders.csv with over 21,000 rows), I found it essential to first create the table structure manually using CREATE TABLE statements in MySQL Workbench, defining all columns, their data types, and primary keys. After creating the empty table, I then used the "Table Data Import Wizard" and selected the option to "Use existing table" to import the CSV data into my pre-defined table structure. This was a good learning point about handling larger files.
7. Executed Queries: Once all tables were imported, the fun began! I started writing and executing the SQL queries to derive insights from the data, referencing the questions provided in the questions.txt file (available in the GitHub repository).
🎯 Questions I Tackled & Insights I Gained
I tackled a variety of questions to extract meaningful insights from the pizza sales data. Here are some of the key questions I addressed, moving from basic to more advanced concepts:
• Retrieve the total number of orders placed.
• Calculate the total revenue generated from pizza sales.
• Identify the highest-priced pizza.
• Identify the most commonly ordered pizza quantity and size.
• List the top 5 most ordered pizza types along with their quantities.
• Find the total quantity of each pizza category ordered.
• Determine the distribution of orders by hour of the day.
• Find the category-wise distribution of pizzas.
• Calculate the average number of pizzas ordered per day. (This one involved a subquery, which was a great challenge!)
• Determine the top 3 most ordered pizza types based on revenue.
• Calculate the percentage contribution of each pizza type/category to total revenue. (This was an "advanced" question, combining subqueries and calculations!)
• Analyse the cumulative revenue generated over time. (I used a subquery and window function here to achieve the cumulative sum!)
• Determine the top 3 most ordered pizza types based on revenue for each pizza category. (This was quite complex, involving multiple subqueries and the RANK() window function!)
🤝 How I'm Showcasing This Project
Once I had completed my analysis, I wanted to effectively showcase my work to potential employers and my professional network. Here's how I went about it:
1. Created a Presentation (PDF): I used Canva to design a professional presentation. I included my project questions, screenshots of my SQL queries, and the corresponding results. This provided a clear and visual representation of my analytical process and findings.
2. Uploaded to GitHub: I created a new repository on GitHub (e.g., pizza-sales-sql-project). I uploaded all relevant files, including my SQL script(s) and the final project presentation PDF. This makes my project publicly accessible and demonstrates my version control skills. I can then easily add this GitHub repository link to my resume.
3. Shared on LinkedIn: I crafted a post on LinkedIn, attaching my project presentation PDF as a document. I briefly described my project, the insights I gained, and the key SQL concepts I applied. I've heard that tagging relevant communities or individuals (like WsCube Tech or Ayushi Jain) can help increase visibility and attract feedback, so I made sure to do that too.
