<h1>Stack - Data Structure</h1>

A **stack** is a linear data structure that follows the **LIFO (Last In, First Out)** principle. This means the last element added to the stack is the first one to be removed. Imagine a stack of plates: you add plates to the top, and when you want to take a plate, you remove the one on top.

Stacks are widely used in programming, especially for tasks that involve reversing, parsing, and managing nested structures (like parentheses in expressions).

### Key Characteristics of a Stack

1.  **LIFO Order**: Elements are added and removed from the same end, called the **top** of the stack.
    
2.  **Restricted Access**: Only the top element of the stack is accessible for reading and writing, making it a controlled data structure.
    

### Common Operations on a Stack

1.  **Push**: Adds an element to the top of the stack.
    
2.  **Pop**: Removes the top element of the stack.
    
3.  **Peek (or Top)**: Returns the top element without removing it.
    
4.  **isEmpty**: Checks if the stack is empty.
    
5.  **isFull** (in bounded stacks): Checks if the stack is full, though this is mostly relevant in limited-capacity stack implementations.
    

### Basic Stack Operations Explained

#### 1\. **Push Operation**

*   **Purpose**: To insert a new element on top of the stack.
    
*   **Process**:
    
    1.  Check if the stack is full (only relevant if the stack has a fixed size).
        
    2.  If not, add the element at the top position of the stack.
        
    3.  Increment the stack pointer (top) by 1 to reflect the new top position.
        
*   **Example**:If the stack initially has \[1, 2, 3\] and we push 4, the stack becomes \[1, 2, 3, 4\].
    

#### 2\. **Pop Operation**

*   **Purpose**: To remove the element at the top of the stack.
    
*   **Process**:
    
    1.  Check if the stack is empty (underflow condition).
        
    2.  If not, access the element at the top of the stack.
        
    3.  Remove the element from the stack and decrement the top pointer by 1.
        
*   **Example**:If the stack has \[1, 2, 3, 4\] and we pop, it removes 4, resulting in \[1, 2, 3\].
    

#### 3\. **Peek (or Top) Operation**

*   **Purpose**: To look at the top element without modifying the stack.
    
*   **Process**:
    
    1.  Check if the stack is empty.
        
    2.  If not, return the element at the top.
        
*   **Example**:If the stack is \[1, 2, 3, 4\], then peek will return 4.
    

#### 4\. **isEmpty Operation**

*   **Purpose**: To check if the stack is empty.
    
*   **Process**:
    
    1.  If the top pointer is at the initial position (usually -1 in an array-based implementation), return True.
        
    2.  Otherwise, return False.
        
*   **Example**:For an empty stack \[\], isEmpty would return True.
    

#### 5\. **isFull Operation**

*   **Purpose**: To check if the stack has reached its maximum capacity.
    
*   **Process**:
    
    1.  If the top pointer is at the maximum position (like size - 1 in a fixed-size array implementation), return True.
        
    2.  Otherwise, return False.
        
*   **Example**:For a stack with a maximum size of 5, if it has \[1, 2, 3, 4, 5\], then isFull will return True.
    

### Applications of Stacks

Stacks are incredibly useful in a variety of scenarios, including:

1.  **Function Call Stack**: Manages function calls and returns in programming.
    
2.  **Expression Evaluation and Parsing**: Used in evaluating expressions (postfix, infix, and prefix) and parsing expressions in compilers.
    
3.  **Undo Mechanisms**: Stores previous actions in applications, allowing users to revert to prior states.
    
4.  **Backtracking Algorithms**: Used in algorithms where previous states need to be stored, like solving mazes or navigating paths.
    
5.  **Balanced Parentheses and Syntax Checking**: Ensures expressions have correct nesting, such as in code or mathematical expressions.</br>


<b>Credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme)