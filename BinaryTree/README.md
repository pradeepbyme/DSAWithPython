<h1>Binary Tree - Data Structure 🌳</h1> 
Binary trees are a fundamental data structure in computer science, used in a variety of applications from search algorithms to data organization. They are a type of hierarchical data structure that consists of nodes, with each node having at most two children, often referred to as the _left_ child and _right_ child.

Here's a detailed look into binary trees, their properties, and the common operations performed on them:

### 1\. **Basic Structure and Properties of Binary Trees**

A binary tree is made up of nodes, where:

*   Each node contains a data element.
    
*   Each node has two pointers (or references) to other nodes, commonly known as the left and right children.
    
*   The node at the top of the hierarchy is called the **root**.
    
*   Nodes that have no children are called **leaf nodes**.
    
*   A **subtree** refers to any node along with its descendants (children, grandchildren, etc.).
    

#### Properties of Binary Trees:

*   **Depth**: The level at which a node exists in the tree, with the root node at level 0.
    
*   **Height**: The maximum depth of any node, or the longest path from the root to a leaf.
    
*   **Complete Binary Tree**: A tree where every level is fully filled except possibly the last, which is filled from left to right.
    
*   **Full Binary Tree**: A tree where every node has either 0 or 2 children.
    
*   **Perfect Binary Tree**: A tree that is both full and complete, with all leaf nodes at the same level.
    

### 2\. **Types of Binary Trees**

Binary trees can take on various forms based on constraints:

*   **Binary Search Tree (BST)**: A binary tree where the left child of a node contains only values less than the node, and the right child contains only values greater.
    
*   **AVL Tree**: A self-balancing BST where the heights of two child subtrees differ by at most one.
    
*   **Red-Black Tree**: Another self-balancing binary tree with specific properties for balancing using colors.
    
*   **Heap**: A binary tree that maintains a "heap" property, where every node is either greater than (max-heap) or less than (min-heap) all its children.
    

### 3\. **Common Operations on Binary Trees**

#### **1\. Insertion**

*   **In a Binary Tree**: Insertion is usually done in the first vacant position found in a level-order traversal.
    
*   **In a Binary Search Tree (BST)**: The new node is added based on its value. If the value is less than the current node, it goes to the left child; if greater, it goes to the right child. This preserves the BST properties.
    

#### **2\. Deletion**

*   **Leaf Node**: If the node is a leaf, simply remove it.
    
*   **Node with One Child**: If the node has one child, delete it and link its child directly to its parent.
    
*   **Node with Two Children**: In a BST, replace the node to be deleted with its in-order successor (smallest node in its right subtree) or in-order predecessor (largest node in its left subtree).
    

#### **3\. Traversal**

Traversal is the process of visiting each node in the tree in a specific order. There are three primary types of depth-first traversal in binary trees:

*   **Inorder Traversal (Left, Root, Right)**:
    
    *   Process all nodes in the left subtree.
        
    *   Process the root node.
        
    *   Process all nodes in the right subtree.
        
    *   **Use**: In a BST, inorder traversal visits nodes in ascending order.
        
*   **Preorder Traversal (Root, Left, Right)**:
    
    *   Process the root node.
        
    *   Process all nodes in the left subtree.
        
    *   Process all nodes in the right subtree.
        
    *   **Use**: Often used for copying or cloning the tree structure.
        
*   **Postorder Traversal (Left, Right, Root)**:
    
    *   Process all nodes in the left subtree.
        
    *   Process all nodes in the right subtree.
        
    *   Process the root node.
        
    *   **Use**: Useful for deleting or freeing nodes as it visits children before the parent.
        
*   **Level-order Traversal (Breadth-First)**:
    
    *   Visit nodes level by level from top to bottom, using a queue.
        
    *   **Use**: Often applied in shortest-path algorithms.
        

#### **4\. Searching**

*   **Binary Search in a BST**: If the tree is a BST, searching can be done efficiently by comparing the target value to each node. If the target is less than the current node, search the left subtree; if greater, search the right subtree.
    
*   **General Search**: For non-BST trees, perform a breadth-first or depth-first traversal and compare each node.
    

#### **5\. Finding Minimum and Maximum**

*   **In a BST**: The minimum value is found at the leftmost node, and the maximum at the rightmost node.
    
*   **In a General Binary Tree**: Requires a complete traversal to check each node’s value.
    

#### **6\. Calculating Height**

*   The height of a binary tree can be calculated recursively by finding the maximum height between the left and right subtrees and adding one for the root node.
    

#### **7\. Mirror of a Binary Tree**

*   This involves swapping the left and right children of all nodes in the tree, effectively flipping the tree.
    

#### **8\. Checking Tree Properties**

*   **Checking if a Tree is Balanced**: A balanced tree has minimal height difference between subtrees. This can be checked by recursively ensuring each node's subtrees differ by no more than one level.
    
*   **Checking if a Tree is a BST**: A binary tree can be checked to see if it maintains the BST property by ensuring each node’s value lies within a valid range depending on its ancestors.
    

### 4\. **Applications of Binary Trees**

*   **Binary Search Trees**: Used in databases, file systems, and for maintaining sorted data efficiently.
    
*   **Heaps**: Applied in priority queues, shortest path algorithms, and heap sort.
    
*   **Tries**: Useful in implementing dictionaries and autocomplete features.
    
*   **Huffman Encoding Trees**: Used in data compression algorithms, like for compressing text files.</br>


<b>Credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme)