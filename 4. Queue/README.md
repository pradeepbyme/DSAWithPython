<h1>Queue - Data Structure</h1>

A **queue** is a linear data structure that follows the **First In, First Out (FIFO)** principle. This means that elements are added to the back (end) of the queue and removed from the front (beginning). The queue data structure is widely used in scenarios where tasks are handled in the order they arrive, like in print spooling, CPU task scheduling, or handling requests in a server.

### 1\. **Types of Queues**

*   **Simple Queue** (or Linear Queue): This is the basic type where elements are inserted at the back and removed from the front. Once an element is dequeued, it cannot be reinserted without moving the remaining elements.
    
*   **Circular Queue**: This is an improvement over a simple queue, where the last position connects to the first position, making the queue circular. This helps in optimizing space usage.
    
*   **Priority Queue**: Each element has a priority associated with it. Elements with higher priority are dequeued before elements with lower priority.
    
*   **Double-Ended Queue (Deque)**: Elements can be added or removed from both ends (front and back) of the queue.
    

### 2\. **Basic Queue Operations**

Queues support several essential operations. Here’s a look at each:

*   **Enqueue**: Adds an element to the back of the queue.
    
*   **Dequeue**: Removes an element from the front of the queue.
    
*   **Front/Peek**: Returns the element at the front of the queue without removing it.
    
*   **Rear**: Returns the element at the back of the queue without removing it.
    
*   **isEmpty**: Checks if the queue is empty.
    
*   **isFull** (optional, especially in fixed-size queues): Checks if the queue has reached its maximum capacity.
    

### 3\. **Queue Operations in Detail**

Here’s a breakdown of how each operation works:

#### Enqueue (Insertion)

*   **Definition**: Adds a new element to the end of the queue.
    
*   **Steps**:
    
    1.  Check if the queue is full. If it is, raise an overflow error (in fixed-size implementations).
        
    2.  If not full, increment the rear pointer and add the new element there.
        

#### Dequeue (Removal)

*   **Definition**: Removes the element at the front of the queue.
    
*   **Steps**:
    
    1.  Check if the queue is empty. If it is, raise an underflow error.
        
    2.  If not empty, remove the element at the front of the queue.
        

#### Front (Peek)

*   **Definition**: Returns the element at the front of the queue without removing it.
    
*   **Steps**:
    
    1.  Check if the queue is empty. If it is, indicate that the queue is empty.
        
    2.  If not empty, return the element at the front.
        

#### isEmpty

*   **Definition**: Checks if the queue has any elements.
    
*   **Steps**:
    
    1.  Return True if the queue length is zero; otherwise, return False.
        

#### isFull (for Fixed-Size Queue)

*   **Definition**: Checks if the queue has reached its maximum capacity.
    
*   **Steps**:
    
    1.  Compare the length of the queue with its maximum capacity.
        
    2.  Return True if the queue is full; otherwise, False.
        

### 4\. **Queue Implementation in Python**

A queue can be implemented using:

*   **List**: Though easy to use, it has drawbacks in terms of efficiency, especially in dequeue operations, as removing an element from the front requires shifting all elements.
    
*   **collections.deque**: A deque (double-ended queue) from Python’s collections module is an efficient choice as it allows O(1) time complexity for both enqueue and dequeue operations.
    

### 5\. **Applications of Queues**

Queues have many applications in computer science and real-world systems:

*   **CPU Scheduling**: Processes are scheduled based on arrival, using a queue.
    
*   **Breadth-First Search (BFS)**: In graph traversal, BFS uses a queue to explore nodes level-by-level.
    
*   **Printers**: Print jobs are managed in a queue, where the first submitted job is printed first.
    
*   **Network Buffers**: Data packets are queued up before processing or sending.</br>


<b>Credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme)