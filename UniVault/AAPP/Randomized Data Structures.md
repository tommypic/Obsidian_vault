
### Dictionaries
- they use a unique search  key
#### List of operations
- min and max, search insert, delete
- list (output the list of all elements by order of key value)
- Union(S1, S2), union of the two dict with the condition that the 
- Split(S,x, S1, S2) split S in S1 and S2
#### Implementation
- Arrays
- Bst
- splay tree
- AVL tree
- random treaps 
- Skip list
### Arrays
1. Ordered:
	- O(logn ) for search
	- O(n) for insert
2.  Unordered
	- O(n) for search
	- O(1) for insert
## Bst 
- each internal node stores an item(k, e) of the dictionary
- key on the left are less and on the right are greater
- problem is that the height is not always nlog(n)
## AVL Tree
- splaying is used to self adjust the tree
- there are rotations that makes the tree of always the same height
- they adjust every time is inserted a new elem
## Splay Tree
- splaying is used to put the more accessed nodes to the top of the tree
- they restructure the tree not only updates but also during search operation
## Treaps
It is a binary tree 
- each element conains a **key** and a **priority**
- they have two proprerty: 
	- normal proprety of bst for value of key
	- the child always have **lowere priority** of the parent
This is the code for inserting :
1. Choose prio(x). 
2. Search for the position of x in the tree.
3. Insert x as a leaf.
4. Restore the heap property. while prio(parent(x)) > prio(x) do if x is left child then RotateRight(parent(x)) else RotateLeft(parent(x)); endif endwhile;








  
  
  