**Task 1: Data Cleaning & Preprocessing**  
**Dataset Source:** [Kaggle - Sales Data](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales)

🔍 Objective

To clean and preprocess the sales dataset by:
- Identifying and handling missing values
- Removing duplicates
- Standardizing formats (text/date)
- Renaming columns
- Ensuring consistent and correct data types

🧰 Tools Used

- Python
- Pandas
- Jupyter Notebook

🧼 Cleaning Steps Performed

1. **Handled Missing Values**
   - Filled `gender` with `'Unknown'` (if missing)
   - Dropped rows missing critical fields like `invoice_id`, `date`, or `time`
   - Checked for and handled nulls in numerical fields (e.g., `rating`)

2. **Removed Duplicate Records**
   - Used `.drop_duplicates()` to remove exact row-level duplicates

3. **Standardized Text Values**
   - Stripped whitespaces and standardized casing in `gender`, `city`, `customer_type`, and `payment` fields

4. **Converted Date Formats**
   - Converted `date` column to a consistent format: `dd-mm-yyyy`

5. **Renamed Column Headers**
   - Converted all column names to lowercase
   - Replaced spaces with underscores to follow `snake_case` naming convention

6. **Checked and Fixed Data Types**
   - Ensured `unit_price`, `quantity`, `tax_5%`, `sales`, `cogs`, `gross_income`, and `rating` were numeric
   - Converted `date` to `datetime` type before formatting

✅ Final Output

- Total records after cleaning: **(fill in after running `.shape[0]`)**
- Missing values successfully handled
- Duplicates removed
- Dataset ready for analysis or modeling
