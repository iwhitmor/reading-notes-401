# Linked Lists

## [Big O: Analysis of Algorithm Efficiency](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)

* Used to describe the efficiency of an algorithm or function

* The efficiency is evaluated and based on 2 factors:

  * Running time
    > The amount of time a function needs to compete

  * Memory space
    > The amount of memory a function uses to store data and instructions

* Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job

* 4 key areas for analysis:

  * **Input Size**

    * Input Size refers to the size of the parameter values that are read by the algorithm. This does not simply refer to the number of parameters an algorithm reads, but takes into account the size of each parameter value as well.

  * **Units of Measurement**

    * To quantify the running time we consider:

    * The time in milliseconds from the start of a function expression until it ends

    * The number of operations that are executed

    * The number of "basic operations" that are executed

    * To quantify memory space we consider:

    * The amount of space needed to hold the code for the algorithm

    * The amount of space needed to hold the input data

    * The amount of space needed for the output data

    * The amount of space needed to hold working space during the calculation

  * **Orders of Growth**

    * We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.

  * **Best case, worst case, and average case**

    * The Big O describes the worst case for algorithm efficiency, however we need to also be aware of the best case and average case

## [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

* What is a linked list?

  * A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

* Terminology:

  * ***Linked list*** - A data structure that contains nodes that links/points to the next node in the list

  * ***Singly*** - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list

  * ***Doubly*** - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node

  * ***Node*** - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link

  * ***Next*** - Each node contains a property called Next. This property contains the reference to the next node

  * ***Head*** - The Head is a reference of type Node to the first node in a linked list

  * ***Current*** - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list

* Traversal

  * When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately

  * The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end

  * When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end

## [What’s a Linked List, Anyway? [Part 1]](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

* One characteristic of linked lists is that they are linear data structures. This means that there is a sequence and an order to how they are constructed and traversed

* The memory that linked lists uses is scattered throughout, instead of with arrays, where the memory all comes from one block

* Linked lists are dynamic data structures

  * Dynamic data structure can shrink and grow in memory. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well 

## [What’s a Linked List, Anyway? [Part 2]](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

* Growing a linked list

  * Just like with an array, we can add elements and remove elements from a linked list. But unlike arrays, we don’t need to allocate memory in advance or copy and re-create our linked list, since we won’t “run out of space” the way we might with a pre-allocated array

* To list, or not to list?

  * A linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element

![linked-list](https://miro.medium.com/max/1400/1*cUehR5S18XSoVLaPNfNzlA.jpeg)

### Additional Resources

* Information taken from links provided above
