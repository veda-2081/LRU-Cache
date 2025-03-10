# LRU-Cache
# Caching 
It is a technique used to store frequently accessed data in a faster storage layer to improve performance and reduce latency. It helps in optimizing repeated computations, reducing database queries, and enhancing user experience by retrieving data quickly.
In-Memory Cache: Redis and MemCache Introduction

# Redis: 
An in-memory key-value store that supports data persistence, transactions, and data structures like lists, sets, and hashes.

# MemCache: 
A distributed memory caching system used to speed up dynamic database-driven websites by caching data in RAM.

# Cache Memory in Computer Organization

Cache memory is a high-speed storage layer between RAM and CPU that stores frequently accessed data to reduce fetch time. It operates in multiple levels:

L1 Cache: Smallest but fastest, located within the CPU.

L2 Cache: Larger but slightly slower, still inside the CPU.

L3 Cache: Shared among multiple cores, further improving performance.

# Different Cache Replacement Strategies

Least Recently Used (LRU): Removes the least recently accessed item.

First-In-First-Out (FIFO): Evicts the oldest item.

Least Frequently Used (LFU): Discards items used least often.

Random Replacement: Removes a randomly selected item.

# Designing LRU Cache Using Doubly Linked List and HashMap

An LRU cache can be efficiently implemented using a doubly linked list (for maintaining order) and a HashMap (for O(1) lookup and insert operations). The HashMap stores keys with references to linked list nodes, while the doubly linked list maintains usage order.
