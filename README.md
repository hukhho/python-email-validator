# Check Existence of Gmail Addresses in an Excel File
## Overview
This Python script uses the openpyxl and validate_email_address libraries to check the validity of email addresses in an Excel file and add the email status to the same file.
## Getting Started
To get started with the script, you'll need to install the following dependencies:

openpyxl
validate_email_address
You can install these dependencies using the following command:

```python
pip install openpyxl validate_email_address
```

## Usage
To use the script, follow these steps
Step 1: Clone the repository
Clone the repository to your local machine using the following command:

```python
pip install openpyxl validate_email_address
git clone https://github.com/<your-username>/<repository-name>.git
```
Step 2: Navigate to the directory
Navigate to the directory containing the script and the input Excel file:

```python
cd <repository-name>
```
Step 3: Run the script
Run the script using the following command:

```
python check_exist_gmail.py
```

Step 4: Check the output

The script will prompt you to select the input Excel file. Once selected, it will process the file and add the email status to a new column. The output file will be saved in the same directory as the input file with "_output" appended to the filename.


## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
Thank you to the creators of openpyxl and validate_email_address for providing the libraries used in this script.
Additional Information

## Input Format
The script expects the input data to be in an Excel file. The file should contain a header row and at least one column containing email addresses. The email addresses can be in any column, but the script will only check the validity of Gmail addresses.

## Output Format
The script adds a new column to the input file containing the email status for each address. The status can be one of the following values:

Live: The email address is valid and exists.
Die: The email address is invalid or does not exist.
Invalid: The cell value is not a valid email address.
The output file will be saved in the same directory as the input file with "_output" appended to the filename.

## Limitations
The script only checks the validity of Gmail addresses. If you need to check the validity of addresses from other domains, you will need to modify the script accordingly.
The script uses a ThreadPoolExecutor to speed up the processing of the input data. However, this may not be suitable for very large files or systems with limited resources. If you experience performance issues, you may need to adjust the number of worker threads or use a different approach to parallel processing.
##Contact
If you have any questions or feedback, please feel free to contact the author at hukhho@gmail.com.
