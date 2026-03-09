# 🔗 Singly Linked Lists vs Doubly Linked Lists

A **Linked List** is a linear data structure where **nodes are connected sequentially**.

Each **node** contains:
- 📦 **Data**
- 🔗 **Reference (pointer)** to another node

This structure forms a **chain of nodes**.
```mermaid
[A | next] → [B | next] → [C | next] → [D | next] → NULL
```

Linked lists are commonly used to implement:

- Stacks
- Queues
- Deques
- Graph algorithms (DFS and BFS)

---

# 📌 Singly Linked Lists

## 🔹 What is a Singly Linked List?

A **singly linked list** is a linked list where each node contains **one reference** pointing to the **next node**.
```mermaid
Head → A → B → C → D → NULL
```

Key characteristics:

- Each node points **only to the next node**
- Traversal is **one-directional**
- You **cannot move backward**

---

## 🧠 Important Nodes

### Head Node
- The **first node** in the list
- Starting point for traversal

### Tail Node
- The **last node**
- Its `next` reference is **NULL**

---

# 🔍 Traversing a Singly Linked List

Traversal begins at the **head node**.

Example traversal:
```mermaid
Head → A → B → C → D → NULL
```

Steps:

1️⃣ Start at **A**  
2️⃣ Move to **B**  
3️⃣ Move to **C**  
4️⃣ Move to **D**  
5️⃣ Stop at **NULL**

Traversal only moves **forward**.

---

# ➕ Inserting Nodes

Linked lists **do not have a fixed size**.

You can insert nodes at:

- Beginning
- Middle
- End

---

## Insert at the Beginning

Steps:

1️⃣ Create new node  
2️⃣ Point it to current head  
3️⃣ Update head to new node  
```mermaid
Before:
Head → A → B → C

Insert E at start

After:
Head → E → A → B → C
```

⏱ **Time Complexity:** `O(1)`  
💾 **Space Complexity:** `O(1)`

---

## Insert at the End

Steps:

1️⃣ Traverse to the **tail node**  
2️⃣ Connect new node  
```mermaid
Before:
A → B → C → NULL

Insert D

After:
A → B → C → D → NULL
```

⏱ **Time Complexity:** `O(n)` (must traverse list)

---

## Insert in the Middle

Steps:

1️⃣ Find previous node  
2️⃣ Update references
```mermaid
Before:
A → B → C

Insert X between B and C

After:
A → B → X → C
```

⏱ **Time Complexity:** `O(n)`

---

# ➖ Removing Nodes

Nodes can also be removed from:

- Beginning
- Middle
- End

---

## Remove from Beginning

Steps:

1️⃣ Move head pointer to next node
```mermaid
Before:
Head → A → B → C

Remove A

After:
Head → B → C
```

⏱ **Time Complexity:** `O(1)`

---

## Remove from Middle

Steps:

1️⃣ Find previous node  
2️⃣ Connect it to the next node  
```mermaid
Before:
A → B → C

Remove B

After:
A → C
```

⏱ **Time Complexity:** `O(n)`

---

## Remove from End

Steps:

1️⃣ Traverse to node before tail  
2️⃣ Remove last connection  
```mermaid
Before:
A → B → C

Remove C

After:
A → B → NULL
```

⏱ **Time Complexity:** `O(n)`

---

# 🔁 Doubly Linked Lists

## 🔹 What is a Doubly Linked List?

A **doubly linked list** stores **two references** in each node:

- Pointer to **next node**
- Pointer to **previous node**
```mermaid
NULL ← A ⇄ B ⇄ C ⇄ D → NULL
```

This allows traversal in **both directions**.

---

# 🔄 Traversal

Doubly linked lists can move:

➡ **Forward**  
⬅ **Backward**

Example:
```mermaid
Forward: A → B → C → D
Backward: D → C → B → A
```

---

# 📌 Tail Reference

Doubly linked lists often store a **tail pointer**.

Benefits:

- Fast insertion at end
- Easy backward traversal

---

# ⚠️ Tradeoffs

Doubly linked lists require **more memory**.

Each node stores:

- Data
- Next pointer
- Previous pointer

This increases memory usage compared to singly linked lists.

---

# ⚙️ Insert and Delete Operations

Operations are **similar to singly linked lists**, but you must update:

- **Next reference**
- **Previous reference**

Example:
```mermaid
A ⇄ B ⇄ C

Insert X between B and C

A ⇄ B ⇄ X ⇄ C
```

---

# ⚖️ Singly vs Doubly Linked Lists

| Feature | Singly Linked List | Doubly Linked List |
|------|------|------|
| References per node | 1 | 2 |
| Traversal | One direction | Two directions |
| Memory usage | Less | More |
| Backward traversal | ❌ Not possible | ✅ Possible |
| Complexity | Simpler | Slightly more complex |

---

# 🎯 Key Takeaways

✅ **Singly Linked Lists**
- One pointer per node
- Less memory
- One-direction traversal

✅ **Doubly Linked Lists**
- Two pointers per node
- Bidirectional traversal
- More flexible but uses more memory

---

# 🚀 Why Linked Lists Are Important

Linked lists are widely used for:

- Dynamic memory allocation
- Implementing stacks and queues
- Graph traversal algorithms
- Memory management systems

Understanding linked lists helps developers build **efficient and flexible data structures**.
