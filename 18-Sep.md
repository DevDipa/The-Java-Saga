# **Tail Recursion**
- A specialized recursion condition where the recursive call itself is the last operation performed by the function. 
- This doesn't require the program to keep track of previous calls on the call stack.
- E.g. of a Tail Recursion:
```java
static void print(int n) {
    System.out.println(n);
    print(n+1);
}
```
- E.g. of a Non-tail Recursion:
```java
static int fibo(int n) {
    if (n < 2) {
        return n;
    } else {
        return fibo(n-1) + fibo(n-2);
    }
}
```

# **Approach to Recursion**
1. Identify if you can break a problem into smaller problems.
2. Write the `recurrence relation` if needed.
3. Draw the Recursion Tree.
4. In the tree: 
   - See the flow of functions (i.e., how they're getting into the stack).
   - Identify, and focus on `Left tree calls` and `Right tree calls` (left or right depends on the formula you create).
5. See how the values get returned at each step.
6. See where the function call will come out from. 

*BONUS*: Practice on pen and paper regularly. Use debuggers on IDE.

## **Types of Recurrence Relation**
1. Linear Recurrence Relation (e.g., fibonacci)
2. Divide and Conquer Recurrence Relation (e.g., Binary search)

`Linear is less efficient than D&C 'cause the large number is getting smaller by very small extent during each recursive call.`

# **Types of Variables in Recursion**
(In/As):
1. Arguments (*get passed onto the next recursive call*)
2. Return Type (*make sure to return the mentioned data type from the subcalls, too; else the code won't work*)
3. Body of Function (*the variables which aren't necessary to pass onto another recursive call are put here*)
