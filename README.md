Voici une version plus lisible, avec un peu plus de structure et de style.

Binary Trees
This repository contains C functions and helper files used to implement and manipulate binary trees for the Holberton School low-level programming curriculum.
​

 Project overview
The main objectives of this project are to understand how binary trees work and how to:

Create and delete binary tree nodes.
​

Traverse a tree in preorder, inorder and postorder.
​

Compute height, depth, size, number of leaves and number of internal nodes.
​

Check if a tree is full or perfect.
​

Find the sibling and uncle of a given node.
​

All code is written in C and follows the Betty style guidelines.
​

 Project structure
Header
binary_trees.h – Contains the binary_tree_t structure definition and all function prototypes.
​

Core functions
0-binary_tree_node.c – Create a binary tree node.
​

1-binary_tree_insert_left.c – Insert a node as the left child of another node.
​

2-binary_tree_insert_right.c – Insert a node as the right child of another node.
​

3-binary_tree_delete.c – Delete an entire binary tree.
​

4-binary_tree_is_leaf.c – Check if a node is a leaf.
​

5-binary_tree_is_root.c – Check if a node is the root of the tree.
​

Traversal
6-binary_tree_preorder.c – Preorder traversal.
​

7-binary_tree_inorder.c – Inorder traversal.
​

8-binary_tree_postorder.c – Postorder traversal.
​

Measurements
9-binary_tree_height.c – Measure the height of a tree.
​

10-binary_tree_depth.c – Measure the depth of a node.
​

11-binary_tree_size.c – Measure the size (number of nodes) of a tree.
​

12-binary_tree_leaves.c – Count the leaves in a tree.
​

13-binary_tree_nodes.c – Count the nodes with at least one child.
​

Properties
14-binary_tree_balance.c – Measure the balance factor of a tree.
​

15-binary_tree_is_full.c – Check if a tree is full.
​

16-binary_tree_is_perfect.c – Check if a tree is perfect.
​

Relations
17-binary_tree_sibling.c – Find the sibling of a node.
​

18-binary_tree_uncle.c – Find the uncle of a node.
​

Helpers
binary_tree_print.c – Helper function to print a binary tree (for debugging and visualization).
​

main.c files – Test files provided for each task (not part of the public API).
​

 Data structure
The binary tree node is defined as:

c
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child
 * @right: Pointer to the right child
 */
typedef struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
} binary_tree_t;
This structure is used by all functions in this repository.
​

🔧 Compilation
All files are compiled using gcc with the following flags:

bash
gcc -Wall -Wextra -Werror -pedantic *.c -o binary_trees
Environment:

Ubuntu 20.04 LTS (or similar).
​

gcc with the flags above.
​

 Usage
Clone the repository.

Compile the files you need together with your own main.c.

Include binary_trees.h in your source files to use the binary tree API.
​

Example:

bash
gcc -Wall -Wextra -Werror -pedantic 0-main.c 0-binary_tree_node.c binary_tree_print.c -o 0-node
./0-node
 Author
Project done as part of the Holberton School low-level programming training by Loïc Cerqueira and collaborators.
​
