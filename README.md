# SQL Server Interview Playbook

**The 50 most-asked SQL interview questions, answered for Microsoft SQL Server.** Diagrams, T-SQL examples and the follow-up questions interviewers ask next. 2026 edition.

By **Deepankar Sir** | [Instagram @datawithdeepankar](https://instagram.com/datawithdeepankar) | [YouTube @deepankarpathak983](https://youtube.com/@deepankarpathak983)

**50** questions | **6** parts | **18** diagrams

---

## Who this is for

Freshers and experienced developers preparing for SQL interviews at:

- **Service companies:** TCS, Infosys, Wipro, Accenture, Cognizant
- **Global capability centres:** JP Morgan, Goldman Sachs, Wells Fargo, Walmart Labs, Target, AmEx
- **Indian product companies:** Razorpay, Swiggy, Cred, Meesho, Zerodha, Flipkart, PhonePe

Every answer is written for **Microsoft SQL Server and T-SQL**.

## What's inside

| Part | Topic | Questions |
|------|-------|-----------|
| 1 | Join Foundations & NULL Logic | Q01 to Q06 |
| 2 | Existence Checks & Advanced Joins | Q07 to Q11 |
| 3 | Window Functions | Q12 to Q22 |
| 4 | Modern T-SQL Toolkit | Q23 to Q30 |
| 5 | Indexes & Query Performance | Q31 to Q40 |
| 6 | Transactions, Isolation & Concurrency | Q41 to Q50 |

Parts 1 to 3 build query-writing skill. Part 4 adds modern T-SQL features. Parts 5 and 6 cover the engine-level topics that separate a fresher from an experienced developer.

## How every question is laid out

- **The interviewer asks:** the question as you are likely to hear it
- **Answer in 30 seconds:** say this first
- **Build the answer step by step:** the structure for a fuller two-minute answer
- **Edge cases that impress:** the details interviewers wait to hear
- **Avoid saying:** common statements that cost candidates the round
- **Likely follow-up:** the next question, with a model answer

## Two-pass study plan

1. **Pass 1 (about 2 hours):** read only the question and the 30-second answer for all 50. Say each answer aloud.
2. **Pass 2:** for every question you could not explain comfortably, work through the steps, the diagram and the code.

## Practice schema

All examples use a simplified **ShopSmart India** retail database (`Customers`, `Orders`, `Payments`, `Employees`, `Wallets`, `Products`, `Sellers`, `Stores`). The schema is on page 2 of the PDF. Create the tables in a practice database to run every snippet.

## The ten traps that decide most SQL rounds

1. A right-table filter in `WHERE` turns a `LEFT JOIN` into an `INNER JOIN` (Q01)
2. One `NULL` in a `NOT IN` subquery returns zero rows, so prefer `NOT EXISTS` (Q07)
3. Joins multiply rows; `EXISTS` does not (Q08)
4. `ROW_NUMBER` drops ties; `DENSE_RANK` keeps them (Q12)
5. The default window frame is `RANGE`, not `ROWS` (Q17)
6. `LAST_VALUE` needs an explicit frame to the end of the partition (Q18)
7. Window functions cannot go in `WHERE`, and SQL Server has no `QUALIFY` (Q21)
8. Functions on a column and implicit conversions block index seeks (Q37)
9. Use `SET XACT_ABORT ON`, or a failed statement can leave a transaction half-done (Q41)
10. SQL Server's `REPEATABLE READ` still allows phantom reads (Q45)

## Requirements

- SQL Server 2017 or later, and SQL Server Management Studio or Azure Data Studio
- A few examples need newer versions, and the playbook marks them: `IS DISTINCT FROM`, `GENERATE_SERIES`, `DATETRUNC` and `IGNORE NULLS` need SQL Server 2022, and the native `json` type needs SQL Server 2025

## Also in this series

**[SQL Interview Kit: 10 Patterns](https://github.com/learnwithdeepankarpathak-dot/sql-interview-kit-10-patterns)** has 10 worked multiple-choice questions plus 20 practice problems with full solutions.

## Follow for more

A new SQL Server interview question every day on Instagram: **[@datawithdeepankar](https://instagram.com/datawithdeepankar)**

Questions about the playbook? Send a DM.

---

*Prepared by Deepankar Sir, MarutiNovaTech.*
