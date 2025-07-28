# **TATA Virtual Internship: Market Basket Analysis Using Apriori**
### **Project Overview**
**This project is part of the TATA Virtual Internship Program and focuses on performing Market Basket Analysis using transactional retail data. The primary goal is to extract meaningful insights about customer purchase behavior through association rule mining using the Apriori algorithm.**

### **Dataset Description**
The dataset used (Online Retail.xlsx) contains transactional data for a UK-based online retail store. It includes the following fields:

- InvoiceNo: Unique invoice number

- StockCode: Product/item code

- Description: Product name

- Quantity: Number of products purchased

- InvoiceDate: Date and time of transaction

- UnitPrice: Price per unit

- CustomerID: Customer identifier

- Country: Country of the customer

### **Key Objectives**
- Clean and preprocess transactional data

- Create a product-basket matrix for the United Kingdom

- Apply the Apriori algorithm to identify frequent itemsets

- Generate and visualize association rules

- Export actionable rules for marketing and business strategy

### **Tools & Libraries Used**
- Python

- Pandas – Data manipulation

- Seaborn / Matplotlib – Data visualization

- Scikit-learn – Model support libraries

- Mlxtend – Association rule mining (apriori, association_rules)

- Google Colab – Development environment

### **Project Workflow**
1. #### **Data Cleaning**

- Remove missing CustomerID

- Create Revenue column from Quantity * UnitPrice

- Parse InvoiceDate to datetime format

2. #### **Market Basket Transformation**

- Filter data for United Kingdom

- Generate a pivot table: InvoiceNo x Product

- Convert to binary matrix (True = purchased, False = not purchased)

3. #### **Association Rule Mining**

- Apply the Apriori algorithm with a minimum support of 1%

- Generate rules with a lift of at least 1.0

- Sort rules by lift to identify strong associations

4. #### **Visualization**

- Bar plot of top 10 rules by lift

- Bubble chart: support vs confidence (lift as bubble size)

5. #### **Export Results**

- Rules exported to CSV format (association_rules.csv)

### **Output**

- association_rules.csv: List of top product associations with metrics like support, confidence, and lift

- Visual charts displaying top rules and relationships

### **How to Run**
1. Open the project in Google Colab

2. Upload the dataset Online Retail.xlsx

3. Run all cells to:

- Clean data

- Apply Apriori

- Generate and download results

**Author**
**Mihir Ughade**
**GitHub: https://github.com/mihir0804**
**LinkedIn: https://www.linkedin.com/in/mihir-ughade-00601223a/**
