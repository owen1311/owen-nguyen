# Smart Finance Assistant: Budget Buddy

## Project Overview

Budget Buddy is a Smart Finance Assistant built with Python, pandas and Gradio. The assistant helps users analyse personal finance transaction data from a CSV file.

The app allows users to upload transaction data, view a finance summary, ask simple finance questions, and calculate savings goals.

## Main Features

- Upload and read a transaction CSV file
- Validate required CSV columns
- Calculate total income
- Calculate total expenses
- Calculate net balance
- Show spending by category
- Answer finance questions using uploaded CSV data
- Provide simple budgeting and saving advice
- Calculate savings goals using a custom tool
- Display the app using a Gradio interface

## Required CSV Format

The CSV file must include the following columns:

| Column | Description |
|---|---|
| date | Date of the transaction |
| description | Short description of the transaction |
| category | Category such as Food, Housing, Transport, Utilities or Income |
| amount | Transaction amount |
| type | Either income or expense |

## Sample CSV

```csv
date,description,category,amount,type
2026-05-01,Salary,Income,2500,income
2026-05-02,Rent,Housing,900,expense
2026-05-03,Groceries,Food,120,expense
2026-05-04,Coffee,Food,8,expense
2026-05-05,Bus ticket,Transport,35,expense
2026-05-06,Phone bill,Utilities,60,expense
2026-05-07,Part-time income,Income,300,income
How to Run the Project
Open smart_finance_assistant.ipynb in Google Colab.
Run the package installation cell.
Run the import library cell.
Run all function cells.
Run the Gradio interface cell.
Open the Gradio link.
Upload sample_transactions.csv.
Use the chatbot and savings goal calculator.
How to Use the App
1. Upload CSV and Summary

Upload a transaction CSV file and click Analyse Transactions.

The app will show:

Total income
Total expenses
Net balance
Spending by category
Basic budget warning or advice
2. Finance Chatbot

After uploading the CSV file, users can ask questions such as:

Give me a summary
What is my highest spending category?
Give me saving advice
Give me budget advice
3. Savings Goal Tool

Users can enter:

Goal amount
Current savings
Monthly saving amount

The tool will calculate how many months are needed to reach the savings goal.

Project Structure
smart-finance-assistant/
│
├── smart_finance_assistant.ipynb
├── README.md
├── diary.md
├── sample_transactions.csv
└── screenshots/
Testing

The notebook includes a testing section with normal cases, edge cases and error cases.

The tests check:

Valid CSV structure
Missing CSV columns
Savings goal calculation
Invalid savings input
Chatbot response before CSV upload
Finance summary calculation
AI Collaboration

AI tools were used to help plan, code, debug and test this project. The AI collaboration process is documented in diary.md.

Author

Owen Nguyen
ISYS2001 Introduction to Business Programming
