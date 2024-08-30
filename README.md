# CreditClean30Days

## Description

**CreditClean30Days** is a Python script designed to process credit check data by filtering out records based on a 30-day window. The script removes duplicate credit check entries that occur within 30 days of each other, retaining only the most relevant records for each customer.

## Features

- **Load Data:** Reads a CSV file with tab-separated values.
- **Clean Data:** Removes unnecessary columns and normalizes data.
- **Filter Data:** Applies a 30-day filter to remove duplicate records.
- **Save Results:** Outputs the cleaned data to a new CSV file.

## Installation

1. **Clone the Repository:**

    ```bash
    git clone <repository-url>
    cd CreditClean30Days
    ```

2. **Install Required Packages:**

   Ensure you have Python installed, and then install the required packages using:

    ```bash
    pip install pandas
    ```

## Usage

1. **Prepare Your Data:**

   Place your input CSV file in the `data/input/` directory. Ensure the file uses tab delimiters and contains the columns expected by the script.

2. **Run the Script:**

   Execute the Python script with:

    ```bash
    python scripts/data_processing.py
    ```

3. **Check Results:**

   The cleaned data will be saved in the `data/output/` directory as `Credit Checks Approval Rates test.csv`.

## File Structure

- **`data/input/`**: Directory for input CSV files.
- **`data/output/`**: Directory for output CSV files.
- **`scripts/data_processing.py`**: The main script for processing the data.
- **`README.md`**: This file, providing an overview and instructions.

## Example Data

**Input CSV**:
- Must be a tab-delimited file with at least the columns: `OCCURRED AT`, `CUSTOMER NAME`, and other relevant fields.

**Output CSV**:
- The output will be a tab-delimited file with the filtered data, excluding records that fall within 30 days of each other.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. Ensure that your code adheres to the project's guidelines and includes appropriate tests.

## Contact

For any questions or feedback, please contact:

- [Olga Kisel](mailto:okisel@protonmail.com)
