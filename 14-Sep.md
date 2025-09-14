# **String**
- The String object is `immutable`. Here, objects are inside a `String Pool` in the Heap memory.

```java
String s1 = "Hello"; //creates an object in the pool
String s2 = "Hello"; //reuses the object of the pool
System.out.println("Hello"); //reuses the object of the pool
String s3 = new String("Hello"); //forces the JVM to explicitly create a new object

```

- The immutability of String objects is for Optimization and Security.
- The (==) comparator compares the two String objects. However, (.equals) only checks the values of the two objects.
- For `Pretty Printing/Formatting` of String objects' values, we use `printf()`.
- `When an int is concatenated with a string, it will be converted into Integer (a Wrapper Class), which is directly gonna call toString(). The toString() has its default formatting code.`

# **StringBuilder**
- The StringBuilder object is `mutable`. That means, we can modify the previous objects without creating a new one.

```java
StringBuilder builder = new StringBuilder("Hello,");
System.out.println(builder.toString());
builder.append(" Uni:)");
System.out.println(builder.toString());

```
