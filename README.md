# Elevate_lab_task1
Task description
# Netflix Dataset Cleaning Project

This project cleans a Netflix dataset using Python (Pandas + NumPy).  
The goal is to standardize the data, fix inconsistencies, remove errors, and prepare the dataset for analysis or machine learning.

# What the Cleaning Script Does

The cleaning script performs the following tasks:

# Load and Inspect Data
- Loads the dataset using Pandas.
- Prints basic information such as shape and column names.

# Clean Column Names
- Converts all column names to lowercase.
- Replaces spaces with underscores.

# Handle Missing Values
- Replaces empty strings with NaN.
- Fills missing numeric values with **median**.
- Fills missing text values with **mode** or `"unknown"`.
- Fills missing dates with the most frequent date.

# Standardize Text Columns
- Converts all text to lowercase.
- Strips extra spaces.

# Fix Country Names
Example:  
- `USA`, `U.S.`, `US` → `united states`  
- `UK`, `england` → `united kingdom`

# Convert Date Columns
- Parses date columns into proper datetime format.
- Creates additional columns ending with `_clean` in `dd-mm-yyyy` format.

#  Remove Duplicates
- Deletes duplicate rows from the dataset.

# Convert Numeric-like Columns
Converts values like:
