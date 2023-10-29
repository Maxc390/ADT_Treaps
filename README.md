# ADT_Treaps
Abstract Data Type: Treap

A Treap is a data structure that combines the properties of a binary search tree (BST) and a max-heap. The name "Treap" is a portmanteau of "tree" and "heap." It is an example of an abstract data type (ADT) used for maintaining a dynamic set of elements with certain operations like insertion, deletion, and search, just like a traditional BST.

Properties:
Binary Search Tree (BST) Property: A Treap is a binary search tree, which means that it satisfies the following properties:

Each node has at most two children: a left child and a right child.
For any given node, all elements in the left subtree have values less than or equal to the node's value, and all elements in the right subtree have values greater than the node's value.

Max-Heap Property: In addition to the BST property, a Treap maintains the following max-heap property:

Each node has a priority value, and the priority of a node is greater than or equal to the priorities of its children. Priorities are used to maintain the heap structure of the Treap.

Random Priorities: A key feature of the Treap is the random assignment of priorities to nodes. Each node's priority is typically generated randomly and is used to ensure the balancing of the tree. This randomness helps maintain good average-case performance for various operations.

Data:
The Treap consists of a collection of nodes, where each node has the following components:
key: A value that is used to determine the node's position in the BST (subject to the BST property).
priority: A randomly assigned value used to maintain the max-heap property.
Operations:
Insertion:

Description: Inserts a new element with a specified key and randomly assigned priority into the Treap while maintaining the BST and max-heap properties.
Input: key (element's value), priority (random priority value).
Output: None.

Deletion:

Description: Removes an element with a specified key from the Treap while preserving the BST and max-heap properties.
Input: key (element's value).
Output: None.

Search:

Description: Searches for an element with a specified key in the Treap and returns the element if found.
Input: key (element's value).
Output: Element with the specified key or indication that the element is not found.
Rotation:

Description: Perform rotation operations to maintain the BST and max-heap properties. Rotations are typically used during insertions and deletions.
Input: None.
Output: None.

Traversal:

Description: Traverses the Treap in various orders (e.g., in-order, pre-order, post-order) to access elements in a particular sequence.
Input: Traversal order.
Output: Elements visited in the specified order.

Size:

Description: Returns the number of elements in the Treap.
Input: None.
Output: Integer representing the number of elements in the Treap.

Empty:

Description: Checks if the Treap is empty.
Input: None.
Output: Boolean indicating whether the Treap is empty.

Time Complexity:
On average, the time complexity of the insert, delete, and search operations is O(log n), where n is the number of elements in the Treap. The random priorities contribute to this expected logarithmic behavior.


