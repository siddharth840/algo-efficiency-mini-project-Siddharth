Project Overview

The goal of this mini-project is to implement multiple algorithms, analyze their performance, and visualize their execution time behaviour as the input size increases.

Algorithms that solve the same problem can differ dramatically in performance based on design choices such as recursion, iteration, and partitioning strategies.
This project helps understand those trade-offs through real experimental profiling.

Algorithms Implemented
Algorithm	Type	Notes
Fibonacci (Naive Recursive)	Recursive	Exponential time
Fibonacci (Dynamic Programming)	Bottom-Up	Linear time
Merge Sort	Divide & Conquer	Guaranteed O(n log n)
Quick Sort	Divide & Conquer	Very fast, but worst case O(n²)
Insertion Sort	Comparison-Based	Efficient for nearly-sorted data
Bubble Sort	Comparison-Based	Slow for large datasets
Selection Sort	Comparison-Based	Consistent O(n²)
Binary Search	Searching	Requires sorted input
Performance Profiling

For each algorithm:

✔ Execution time measured using time.perf_counter()
✔ Repeated runs to reduce random variation
✔ Results plotted using matplotlib

Input Size Strategy
Class	Algorithms	Input Sizes
O(n log n)	Merge Sort, Quick Sort	100 → 10,000
O(n²)	Insertion, Bubble, Selection	100 → 2,000
Exponential	Fibonacci (Recursive)	5 → 30
O(log n)	Binary Search	100 → 10,000
O(n)	Fibonacci (DP)	1000 → 10,000
 Output & Visualizations

The notebook generates:

 execution_time_plots.png
A combined figure showing timing curves for:

n log n algorithms

n² algorithms

Binary Search

Fibonacci (Recursive vs DP)

The plot clearly shows how algorithms diverge in efficiency as the input grows.

 Key Insights & Findings

🔹 Algorithms with O(n log n) complexity scale efficiently and remain practical for large inputs
🔹 O(n²) algorithms become significantly slower as input size increases
🔹 Binary Search time per query is extremely small due to logarithmic growth
🔹 Recursive Fibonacci grows exponentially and becomes infeasible beyond n ≈ 30
🔹 Dynamic Programming Fibonacci is highly efficient and can handle large n easily

 Repository Contents (recommended structure)
algo-efficiency-mini-project-<yourname>/
│
├── algo_analysis_notebook.ipynb
├── execution_time_plots.png
├── README.md
├── requirements.txt
└── .gitignore

 How to Run the Notebook
1️Install dependencies
pip install -r requirements.txt

2️ Run the notebook
jupyter notebook algo_analysis_notebook.ipynb


No external datasets are required — the notebook generates random input lists automatically.

 Citations & References

CLRS – Introduction to Algorithms

Python Documentation – time, memory_profiler, and matplotlib

 Acknowledgement

This project was completed as part of Design and Analysis of Algorithms Lab (ENCA351) in the School of Engineering & Technology, K.R. Mangalam University.


Let me know if you want:
🔸 requirements.txt + .gitignore
🔸 converting notebook code into separate .py files
🔸 exporting the project into a ZIP folder
🔸 submitting a GitHub-ready folder automatically
