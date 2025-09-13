# **Insertion Sort**
- `Prime Idea: Sort the array partially.`
- In the Pass 0 (i = 0), sort till index 1.
- In the Pass 1 (i = 1), sort till index 2, and so on...
- For every index, *insert* that index's element at the correct index at its L.H.S.
- The outer loop (i) goes from 0 through less than/equal to (arr.length - 2) so that (j + 1) remains relevant in the inner loop (j).
- If element at j is < element at (j-1), swap them; else break the loop.
- Space Complexity: O(1).
- Time Complexity: O(N^2) for the worst and O(N) for the best case.