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

4. What is the space complexity of your `breadth_first_for_each` method?

5. What is the runtime complexity of your `heapsort` function?

6. What is the space complexity of the `heapsort` function? Recall that your implementation should return a new array with the sorted data. What would be the space complexity if your function instead altered the input array?
Because in this implementation I'm keeping an array (that will be returned in the end), the space complexity
is O(n) because the memory needed for the array will grow as the input grows.
If we were to order in place, it would be O(1) since it wouldn't need any additional space to hold elements.