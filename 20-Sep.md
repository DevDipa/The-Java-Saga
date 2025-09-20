# **Notations**
- We generally have 5 different notations:

1. **Big-oh Notation**
- `Gives the Upper bound`
- For an instance, if an algorithm have a Time Complexity (TC) of O(N^3), the algorithm can't exceed TC of O(N^3). However, it can have lesser values than O(N^3).

2. **Big Omega Notation**
- `Gives the Lower Bound`
- It is the exact opposite of Big-oh, i.e., the algorithm will take at least a certain value (e.g., Ω(N^3)), not lesser.

3. **Theta Notation**
- `Gives both Upper and Lower Bound`
- Denoted by θ(f(N)).

4. **Little-oh Notation**
- `Gives not-so-strict Upper Bound`
- E.g., for o(N^3), the algorithm will technically have a complexity which is always less than, not equal to N^3.

5. **Little Omega Notation**
- `Gives not-so-strict Lower Bound`
- E.g., for ω(N^3), the algorithm will technically have a complexity which is always nore than, not equal to N^3. 


# **Space Complexity**
- *Auxiliary space is the extra space or temporary space used by an algorithm.*
- Space complexity of an algorithm is the total space taken by the algorithm with respect to the input size. `It includes both Auxiliary Space and Space used by the  input.`


# **Time and Space Complexity in Recursion**
- In recursion, not more than one function call at the same level in the Recursion Tree will be in the Stack at the same time.
- Hence, `Space Complexity = Height of the Tree`.
