# Algorithms_Python
I am dumping all my algorithm problems in this repository.
My ultimate aim is to do ML, DL and AI.
So to achieve those coding is required. To make my coding strong I have decided to learn all the algorithms.
Hope this helps everyone with same passion. 

And please note that I am working on my own. I am not forking any Repos or copying them. This is solely my work.

## Linear Search:
A simple approach is to do a linear search, i.e  

Start from the leftmost element of arr[] and one by one compare x with each element of arr[]
If x matches with an element, return the index.
If x doesn’t match with any of elements, print that the element is not found. 
The time complexity of the above algorithm is O(n). 

Linear search is rarely used practically because other search algorithms such as the binary search algorithm and hash tables allow significantly faster-searching comparison to Linear search.

### Improve Linear Search Worst-Case Complexity

if element Found at last  O(n) to O(1)

if element Not found O(n) to O(n/2)

## Binary Search
Given a sorted array arr[] of n elements, write a function to search a given element x in arr[].
A simple approach is to do linear search.The time complexity of above algorithm is O(n). Another approach to perform the same task is using Binary Search.

Binary Search: Search a sorted array by repeatedly dividing the search interval in half. Begin with an interval covering the whole array. If the value of the search key is less than the item in the middle of the interval, narrow the interval to the lower half. Otherwise narrow it to the upper half. Repeatedly check until the value is found or the interval is empty.

The idea of binary search is to use the information that the array is sorted and reduce the time complexity to O(Log n).

### We basically ignore half of the elements just after one comparison.

-Compare x with the middle element.

-If x matches with middle element, we return the mid index.

-Else If x is greater than the mid element, then x can only lie in right half subarray after the mid element. So we recur for right half.

-Else (x is smaller) recur for the left half.

### Time Complexity:

#### The time complexity of Binary Search can be written as

T(n) = T(n/2) + c 

The above recurrence can be solved either using Recurrence T ree method or Master method. It falls in case II of Master Method and solution of the recurrence is Theta(Logn).

Auxiliary Space: O(1) in case of iterative implementation. In case of recursive implementation, O(Logn) recursion call stack space.
