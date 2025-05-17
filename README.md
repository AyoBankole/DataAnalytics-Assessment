# Customer Savings and Investment Analysis

This repository contains a comprehensive set of SQL scripts and data assessment files designed to analyze customer savings and investment behaviors. The project focuses on customer segmentation, inactivity detection, and financial metric calculations using MySQL.

## Contents

- **adashi_assessment.sql**  
  Defines the database schema and tables for the `adashi_staging` database.

- **Assessment_Q1.sql**  
  Queries to identify users with regular savings and investment activities, including summaries of deposits.

- **Assessment_Q2.sql**  
  Queries to categorize customers based on their transaction frequency (High, Medium, Low) and summarize activity metrics.

- **Assessment_Q3.sql**  
  Queries to detect inactive savings plans, providing inactivity durations and last transaction dates.

- **Assessment_Q4.sql**  
  Queries to calculate key customer metrics such as tenure, total transactions, and estimated Customer Lifetime Value (CLV).

## Purpose

These scripts serve as data analytics assessments aimed at understanding customer financial behavior, segmenting users by activity levels, and calculating important business metrics to inform decision-making.

## Usage

1. Import the `adashi_assessment.sql` file to set up the database schema.
2. Run each assessment SQL script (`Assessment_Q1.sql` to `Assessment_Q4.sql`) on the database.
3. Review the query results to analyze customer savings and investment patterns.

## Requirements

- MySQL Server (version 5.7+ recommended)
- Access to the `adashi_staging` database or equivalent with the relevant tables.

## Contact

For questions or contributions, please open an issue or submit a pull request.

---

*This repository is intended for educational and assessment purposes related to customer financial data analytics.*
