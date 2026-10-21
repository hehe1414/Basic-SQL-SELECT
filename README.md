# Basic SQL SELECT – Northwind

**Task 21 – Basic SQL SELECT**
Veda Technology | Data Analytics Track | Level 1, Day 21

## About
I wrote 10 simple SQL queries using `SELECT`, `WHERE` and `ORDER BY` (plus `DISTINCT`, `TOP`, `AND`, `IN`, `LIKE` and column aliases) on the Northwind sample database, and saved a screenshot of each output.

**Where I ran them:** the W3Schools Try-SQL editor, which has the Northwind sample database (it runs SQLite).

## What I practiced
| Keyword | What it does |
|---------|--------------|
| `SELECT` | Chooses which columns to show |
| `FROM` | Says which table to read |
| `WHERE` | Keeps only the rows that match a condition |
| `ORDER BY` | Sorts the result (`ASC` is the default, `DESC` is highest first) |
| `DISTINCT` | Removes duplicate values |
| `TOP` (SQL Server) / `LIMIT` (MySQL, PostgreSQL) | Shows only the first N rows |
| `AND`, `IN`, `LIKE` | Combine conditions, match a list, match a pattern |
| `AS` | Gives a column a friendlier name |

## The 10 queries and their outputs
| # | What the query does | Rows returned | Output |
|---|--------------------|---------------|--------|
| 1 | Shows everything in the Customers table | 91 | `outputs/q1.png` |
| 2 | Shows only customer name, city and country | 91 | `outputs/q2.png` |
| 3 | Lists each country once | 21 | `outputs/q3.png` |
| 4 | Finds customers from Germany | 11 | `outputs/q4.png` |
| 5 | Finds products that cost more than 50 | 7 | `outputs/q5.png` |
| 6 | Lists products from most to least expensive | 77 | `outputs/q6.png` |
| 7 | Shows the 5 most expensive products (uses `TOP 5`) | 5 | `outputs/q7.png` |
| 8 | Finds customers in Berlin, Germany | 1 | `outputs/q8.png` |
| 9 | Customers from France, Spain or Italy, sorted | 19 | `outputs/q9.png` |
| 10 | Products starting with C, with aliases | 9 | `outputs/q10.png` |

The full queries are in `queries.sql`, written with the keywords in capitals and one clause per line so they are easy to read.

## What I learned
- Start with a simple `SELECT *` and then narrow it down with specific columns and `WHERE`
- `ORDER BY ... DESC` plus `TOP` (SQL Server) or `LIMIT` (MySQL and PostgreSQL) gives a quick top-N list. My first attempt with `LIMIT` gave a syntax error in SQL Server, which taught me that the same idea is written differently in different databases
- Formatting a query with one clause per line makes it much easier to read and fix

## Files
- `queries.sql` – the 10 queries
- `outputs/` – a screenshot of each query output
- `README.md`

## Tools used
SQL (Northwind sample database)

## Author
Rabia
