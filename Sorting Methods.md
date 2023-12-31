[HOME](README.md)

# Overview

Sorting algorithms are used to reorder items in a list or array according to a comparison operator on the elements. The efficiency of an algorithm is evaluated based on time complexity (how the execution time increases with the size of the input) and space complexity (how much extra memory the algorithm requires).

## Common Sorting Algorithms

1. **Bubble Sort:**
    - Description: Compares each pair of adjacent items and swaps them if they are in the wrong order. This process is repeated until no swaps are needed.
    - Time Complexity: Average and worst-case are $$O(n^2)$$; best case is $$O(n)$$ when the array is already sorted.
    - Space Complexity: $$O(1)$$ because it is an in-place sorting algorithm.
    - Usage: In educational contexts due to its simplicity, but rarely used in practice because of inefficiency.
2. **Selection Sort:**
    - Description: Divides the input list into two parts: a sorted sublist of items which is built up from left to right and a sublist of the remaining unsorted items. It repeatedly selects the smallest (or largest) element from the unsorted sublist, exchanges it with the leftmost unsorted element, and moves the sublist boundaries one element to the right.
    - Time Complexity: Always $$O(n^2)$$, where n is the number of items.
    - Space Complexity: $$O(1)$$, as it is in-place.
    - Usage: On small lists or when the cost of swapping items is significant.
3. **Insertion Sort:**
    - Description: Builds the final sorted array one item at a time. It is much less efficient on large lists than more advanced algorithms such as quicksort, heapsort, or merge sort.
    - Time Complexity: Average and worst-case are $$O(n^2)$$; best case is $$O(n)$$.
    - Space Complexity: $$O(1)$$.
    - Usage: Efficient for (quite) small data sets, much like other quadratic sorting algorithms.
4. **Shell Sort:**
    - Description: An in-place comparison sort which starts by sorting pairs of elements far apart from each other, then progressively reducing the gap between elements to be compared.
    - Time Complexity: Depends on the gap sequence; the best known is $$O(n \log^2 n)$$.
    - Space Complexity: $$O(1)$$.
    - Usage: Can be a good choice for medium-sized lists and where memory space is at a premium.
5. **Merge Sort:**
    - Description: Divides the unsorted list into n sublists, each containing one element, then repeatedly merges sublists to produce new sorted sublists until there is only one sublist remaining.
    - Time Complexity: $$O(n \log n)$$ in all cases.
    - Space Complexity: $$O(n)$$ due to the use of auxiliary space.
    - Usage: Efficient for large data sets; often used in external sorting.
6. **Quick Sort:**
    - Description: Selects a ‘pivot’ element from the array and partitions the other elements into two sub-arrays, according to whether they are less than or greater than the pivot. The sub-arrays are then sorted recursively.
    - Time Complexity: Average case $$O(n \log n)$$, but worst-case is $$O(n^2)$$. However, this is rare and can be avoided with high-probability by choosing good pivot elements.
    - Space Complexity: $$O(\log n)$$ on average due to recursion stack.
    - Usage: Frequently used, as it is efficient and has a good average case performance.

## Stability in Sorting
- A sorting algorithm is said to be stable if two objects with equal keys appear in the same order in the sorted output as they appear in the input array to be sorted.
- Bubble sort, merge sort, and insertion sort are examples of stable sorting algorithms, while quicksort is not stable.

## In-Place and Not In-Place Sorting
- An in-place sorting algorithm uses a small, constant amount of extra space.
- Algorithms such as quicksort is in-place as they do not require additional memory proportional to the input size, while merge sort requires extra space.

## Conclusion
The choice of sorting algorithm depends on the size and nature of the data, the complexity requirements of the application, and the memory space available. Understanding these algorithms is crucial for software developers because sorting is often a primary operation in data processing and optimization tasks. Each sorting algorithm has its own trade-offs, and in practice, some programming languages and libraries use a combination of sorting algorithms to optimize for various datasets.
