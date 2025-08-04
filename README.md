# Sales_Dataset_Cleaning_Task1
A data cleaning project focused on identifying and resolving common real-world data issues using Microsoft Excel. This project covers handling missing values, removing duplicates, standardizing inconsistent entries, correcting data types, and formatting date fields — all performed manually without code to build practical spreadsheet skills.


## 📂 Files in This Repository

| File Name                 | Description                                  |
|--------------------------|----------------------------------------------|
| `sales_data_dirty_500.csv` | Raw sales data with 500 records containing various data quality issues |
| `sales_data_cleaned.xlsx`  | Fully cleaned and formatted dataset, ready for analysis |
| `README.md`                | Overview of the project and steps followed |

---

## 📊 Columns in the Dataset

- `Customer ID` — Unique ID for each customer
- `Name` — Customer name (with some missing values)
- `Age` — Age in years (some entries are missing or non-numeric)
- `Gender` — Gender of customer (inconsistent capitalization)
- `Country` — Country name (inconsistent values)
- `Date of Purchase` — Date (in mixed formats and sometimes missing)
- `Product` — Product purchased (Tablet, Laptop, Mobile)
- `Amount` — Sale amount (with some missing values)

---

## 🔧 Cleaning Steps Performed

### 1. ✅ **Identified and Handled Missing Values**
- Detected missing values in `Name`, `Age`, `Amount`, and `Date of Purchase`.
- Filled missing numeric values (like `Age` and `Amount`) with the **average** or a **placeholder**.
- Filled missing text fields (like `Name`) with `"Unknown"`.

### 2. 🔁 **Removed Duplicate Rows**
- Highlighted and removed full duplicate entries using Excel’s **Remove Duplicates** tool.

### 3. 🧼 **Standardized Text Fields**
- Standardized `Gender` values (e.g., `"FEMALE"`, `"female"` → `"Female"`)
- Cleaned `Country` names (e.g., `"INDIA"`, `"india"`, `"U.S."` → `"India"`, `"United States"`)
- Applied the `PROPER()` function to capitalize names properly.

### 4. 📅 **Fixed Date Formatting**
- Converted inconsistent date formats (`dd-mm-yyyy`, `dd/mm/yyyy`, `dd.mm.yyyy`) into a consistent format using Excel’s **Text to Columns** and **Format Cells**.

### 5. 🏷️ **Renamed Column Headers**
- Removed extra spaces and applied lowercase formatting for clarity and consistency.

### 6. 🔢 **Corrected Data Types**
- Converted `Age` from text (e.g., `"thirty one"`) to numeric values.
- Ensured `Amount` and `Date of Purchase` columns had the correct data types.

---

## 🎯 Goal of the Project

The main objective was to **practice data cleaning skills** using Excel, understanding how to identify and fix dirty data manually. This experience is valuable for analysts who work in environments where tools like Excel are widely used for data wrangling.

---

## 📈 Possible Next Steps

- Analyze the cleaned data using PivotTables or charts
- Perform the same cleaning steps in Python using pandas
- Add data validation rules to prevent future errors

---

## 💡 Tools Used

- Microsoft Excel (2016 or later)

---

## 🧠 Learning Outcomes

- Gained hands-on experience in identifying and cleaning dirty data
- Learned how to use Excel functions like `PROPER()`, `COUNTIF()`, `IFERROR()`, and filtering tools
- Practiced real-world data cleaning workflows without code

---

Feel free to fork this repo, use the dataset for your own practice, or contribute improvements!
