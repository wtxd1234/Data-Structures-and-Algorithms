# Overview
Hashing is a technique used to uniquely identify a specific object from a group of similar objects. In computer science, hashing refers to the process of mapping data of arbitrary size to data of fixed size (hash values, hash codes, or simply hashes).

## Hash Tables
- *Hash Table*: A data structure that implements an associative array, a structure that can map keys to values. A hash table uses a hash function to compute an index into an array of buckets or slots, from which the desired value can be found.

## Hash Function
- *Hash Function*: An algorithm that takes an input (or 'key') and returns a fixed-size string of bytes. The output is typically a 'hash code' which is used to index a hash table holding the data or records.

## Properties
- *Deterministic*: The same input will always produce the same hash value.
- *Efficient*: Computing the hash value should be fast.
- *Uniform Distribution*: Hash values should be uniformly distributed across the hash table to avoid clustering.

## Collision
When two different inputs produce the same hash value, a collision occurs. Handling collisions is a significant aspect of hash table design.

### Collision Resolution Techniques
1. *Separate Chaining*: Each bucket is independent, and has some sort of list of entries with the same index. The data structure used for this list can be a linked list, a binary search tree, or even another hash table.
2. *Open Addressing*: All entry records are stored within the array itself. When a new entry needs to be inserted, the buckets are examined, starting with the hashed-to slot and proceeding in some sequence until an unoccupied slot is found.

## Separate Chaining
- *Description*: In separate chaining, each bucket in the hash table points to a linked list of entries that collide at the same index.
- *Pros*:
  - Simple to implement.
  - Hash table expansion is less critical.
  - Performance degrades gracefully.
- *Cons*:
  - Memory overhead due to pointers.
  - Cache performance of the structure can be poor.

## Open Addressing
- *Description*: All elements are stored in the array itself and each bucket can be in three states: empty, occupied, or deleted (tombstone).
- *Methods*:
  - *Linear Probing*: When a collision occurs, the algorithm checks the next bucket.
  - *Quadratic Probing*: Increases the hash value by a quadratic function of the number of probes.
  - *Double Hashing*: Uses a secondary hash function to calculate the probe sequence.
- *Pros*:
  - Better cache performance.
  - More consistent performance.
- *Cons*:
  - Clustering can occur, leading to longer search times.
  - Deletion is more complex.
  - Rehashing can be costly.

## Rehashing
- *Rehashing*: When the load factor (number of entries divided by the number of buckets) grows too large, the hash table may need to be resized and all existing entries rehashed to the new size table.

## Load Factor
- *Load Factor*: A measure that decides when to increase the size of the hash table (rehash). It's calculated as the number of stored entries divided by the number of buckets.

## Applications
- Implementing associative arrays.
- Database indexing.
- Caches.
- Sets.
- Counting distinct elements.

## Complexity
- *Average Case*: For searching, insertion, and deletion operations, the complexity is O(1).
- *Worst Case*: In scenarios with many collisions, the complexity can degrade to O(n).

## Conclusion
Hashing is a powerful technique for efficient searching and data retrieval. The choice between separate chaining and open addressing depends on the use case, expected number of collisions, memory availability, and performance requirements. Understanding the nuances of hashing and collision resolution is crucial for developing efficient data storage and retrieval mechanisms.
