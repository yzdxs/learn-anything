#[data structures](https://my.mindnode.com/wFP5M2WyuNoFEtCaV8osgMJiYDydghpVJQCn9SUb)

![](http://i.imgur.com/NuNyX2r.jpg)


#mindmap index 🗄️

# [array](http://www.wikiwand.com/en/Array_data_structure)


## description

### array is a **container** which can hold a **fix number of items** and these items should be of the **same type**

### need to understand

- element

	- each item stored in an array is called an element

- index

	- each location of an element in an array has a numerical index, which is used to identify the element

## types of array

### linear array

- a linear array is a list of a finite number of n homogeneous data elements (that is data elements of the same type)

	- such that

		- 1. the elements of the arrays are referenced respectively by an **index set** consisting of **n** consecutive numbers

		- 2. the elements of the arrays are stored respectively in **successive memory locations**

- the number **n** of elements is called the **length** or **size** of the array

- 

- 

- representation of linear array in memory

### multidimensional array

- two-dimensional

	- 

	- 

	- rows of a 2D array

	- columns of a 2D array

	- 

## ops

### unsorted array

- insert: O(1)

- delete: O(1)

	- First swap the element you want to delete to the end of the array, then reduce the array size by one element.

- search: O(n)

	- have to see all in worst case

- space usage: O(n)

### sorted array

- insert: O(n)

- delete: O(n)

- search: O(log n)

	- binary search

- space usage: O(n)

### value-indexed array

- insert: O(1)

- delete: O(1)

- search: O(1)

- space usage: O(n)

## notes

## images

### 

### 

## resources

### [overview](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Arrays/arrays.html)


# [collection (ADT)](http://www.wikiwand.com/en/Collection_(abstract_data_type))


## desc

### In [computer science](http://www.wikiwand.com/en/Computer_science), a collection or container is a grouping of some variable number of data items (possibly zero) that have some shared significance to the problem being solved and need to be operated upon together in some controlled fashion

### Generally, the data items will be of the same type or, in languages supporting inheritance, derived from some common ancestor type

### A collection is a concept applicable to [abstract data types](http://www.wikiwand.com/en/Abstract_data_type), and does not prescribe a specific implementation as a concrete [data structure](http://www.wikiwand.com/en/Data_structure), though often there is a conventional choice (see [Container](http://www.wikiwand.com/en/Container_(type_theory)) for [type theory](http://www.wikiwand.com/en/Type_theory) discussion)

## res


# abstract data type (ADT)


## def

### A set of data values and associated operations that are precisely specified independent of any particular implementation

## notes

### [what is the difference between ADT and data structures?](https://www.quora.com/What-is-the-differences-between-abstract-data-type-and-user-defined-data-type)

- data types

	- **Data types** are **classification of data** in **any programming language** - for example integers, characters, floats etc.

- Abstract data types

	- An **ADT** is just a **theoretical concept** - it's **how any type should look: what operation are allowed** etc. **Implementation is not a part of ADT's**. 

	- Take for example Stacks. A stack ADT can have the operations push, pop, peek. These three operations define what the type can be irrespective of the language of the implementation.

	- One misbelief many people have is that ADT is a concept of OOP. That's just not true. Coming back to our stack, you could implement stack in Ruby (complete OOP), Java (object oriented), Racket (pseudo-OOP), C (procedural) etc. All would have (at least) the same three operations.

## img

### 

### 

### 

- essentially ADT is an abstraction over some functionality

### definition

### ADT implementations

- more implementations

- 

## res

### [overview](https://xlinux.nist.gov/dads/HTML/abstractDataType.html)


# atomic and composite data


## atomic data

### data that consists of a single piece of information

- i.e. integer number 4562

## composite data

### data that can be broken into subfields that have meaning

- i.e. telephone number


# [what is data structure?](https://www.wikiwand.com/en/Data%20structure)


## desc

### machine data representation

### an aggregate of atomic and composite data into a set with defined relationships

- in this definition

- structure means a set of rules that holds the data together

## notes

### the idea is to represent data in the most efficient way possible for the task at hand


# [set (ADT)](http://www.wikiwand.com/en/Set_(abstract_data_type))


## desc

### In [computer science](http://www.wikiwand.com/en/Computer_science), a set is an [abstract data type](http://www.wikiwand.com/en/Abstract_data_type) that can store certain values, without any particular [order](http://www.wikiwand.com/en/Sequence), and no repeated values. 

### It is a computer implementation of the [mathematical](http://www.wikiwand.com/en/Mathematics) concept of a [finite set. ](http://www.wikiwand.com/en/Finite_set)

### Unlike most other [collection](http://www.wikiwand.com/en/Collection_(abstract_data_type)) types, rather than retrieving a specific element from a set, one typically tests a value for membership in a set

## res


# max-heap


## max-heap property

### Each [node](https://xlinux.nist.gov/dads/HTML/node.html) in a [tree](https://xlinux.nist.gov/dads/HTML/tree.html) has a [key](https://xlinux.nist.gov/dads/HTML/key.html) which is less than or equal to the key of its [parent.](https://xlinux.nist.gov/dads/HTML/parent.html)


# [s- expression](http://www.wikiwand.com/en/S-expression)


## RESEARCH: 


# min-heap


## min-heap property

### Each [node](https://xlinux.nist.gov/dads/HTML/node.html) in a [tree](https://xlinux.nist.gov/dads/HTML/tree.html) has a [key](https://xlinux.nist.gov/dads/HTML/key.html) which is greater than or equal to the key of its [parent.](https://xlinux.nist.gov/dads/HTML/parent.html)


# heapify


## **Fixing a node and** its **children in order to form a valid Heap** is often **called heapify**!

### We see that the three green nodes destroy the structure of our heap, because the root (1) is smaller than its children (4) and (5)

### Thus we need to fix this problem and what we’re going to do is to swap the root with its biggest child.

## algo

### We first need to know which is the greatest out of the three items, than in case it is not the root, swap its value with the root!

- As you can see on the picture to the left, the i-th item is first compared to its left child. The greater of these two items is compared to the right child

- Note that we don’t swap them – we just compare them to get which one is greater.

- Once we find the greatest of these three values we swap them with the root in case it’s not the root value.

- Although now these three elements form a heap, by swapping the root with one of its children may destroy the heap constructed out of this child

- That is why we continue the same procedure with it.

	- This actually gives us the procedure to heapify the three nodes constructed out of the i-th item and its children.

	- However to build a heap from an arbitrary array we should perform this operation starting from floor(len[A] / 2) down to the first item in the array.

## notes

### running time of building a heap: O(n)

### heapify: O(log n)

- for all elements

- When heapify is called, the running time depends on how far an element might move down in tree before the process terminates. In other words, it depends on the height of the element in the heap. In the worst case, the element might go down all the way to the leaf level.

## res

### [amazing overview](http://www.stoimen.com/blog/2012/08/07/computer-algorithms-heap-and-heapsort-data-structure/)


# priority queue


# [tree-based](http://www.wikiwand.com/en/Tree_(data_structure))


## [heaps](http://www.wikiwand.com/en/Heap_(data_structure))

### desc

- tree-based data structure that satisfies the **heap property**

- heap is a **complete binary tree**, where **all** the **parents** are **greater than their children (max heap**)

	- If **all** the **children** are **greater** than their **parents** it is considered to call the heap a **min-heap**

- what is a complete binary tree?

	- all the levels are full, except the last one, where all the items are placed on the left

- Combined with the fact that each node contains a greater key than its children, a heap may look like this tree

	- In a max-heap each node contains a greater value than its children. Respectively in a min-heap each node contains a smaller value than its parent!

- if we put indices next to each node of this tree, starting from the root (index 1) and continuing from left to right on each level, we’ll get the following tree

	- Putting indices right to each node reveals the secret of the heap. The i-th node has left child exactly with the index 2*i, and right child with index 2*i+1!

	- This particular order gives us the possibility to store each heap in an array.

		- heap as array

- Since in a heap its greater element is in the root of the tree (for max-heap, respectively in a min-heap its smallest element is the root) we need to answer two questions

	- 1. How to build a heap out of an ordinary array?

	- 2. After extracting the root, which is the greatest (smallest) item, how can we rebuild the heap in order to keep it a heap again?

- how to build a heap?

	- let’s take a look on a ordinary binary tree with only three nodes

- Building a random array into a heap isn’t that difficult since we know that half of the complete tree items lay in it’s lowest level! Thus we start from floor(len[A] / 2)!

	- Why? Well, a complete binary tree with a full last level contains n/2 + 1 nodes in it.

	- They don’t have children, thus we don’t need to check them – they are “sorted”. Indeed if we start from an item on the right of floor(len[A] / 2) there won’t be items with indices 2*i and 2*i + 1.

### ops

- in detail

	- basic

		- find max or find min

			- find a maximum item of a max-heap, or a minimum item of a min-heap, respectively (a.k.a. peek)

		- insert

			- adding a new key to the heap (a.k.a. push)

		- extract-min [or extract-max]

			- returns the node of minimum value from a min heap [or maximum value from a max heap] after removing it from the heap (a.k.a. pop)

		- delete-max or delete-min

			- removing the root node of a max- or min-heap respectively

		- replace

			- pop root and push a new key, more efficient than pop followed by push, since only need to balance once, not twice, and appropriate for fixed-size heaps.

	- creation

		- create-heap - O(n)

			- create an empty heap

		- heapify

			- create a heap out of given array of elements

		- merge (union)

			- joining two heaps to form a valid new heap containing all the elements of both, preserving the original heaps

		- meld

			- joining two heaps to form a valid new heap containing all the elements of both, destroying the original heaps

	- inspection

		- size

			- return the number of items in the heap

		- is-empty

			- return true if the heap is empty, false otherwise

	- internal

		- increase-key or decrease-key

			- updating a key within a max- or min-heap, respectively

		- delete

			- delete an arbitrary node (followed by moving last node and sifting to maintain heap)

		- sift-up

			- move a node up in the tree, as long as needed; used to restore heap condition after insertion 

				- called "sift" because node moves up the tree until it reaches the correct level, as in a sieve

		- sift-down

			- move a node down in the tree, similar to sift-up; used to restore heap condition after deletion or replacement

- running time

	- insert: O(log n)

	- delete: O(log n)

		- The deletion cost is **O(log n**) for the **minimum** or **maximum, O(n**) for an **arbitrary element**.

	- search: O(n)

	- space usage: O(n)

### images

- 

	- example of a max heap

### notes

### res

- [amazing overview](http://www.stoimen.com/blog/2012/08/07/computer-algorithms-heap-and-heapsort-data-structure/)

## BST binary search tree

### desc

- A data struc­ture in which we have nodes con­tain­ing data and two ref­er­ences to other nodes, one on the left and one on the right.

### ops

- balanced binary tree

	- insert: O(log n)

	- delete: O(log n)

	- search: O(log n)

	- space usage: O(n)

### img

- definition of BST

### res

- [implementation of it](http://algorithms.tutorialhorizon.com/binary-search-tree-complete-implementation/)

## [RBT red black tree](http://www.wikiwand.com/en/Red%E2%80%93black_tree)

### desc

- A red–black tree is a kind of [self-balancing binary search tree](http://www.wikiwand.com/en/Self-balancing_binary_search_tree)

- Each node of the binary tree has an extra bit, and that bit is often interpreted as the color (red or black) of the node

- These color bits are used to ensure the tree remains approximately balanced during insertions and deletions.

### rules

- 1. every node is coloured either red or black

- 2. the root is black

- 3. if a node is red, all of its children are black (a.k.a. the red rule)

- 4. every path from a node to a null link must contain the same number of black nodes (a.k.a. the path rule)

### implications of the rules

- if a red node has any children, it must have two children and they must be black

- if a black node has only one child, that child must be a red leaf

- due to the rules, there are limits on how unbalanced a red black tree may become

### ops

- insert: O(log n)

- retrieve: O(log n)

- delete: O(log n)

### prop

- if a red black tree is complete, with all black nodes except for red leaves at the lowest level, the height will be minimal

	- ~log n

- to get the max height for N elements, there should be as many red nodes as possible down one path and all other nodes are black

	- this means the max height would < 2 * log N

- every simple path from a node to a descendant leaf contains the same number of black nodes

### img

- example of RBT

- maintaining the red black properties in a tree

### notes

- it follows **BST** property

	- where right child is > parent

	- and left child is < parent

- the **root** of **RBT** is always **black**

- path:

	- a unique series of links (edges) traverses from the root to each node

		- the number of edges (links) that must be followed is the path length

- in red black trees paths from the root to elements with 0 or 1 child are of interest

- [a tree with all nodes black can be a red-black tree](a%20tree%20with%20all%20nodes%20black%20can%20be%20a%20red-black%20tree)

	- The tree has to be a perfect binary tree (all leaves are at the same depth or same level, and in which every parent has two children) and so, it is the only tree whose Black height equals to its tree height

- by convention, NULL nodes are black

### res

## [R-tree](http://www.wikiwand.com/en/R-tree)

### RESEARCH: 


# common running times and scenarios


## 


# [linked lists](https://www.wikiwand.com/en/Linked%20list)


## description

### a linked list is a **set of dynamically allocated nodes, arranged** in such a way that **each node contains one value** and **one pointer**

### the **pointer always** eb to the **next member on the list**

### **if** the **pointer** is **NULL**, then it is the **last node** in the list

### a linked list is held using a **local pointer variable** which **points** to the **first item of the list**

### 

### defining it in C

## ops

### unsorted linked list

- insert: O(1)*

	- The cost to add or delete an element into a known location in the list (i.e. if you have an iterator to the location) is O(1). If you don't know the location, then you need to traverse the list to the location of deletion/insertion, which takes O(n) time.

- delete: O(1)*

- search: O(n)

- space usage: O(n)

### sorted linked list

- insert: O(n)*

- delete: O(1)*

- search: O(n)

- space usage: O(n)

## images

### 

## notes

### essentially, linked lists function as an array that can **grow** and **shrink** as needed

- from any point in the array

### linked lists have a few advantages over arrays

- 2. there is no need to define an initial size

- 1. items can be added or removed from the middle of the list

### disadvantages

- 1. there is no “random” access

	- it is impossible to reach the nth item in the array without first iterating over all items up until that item

	- this means we have to start from the beginning of the list and count how many times we advance in the list until we get to the desired item

- 2. dynamic memory allocation and pointers are required, which complicates the code and increases the risk of memory leaks and segment faults

- 3. linked lists have a much larger overhead over arrays since linked list items are dynamically allocated (which is less efficient in memory usage) and each item in the list also must store an additional pointer

### they are not **cache friendly**

- and **degenerate** on collision attacks to O(n/2) behaviour

## resources

### [linked list in c ](http://www.learn-c.org/en/Linked_lists)


# [hash tables](https://www.wikiwand.com/en/Hash_table)


## desc

### hash table (hash map) is a [data structure](https://www.wikiwand.com/en/Data_structure) used to implement an [associative array](https://www.wikiwand.com/en/Associative_array), a structure that can map [keys](https://www.wikiwand.com/en/Unique_key) to [values](https://www.wikiwand.com/en/Value_(computer_science))

### a hash table uses a [hash function](https://www.wikiwand.com/en/Hash_function) to compute an index into an array of buckets or slots, from which the desired value can be found

## img

## notes

## res


# [dictionaries](https://www.wikiwand.com/en/Dictionary%20%28data%20structure%29)


## desc

### In [computer science](https://www.wikiwand.com/en/Computer_science), an associative array, map, symbol table, or dictionary is an [abstract data type](https://www.wikiwand.com/en/Abstract_data_type) composed of a [collection](https://www.wikiwand.com/en/Collection_(computing)) of ([key, value](https://www.wikiwand.com/en/Attribute%E2%80%93value_pair)) pairs, such that each possible key appears at most once in the collection.

## operations

### the addition of a pair to the collection

### the removal of a pair from the collection

### the modification of an existing pair

### the lookup of a value associated with a particular key

## notes

### [what is the difference between a hash and a dictionary](http://softwareengineering.stackexchange.com/a/30931)

- Hash is an extremely poorly named data structure where the programmer has confused the interface with implementation (and was too lazy to write the full name, i.e. HashTable instead resorting to an abbreviation, Hash)

- Dictionary is the “[correct” name](http://xlinux.nist.gov/dads/HTML/dictionary.html) of the interface (= the [ADT](http://xlinux.nist.gov/dads/HTML/abstractDataType.html)), i.e. an associative container that maps (usually unique) keys to (not necessarily unique) values

	- A **hash table** is **one possible implementation of such a dictionary** that **provides quite good access characteristics** (in terms of runtime) and is **therefore often** the **default implementation**.

		- Such an implementation has two important properties:

			- 1. the keys have to be hashable and equality comparable.

			- 2. the entries appear in no particular order in the dictionary.

		- For a key to be hashable means that we can compute a numeric value from a key which is subsequently used as an index in an array

		- There exist alternative implementations of the dictionary data structure that impose an ordering on the keys – this is often called a sorted dictionary (and is usually implemented in terms of a search tree, though other efficient implementations exist).

- in summary

	- a dictionary is an ADT that maps keys to values.

	- There are several possible implementations of this ADT, of which the hash table is one

	- Hash is a misnomer but in context it’s equivalent to a dictionary that is implemented in terms of a hash table.

- in short

	- “**Dictionary**" is the **name of the concept**. A **hashtable** is a **possible implementation**.

## img

## res


# stacks


# graphs


# skip list


# queues


# maps

