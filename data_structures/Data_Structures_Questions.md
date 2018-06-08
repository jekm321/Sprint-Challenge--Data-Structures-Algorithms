Add your answers to the questions below.

1. What is the runtime complexity of your `depthFirstForEach` method?   --> O(n) each node visited once

2. What is the space complexity of your `depthFirstForEach` function?   --> O(n) ? not sure, didnt store any references

3. What is the runtime complexity of your `breadthFirstForEach` method? --> O(n) each node visited once

4. What is the space complexity of your `breadthFirstForEach` method?   --> O(n) each node value in an array once

5. What is the runtime complexity of your `heapsort` function?  --> O(n logn) each node is multiple times when making the heap as well as the constant bubbling/sifting done while deleting, but never is n number of nodes visited n number of times.

6. What is the space complexity of the `heapsort` function? Recall that your implementation should return a new array with the sorted data. What would be the space complexity if your function instead altered the input array?    A--> O(n), it makes a Heap array, and as the sorted array is filled, the heap is deleted so no extra space, just n space for the initial array which is transfered into the answer array.   B--> O(1), since in an alter it doesnt use any extra sapce.