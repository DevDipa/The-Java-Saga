# **Introduction to Time Complexity**
- `Time Complexity != Time Taken`
- In fact, time complexity is a mathematical function that indicates how time will grow when the input grows.
- For large numbers, the Linear Search will take more time than the Binary Search.
- In general, for large values: `*O(1) < O(log N) < O(N) < O(2^N)*`, i.e., Constant TC < takes the least amount of time, whereas Exponential TC takes the most time. We can adjust other forms of TC in between these 4 by applying basic mathematical knowledge.

# **Things to Consider**
1. Always look for the `Worst case` time complexity.
2. Always think about large or infinte values.
3. Always ignore the constant.
4. Always ignore the less dominating terms. 