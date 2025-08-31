# **Stack and Heap Memory**
- In Java, primitives are stored in Stack while objects are stored in Heap.
- The initialization of array objects follows Dynamic Memory Allocation (DMA) and the objects aren't continuous in the heap.
- `Null ` is assigned to non-primitive data types only, and is the default value of reference variables.

## **Visualization**
- Suppose we have:

```java
String str = new String[4];
str[0] = "aa";
str[1] = "bb";
str[2] = "cc";
str[3] = "dd";
```
- The 'str' being a reference variable, is stored in the stack. It points to the String object in the heap.
- In the heap, the String object looks like: [str[0], str[1], str[2], str[3]]. These are nothing but the references to further objects in the heap that contain aa, bb, cc and dd respectively.

- But, if the case was:

```java
int[] arr = new int[4];
arr[0] = 1;
arr[1] = 2;
arr[2] = 3;
arr[3] = 4;
```

- The 'arr' would be in the stack, referring to the int object i.e., [1,2,3,4].
- That's it! There's no indirect reference in the heap this time.
 