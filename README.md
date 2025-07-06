# Splitwise Expense Balancer

*Greedy recursion-based group expense splitter*

## 📌 Overview

This project implements a Splitwise-style group expense settlement system in C++. It takes a list of people with net balances (positive for those who should receive money and negative for those who owe money) and calculates the minimal number of transactions needed to settle all debts using a greedy recursive approach.

## 💡 How It Works

- Debtors and creditors are matched optimally to minimize total transactions.
- In each recursive step, the person with the highest debt pays the person with the highest credit.
- The process continues until all balances become zero.

## 🧠 Example

### Input:
```plaintext
A: -5  
B: 25  
C: -20  
D: 25  
E: -20  
F: -5

Output:
C needs to pay D: 20.00  
E needs to pay B: 20.00  
A needs to pay D: 5.00  
F needs to pay B: 5.00

🔧 Technologies Used
Language: C++

Concepts: Greedy Algorithm, Recursion, Floating-point Rounding

Libraries: unordered_map, algorithm, cmath, iomanip
