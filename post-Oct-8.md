# Things learned so far 
  ## Layers of computing system
  
  ### Information
  machine language, binary numbers, data representation of text…
  ### Hardware
  #### The physical components of a computer or electronic device.
  **Firmware**: A specific type of software that is embedded into hardware devices.
  Ram: random access memory<br>
  CPU: central process unit<br>
  GPU: graphic process unit (graphic card)<br>
  SSD: solid state drive<br>
  HDD: hard disk drive<br>
  ### programming
  how to program, apply logic in simple way. (sequential: 1,2,3; <br>
  choice: if, else, then that…(branching(if else));<br>
  batch processing(looping, for i in range)→ algorithm. sorting, searching.<br>
  ### operating system
  A type of system software that manages hardware and software resources on a computer.
  - Acts as an intermediary between users/applications and hardware.
  - Manages system resources, including the CPU, memory, storage, and input/output devices.
  - Provides a user interface (UI) for interaction, such as command-line or graphical interfaces.
  - Handles tasks like file management, process management, security, and multitasking.
  - Examples include Windows, macOS, Linux, and Android.
  ### applications
  Applications, often referred to as apps, are software programs designed to perform specific tasks for users. They can be installed on various devices, including computers, smartphones, tablets, and other electronic devices.
  ### network(communication)
  cable, datalink, network, transport, section, presentation, application.

  ## Linked list (HL)
  ### single
  single head, single tail (first and last node) <br>each pointer works in one direction only
  ### double
  single head, single tail (first and last node)<br>each pointer works in one direction only
  ### circular
  single head<br>one pointer for each node, last tail node’s pointer points to the head, no tail, no null
  ### misc
  array is a non-editable static data structure<br>
  index(address, start with 0,1,2,3…) usually written: num[this is the index placeholder]<br>
  units in linked list:<br>node, data, pointer, head(contains pointer to the first node), tail(point to null, or the head depending on if it is circular)<br>
  pointers and data are the field/attribute of node<br>
  linked list can be empty<br>
  length of linked list depends on number of elements<br>
  last node contains a null pointer<br>
  double linked list has predecessor pointing to the previous node, so can go back<br>

  ## Data representation
  https://www.canva.com/design/DAGRQzUBbQE/SAd1et0YhybexDDyu771vQ/view?utm_content=DAGRQzUBbQE&utm_campaign=designshare&utm_medium=link&utm_source=editor
  ## Logic gates
  ### And gate
  Outputs true (1) only if both inputs A and B are true (1).
  ### Or gate
  Outputs true (1) if at least one input A or B is true (1).
  ### Not gate
  Outputs the opposite of the input A. If A is true (1), output is false (0), and vice versa.
  ### Xor gate
  Outputs true (1) if exactly one of the inputs A or B is true (1), but not both. (so true when the two inputs are different)
  ### Nor gate
  Outputs true (1) only if both inputs A and B are false (0). It is the opposite of the OR gate.
  ### Nand gate
  Outputs false (0) only if both inputs A and B are true (1). It is the opposite of the AND gate.
  
  ## Tree traversal
  ### rooted tree
  there will always be a root at the top<br>
  then a link/reference/pointer to another node<br>
  every other node is a descendant/child of the root.<br>
  leaf nodes are the edge-most nodes. so they don't have children.<br>
  the parent leads to 2 children.<br>
  tree can have multiple nodes, but in the binary tree, there will be only 2 children for a parent. called left-child and right-child. so each child also has only 1 parent.<br>
  the root can point to null if there is no child, but it can also point to the first node<br>
  a node can contain values and must contain 2 pointers even if there is no child, it will just point to null<br>
  ### Traversal of a Binary tree
  means to visit each node of the tree in some order<br>
  go to the node, see the value, and do something.<br>
  searching is comparing every node we travel to the value we are looking for.<br>
  three principal ways of traversing a binary tree:<br>
  1. pre-order traversal<br>
    a. imagine a flag before every node on the left of the node. Traverse it starting from root node, touching the flag of it. (read out the value of root) then go down from left to the child and child of child. Like wrapping the tree.<br>
    b. so always start from higher parent node, coming down to its left-child then left-child of left child. if it reaches the edge, it goes to the right. always left first.<br>
![Inorder-Traversal-of-Binary-Tree](https://github.com/user-attachments/assets/3b893a2c-1b4e-438f-aae5-9ed8f93dea64)<br>
  2. in-order traversal<br>
    a. start from left, all the way to left leaf, visit the left sub-tree, and visit the root of the left sub-tree. then go left root, right child then root then left child of right parent.<br>
    b. flags are on the bottom of each node<br>
<img width="782" alt="Inorder-binarytree-image4-c7MYU1Kf" src="https://github.com/user-attachments/assets/e9c4b8fd-f621-4f5a-a757-5823f2c6148b"><br>
  3. postorder traversal<br>
    a. go with the same direction of pre-order, but flags are on the right side.<br>
    b. the main root will be visited last.<br><br>
![Postorder-Traversal-of-Binary-Tree](https://github.com/user-attachments/assets/47d26c33-fec1-4d80-b4c1-3e4cc5997892)<br>


