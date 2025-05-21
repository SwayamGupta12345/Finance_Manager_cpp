# Finance Manager (C++)

A comprehensive, menu-driven personal finance management application written in C++. This project provides tools for tracking expenses, optimizing credit card and loan payments, simulating rent vs. buy decisions, portfolio optimization, budgeting, fraud detection, data compression, and much more—all through a single command-line interface.

---

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Modules and Algorithms](#modules-and-algorithms)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [Authors](#authors)
- [License](#license)

---

## Features

- **Expense Tracking:** Add, update, delete, and display essential and non-essential expenses, stored in a CSV file.
- **Budget Planning:** Design a personalized monthly budget based on your income.
- **Savings Optimization:** Set savings goals and optimize non-essential expenses to help reach your targets (dynamic programming).
- **Credit Card Payment Strategy:** Minimize credit card interest by prioritizing payments (greedy algorithms).
- **Loan Repayment Optimization:** Distribute leftover income to loans with highest interest-to-amount ratios for minimal interest paid.
- **Investment Portfolio Optimization:** Allocate a risk budget to maximize returns (fractional knapsack/greedy).
- **Fraud Detection:** Detect anomalous or fraudulent transactions via statistical analysis of expense patterns.
- **Travel Expense Minimization:** Find minimum travel costs (Dijkstra’s algorithm with hotel/flight options).
- **Rent vs Buy Simulator:** Compare cumulative costs of renting vs. buying property over time.
- **Inventory Optimization:** Optimize product selection for storage to maximize profit (dynamic programming/0-1 knapsack).
- **Recurring Expense Scheduler:** Schedule recurring bills to minimize penalty payments.
- **Emergency Fund Allocation:** Model expenses as a graph and minimize emergency fund transfers (Kruskal’s algorithm/minimum spanning tree).
- **Data Compression & Encryption:** Huffman encoding for CSV compression and Caesar cipher for file encryption/decryption.

---

## Demo

On running the program, you’ll see a menu like:

```
Expense Tracker Menu:
1. Display Expenses
2. Add Expense
3. Update Expense
4. Delete Expense
5. Design A budget plan
6. Allocate Emergency Funds
7. Compress Data
8. Decompress Data
9. Optimize Savings
10. Credit Card Payment Strategy
11. Best Flight optimization
12. Loan Repayment Strategy
13. Investment Portfolio Optimization
14. Encrypt CSV
15. Decrypt CSV
16. Rent vs Buy
17. Inventory Optimizer
18. Recurring Expense Scheduler
19. Exit
```

---

## Getting Started

### Prerequisites

- C++17 compatible compiler (tested with g++)
- Windows (uses `<windows.h>` for `Sleep`; adjust for Linux/Mac if needed)
- Standard C++ libraries

### Build

```bash
g++ aps.cpp -o finance_manager
```

### Run

```bash
./finance_manager
```

---

## Usage

1. **Add expenses:** Enter daily essential (food, work, travel) and non-essential (snacks, fun, extra) expenses. Each entry can be assigned to a payment card.
2. **Update/Delete expenses:** Change or remove entries by date.
3. **Budgeting:** Input your monthly income to generate a suggested budget.
4. **Optimize savings:** Set a goal and let the app suggest non-essential expense reductions.
5. **Credit/Loan optimization:** Input payment and loan details to receive optimized payment plans.
6. **Travel, rent/buy, inventory:** Simulate scenarios and optimize decisions using built-in algorithms.
7. **Data compression/encryption:** Secure or compress your CSV files as needed.

All data is stored in CSV files in the project directory.

---

## Modules and Algorithms

- **Expense Management:** File I/O, input validation, and dynamic 2D vectors.
- **Savings Optimization:** Dynamic programming subset sum.
- **Credit Card Payments:** Greedy approach (minimize interest).
- **Loans:** Greedy sorting by interest-to-amount.
- **Investments:** Fractional knapsack (greedy).
- **Fraud Detection:** Mean/standard deviation anomaly detection.
- **Travel:** Dijkstra’s algorithm for shortest path with hotel/flight costs.
- **Rent vs Buy:** Simulation with compound interest and rent hikes.
- **Inventory:** 0-1 Knapsack.
- **Recurring Bills:** Scheduling to minimize penalty.
- **Emergency Fund:** Kruskal’s MST for minimum transfer cost.
- **Compression:** Huffman encoding.
- **Encryption:** Caesar cipher for CSV files.

---

## File Structure

- `aps.cpp`, `aps.h` – Main application code and headers
- `OctExpenses.csv` – Stores expense data
- `carddetails.csv` – Stores card usage data
- `travelinput.txt` – Travel data (for travel module)
- Other generated files: `compress.csv`, `encrypted_Expenses.csv`, etc.

---

## Dependencies

- Standard C++17 libraries
- `<windows.h>` (replace `Sleep()` for cross-platform support if needed)

---

## Contributing

Contributions are welcome!
- Fork this repo
- Create a feature branch
- Submit a pull request

---

## Authors

- Swayam Gupta
- Rishu
- Maanya Gupta
- Priyanshu Rawat

---

## License

This project is licensed under the MIT License.

---

## Notes

- All data is stored locally in CSV files; be sure to back up your data.
- For any issues or suggestions, open an issue on GitHub.

---

**Happy Budgeting!**

---
