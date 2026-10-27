# E-Commerce Order Data Analysis

## 📌 Project Overview
This project focuses on cleaning, analyzing, and understanding an **E-Commerce Order Dataset** using Python and Pandas. The dataset contains information about customers, products, orders, payment modes, quantities, prices, discounts, and ratings.

## 🛠️ Technologies Used
- Python
- Pandas
- Google Colab / Jupyter Notebook
- CSV

## 📂 Dataset
**File:** `Ecommerce_Order_Test_Dataset.csv`

- **Rows:** 101
- **Columns:** 13

### Columns

| Column          | Description       |
| --------------- | ----------------- |
| `Order_ID`      | Unique order ID   |
| `Order_Date`    | Date of order     |
| `Delivery_Date` | Delivery date     |
| `Customer_Name` | Customer name     |
| `Gender`        | Customer gender   |
| `City`          | Customer city     |
| `Category`      | Product category  |
| `Product`       | Product name      |
| `Payment_Mode`  | Payment method    |
| `Quantity`      | Quantity ordered  |
| `Unit_Price`    | Price of one unit |
| `Discount`      | Discount value    |
| `Rating`        | Customer rating   |

## 🔍 Tasks Performed

### Q1. Load and Inspect
- Loaded the CSV file into a DataFrame named `df`.
- Displayed the first 5 rows.
- Displayed the number of rows and columns.
- Displayed all column names.

### Q2. Understand the Dataset
- Used `info()` to display basic information.
- Used `describe()` to display the statistical summary of numerical columns.

### Q3. Handle Missing Values
- Found missing values in each column.
- Filled missing `City` values with `"Unknown"`.
- Filled missing `Customer_Name` values with `"Unknown"`.
- Filled missing `Rating` values with the mean rating.
- Filled missing `Payment_Mode` values with `"Unknown"`.

### Q4. Remove Duplicates
- Found the number of duplicate rows.
- Removed duplicate rows.
- Displayed the new shape of the DataFrame.

### Q5. Data Validation (Added for Completeness)
- Verified data types of all columns.
- Ensured date columns (`Order_Date`, `Delivery_Date`) are in the correct datetime format.
- Checked for any remaining inconsistencies.

### Q6. Clean Text Data
Cleaned the following columns:
- `Gender`
- `City`
- `Payment_Mode`

Used `strip()` to remove unnecessary spaces and `title()` to make the text formatting consistent. Displayed the unique values after cleaning.

### Q7. Create New Columns
Created three new calculated columns:

**Total Price**
```text
Total Price = Quantity × Unit Price
