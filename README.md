Analyze in detail your written algorithms in Part (a).
Time Complexity:

Building the Max Heap:
heapify takes O(log n) time, and we apply it to each node in the tree, starting from the last non-leaf node. Hence, building the heap takes O(n).

Heapsort:
For each of the n-1 elements, we swap the root with the last element and then apply heapify, which takes O(log n) time. Therefore, heapsort has a time complexity of O(n log n).

Space Complexity:
Heapsort is an in-place sorting algorithm, meaning it doesn’t require extra space other than the input array. Thus, the space complexity is O(1).

Best, Average, and Worst Case Complexity:
All cases have the same time complexity of O(n log n) for heapsort, since both building the heap and performing the sort require the same steps.

b. Analyze in detail your written algorithms in Part (a).
Time Complexity:

Sorting the Edges: Sorting the edges takes O(E log E), where E is the number of edges.
Union-Find Operations: Both find and union operations take almost constant time, O(α(n)), where α(n) is the inverse Ackermann function. This is very slow-growing and can be approximated as constant for practical values of n. Therefore, the union-find operations contribute O(E α(n)) to the time complexity.
The overall time complexity is dominated by the sorting step, so it is O(E log E), where E is the number of edges in the graph.

Space Complexity:
The space complexity is O(V + E) for storing the graph edges, the disjoint set, and the MST.
