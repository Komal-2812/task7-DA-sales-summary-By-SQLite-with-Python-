📊 Task 7: Basic Sales Summary using SQLite & Python

📌 Objective

This task demonstrates how to connect Python with a local SQLite database, perform basic sales analysis using SQL queries, and visualize the results using `matplotlib`.

I am generate a **sales summary** showing the **total quantity sold** and **revenue** for each product, displayed as both printed output and a simple bar chart.

🛠️ Tools & Libraries Used

   **Python**: Core language for scripting
   
   **SQLite (`sqlite3`)**: Lightweight builtin database for storage and querying
   
   **pandas**: To load SQL results into DataFrames
   
   **matplotlib**: For basic data visualization

📁 Dataset Details

  A single SQLite database file named `sales_data.db` containing one table:
  
   Table: `sales`
  
   Column   | Type    | Description            
   id       | INTEGER | Primary key (auto)     
   product  | TEXT    | Product name           
   quantity | INTEGER | Units sold             
   price    | REAL    | Price per unit         

⚙️ What This Project Does :-
   📥 **Connects** to `sales_data.db` (creates it if not found)
   
   🧱 **Creates the `sales` table** if it doesn't already exist
   
   ➕ **Inserts sample data** for 5 products
   
   🧮 **Runs an SQL query** to calculate:
     Total quantity sold per product
     Total revenue per product (`SUM(quantity * price)`)
     
   🐼 **Loads results into a pandas DataFrame**
   
   🖨️ **Prints the summary** in tabular form
   
   📊 **Displays a bar chart** of revenue by product
   
   💾 **Saves the chart** as `sales_chart.png`

✅ Output Example

 📋 Console Output:
 product  | total_qty | revenue 
 Pen      | 10        | 50.0    
 Notebook | 5         | 100.0   
 Pencil   | 15        | 30.0    
 Eraser   | 20        | 20.0    
 Marker   | 7         | 70.0    

 📊 Bar Chart Output:
 A bar chart displaying revenue by product (saved as `sales_chart.png`)

🧠 Key Learning Outcomes

 Writing and executing **basic SQL queries inside Python**
 Using `pandas` to **manipulate and display SQL query results**
 Creating **basic visualizations** with `matplotlib`
 Understanding how to **combine database + analysis + visualization** in one pipeline

