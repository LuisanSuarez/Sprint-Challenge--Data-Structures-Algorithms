Add your answers to the Algorithms exercises here.
Exercise I1
a) Runtime is: O(n).
The constraint on the while loop is n^3. However,
every time we run the loop we increment by n^2.
Simple division yields n. Or, if we add n^2  to
itself n times (multiply n^2 by n), we get n^3.

b) Runtime complexity is O(n^3)
First Loop: O(n)
Second Loop: O(n)
Third Loop: O(n)
Fourth Loop: O(1)   #this is ignorable in presence of O(n)s


c) O(1)

Exercise II
If we want to minimize the number of eggs dropped (i.e. our number of attempts at figuring out f), we
do binary search: start on the math.floor(n/2)'th floor, and see if it breaks. If it does, we check the middle floor of the lower half (n/4). If it doesn't break, we check the middle floor of the upper half (3n/4).
We'd find it in O(log(n)) time

Now, if we wanted to minimize the number of eggs _broken_, we'd start from the bottom and go up one by one until the first egg broke. Then we'd know that _f_ is the floor that came before. 
We'd find it in O((n)) time.

