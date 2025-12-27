# Retail Sales Data Cleaning

This project cleans and prepares a retail sales transactions dataset (1,194 rows, 12 columns) for analysis of revenue and profit by time, product, and region.

## Dataset

- Each row represents a single product line within a customer order.
- Key fields: Amount, Profit, Quantity, Category, Sub-Category, PaymentMode, Order Date, State, City, Year-Month.

## Data Quality Checks

- Inspected structure and types using `head()`, `info()`, and `describe()`.
- Verified there are no missing values or duplicate rows.
- Reviewed category, sub-category and payment mode values for consistent naming.

## Cleaning and Transformations

- Converted `Order Date` from text to datetime and created separate `Year` and `Month` columns.
- Trimmed whitespace in text columns and enforced numeric types for Amount, Profit and Quantity.
- Saved the cleaned dataset as `data/cleaned/cleaned_data.csv`.

## Repository Structure

- `data/raw/raw_data.csv` – original dataset.
- `data/cleaned/cleaned_data.csv` – cleaned, analysis-ready dataset.
- `notebooks/retail_sales_cleaning.ipynb` – Python notebook with profiling and cleaning code.
- `docs/Retail_Sales_Data_Dictionary_and_Quality_Report.docx` – data dictionary and quality assessment.
