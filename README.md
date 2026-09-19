````markdown
# 📞 Customer Call List Data Cleaning

## 📌 Project Overview

This project focuses on **cleaning and preprocessing a customer call list dataset** using Python and Pandas.

The dataset contains customer information such as names, phone numbers, addresses, payment status, and contact preferences. The main goal is to transform messy raw data into a cleaner and more consistent format.

## 🎯 Objectives

- Remove duplicate records
- Remove unnecessary columns
- Clean customer names
- Standardize phone numbers
- Handle missing and invalid values
- Standardize customer status fields
- Split address information into separate columns
- Prepare the dataset for further analysis

## 🧹 Data Cleaning Steps

### 1. Load the Dataset

The Excel dataset is loaded using Pandas.

```python
import pandas as pd

data = pd.read_excel("Customer Call List.xlsx")
````

### 2. Remove Duplicates

Duplicate customer records are identified and removed.

```python
data = data.drop_duplicates()
```

### 3. Remove Unnecessary Columns

The `Not_Useful_Column` is removed because it is not required for the analysis.

### 4. Clean Names

Unwanted characters from the `Last_Name` column are removed to make the names consistent.

### 5. Clean Phone Numbers

Different phone number formats are standardized by removing unwanted characters and maintaining a consistent format.

### 6. Standardize Customer Status

The `Paying Customer` and `Do_Not_Contact` columns contain values such as `Yes`, `No`, `Y`, and `N`.

These values are standardized into a consistent format.

### 7. Clean Address Data

The `Address` column is separated into:

* `Street_Address`
* `State`
* `Zip_code`

This makes the address information easier to work with.

### 8. Handle Missing Values

Missing values and text representations such as `NaN`, `N/a`, `None`, and similar values are cleaned and replaced appropriately.

## 📊 Dataset Columns

The dataset contains customer-related information including:

* `CustomerID`
* `First_Name`
* `Last_Name`
* `Phone_Number`
* `Address`
* `Paying Customer`
* `Do_Not_Contact`

After cleaning, additional address fields such as `Street_Address`, `State`, and `Zip_code` are created.

## 🛠️ Technologies Used

* Python
* Pandas
* Jupyter Notebook
* Microsoft Excel

## 📁 Project Structure

```text
Customer-Call-List-Cleaning/
│
├── Customer_Call_List_Cleaning.ipynb
├── Customer Call List.xlsx
└── README.md
```

## 💡 Key Learning

This project helped me practice important **data-cleaning techniques using Pandas**, including:

* Duplicate removal
* Column manipulation
* String cleaning
* Missing-value handling
* Data standardization
* Data transformation

## 👩‍💻 Author

**Harshitha**

```
```
