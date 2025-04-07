# Mall Customer Data Cleaning

## Task Description

This task involved cleaning and preprocessing a raw dataset of mall customer data. The goal was to prepare the data for further analysis by handling missing values, removing duplicates, standardizing text, and ensuring consistent data types.

## Steps Taken

1.  **Loading the Dataset:**
    * The dataset "Mall_Customers.csv" was loaded using pandas.

2.  **Handling Missing Values:**
    * Missing values were removed using `dropna()`. The number of rows dropped was printed to the console.

3.  **Removing Duplicates:**
    * Duplicate rows were removed using `drop_duplicates()`. The number of duplicate rows removed was also printed.

4.  **Standardizing Text Fields:**
    * The "Gender" column was standardized to lowercase and stripped of leading/trailing spaces using `str.lower()` and `str.strip()`.
    * Column names were converted to lowercase and spaces were replaced with underscores for consistency.

5.  **Fixing Data Types:**
    * The "Age" column was converted to integer type using `astype(int)`.
    * The "Annual Income (k$)" column was converted to float type using `astype(float)`.
    * The "Spending Score (1-100)" column was converted to float type using `astype(float)`.

6.  **Saving Cleaned Dataset:**
    * The cleaned dataset was saved to a new CSV file named "Mall_Customers_Cleaned.csv" using `to_csv()`.

7.  **Information display:**
    * The info and head of the dataframe was printed before and after cleaning.

## Challenges

* The original column name "Annual Income (k$)" required careful handling during the renaming process to ensure the correct column name was used for data type conversion.
* Understanding the proper use of the pandas string methods for standardization.

## Final Cleaned Dataset

The final cleaned dataset, "Mall_Customers_Cleaned.csv", is now free of missing values and duplicates, and has consistent text and data types, making it ready for analysis.

## Code Explanation

The python code uses the pandas library to read, clean, and write the csv data. The code first loads the data, then drops null and duplicate values. After that the gender column and all columns are standardized. Finally the data types of the age, annual income, and spending score columns are changed to their correct types. The data is then saved to a new csv file.

## How to Run the Code

1.  Ensure you have pandas installed (`pip install pandas`).
2.  Place the "Mall_Customers.csv" dataset in the same directory as the Python script or Colab notebook.
3.  Run the Python script or Colab notebook.
4.  The cleaned dataset "Mall_Customers_Cleaned.csv" will be created in the same directory.
