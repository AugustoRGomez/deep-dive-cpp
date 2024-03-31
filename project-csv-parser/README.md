# Project description
CSV File Parsing:
* Write a program that reads data from a CSV (Comma-Separated Values) file and displays it in a tabular format.
* Handle cases where values may contain commas or newline characters by using quotation marks.

# Objectives
* Master strin and file manipulation.

# Detailed description
Parse a CSV (Comma-Separated Values) file and display its contents in a tabular format. Here's a more detailed explanation of how you can approach this exercise:

1. Understanding CSV Format:

CSV files typically consist of rows of data, with each row separated by a newline character ('\n').
Within each row, individual data fields are separated by commas (,).
Sometimes, data fields may be enclosed within quotation marks (""), especially if they contain commas or newline characters themselves.

2. Reading the CSV File:

Open the CSV file using std::ifstream from the <fstream> header.
Read the contents of the file line by line using std::getline.
For each line, parse the individual data fields by splitting the line at each comma. You can use std::istringstream or string manipulation functions like std::stringstream and std::getline to accomplish this.
Store the parsed data fields in a suitable data structure, such as a two-dimensional std::vector or a custom-defined class representing a row of data.

3. Displaying the Data in Tabular Format:

Once you have parsed the CSV file and stored its contents, iterate over the data structure.
Print each row of data in a tabular format, aligning the columns properly.
You may need to determine the maximum width of each column to ensure proper alignment. You can do this by iterating over the data once to find the maximum length of each field.
You can use std::setw from the <iomanip> header to set the width of each column when printing.

4. Handling Quoted Fields:

If a data field is enclosed within quotation marks, it should be treated as a single field, even if it contains commas.
Modify your parsing logic to handle quoted fields appropriately. You may need to consider cases where quotation marks are escaped within quoted fields (e.g., "" to represent a single quotation mark).

5. Error Handling:

Consider how you will handle errors such as missing or malformed fields in the CSV file.
Provide informative error messages or logging to help users understand and troubleshoot any issues that arise.