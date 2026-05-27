# 💰 Smart Finance Assistant: Budget Buddy


## 📌 Project Overview

**Budget Buddy** is a Smart Finance Assistant built with **Python, pandas, and Gradio**.

The assistant helps users analyse personal finance transaction data from a CSV file. Users can upload transaction data, view a finance summary, ask simple finance questions, and calculate savings goals through an interactive Gradio interface.

This project was developed for the **ISYS2001 Introduction to Business Programming** final programming project.

---

## 🚀 Main Features

- Upload and read a transaction CSV file
- Validate required CSV columns
- Calculate total income
- Calculate total expenses
- Calculate net balance
- Show spending by category
- Answer finance questions using uploaded CSV data
- Provide simple budgeting and saving advice
- Calculate savings goals using a custom tool
- Display the app using a Gradio web interface
- Include testing and debugging examples in the notebook

---

## 📂 Required CSV Format

The CSV file must include the following columns:

| Column | Description |
|---|---|
| `date` | Date of the transaction |
| `description` | Short description of the transaction |
| `category` | Category such as Food, Housing, Transport, Utilities or Income |
| `amount` | Transaction amount |
| `type` | Either `income` or `expense` |

---

## 🧾 Sample CSV

```csv
date,description,category,amount,type
2026-05-01,Salary,Income,2500,income
2026-05-02,Rent,Housing,900,expense
2026-05-03,Groceries,Food,120,expense
2026-05-04,Coffee,Food,8,expense
2026-05-05,Bus ticket,Transport,35,expense
2026-05-06,Phone bill,Utilities,60,expense
2026-05-07,Part-time income,Income,300,income
```

The sample file used for testing is included in this repository as:

```text
sample_transactions.csv
```

---

## ▶️ How to Run the Project

1. Open `starter_notebook.ipynb` in Google Colab.
2. Run the package installation cell.
3. Run the import library cell.
4. Run all function cells.
5. Run the Gradio interface cell.
6. Open the Gradio link.
7. Upload `sample_transactions.csv`.
8. Use the finance chatbot and savings goal calculator.

---

## 🖥️ How to Use the App

### 1. Upload CSV and Summary

Upload a transaction CSV file and click **Analyse Transactions**.

The app will show:

- Total income
- Total expenses
- Net balance
- Spending by category
- Basic budget warning or advice

---

### 2. Finance Chatbot

After uploading the CSV file, users can ask questions such as:

- Give me a summary
- What is my highest spending category?
- Give me saving advice
- Give me budget advice

The chatbot uses uploaded CSV data to provide simple finance-related responses.

---

### 3. Savings Goal Tool

Users can enter:

- Goal amount
- Current savings
- Monthly saving amount

The tool calculates how many months are needed to reach the savings goal.

---

## 🧠 Project Components

| Component | Description |
|---|---|
| CSV Processing | Loads, validates, and cleans transaction data |
| Finance Summary | Calculates income, expenses, net balance, and spending by category |
| RAG-style Context | Retrieves relevant information from uploaded CSV data |
| Finance Chatbot | Answers finance questions using uploaded transaction data |
| Custom Tool | Calculates savings goal timeline |
| Gradio UI | Provides an interactive web interface |
| Testing Section | Tests normal, edge, and error cases |

---

## 🗂️ Project Structure

```text
owen-nguyen/
│
├── README.md
├── LICENSE
├── diary.md
├── sample_transactions.csv
├── starter_notebook.ipynb
├── smart_finance_project.md
└── AI-CONVERSATIONS/
```

---

## 📄 Main Files

| File | Purpose |
|---|---|
| `starter_notebook.ipynb` | Main Google Colab notebook containing the Smart Finance Assistant code, six-step methodology, testing section, and Gradio app |
| `README.md` | Project overview, features, CSV format, setup instructions, and project structure |
| `diary.md` | Developer diary documenting AI collaboration and weekly progress |
| `sample_transactions.csv` | Sample transaction data used to test the finance assistant |
| `AI-CONVERSATIONS/` | Folder containing AI evidence screenshots or conversation evidence |
| `LICENSE` | MIT License from the starter template |
| `smart_finance_project.md` | Additional project notes or documentation |

---

## ✅ Testing

The notebook includes a testing section with normal cases, edge cases, and error cases.

The tests check:

- Valid CSV structure
- Missing CSV columns
- Savings goal calculation
- Invalid savings input
- Chatbot response before CSV upload
- Finance summary calculation

Testing was included to confirm that the assistant works correctly and handles common user errors.

---

## 🤖 AI Collaboration

AI tools were used to help plan, code, debug, and test this project.

The AI collaboration process is documented in:

```text
diary.md
```

The diary includes evidence of AI use, context, and reflections on what worked, what needed improvement, and what was learned during development.

---

## 📚 Starter Template and License

This project was developed using the Smart Finance Assistant starter template by **Michael Borck** and modified for the ISYS2001 final programming project.

The original template is provided under the MIT License. The license file is included in this repository.

---

## 👤 Author

**Owen Nguyen**  
ISYS2001 Introduction to Business Programming  
Smart Finance Assistant Final Programming Project
