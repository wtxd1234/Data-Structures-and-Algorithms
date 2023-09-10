# Chapter 2: Arrays, Iteration, Invariants
- data is stored in computer as patterns of bits

## 2.1 Arrays
- array: store an ordered collection of items
  - array items are typically stored in a sequence of computer memory locations
```
a = [1,4,17,3,90,79,4,6,81]

* array a has 9 items
* its size is 9
*its positions are 0,1,2,3,4,5,6,7,8

```
- for any integer i denoting a position, we write a[i] to denote the element in the i<sup>th</sup> position
  - for example, element in the 8<sup>th</sup> position is 81, we use the notation a[8] to denote this element
  - position i is called an index (plural is indices)
 
- in most modern programming languages, = denotes assignment, while equality is expressed by ==
  - = is typically used in its mathematical meaning, unless it is used as part of code or pseudocode

## 2.2 Loops and Iteration
- loop: repeating a process a certain number of times
```
in pseudocode,

For i = 1,...,N,
do something


in programming languages,

for( i=0 ; i<N ; i++ ){
//do something
}


a counter i keep tracks of doing "the something" N times

```
- iteration: cycles
  - there is iteration over the index i

```
the general for-loop structure is

for( INITIALIZATION ; CONDITION ; UPDATE ){
  REPEATED PROCESS
}


or


INITIALIZATION
if ( not CONDITION ) go to LOOP FINISHED
LOOP START
  REPEATED PROCESS
  UPDATE
  if ( CONDITION ) go to LOOP START
LOOP FINISHED

```

## 2.3 Invariants
- invariant: a condition that does not change during execution of a given program or algorithm
  - it is important for data structures and algorithms because they enable correctness proofs and verification

- loop-invariant: a condition that is true at the beginning and end of every iteration of the given loop
```
minimum(int n, float a[n]){
  float min = a[0];
  // min equals the minimum item in a[0],...,a[0]
  for (int i = 1 ; i != n ; i++){
    // min equals the minimum item in a[0],...,a[i-1]
    if (a[i] < min) min = a[i];
  }
  // min equals the minimum item in a[0],...,a[i-1], and i==n
  return min;
}


* this is a kind of proof by induction:
the invariant is true at the start of the loop,
and is preserved by each iteration of the loop,
therefore it must be true at the end of the loop

开头对，中间每个循环也对，那么结尾一定对

```
