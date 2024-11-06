<h1>Binary Heap - Data structure</h1>

A **binary heap** is a complete binary tree that satisfies the heap property. It’s a specific type of binary tree structure where each parent node has a specific relationship with its children, making it very efficient for tasks that require quick access to the smallest or largest elements, such as implementing priority queues.

Binary heaps are of two types:

1.  **Min-Heap**: In a min-heap, the key at the root is the minimum among all keys in the heap. Every parent node has a value smaller than or equal to the values of its children.
    
2.  **Max-Heap**: In a max-heap, the key at the root is the maximum among all keys in the heap. Every parent node has a value greater than or equal to the values of its children.
    

### Characteristics of Binary Heaps

*   **Complete Binary Tree**: All levels of the tree are fully filled except possibly for the last level, which is filled from left to right. This structure ensures the tree is balanced and height remains logarithmic (O(log n)).
    
*   **Heap Property**: Each node must satisfy the min-heap or max-heap property.
    
*   **Array Representation**: Binary heaps are often implemented using arrays due to their compactness and efficient indexing. For a node at index i, its left child is at index 2\*i + 1, and the right child is at index 2\*i + 2. The parent node of any node i is located at (i - 1) // 2.
    

### Basic Operations on Binary Heaps

Binary heaps support several essential operations:

#### 1\. **Insert**

*   **Description**: Insertion adds a new element to the heap while maintaining the heap property.
    
*   **Process**:
    
    1.  Place the new element at the end of the array (the last position in the heap).
        
    2.  "Heapify Up" (also called bubble up or sift up): Compare the new element with its parent, and if it violates the heap property, swap them.
        
    3.  Continue moving the element up the tree until the heap property is restored.
        
*   **Time Complexity**: O(log n) due to the height of the tree.
    

#### 2\. **Extract Min / Extract Max**

*   **Description**: This operation removes and returns the root element, which is the minimum in a min-heap or maximum in a max-heap.
    
*   **Process**:
    
    1.  Replace the root with the last element in the heap (to maintain the complete binary tree structure).
        
    2.  Remove the last element.
        
    3.  "Heapify Down" (also called bubble down or sift down): Starting from the root, swap the element with its smallest (or largest, in a max-heap) child if it violates the heap property.
        
    4.  Repeat until the heap property is restored.
        
*   **Time Complexity**: O(log n).
    

#### 3\. **Peek / Get Min or Max**

*   **Description**: This operation returns the minimum (or maximum) element without removing it from the heap.
    
*   **Process**: Simply return the root element.
    
*   **Time Complexity**: O(1).
    

#### 4\. **Delete**

*   **Description**: Delete an arbitrary element from the heap while maintaining the heap property.
    
*   **Process**:
    
    1.  Replace the element to be deleted with the last element in the heap.
        
    2.  Remove the last element.
        
    3.  Perform "Heapify Up" if the replaced element is smaller than its parent (min-heap) or "Heapify Down" if it’s larger than its children.
        
*   **Time Complexity**: O(log n), due to heapify operations.
    

#### 5\. **Build Heap**

*   **Description**: This operation constructs a heap from an unordered array of elements.
    
*   **Process**:
    
    1.  For each non-leaf node (starting from the last non-leaf node up to the root), perform the "Heapify Down" operation.
        
    2.  This builds a valid binary heap from the bottom up.
        
*   **Time Complexity**: O(n), which is more efficient than performing individual insertions for each element.
    

### Applications of Binary Heaps

1.  **Priority Queues**: Binary heaps are commonly used to implement priority queues, as they allow fast access to the highest or lowest priority element.
    
2.  **Heap Sort**: An efficient comparison-based sorting algorithm that uses a binary heap to sort elements in O(n log n) time.
    
3.  **Graph Algorithms**: Many graph algorithms, like Dijkstra’s shortest path, use heaps for efficient retrieval of minimum weights or distances.
    
4.  **Scheduling**: Binary heaps help in task scheduling where tasks with the highest priority are executed first.
    

### Advantages of Binary Heaps

*   **Efficiency**: The array representation makes it memory-efficient, and accessing the minimum or maximum element is constant-time.
    
*   **Logarithmic Insertions and Deletions**: The tree’s balanced structure ensures that insertions, deletions, and extractions are efficient, with logarithmic complexity.
    
*   **Versatility in Applications**: Useful for various applications involving priority management or sorted order processing.
    

### Disadvantages of Binary Heaps

*   **Fixed Priority Retrieval**: Binary heaps are excellent for retrieving the smallest or largest element but inefficient for retrieving arbitrary elements within the heap.
    
*   **Limited Flexibility**: Binary heaps don’t support efficient search for non-root elements, as they are not organized by order other than the root’s priority relationship with its children.</br>


<b>Credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme)