# Stock Selection Optimization System

A university-level optimization project that compares multiple algorithmic approaches for solving budget-constrained stock selection problems using real-world historical stock datasets.

---

# Project Overview

This project presents a Stock Selection Optimization System designed to maximize investment profit while staying within a limited investment budget. The problem is modeled using the classical **0/1 Knapsack Problem** formulation.

The system compares multiple algorithms from different algorithm design families, including:

* Greedy Algorithm
* Dynamic Programming (0/1 Knapsack)
* Brute Force Exhaustive Search

The project also includes:

* Experimental complexity analysis
* Performance comparison
* Flask-based interactive dashboard
* Real-world stock datasets from Kaggle

---

# Objectives

* Implement multiple optimization algorithms
* Compare execution time and scalability
* Analyze computational complexity
* Maximize total expected profit under budget constraints
* Study the trade-off between speed and optimization accuracy

---

# Algorithms Used

## 1. Greedy Algorithm

* Design Family: Greedy
* Complexity: O(n log n)
* Fast approximate solution
* Uses profit-to-cost ratio

## 2. Dynamic Programming

* Design Family: Dynamic Programming
* Complexity: O(nW)
* Guarantees optimal solution
* Uses 0/1 Knapsack optimization

## 3. Brute Force

* Design Family: Exhaustive Search
* Complexity: O(2ⁿ)
* Evaluates all possible stock combinations
* Used mainly for comparison and benchmarking

---

# Technologies Used

* Python
* Flask
* CSV datasets
* HTML/CSS
* JavaScript
* itertools
* statistics
* time.perf_counter()

---

# Dataset

The project uses historical stock market datasets collected from Kaggle.

Dataset includes:

* Open price
* Close price
* High price
* Low price
* Volume
* Date

The stock selection problem is transformed into a 0/1 Knapsack optimization problem where:

* Stock price → item weight
* Expected profit → item value
* Investment budget → knapsack capacity

---

# Project Structure

```bash
project/
│
├── algorithms/
│   ├── greedy.py
│   ├── knapsack.py
│   └── brute_force.py
│
├── services/
│   └── data_loader.py
│
├── templates/
│   ├── index.html
│   └── dashboard.html
│
├── dataset/
│   ├── archive/
│   └── company_names.csv
│
├── static/
│
├── app.py
└── README.md
```

---

# Experimental Analysis

The implemented algorithms were experimentally evaluated using:

* Different dataset sizes
* Multiple budget configurations
* Best-case scenarios
* Average-case scenarios
* Worst-case scenarios

Measured Metrics:

* Execution time
* Total profit
* Scalability
* Optimization quality
* Computational complexity

---

# Running the Project

## 1. Clone the repository

```bash
git clone <repository-link>
cd stock-selection-system
```

## 2. Install dependencies

```bash
pip install flask yfinance
```

## 3. Run the application

```bash
python app.py
```

## 4. Open the dashboard

```bash
http://127.0.0.1:5000
```

---

# Dashboard Features

* Select stock datasets
* Define investment budget
* Execute optimization algorithms
* Compare execution times
* Visualize optimization results
* Analyze scalability behavior

---

# Experimental Results Summary

| Algorithm           | Speed     | Optimization Quality | Scalability |
| ------------------- | --------- | -------------------- | ----------- |
| Greedy              | Very Fast | Approximate          | High        |
| Dynamic Programming | Medium    | Optimal              | Medium      |
| Brute Force         | Very Slow | Optimal              | Low         |

---

# Conclusion

The project demonstrates how different algorithmic paradigms can be applied to solve real-world combinatorial optimization problems efficiently.

The experimental comparison showed that:

* Greedy provides fast approximate solutions
* Dynamic Programming achieves optimal results
* Brute Force guarantees correctness but suffers from exponential growth

The project highlights the importance of computational complexity analysis when selecting algorithms for large-scale optimization systems.

---

# Future Improvements

Possible future enhancements include:

* Machine learning-based stock prediction
* Genetic Algorithms
* Branch and Bound optimization
* Real-time stock market integration
* Advanced portfolio optimization techniques

---

# Authors

* Wesam Almalki
* Ahmad Albouainain
* Anas Hamzi
* Fahad Alotaibi
* Faris Alshahrani
* Fawaz Alshahrani

---

# Instructor

Dr. Nasro Min Allah

