# C++ Banking System & Algorithm Benchmark

## 📌 Overview
This project contains a comprehensive C++ banking simulation alongside a performance benchmarking tool. It demonstrates the practical application of object-oriented programming (OOP), file handling (JSON parsing), and core data structures (Stacks, Queues, Vectors) to manage bank accounts, loans, and customer service. Additionally, it includes a module to analyze the time complexity of various sorting and searching algorithms.

## 🚀 Features

### 1. Advanced Banking System (`banking_system.cpp`)
A full-featured bank management application simulating real-world financial logic.
* **Account Management:** Create new accounts, check balances, and list all active accounts.
* **Transactions:** Deposit, withdraw, and securely transfer money between accounts with PIN verification.
* **Loan Management:** Create loans with varying interest rates and tenures.
* **EMI Calculations:** Uses compound interest formulas to calculate Equated Monthly Installments and allows users to pay off their dues.

### 2. Intermediate Banking System (`banking_system_medium.cpp`)
A streamlined version focusing on the implementation of specific data structures.
* **Transaction History (Stack):** Implements a LIFO (Last-In, First-Out) `undoStack` allowing tellers to instantly revert the most recent withdrawal.
* **Customer Service (Queue):** Implements a FIFO (First-In, First-Out) `serviceQueue` to add customers to a waiting line and serve them sequentially.

### 3. Algorithm Benchmarking (`benchmark_compare.cpp`)
A testing module to compare the efficiency of standard algorithms on the bank's database.
* **Sorting:** Compares the execution time of a custom **Insertion Sort** ($O(N^2)$) against C++'s highly optimized `std::sort` ($O(N \log N)$).
* **Searching:** Compares **Linear Search** ($O(N)$) against **Binary Search** ($O(\log N)$) across thousands of queries to demonstrate performance scaling.

## 📂 File Structure
* `banking_system.cpp` - Source code for the advanced banking app.
* `banking_system_medium.cpp` - Source code for the medium-tier app with undo/queue features.
* `benchmark_compare.cpp` - Source code for the algorithm performance tests.
* `accounts.json` - The local text-based database storing all account details, loans, dues, and transaction histories.
* `banking_system`, `banking_system_medium`, `benchmark_compare` - Pre-compiled binary executables.

## 🛠️ Compilation & Execution

To compile the source files from scratch, you will need a C++ compiler (like GCC or Clang) that supports C++11 or higher.

**1. Compiling the files:**
Open your terminal and run the following commands:
```bash
g++ -std=c++11 banking_system.cpp -o banking_system
g++ -std=c++11 banking_system_medium.cpp -o banking_system_medium
g++ -std=c++11 benchmark_compare.cpp -o benchmark_compare
