## MATLAB Practical: Searching and Sorting Algorithms Performance

### Overview
This practical covers two important algorithmic concepts in MATLAB: **searching** and **sorting**. It demonstrates the implementation of Linear Search and Binary Search on a large array, compares their execution times, and implements Selection Sort to sort an array.

---

### Sections

1. **Searching Algorithms on a Random Array**
   - An array of 1000 random integers is generated.
   - A target element is randomly selected from this array.
   
   - **Linear Search:**
     - Iterates through the array sequentially to find the target.
     - Measures the time taken to locate the target.
     - Time complexity: O(n).
   
   - **Binary Search:**
     - The array is first sorted using MATLAB’s built-in `sort` function.
     - Uses the divide-and-conquer approach to find the target efficiently.
     - Measures the time taken to locate the target.
     - Time complexity: O(log n).

   - The execution times of both search methods are printed and compared.
   - Note: Although binary search is theoretically faster, the time to sort the array beforehand may impact overall timing.

---

2. **Selection Sort Algorithm**
   - Implements the Selection Sort algorithm on a small example array.
   - Algorithm finds the minimum element from the unsorted portion and swaps it with the first unsorted element.
   - Continues until the entire array is sorted.
   - Selection Sort time complexity: O(n²).
   - Prints the sorted array after completion.

---

### Key Learnings
- **Linear Search** is simple but inefficient for large data.
- **Binary Search** is much faster on sorted data but requires the initial sorting step.
- **Selection Sort** is a straightforward sorting algorithm useful for educational purposes but inefficient for large arrays.
- Practical demonstrates measuring execution time for different algorithms using `tic` and `toc`.

---

### Sample Output
- Linear Search Time: ~0.000626 seconds
- Binary Search Time: ~0.001311 seconds (excluding sorting time)
- Sorted array after Selection Sort: `[11 12 22 25 64]`

---

This practical reinforces algorithmic efficiency concepts and practical timing measurements in MATLAB.
