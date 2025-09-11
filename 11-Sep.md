# **Bubble Sort**
- aka *Sinking/Exchange Sort*
- Done in passes: Pass 0, Pass 1, and so on...

## For Ascending Sort:
- At the end of Pass 0, the last element finds its place.
- Similarly, in the next pass, the second last element finds its place, and so on...
- `i` will be used for the outer loop, which represents the passes, 0 to length.
- `j` will be used for the inner loop, which will go till `length - i`.
- Space complexity is constant O(1).
- Time Complexity:
 1. when the array is sorted -> O(N).
 2. when the array is sorted in opposite order -> O(N^2).