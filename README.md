## MATLAB Practical: Time Complexity and Search Algorithms

### Overview
This practical demonstrates the measurement of execution time in MATLAB for basic operations and two search algorithms: **Linear Search** and **Binary Search**. It highlights how time complexity affects the performance of these algorithms.

---

### Sections

1. **Measuring Execution Time for a Simple Loop**
   - Runs a loop from 1 to `n` and displays each number.
   - Measures and prints elapsed time using `tic` and `toc`.
   - Shows how execution time increases with larger `n`.

2. **Conditional Statement Execution Time**
   - Checks if a variable equals a certain value.
   - Measures how quickly a simple conditional executes.

3. **Linear Search**
   - Searches for a target value in an unsorted array by checking each element sequentially.
   - Stops when the target is found or the array ends.
   - Prints the index of the target element if found.
   - Measures the elapsed time taken for the search.
   - Time complexity: O(n) — grows linearly with the array size.

4. **Binary Search**
   - Searches for a target value in a **sorted** array using the divide-and-conquer approach.
   - Repeatedly divides the search interval in half until the target is found or the interval is empty.
   - Prints the index of the target element if found.
   - Measures the elapsed time taken for the search.
   - Time complexity: O(log n) — much faster for large sorted arrays compared to linear search.

---

### Key Learnings

- **Execution time measurement** in MATLAB is performed using `tic` and `toc`.
- **Linear search** is simple but inefficient for large arrays.
- **Binary search** requires sorted data but is significantly faster.
- The practical demonstrates how algorithm choice affects performance and execution time.

---

### Sample Output Times

| Operation               | Sample Elapsed Time (seconds) |
|------------------------|-------------------------------|
| Loop for n=1000         | ~0.0276                       |
| Linear Search (target=9)| ~0.0008                       |
| Binary Search (target=42)| ~0.0001                      |

---

This practical helps in understanding both the theoretical and practical aspects of algorithm time complexity and performance measurement.
