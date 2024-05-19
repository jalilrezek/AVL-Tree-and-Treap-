Binary search trees are essential data structures to organize information for quick and efficient searches. However, in the worst-case, they degenerate to linear data structures with
O(N) operations.

AVL Tree and Treap are binary trees that have additional rebalancing operations to avoid the worst-case scenario and preserve O(lg N) operations. AVL tree relies on tracking balance 
factors of individual nodes and rebalancing whenever necessary, so that it is always balanced. Treap relies on the assignment of random priorities so that it is extremely improbable
that the tree will be significantly imbalanced at any point in time.

I implemented these data structures with a test-first paradigm, testing each new function as I added it.

Lastly, I used JMH Runtime Test to compare the performance of these data structures and a regular binary search tree on large datasets.

The AVL implementation is at main/java/hw6/bst/AvlTreeMap.java

The Treap is at main/java/hw6/bst/TreapMap.java

AVL tests are at test/java/hw6/AvlTreeMapTest.java

Treap tests are at test/java/hw6/TreapMapTest.java

Findings from benchmarking tests are at main/java/hw6/README.md


