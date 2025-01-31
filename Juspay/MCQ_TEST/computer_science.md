# 📌 Computer Science & System Understanding - Comprehensive Notes & Formulas

---

## 📍 1. Computer Science

---

### 1.1 **Algorithm Complexity & Data Structures**
| Concept                        | Formula / Definition                                       | Description |
|--------------------------------|-----------------------------------------------------------|-------------|
| **Big-O Notation**              | `O(1)`, `O(log n)`, `O(n)`, `O(n²)`, `O(2^n)`, `O(n!)`  | Describes algorithm efficiency |
| **Time Complexity - Best Case** | `Ω(f(n))`                                               | Lower bound on running time |
| **Time Complexity - Average Case** | `Θ(f(n))`                                           | Expected performance |
| **Time Complexity - Worst Case** | `O(f(n))`                                             | Upper bound on running time |
| **Recurrence Relation**         | `T(n) = aT(n/b) + f(n)`                              | Master theorem format |
| **Space Complexity**            | `O(n)` (Arrays), `O(log n)` (Recursive Calls)         | Memory required by algorithm |

---

### 1.2 **Searching Algorithms**
| Algorithm      | Complexity  | Description |
|---------------|------------|-------------|
| **Linear Search**  | `O(n)` | Searches sequentially through an array |
| **Binary Search**  | `O(log n)` | Divides search space in half (for sorted arrays) |

---

### 1.3 **Sorting Algorithms**
| Sorting Algorithm | Best Case | Average Case | Worst Case | Description |
|------------------|----------|--------------|------------|-------------|
| **Bubble Sort** | `O(n)` | `O(n²)` | `O(n²)` | Repeatedly swaps adjacent elements |
| **Selection Sort** | `O(n²)` | `O(n²)` | `O(n²)` | Selects smallest element and places it in order |
| **Insertion Sort** | `O(n)` | `O(n²)` | `O(n²)` | Inserts each element into the sorted portion |
| **Merge Sort** | `O(n log n)` | `O(n log n)` | `O(n log n)` | Uses divide and conquer |
| **Quick Sort** | `O(n log n)` | `O(n log n)` | `O(n²)` | Uses pivot for partitioning |

---

### 1.4 **Data Structures**
| Data Structure | Operations | Complexity |
|---------------|------------|------------|
| **Array** | Insert: `O(1)`, Search: `O(n)`, Delete: `O(n)` | Fixed-size memory allocation |
| **Linked List** | Insert/Delete: `O(1)`, Search: `O(n)` | Dynamic memory allocation |
| **Stack (LIFO)** | `push()`, `pop()`, `peek()` → `O(1)` | Last-In-First-Out |
| **Queue (FIFO)** | `enqueue()`, `dequeue()` → `O(1)` | First-In-First-Out |
| **Binary Search Tree (BST)** | Insert/Search/Delete: `O(log n)` | Sorted hierarchical structure |

---

### 1.5 **Graph Theory**
| Concept | Definition / Formula | Description |
|---------|----------------------|-------------|
| **Graph Representation** | `G(V, E)` where `V` = vertices, `E` = edges | Defines connections between nodes |
| **Adjacency Matrix** | `O(V²)` space | Stores edges in a matrix |
| **Adjacency List** | `O(V + E)` space | Stores edges in a list |
| **Dijkstra’s Algorithm** | `O(V log V)` | Finds shortest path in weighted graph |
| **Floyd Warshall Algorithm** | `O(V³)` | Finds shortest paths between all pairs |

---

### 1.6 **Compilers**
| Concept | Definition |
|---------|------------|
| **Lexical Analysis** | Tokenizes source code into meaningful units |
| **Syntax Analysis** | Checks grammatical structure of the code (Parsing) |
| **Semantic Analysis** | Ensures logic and meaning of code is correct |
| **Intermediate Code Generation** | Converts source code into intermediate representation |
| **Code Optimization** | Improves efficiency of code before final compilation |
| **Code Generation** | Produces machine-level instructions |

---

### 1.7 **Computer Architecture**
| Concept | Definition |
|---------|------------|
| **Von Neumann Architecture** | Uses a single memory for data and instructions |
| **Harvard Architecture** | Uses separate memories for data and instructions |
| **RISC vs. CISC** | RISC: Simple instructions, fast execution. CISC: Complex instructions, fewer instructions per program |
| **Cache Memory** | Stores frequently accessed data for faster retrieval |

---

## 📍 2. System Understanding

---

### 2.1 **Operating Systems**
| Concept | Definition |
|---------|------------|
| **Process Scheduling** | Determines order of process execution |
| **Threading** | Allows parallel execution within a process |
| **Deadlock** | Occurs when processes wait indefinitely for resources |
| **Paging** | Divides memory into fixed-size blocks to manage fragmentation |
| **Virtual Memory** | Extends RAM using disk storage |

---

### 2.2 **Networking**
| Concept | Definition |
|---------|------------|
| **TCP/IP Model** | Application → Transport → Network → Link |
| **OSI Model** | 7 layers: Physical, Data Link, Network, Transport, Session, Presentation, Application |
| **IPv4 Addressing** | Uses 32-bit addressing |
| **IPv6 Addressing** | Uses 128-bit addressing |

---

### 2.3 **Database Management (SQL)**
| Query | Syntax |
|-------|--------|
| **SELECT** | `SELECT column FROM table WHERE condition;` |
| **INSERT** | `INSERT INTO table (col1, col2) VALUES (val1, val2);` |
| **UPDATE** | `UPDATE table SET column=value WHERE condition;` |
| **DELETE** | `DELETE FROM table WHERE condition;` |

---

### 2.4 **Computer Security**
| Concept | Definition |
|---------|------------|
| **Encryption** | Converts data into unreadable format using cryptographic keys |
| **Hashing** | Generates a fixed-size hash from input data |
| **Public Key Cryptography** | Uses asymmetric encryption for secure communication |

---

### 2.5 **Cloud Computing**
| Concept | Definition |
|---------|------------|
| **Virtualization** | Running multiple OS on one physical machine |
| **SaaS** | Software as a Service - Applications hosted on the cloud |
| **PaaS** | Platform as a Service - Cloud-based app development environment |
| **IaaS** | Infrastructure as a Service - Virtual servers and storage |

---
