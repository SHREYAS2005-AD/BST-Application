 Application of Trees (Binary Search Tree)

 Scenario

Consider a **student record management system** where each student is identified by a unique roll number.

* New students are added → Insert into BST
* Records need to be viewed in sorted order → Inorder traversal
* Specific student record may need removal → Delete operation

A Binary Search Tree (BST) is used to efficiently manage these operations.

---

 Justification

Binary Search Tree is chosen because:

* It maintains **sorted order automatically**
* Allows **fast searching, insertion, and deletion**
* Efficient for dynamic datasets (size not fixed)
* Traversals provide structured outputs:

  * Inorder → Sorted data
  * Preorder/Postorder → Tree structure understanding



## Algorithm

### 1. Insertion

1. Create a new node
2. If root is NULL → make new node as root
3. Compare data:

   * If smaller → go to left subtree
   * If larger → go to right subtree
4. Repeat until correct position is found
5. Insert node

---

### 2. Inorder Traversal (LNR)

1. Traverse left subtree
2. Visit root
3. Traverse right subtree

---

### 3. Preorder Traversal (NLR)

1. Visit root
2. Traverse left subtree
3. Traverse right subtree

---

### 4. Postorder Traversal (LRN)

1. Traverse left subtree
2. Traverse right subtree
3. Visit root

---

### 5. Deletion

1. Search for node
2. Case handling:

   * Leaf node → delete directly
   * One child → replace with child
   * Two children → replace with inorder successor

---

## ⏱ Time Complexity

| Operation  | Average Case | Worst Case |
| ---------- | ------------ | ---------- |
| Insertion  | O(log n)     | O(n)       |
| Deletion   | O(log n)     | O(n)       |
| Searching  | O(log n)     | O(n)       |
| Traversals | O(n)         | O(n)       |

---

##  Code

(Refer to bst.c uploaded in repository)

---

##  Execution

### Steps to Run:

1. Compile the program:

```
gcc bst.c -o bst
```

2. Execute:

```
./bst
```

---

##  GitHub Repository

The complete implementation is available here:

 https://github.com/SHREYAS2005-AD/BST-Application

---

##  Author

Shreyas
