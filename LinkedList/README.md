<h1>Linked List - Data Structure</h1>
Linked lists are a fundamental data structure that consist of nodes connected sequentially. Each node in a linked list has two components:

1.  **Data**: Holds the actual value or data the node is storing.
    
2.  **Pointer (or Reference)**: Holds a reference to the next node in the sequence.
    

Linked lists are dynamic data structures, meaning they do not require a fixed size and can grow or shrink in memory as needed. They are particularly useful when frequent insertions and deletions are needed, as these operations can be more efficient than in arrays.

### Types of Linked Lists

1.  **Singly Linked List**:
    
    *   Each node has a reference to the next node.
        
    *   It allows traversal only in one direction (forward).
        
2.  **Doubly Linked List**:
    
    *   Each node has two references: one to the next node and one to the previous node.
        
    *   This allows traversal in both directions (forward and backward).
        
3.  **Circular Linked List**:
    
    *   The last node’s next reference points back to the first node, creating a circular structure.
        
    *   Can be singly or doubly linked.
        

### Operations on Linked Lists

#### 1\. **Insertion**

*   **At the Beginning**:
    
    *   Create a new node.
        
    *   Point the new node’s next to the current head of the list.
        
    *   Update the head of the list to be the new node.
        
*   **At the End**:
    
    *   Traverse to the last node.
        
    *   Set the last node’s next to the new node.
        
    *   For a doubly linked list, also set the new node’s prev to the last node.
        
*   **At a Specific Position**:
    
    *   Traverse to the node just before the desired position.
        
    *   Set the new node’s next to the next node in the list.
        
    *   Update the previous node’s next to the new node.
        

#### 2\. **Deletion**

*   **From the Beginning**:
    
    *   Change the head to point to the next node.
        
*   **From the End**:
    
    *   Traverse to the second-to-last node.
        
    *   Set its next to None.
        
*   **From a Specific Position**:
    
    *   Traverse to the node just before the desired position.
        
    *   Update its next to skip the node to be deleted.
        

#### 3\. **Traversal**

*   Traversing a linked list involves starting at the head and moving from node to node by following the next pointers.
    
*   For a doubly linked list, you can traverse both forward and backward.
    

#### 4\. **Searching**

*   Searching in a linked list involves traversing from the head until the target value is found or the end of the list is reached.
    
*   Time complexity for searching is O(n)O(n)O(n) because, in the worst case, each node must be visited.
    

#### 5\. **Reversing a Linked List**

*   Reversing a linked list involves reversing the direction of the next pointers for each node.
    
*   For a singly linked list, keep track of the previous node, current node, and the next node while iterating through the list.
    

#### 6\. **Detecting a Cycle in a Linked List**

*   Use **Floyd’s Cycle Detection Algorithm** (or the Tortoise and Hare algorithm).
    
*   It involves two pointers, one moving at normal speed (slow) and the other moving twice as fast (fast). If they meet, there is a cycle.
    

### Advantages and Disadvantages

**Advantages**:

*   **Dynamic Size**: No need to specify initial size, as in arrays.
    
*   **Efficient Insertions/Deletions**: Unlike arrays, elements can be added or removed without shifting other elements.
    

**Disadvantages**:

*   **No Random Access**: Accessing elements is linear (O(n)), unlike arrays.
    
*   **Extra Memory for Pointers**: Each node stores an extra reference to the next node, increasing memory usage.


<b>credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme) 