## Exercise: Console-based GUI for International Bank Database

### Objective:
Create a console-based GUI application for managing an international bank database. The application should allow users to search for accounts by Account ID or Customer Name, create new accounts, delete accounts, and display the database. Additionally, the application should load the database from a CSV file when started and save the updated database to the same CSV file when closed.

### Features:
1. **Search Accounts:** Users should be able to search for accounts by Account ID or Customer Name. If multiple accounts match the search criteria, display all matching accounts.

2. **Create Account:** Users should be able to create a new account by providing customer details such as Customer Name, Customer Age, Customer City, Customer Country, Bank Account Number, and Current Amount of Money. The Customer ID should be automatically assigned based on the current number of accounts in the database.

3. **Delete Account:** Users should be able to delete an account by entering the Account ID.

4. **Display Database:** Users should have the option to display the entire database, showing all account details.

5. **Load Database:** The application should load the database from a CSV file when started. The CSV file should have the following columns: "Customer ID", "Customer Name", "Customer Age", "Customer City", "Customer Country", "Bank Account Number", and "Current Amount of Money".

6. **Save Database:** When the application is closed, it should save the updated database to the same CSV file, overwriting the existing data.

7. **Error Handling:** The application should raise a warning if the provided CSV file is malformed or corrupted, indicating that the database cannot be loaded.

### Instructions:
1. Upon starting the application, load the database from the CSV file.
2. Display a menu with options to search accounts, create account, delete account, display database, and exit.
3. Implement each feature as described above.
4. Ensure error handling for cases such as invalid input, non-existent accounts, and file loading errors.
5. When the application is closed, save the updated database to the CSV file.

### CSV Database Examples:
- Use the provided CSV databases (`well_formed_database.csv` and `malformed_database.csv`) to test your application. These databases contain sample account data.
- The well-formed database (`well_formed_database.csv`) has properly formatted data for all entries.
- The malformed database (`malformed_database.csv`) contains some entries with missing bank account numbers and other formatting issues.

### Additional Notes:
- You can choose any programming language for implementing the application, but make sure it runs in a console environment.
- Focus on creating a user-friendly interface and robust error handling.
- Test your application thoroughly with different scenarios to ensure its correctness.
