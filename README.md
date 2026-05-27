# Customer Order Analysis — Python Project

A Python-based data analysis project (Jupyter Notebook) that simulates a retail
customer order system and performs business intelligence analysis using core Python
data structures — lists, tuples, dictionaries, and sets.

---

## 📋 Project Overview

The project works with a dataset of 10 customers and 26 orders across 3 product
categories (Electronics, Clothing, Home Essentials) and performs end-to-end
customer and revenue analysis without using any external libraries.

---

## 🗂️ Dataset

**10 Customers:** Alice Johnson, Bob Smith, Charlie Davis, Diana Martinez,
Ethan Brown, Fiona Wilson, George Taylor, Hannah Lee, Ivan Anderson, Julia Thomas

**26 Orders** across 3 categories:
- Electronics (Laptop, Smartphone, Gaming Console, Tablet, Smart Watch, etc.)
- Clothing (Jeans, Sneakers, Jacket, Dress, Running Shoes, etc.)
- Home Essentials (Coffee Maker, Blender, Microwave, Yoga Mat, etc.)

---

## 📊 Tasks Performed

### Task 1 — Store Customer Orders
- Created a list of customer names
- Stored all orders as tuples `(customer_name, product, price, category)`
- Built a dictionary mapping each customer to their list of ordered products

### Task 2 — Product Classification
- Mapped every product to its category using a dictionary
- Extracted unique categories using a set
- Displayed all 26 products sorted alphabetically with their categories

### Task 3 — Customer Spending Analysis
- Calculated total spending per customer by iterating over order dictionaries
- Classified customers into three tiers:
  - **High-Value Buyer** — spending > $100
  - **Moderate Buyer** — $50 ≤ spending ≤ $100
  - **Low-Value Buyer** — spending < $50
- Displayed spending summary and classification distribution

### Task 4 — Business Insights
- Total revenue per product category with percentage contribution
- Identified unique products using a set
- Used list comprehension to find all Electronics buyers
- Identified **Top 3 highest-spending customers**

### Task 5 — Organized Data Display & Additional Insights
- Detailed per-customer breakdown of products, spending, and classification
- Found customers who purchased from **multiple categories**
- Used **set intersection** to find customers who bought both Electronics and Clothing
- Average order value per category
- Revenue contribution by customer type (High / Moderate / Low)
- Final summary statistics

---

## 📈 Sample Output
Total Revenue: $3,750.00
Total Customers: 10
Total Orders: 26
Total Unique Products: 26
Total Product Categories: 3
Average Customer Spending: $375.00
Highest Spending Customer: Alice Johnson ($890.00)
Most Profitable Category: Electronics

---

## 🐛 Known Issue

Task 4 has a cell ordering bug — `unique_products` and `category_revenue`
are defined after they are first referenced in the notebook. Re-running
cells in the correct order resolves this. A fix would be to move the
variable definitions to the top of Task 4's cell.

---

## 🛠️ Concepts Used

- Lists, Tuples, Dictionaries, Sets
- List comprehension
- Dictionary iteration and `.items()`
- Set operations (intersection, union)
- Lambda functions with `sorted()`
- f-strings and formatted output
- Conditional classification logic

---

## 🚀 How to Run

1. Open the `.ipynb` file in Jupyter Notebook or JupyterLab
2. Run all cells **in order** from top to bottom
3. If you get a `NameError`, restart the kernel and run all cells again

---

## 📌 Tools Used

- Python 3.13
- Jupyter Notebook (Anaconda/conda environment)
- No external libraries used — pure Python only
