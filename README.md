# 🧠 LRU Cache

## 📌 Project Description

Caching is a technique used to store frequently accessed data in a faster storage layer to improve performance and reduce latency. It optimizes repeated computations, reduces database queries, and enhances user experience by retrieving data quickly.

---

## 🔃 In-Memory Caching Systems

### 🔹 Redis
An in-memory key-value store that supports:
- Data persistence
- Transactions
- Advanced data structures (lists, sets, hashes)

### 🔹 MemCache
A distributed memory caching system used to speed up dynamic database-driven websites by caching data in RAM.

---

## 🖥️ Cache Memory in Computer Organization

Cache memory is a high-speed storage layer between RAM and the CPU that stores frequently accessed data to reduce fetch time.

### 📊 Levels of Cache:
- **L1 Cache**: Smallest but fastest, located within the CPU.
- **L2 Cache**: Larger but slightly slower, still inside the CPU.
- **L3 Cache**: Shared among multiple CPU cores for higher performance.

---

## ♻️ Cache Replacement Strategies

- **Least Recently Used (LRU)**: Removes the least recently accessed item.
- **First-In-First-Out (FIFO)**: Evicts the oldest item.
- **Least Frequently Used (LFU)**: Discards items used least often.
- **Random Replacement**: Removes a randomly selected item.

---

## 🛠️ LRU Cache Design (Java)

### ✅ Data Structures Used:
- **HashMap** for O(1) access
- **Doubly Linked List** to maintain order of usage

### 📌 How It Works:
- The **HashMap** maps keys to nodes in the doubly linked list.
- The **Doubly Linked List** maintains the order of elements (most recently used at the front, least at the back).
- On access or insertion, nodes are moved to the front.
- When capacity is exceeded, the node at the tail (least recently used) is evicted.

---

## 📁 File Structure

```

├── .gitignore       # Ignore config
├── LICENSE          # MIT License
├── README.md        # Documentation
├── LRU.java         # Java implementation of LRU Cache

```

---

## 📄 License

This project is licensed under the **MIT License**.  
See the `LICENSE` file for more details.

---

## 🙌 Contributions

Pull requests and suggestions are welcome!  
If you find a bug or want to improve this project, feel free to fork and contribute.
