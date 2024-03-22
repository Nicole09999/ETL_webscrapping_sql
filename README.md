# ETL Operations on world largest banks Data

This Python script performs ETL (Extract, Transform, Load) operations on data related to the largest banks, extracted from a Wikipedia page.

## Objective:
The objective of this script is to extract information about the largest banks from a Wikipedia page, transform the data by converting market capitalization values to different currencies, and load the transformed data into a CSV file and a SQLite database.

## Prerequisites:
Ensure that the following libraries are installed:
- `requests`: For making HTTP requests to retrieve web pages.
- `BeautifulSoup`: For parsing HTML content.
- `pandas`: For data manipulation and analysis.
- `sqlite3`: For working with SQLite databases.
- `numpy`: For numerical computing.
- `datetime`: For working with dates and times.

## Usage:
1. Install the required libraries mentioned above.
2. Run the script `bank_data_etl.py`.
3. The script will perform the following operations:
   - Extract data from the Wikipedia page containing information about the largest banks.
   - Transform the data by converting market capitalization values to GBP, EUR, and INR.
   - Load the transformed data into a CSV file and a SQLite database.
   - Execute predefined queries on the database to demonstrate data retrieval.
4. Review the log file `code_log.txt` for details on each stage of the process.

## Files:
- `bank_data_etl.py`: Main Python script for ETL operations.
- `exchange_rate.csv`: CSV file containing exchange rates for currency conversion.
- `Banks.db`: SQLite database file where the data is loaded.
- `Largest_banks_data.csv`: CSV file containing the transformed data.

## Functions:
- `extract(url, table_attribs)`: Extracts data from the Wikipedia page and returns a DataFrame.
- `transform(df, csv_path)`: Transforms the DataFrame by converting market cap to different currencies.
- `load_to_csv(df, output_path)`: Saves the DataFrame as a CSV file.
- `load_to_db(df, sql_connection, table_name)`: Loads the DataFrame into a SQLite database.
- `run_query(query_statement, sql_connection)`: Executes SQL queries on the database.

## Logging:
The script logs each stage of the ETL process to the `code_log.txt` file, including timestamps for tracking execution progress.

---

This README provides an overview of the code, its usage, prerequisites, files involved, functions, and logging. Please ensure that the prerequisites are met before running the script, and refer to the log file for detailed progress updates during execution.

<img width="323" alt="Task_1_log_function" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/0b0abbf2-f2bc-4abd-b707-806dae24172d">
<img width="960" alt="Task_2a_extract" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/955abcf8-150b-4b36-b8d0-8fa545f6368d">
<img width="607" alt="task_2c_extract" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/d5c71fb7-b531-4cbc-8d18-7f22c57db111">
<img width="476" alt="task_2b_extract" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/cf2d5ece-d139-4346-9c41-ff6cb1a51214">

<img width="469" alt="task_3a_transform" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/45422e98-f854-4d2f-ae39-7feb57bcd937">
<img width="517" alt="Task_4_csv" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/f1a9a3ee-9365-42c4-9652-f46ac41b1db8">
<img width="488" alt="Task_4_5_save_file" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/fae68176-0834-4edc-ae61-eac7c0b25754">
<img width="665" alt="Task_6_SQL" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/c07cb170-99a4-4093-aac0-095b43289b66">
<img width="593" alt="task_3b_transform" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/5c552eec-6677-49ab-950a-9e8adeabc480">
<img width="488" alt="Task_7_log_content" src="https://github.com/Nicole09999/ETL_webscrapping_sql/assets/106644205/322c71f7-2671-4662-b00d-1c5f645c6b46">

