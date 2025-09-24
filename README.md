# TanyahMadondoDAA-Project-1

# Project 1 – Option 0: Time Complexity Analysis

## 📌 Problem Statement
We are required to analyze the following program:

```cpp
int j = 2;
while (j < n) {
    int k = j;
    while (k < n) {
        Sum += a[j] * b[k];
        k = k * k;
    }
    j = 2 * j;
}
This program contains two nested loops:
Outer loop doubles j each time → about log(n) iterations.
Inner loop squares k each time → about log(log(n)) iterations.
Overall complexity: O(logn⋅loglogn)

Implementation
The file project1.py contains:
A Python implementation of the algorithm (Option 0).
Code to measure execution time for different values of n.
Output of results for analysis.

How to Run
Clone the repository or download the files.
git clone https://github.com/YOUR_USERNAME/DAA_Project1.git
cd DAA_Project1

Run the Python script:
python3 project1.py

Example output:

Results:
n = 10000: 4.0531158447265625e-06 seconds
n = 100000: 5.245208740234375e-06 seconds
n = 1000000: 2.09808349609375e-05 seconds
n = 10000000: 2.6702880859375e-05 seconds
n = 100000000: 0.0001442432403564453 seconds

Results & Analysis
Theoretical complexity: O(log n · log log n)
Experimental measurements: Collected runtimes for increasing values of n.
Both show the same growth trend, confirming the analysis.
