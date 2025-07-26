# Pandas
## Python - Pandas : Data Cleaning &amp; EDA

### Data Cleaning with Pandas: Customer Call List
This project demonstrates basic data cleaning and preparation techniques using the pandas library in Python. The goal is to take a messy customer call list, clean it up, and make it ready for use. The entire process is documented in the Data Cleaning.ipynb Jupyter Notebook.

📝 Project Overview
The main objective of this project is to apply various data cleaning methods to a raw customer call list from an Excel file. This includes handling duplicate entries, correcting formatting inconsistencies, parsing and splitting columns, and removing irrelevant data. By the end of this process, the dataset is transformed into a clean, well-structured format that can be easily used for analysis or by a call center.

🧹 Data Cleaning Steps
The following cleaning and transformation tasks were performed on the dataset:

Duplicate Removal: All duplicate rows were identified and removed to ensure data integrity.

Standardizing Text Data:

In the Last_Name column, unnecessary characters like . , _ , and / were removed from the names.

The Paying Customer and Do_Not_Contact columns were standardized to use 'Y' for "Yes" and 'N' for "No".

Cleaning and Formatting the Phone Numbers:

Removed all non-alphanumeric characters (e.g., -, /, |) from the Phone_Number column.

Formatted the phone numbers into a consistent XXX-XXX-XXXX format.

Handled and removed invalid entries like N/a and NaN values.

Address Parsing:

The Address column was split into three new columns: Street_Address, State, and Zipcode for better organization and usability.

Handling Missing Data:

Empty and NaN values were filled with empty strings to maintain consistency.

Removing Unwanted Records:

Rows with a 'Y' in the Do_Not_Contact column were removed, as these customers should not be called.

Any records without a valid phone number were also removed to create a useful call list.

Final Touches:

The Not_Useful_Column was dropped as it contained no valuable information.

The DataFrame index was reset after all the cleaning and filtering steps to ensure a clean final output.

🛠️ Tools and Libraries Used
Python: The core programming language for data manipulation.

Pandas: A powerful library for data analysis and manipulation, used for all data cleaning tasks.

Jupyter Notebook: An interactive environment to write and execute the Python code.



jupyter notebook
Open the notebook:
In the Jupyter Notebook interface, open the Data Cleaning.ipynb file and run the cells sequentially to see the data cleaning process in action.
