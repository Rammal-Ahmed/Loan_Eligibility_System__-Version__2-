# Bank Loan Eligibility Report (Version 2)

A simple command-line program written in Python that checks whether a customer meets the basic criteria for a bank loan. You enter a few details, and it prints a neat financial summary followed by a clear, criterion-by-criterion eligibility result.

This is Version 2 of the project. The first version only gave a yes or no. This one explains *why*, so the result is easier to read and trust.

---

## What it does

- Takes the customer's name, age, monthly income, account balance and existing loan amount
- Calculates the annual income automatically
- Prints a formatted financial summary
- Checks three eligibility criteria and shows a reason whenever one is not met
- Ends with a final status: eligible for further review, or not eligible

## Eligibility criteria

| Criteria | Requirement |
|---|---|
| Age | Between 18 and 95 years |
| Monthly income | At least Rs. 30,000 |
| Existing loan | Below Rs. 500,000 |

A customer needs to pass all three to be marked as *Eligible for Further Review*. Account balance is recorded in the summary but is not part of the eligibility check in this version.

## Getting started

You only need Python 3 installed. No external libraries are used.

```bash
# clone the repository
git clone https://github.com/your-username/bank-loan-eligibility-report.git

# move into the folder
cd bank-loan-eligibility-report

# run the program
python loan_eligibility.py
```

## Sample run

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   BANK LOAN ELIGIBILITY REPORT (VERSION 2)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Enter Customer Name: Ayesha Khan
Enter Customer Age: 28
Enter Current Monthly Income Rs: 65000
Enter Current Account Balance Rs: 150000
Enter Existing Pending Loan Amount Rs: 200000

=============================================
          CUSTOMER FINANCIAL SUMMARY
=============================================

Customer Name       : Ayesha Khan
Customer Age        : 28
Monthly Income      : Rs  65000
Annual Income       : Rs  780000
Account Balance     : Rs  150000
Existing Loan       : Rs  200000

=============================================
            ELIGIBILITY ASSESSMENT
=============================================

Age Criteria        : Eligible
Income Criteria     : Eligible
Existing Loan       : Eligible

=============================================

Status: Eligible for Further Review
Your details meet the basic eligibility criteria
```

If a criterion is not met, the report points it out with a short reason, for example:

```
Income Criteria     : Not Eligible
Reason: Minimum monthly income is Rs. 30,000/-
```

## What I practiced

- Taking and converting user input with `input()` and `int()`
- Decision making with `if` / `else` and combined conditions
- Using a flag variable (`eligible`) to track the overall result
- Formatting terminal output with `center()` and string repetition

## Ideas for the next version

- Handle invalid input (letters instead of numbers, negative values)
- Add a loan amount request and compare it with income
- Use functions to split the code into smaller, reusable parts
- Save each report to a text or CSV file
- Let the program run for multiple customers in one session

## Note

This is a learning project built to practice Python fundamentals. The criteria are simple examples and do not reflect the real lending policy of any bank.

## Author

Rammal Ahmed
LinkedIn: www.linkedin.com/in/rammal-ahmed-58184b325     GitHub: https://github.com/Rammal-Ahmed

Feedback and suggestions are always welcome
