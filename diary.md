# 📓 Developer Diary – Smart Finance Assistant

This developer diary documents how I used AI tools during the development of my Smart Finance Assistant project. AI was used as a coding and planning support tool, but all outputs were reviewed, tested, modified, and validated before being included in the final project.

---

## Week 8 AI Evidence Package – Project Planning and Theme Selection

### Artifact

<img width="1088" height="778" alt="week8_ai_interaction png" src="https://github.com/user-attachments/assets/d6abe14b-2f18-44d0-a046-555125cd7f66" />

### Context

I used AI to understand the Smart Finance Assistant assignment requirements and choose a project idea that was realistic, useful, and suitable for my programming level.

### Prompt Used

I need to complete a final programming project called Smart Finance Assistant for ISYS2001. The project requires a chatbot, RAG component, custom agent tool, Gradio UI, testing section, README, diary.md, and GitHub commits. Can you explain the assignment requirements in simple words and suggest a simple finance assistant idea that is suitable for a beginner?

### Reflection

At the beginning of the project, I was unsure how the required components connected together. The assignment required a chatbot, a RAG component, a custom agent tool, a Gradio interface, testing, a README file, a developer diary, and GitHub progress evidence. AI helped me break these requirements into smaller parts and understand that the project should be built as a complete application rather than separate pieces of code.

AI suggested several possible themes, including investment tracking, currency conversion, savings coaching, and budget analysis. I chose the **Budget Buddy** theme because it directly solves a practical finance problem: helping users understand their income, expenses, spending categories, and savings goals from a CSV file.

This week helped me understand the importance of planning before coding. I learned that a strong programming project should have a clear user problem, clear inputs and outputs, and a simple workflow that can be tested. I also learned that AI is most useful when it helps organise ideas, but I still need to make the final decisions based on the assignment rubric and my own ability.

---

## Week 9 AI Evidence Package – CSV Structure, Inputs, Outputs, and Pseudocode

### Artifact

<img width="1070" height="783" alt="week9_ai_interaction png" src="https://github.com/user-attachments/assets/f22dfbfa-59c9-4f3a-afde-441ba4d17212" />

### Context

I used AI to design the CSV structure, identify the required inputs and outputs, and write pseudocode before starting the Python implementation.

### Prompt Used

For my Smart Finance Assistant project, I chose the Budget Buddy theme. Can you help me design the CSV structure, identify the inputs and outputs, and write pseudocode before I start coding?

### Reflection

This week focused on planning the data structure and program logic. AI helped me design a simple and consistent CSV format with the columns `date`, `description`, `category`, `amount`, and `type`. This structure was important because the rest of the project depends on the CSV file being readable and predictable.

AI also helped me identify the main inputs and outputs of the application. The inputs include the transaction CSV file, user chatbot questions, savings goal amount, current savings, and monthly saving amount. The outputs include total income, total expenses, net balance, spending by category, chatbot advice, and savings goal results.

The pseudocode helped me understand the workflow before writing Python code. Instead of jumping straight into coding, I planned the steps: validate the CSV, clean the data, calculate summaries, create a RAG-style context, connect the chatbot, build the savings calculator, and finally create the Gradio interface.

I learned that pseudocode is useful because it reduces confusion during coding. It also helped me follow the six-step development methodology required in the assignment. AI gave me a starting structure, but I adjusted it to match my Budget Buddy theme and the final features I wanted to build.

---

## Week 10 AI Evidence Package – CSV Data Processing and Finance Summary Functions

### Artifact

<img width="1193" height="784" alt="week10_ai_interaction png" src="https://github.com/user-attachments/assets/3b482e6c-35bc-400a-ae16-f12fde126668" />

### Context

I used AI to help write Python functions for validating, loading, cleaning, and summarising transaction data from a CSV file.

### Prompt Used

I am building a Budget Buddy finance assistant in Python. Can you help me write functions to validate a CSV file, load transaction data, clean the data, and summarise total income, total expenses, net balance, and spending by category?

### Reflection

This week was focused on building the core data processing functions. AI helped me write functions such as `validate_csv()`, `load_transactions()`, and `summarise_transactions()`. These functions became the foundation of the project because the chatbot and Gradio interface rely on clean transaction data.

The most useful part of AI assistance was helping me think about validation and error handling. For example, the program needed to check whether the CSV file contained the required columns. It also needed to convert the `amount` column into numeric values and clean text fields such as `type`, `category`, and `description`.

During development, I discovered that small data issues can break the program. For example, uploading a file with missing column names caused an error. AI helped me understand how to return clear error messages instead of allowing the program to crash. I also learned how to use pandas functions such as `pd.read_csv()`, `pd.to_numeric()`, `groupby()`, and `sum()`.

I did not simply copy the AI-generated code without checking it. I tested the functions using sample transaction data and changed the code when needed. This helped me understand how the functions worked and improved my confidence with pandas and data cleaning.

---

## Week 11 AI Evidence Package – Chatbot, RAG-Style Context, Custom Tool, and Gradio UI

### Artifact

<img width="1139" height="781" alt="week11_ai_interaction png" src="https://github.com/user-attachments/assets/a5c94bcf-204a-49e6-bdf1-a9bac4c6cedf" />

### Context

I used AI to help connect the finance summary functions into a complete Gradio application with three tabs: CSV upload, finance chatbot, and savings goal tool.

### Prompt Used

Can you help me connect my Smart Finance Assistant functions into a Gradio app with three tabs: Upload CSV and Summary, Finance Chatbot, and Savings Goal Tool? The chatbot should answer questions based on the uploaded CSV data, and the savings goal tool should calculate how many months are needed to reach a savings target.

### Reflection

This week was the most important development stage because I connected the separate functions into one interactive application. AI helped me design a Gradio interface with three clear tabs: **Upload CSV and Summary**, **Finance Chatbot**, and **Savings Goal Tool**. This made the project easier for users to interact with compared to running separate code cells.

AI also helped me create a simple RAG-style component. In my project, the chatbot retrieves relevant information from the uploaded CSV data, such as total income, total expenses, net balance, top spending categories, and recent transactions. The chatbot then uses this retrieved context to answer finance-related questions. This is a simple version of RAG, but it still demonstrates the key idea of answering based on retrieved data rather than giving completely general responses.

The custom tool in my project is the savings goal calculator. It takes a goal amount, current savings, and monthly saving amount, then calculates the number of months required to reach the goal. This tool improves the business relevance of the project because it gives users a practical planning result.

One challenge was making sure the chatbot used the uploaded CSV file rather than fixed sample data. AI suggested storing the uploaded dataframe so that other functions could reuse it. I tested this by uploading `sample_transactions.csv`, asking chatbot questions, and checking whether the response matched the uploaded data.

I learned that building an application is not only about writing functions. It also requires connecting functions together, designing a usable interface, handling user input, and making sure each component works as part of the full system.

---

## Week 12 AI Evidence Package – Testing, Debugging, and Final Refinement

### Artifact

<img width="1084" height="725" alt="week12_ai_interaction png" src="https://github.com/user-attachments/assets/284f40b2-b61e-4bba-8287-87e1cee497a6" />

### Context

I used AI to create a testing and debugging section for the notebook and improve the reliability of the final application.

### Prompt Used

Can you help me create a testing and debugging section for my Smart Finance Assistant notebook? I need tests for valid CSV data, missing CSV columns, savings goal calculation, invalid savings input, chatbot use before CSV upload, and finance summary calculation.

### Reflection

This week focused on testing and debugging. AI helped me identify important test cases for normal situations, edge cases, and error cases. I added tests for valid CSV data, missing CSV columns, savings goal calculation, already reached savings goal, invalid monthly saving amount, chatbot use before CSV upload, and finance summary calculation.

Testing helped me find and understand problems in the project. For example, I had issues with CSV files missing required columns and Gradio app links not opening correctly. I also learned that the Gradio app can keep a cell running because it is hosting the interface. To manage this, I adjusted the launch settings and made sure the testing section could still be shown clearly in the notebook.

AI helped me generate testing ideas, but I reviewed the tests to make sure they matched my actual functions. I used `assert` statements because they clearly show whether a function produces the expected result. This made the testing section stronger than only printing outputs.

This week improved the reliability of the final project. I learned that debugging is an important part of programming because a project should not only work with perfect data. It should also handle user mistakes, missing files, invalid values, and unexpected input.

---

# Final Reflection

This project helped me improve my programming, problem-solving, and AI collaboration skills. I learned how to build a small end-to-end finance application using Python, pandas, and Gradio.

The most important technical skills I developed were:

- loading and validating CSV files
- cleaning transaction data
- calculating income, expenses, net balance, and category spending
- creating a simple RAG-style context from uploaded data
- building a finance chatbot
- creating a custom savings goal calculator tool
- designing a Gradio web interface
- writing tests for normal and error cases

AI was useful throughout the project, especially for planning, explaining code structure, generating first drafts, and suggesting tests. However, I learned that AI-generated code still needs to be checked carefully. I had to test the code, understand what each function did, fix errors, and make sure the final notebook matched the assignment rubric.

The main challenge was connecting all components into one working application. The project required more than just writing individual functions. I had to make sure the CSV upload, finance summary, chatbot, RAG-style context, savings tool, Gradio interface, and testing section all worked together.

Overall, this project helped me understand how AI can support software development while still requiring human judgement, testing, and responsibility. I now feel more confident using AI as a coding assistant and building simple business-focused applications in Python.
