# **Linear Search**
- Start searching from the first element of the array till you find the desired element.
- The time complexity in the worst-case scenario is O(n) i.e., the time requuired depends on the size of inputs.

# **Binary Search**
- Works on `sorted` arrays (either ascending or descending).
- Assuming an ascending array, the steps involved are:
 1. Find the `MIDDLE` element. 
 2. Check if *target > middle*. If yes, search on the `right side` of the middle element; else on the `left side`.
 3. If *middle == target*, return middle.

- For traversing, 2 pointers `start` and `end` are used. 
- Whenever *start > end*, it signifies the target isn't present within the given array.

- The time complexity in the worst-case scenerio is `log(N)`, where N = the number of array elements.
- Clearly, Binary search is more effective than Linear search in terms of time complexity.

## **Order-Agnostic Binary Search**
- Basically, we don't know whether the sorted array is in ascending or descending order.
- Here, we compare the first and the last elements of the array. 