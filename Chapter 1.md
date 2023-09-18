# Chapter 1
## Algorithms
What is an algorithm?
- __A procedure or formula for solving a problem__

```
findMax(Array)
{
     declare a variable to store 
     maximum value
     max = Array[0]
     Start do loop
     Compare max with all array 
     values
     if array_value > max
     max = array_value
     End Loop
     print max value
}

```

Where do algorithms come from?
- Named for the ninth-century Persian mathematician _al-Khwarizmi_
- __Derived from the need to solve a specific problem__

Why do we study algorithms? 
- __To understand how they work__
- To be able to know when to use them, adapt them to new problems, create new algorithms that are better than the existing ones (not all of us) 
- Better? In what way? 
  - Faster 
  - Less space used 
  - More general

## Properties of Algorithms

Properties of Algorithms
- ___Correctness___
  - It is easy to show an algorithm is incorrect, just __find a case where the algorithm fails__.
  - __Showing that an algorithm is correct is a much more difficult proposition__ .
  - Correctness can be shown __formally or informally__.
- ___Efficiency___
  - A measure of __speed__, how many basic steps are needed to complete a task?
  - A measure of __space__, how much storage is needed?
- ___Applicability___
  - What is the domain of the algorithm?
  - What sub domain is the algorithm efficient in?

## Data Structures

___Data structure___: A __systematic way of organizing a collection of data__.
  - Allows for efficient access by the algorithm
  - Uses a minimum of storage

2 types of data structures: 
1. ___Static data structure___:  One whose __capacity is fixed at creation__.
    - E.g.: array
2. ___dynamic data structure___: one whose __capacity is variable__, so it can __expand or contract at any time__.
    - E.g.: linked list, binary tree

- Array: A __fixed__ number of __data items__ of the __same type__.

## Examples

Multiplication乘法
1. Long multiplication

- 931 * 88 = ?

![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/1a2af6ca-2113-42d6-ad1a-5f0d36be7da7)

   
2. Multiplication à la russe

- 931 * 88 = ?
    - Step 1:    
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/055ae37c-1420-49aa-ae89-ca947614b0b8)

    - Step 2:
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/b627ce3d-7854-4017-b51f-3f0f077dbc4b)

    - Step 3:
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/7cf49d76-542f-4beb-ae1a-90fd8e11736a)

    - Step 4:
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/a55c8aa0-b6d3-4403-910e-4b3b1262d033)

    - Step 5:
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/7ba48d2d-2401-48de-b84f-dc725e5a01b4)


3. Divide and conquer multiplication

- 931 * 1234 = ?
    - Step 1: Split each number into __right half__ and __left half__
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/a84878b6-4c4b-4b1d-99d9-6e753049ea7c)

    - Step 2: Let the two numbers 931 and 1234 as __a__ and __b__ respectively.Thus, Left-half of a __(al) = 09__, Right-half of a __(ar) = 31__, Left-half of b __(bl) = 12__ and Right-half of b __(br) = 34__.

    - Step 3:
![image](https://github.com/wtxd1234/Data-Structures-and-Algorithms/assets/41671135/e971b685-e89a-490a-ac2d-31ab9c657d3b)

## Analysis of Algorithms
- to determine the amount of resources (such as time and storage) necessary to execute it
- 2 ways to analyze an algorithm:
    1. ___Empirical analysis___: research that derives its data by means of direct __observation__ or __experiment__
       - Limitations of Experiments: same hardware and software specs, same time, ...
    2. ___Theoretical analysis___: Uses a __high-level description of the algorithm__ (Pseudo-code) instead of an implementation (Programming languages)
