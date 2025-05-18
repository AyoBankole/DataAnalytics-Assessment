# Customer Savings and Investment Analysis -DataAnalytics-Assessment

This repository contains SQL scripts developed to analyze customer savings and investment behavior using MySQL. The assessment is divided into four questions, each focusing on a specific area of user behavior or data insight.

---

## Repository Structure

```
DataAnalytics-Assessment/
│
├── Assessment_Q1.sql       # Identifies users with regular savings/investment activities
├── Assessment_Q2.sql       # Categorizes users by transaction frequency
├── Assessment_Q3.sql       # Detects inactive savings plans
├── Assessment_Q4.sql       # Calculates tenure, transactions, and CLV
│
└── README.md               # Project overview, methodology, and challenges
```

---

## Per-Question Explanations

### **Assessment_Q1.sql** – Regular Savers & Investors
**Approach:**  
This query identifies users who actively save or invest by filtering transactions with a confirmed status. It calculates total deposits, identifies those saving monthly, and highlights consistent behavior. The result helps in segmenting users who are financially disciplined.

---

### **Assessment_Q2.sql** – Customer Categorization by Frequency
**Approach:**  
Users are classified into `High`, `Medium`, or `Low` transaction categories based on the frequency of confirmed deposits. I used `CASE` statements along with `COUNT` and `GROUP BY` to summarize how often users transact, providing useful input for targeted marketing or engagement.

---

### **Assessment_Q3.sql** – Inactive Savings Plans
**Approach:**  
This query identifies savings accounts that haven't had a confirmed transaction in over 90 days. By using `MAX(transaction_date)` and comparing with the current date, I was able to detect dormancy. This is useful for flagging inactive accounts for re-engagement strategies.

---

### **Assessment_Q4.sql** – Tenure, Transactions & CLV
**Approach:**  
This query calculates:
- **Customer Tenure** using `TIMESTAMPDIFF`
- **Total Transactions** with `COUNT`
- **Estimated CLV** with a derived formula using average confirmed deposit and tenure-adjusted transaction rate

It provides a summary metric to estimate long-term customer value.

---

## Challenges Encountered

### 1. **Using MySQL CLI for the First Time**
Coming from tools like Azure Data Studio and Oracle APEX, MySQL CLI was unfamiliar at first. However, my experience with terminal-based development helped me adapt quickly. I became efficient with command-line querying, database creation, and troubleshooting syntax errors.

### 2. **Formatting and Copying Queries**
I initially ran and wrote queries in Oracle APEX for better formatting. However, copying queries with inline comments into MySQL CLI introduced formatting issues. I resolved this by writing queries and comments in a text editor (VS Code or Notepad) before pasting into the CLI to ensure proper formatting.

### 3. **Saving Queries from MySQL CLI**
Since MySQL CLI doesn’t support saving queries natively, I manually copied my work and organized it into `.sql` files. This preserved formatting and ensured the code was clean and ready for version control.

### 4. **Git and GitHub Issues**
- I mistakenly added large database files to my repo, causing errors when pushing to GitHub.
- I encountered a `fatal: refusing to merge unrelated histories` error due to a mismatch between local and remote histories.
- I resolved this by:
  - Deleting large files locally and committing changes
  - Using `git pull origin main --allow-unrelated-histories`
  - Resetting the push with proper `.sql` files only

---

## Final Reflection

Completing this assessment within 48 hours tested not just my SQL knowledge but also my adaptability and problem-solving mindset.  
> **Resilience wasn’t an option — it became a tool.**

This project taught me that knowing how to query a database is important, but knowing how to troubleshoot, manage your tools, and complete the cycle from analysis to delivery is what makes a strong data analyst.

---

## Author

**Ayobami Ogunsanya**  
🔗 [GitHub Profile](https://github.com/AyoBankole)

*This repository is intended for educational and assessment purposes related to customer financial data analytics.*
