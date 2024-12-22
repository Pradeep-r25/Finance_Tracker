# Finance_Tracker
A Python-based Personal Finance Manager to help users track and analyze their financial transactions. This project simplifies expense and income management by storing transactions in a CSV file and providing features like transaction filtering, summary reports, and graphical analysis.

## Features
- Add new income/expense transactions.
- View transactions and a summary of income, expense, and net savings within a specified date range.
- Plot income and expense trends over time.

## Requirements
- Python 3.x
- Libraries:
  - pandas
  - matplotlib
  - datetime

You can install the required libraries by running:
```bash
pip install pandas matplotlib
Files
main.py: Main script that handles the logic for adding transactions, viewing transactions, and plotting data.
data_entry.py: Contains helper functions for data input, including getting the date, amount, category (income or expense), and description.
finance_data.csv: CSV file where all transactions are stored.
How to Run the Program
Step 1: Install Dependencies
First, ensure you have Python 3.x installed. Then, open a terminal and navigate to the project directory.

Install the required libraries by running:

bash
Copy code
pip install pandas matplotlib
Step 2: Run the Program
To run the main.py script, open a terminal or command prompt in the project folder and execute the following command:

bash
Copy code
python main.py
Step 3: Interact with the Program
Once the program is running, you will see a menu with the following options:

Add a new transaction
View transactions and a summary within a date range
Exit
You can follow the prompts to add transactions, view transaction summaries for specific date ranges, and visualize the income/expense data in graphical format.

Example Usage
bash
Copy code
1. Add a new transaction
2. View Transactions and a summary within a date range
3. Exit
Enter Your Choice (1-3): 1
Enter the date of the transaction (dd-mm-yyyy) or press Enter for today's date: 21-12-2024
Enter the amount: 1000
Enter the Category ('I' for Income or 'E' for Expense): I
Enter a description (optional): Freelance work

1. Add a new transaction
2. View Transactions and a summary within a date range
3. Exit
Enter Your Choice (1-3): 2
Enter the start date (dd-mm-yyyy): 01-12-2024
Enter the end date (dd-mm-yyyy): 21-12-2024
Transactions from 01-12-2024 to 21-12-2024
date        amount  category    description
21-12-2024   1000.0   Income    Freelance work

Summary:
Total Income: Rs. 1000.00
Total Expense: Rs. 0.00
Net Savings: Rs. 1000.00
Do you want to see a plot? (y/n) y
Directory Structure
bash
Copy code
finance_tracker/
├── main.py              # Main script
├── data_entry.py        # Input helper functions
├── finance_data.csv     # CSV data file
└── README.md            # Project documentation
Notes
The CSV file stores the data in the format dd-mm-yyyy for dates, and each transaction includes the amount, category (Income or Expense), and an optional description.
The program uses matplotlib to plot income and expense trends over time.
