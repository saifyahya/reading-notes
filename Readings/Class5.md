## Linked List
A linked list is a data structure consisting of nodes that are connected to each other. Each node contains data and a reference to the next node in the sequence. Linked lists come in different types, with singly linked lists having a single reference to the next node, and doubly linked lists having references to both the next and previous nodes.

## Terminology
Linked List: A data structure with nodes linked to each other.
Singly Linked List: Each node has a reference to the next node.
Doubly Linked List: Each node has references to both the next and previous nodes.
Node: An individual item in a linked list containing data and references.
Next: The reference to the next node in the list.
Head: The reference to the first node in the linked list.
Current: A reference used during traversal to point to the current node.
Traversal: Traversal through a linked list involves moving from node to node using the "Next" reference until the end of the list is reached. This is typically done using a while loop. Traversal is crucial for operations like searching and printing.

## Big O
Adding a Node (O(1)): Adding a node to the beginning of a linked list has a time complexity of O(1). To add a new node, a new node object is created, its "Next" reference is set to the current head, and then the head is updated to point to the new node.

Adding a Node (O(n)): Adding a node to the middle of a linked list has a time complexity of O(n). The linked list must be traversed until the desired insertion point is found. The new node's "Next" reference is set to the node that was originally next, and the previous node's "Next" reference is updated to point to the new node.