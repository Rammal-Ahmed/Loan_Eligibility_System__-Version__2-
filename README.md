Bank Loan Eligibility Report (Version 2)
A beginner-friendly Python console application that collects customer details, summarizes key financial information, and checks basic loan eligibility criteria in a clean, formatted report.
Overview
This project demonstrates how Python can be used to collect user input, perform simple calculations, apply conditional logic, and present results in a readable console report. It calculates annual income from monthly income and provides a preliminary eligibility outcome based on the rules defined in the program.
Note: This is an educational project, not a real bank assessment or a guarantee of loan approval. Actual lending decisions depend on each lender's policies and a wider range of financial information.

Features
- Collects the customer's name, age, monthly income, account balance, and existing pending loan amount.
- Calculates annual income from monthly income.
- Displays a structured customer financial summary.
- Checks age, minimum monthly income, and existing loan criteria individually.
- Explains which eligibility criteria are not met.
- Presents a final preliminary status in a formatted console report.
Eligibility Rules
The program marks a customer as eligible for further review only when all three checks pass.
Criterion	Rule
Age	18 to 95 years, inclusive
Monthly income	At least Rs. 30,000
Existing pending loan	Less than Rs. 500,000


Implementation detail: The account balance is collected and shown in the report, but it is not currently used in the eligibility decision.
Suggested Project Structure
bank-loan-eligibility-report/
├── README.md
├── loan_eligibility.py
└── .gitignore
Keep the Python source file at the project root and use the README as the first place visitors go to understand the project.
Requirements
- Python 3
- No third-party packages are required
How to Run
1. Install Python 3 if it is not already installed.
2. Save the program in a file named loan_eligibility.py.
3. Open the project folder in VS Code.
4. Open the integrated terminal from Terminal → New Terminal.
5. Run the program:
   python loan_eligibility.py
   On Windows, you can also try:
   py loan_eligibility.py
6. Enter the requested customer details when prompted. Use numeric values for age and financial amounts.
Example
For a customer aged 30 with a monthly income of Rs. 60,000 and an existing pending loan of Rs. 200,000, the three eligibility checks pass. The report displays Eligible for Further Review. This is only the result of the program's predefined rules.
Concepts Practised
- input() and type conversion with int()
- Variables and arithmetic operations
- if / else conditional statements
- Boolean flags for tracking eligibility
- Formatted console output using print() and string methods
Possible Improvements
- Validate input to handle non-numeric or negative values gracefully.
- Add further checks, such as account balance, if the project requirements define how they should affect eligibility.
- Separate the assessment logic into functions and add automated tests.
