Add your answers to the questions below.

1. What is the runtime complexity of your `depth_first_for_each` method?
The runtime complexity is O(n) because we're executing one callback to every 
node in the tree.

2. What is the space complexity of your `depth_first_for_each` function?
The space complexity is 0(depth) with 'depth' being the count of the longest
branch from root to leaf. This is because we're recurisvely calling all the
way to the bottom until the leaf before moving on to the next branch, so the
function keeps track of where it is until it reaches the final node and exits
to the next command.

3. What is the runtime complexity of your `breadth_first_for_each` method?
O(n). Same as ans#1, it'll go through every node in the tree. The only difference
is the order. 

4. What is the space complexity of your `breadth_first_for_each` method?
O(n) because it'll use a little over n/2 of memory. The most memory we'll need
will be the last level of a balanced tree, when the last node of the next-to-last level adds
all of it's children. We'll have popped all other nodes except those in the
last level. The tree's size is the number of nodes in the last level*2-1. 
O(n/2) turns into O(n)

5. What is the runtime complexity of your `heapsort` function?
O(nlog(n)).
Heap.delete() is run n times, and every Heap.delete() operation runs in
log(n) time. 

6. What is the space complexity of the `heapsort` function? Recall that your implementation should return a new array with the sorted data. What would be the space complexity if your function instead altered the input array?
Because in this implementation I'm keeping an array (that will be returned in the end), the space complexity
is O(n) because the memory needed for the array will grow as the input grows.
If we were to order in place, it would be O(1) since it wouldn't need any additional space to hold elements.