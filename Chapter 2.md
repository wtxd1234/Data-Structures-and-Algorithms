# Chapter 2
## Big O Notation
Big O Notation
- to describe the __performance or complexity__ of an algorithm
  - __Time complexity__ – how much time it takes to run completely?
  - __Space complexity__ – how much extra space does it require in the process?
    - O(1) - An algorithm that will always execute at the same time (Constant) regardless of size
    - O(n) - An algorithm that will grow linearly and in direct proportion to input data size.
    - O(n2) - An algorithm whose performance is directly proportional to the square of the input data size. (usually nested loops)
    - O(log N) - Logarithms

![aa88c2f1-f3ec-4138-a9b9-874a5bf000a2](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/3155b58e-40f8-4c4c-86f8-798484791a92)

## 6 Sorting Algorithms 

1. Insertion Sort (一层一层scan同时排美美，一直重复到最后一层)

    1. Every iteration迭代 of insertion sort the 1st element of the unsorted sub list from the input data is transferred to the sorted sub list by inserting it into the correct position.
    2. Step 1 is repeated until no input element remain. 
    3. The resulting list after k iteration has the properly where the first k entries are sorted.

2. Selection Sort (找出小的然后排小到大直到最后)

    1. Find the minimum value in the list. 
    2. Swap with the value in the first position.
    3. Repeat the steps above for the remainder of the list. 

3. Bubble Sort (同时比较两个东西然后把他们放在对的排列，一直重复到全部排列对)

    1. Stepping through the list to be sorted.
    2. Comparing 2 items at a time, swap them if they are in the wrong order.
    3. Repeat step 1 until no swaps are needed.

4. Shell Sort
5. Merge Sort
6. Quick Sort