# **Exception Handling**

- JVM responds to an exception in the following ways:
  1. Creates an object of the exception (like `Exception e`).
  2. Informs about the name, description, and position of the exception via the object.
  3. Throws the exception.
  4. Handles the exception.

---

# **General Info**
- The *Exception* class extends the class *Throwable*.
- The *Throwable* class has another subclass called *Error*.
- Basically:
  - **Exception** → an unexpected event that **can be handled** (e.g., `ArithmeticException`).
  - **Error** → something that **cannot be handled** (e.g., `OutOfMemoryError`, server crash).

---

# **Types of Exception**
1. **Checked (Compile-time) Exceptions**  
   Examples: `FileNotFoundException`, `SQLException`, `IOException`, `ClassNotFoundException`.

2. **Unchecked (Run-time) Exceptions**  
   Examples: `ArithmeticException`, `ArrayIndexOutOfBoundsException`, `NullPointerException`, `IllegalThreadStateException`.

---

# **5 Used Keywords**
- `try`
- `catch`
- `throw`
- `throws`
- `finally`

**Notes:**  
1. `try` must always come with either `catch` or `finally`.  
2. Nested try-catch-finally blocks are possible.  

---

# **New Features**

## 1. Multi-catch Block
- You can handle multiple exceptions in a single `catch`.  
- The parent exception class (`Exception`) must always come last.  

```java
try {
    // code
} catch (ArithmeticException | NullPointerException e) {
    System.out.println("Specific exception: " + e);
} catch (Exception e) {
    System.out.println("General exception: " + e);
}
```


## 2. Try-with-Resources
- Introduced in Java 7.
- Used when working with resources like files, DB connections, streams.
- Automatically closes resources (no need for finally).

```java
try (BufferedReader br = new BufferedReader(new FileReader("data.txt"))) {
    String line;
    while ((line = br.readLine()) != null) {
        System.out.println(line);
    }
} catch (IOException e) {
    e.printStackTrace();
}
```

# **throw v/s throws**
- `throws` (used in method signature)
- Declares exceptions a method can throw.
- Used for checked exceptions.

```java
public static void readFile(String path) throws IOException {
    FileReader fr = new FileReader(path);
}
```

- `throw` (used inside method body)
- Used to explicitly create and throw an exception object.

```java
try {
    int age = 15;
    if (age < 18) {
        throw new ArithmeticException("Not eligible to vote!");
    }
} catch (ArithmeticException e) {
    System.out.println(e.getMessage());
}
```
