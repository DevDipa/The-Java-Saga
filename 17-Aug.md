# **G.K**
- You can make your own packages in Java. Those are simply the folders that hold different classes and sub-classes.
- *Encapsulation* is about Data-hiding while *Abstraction* is about hiding the implementation details, since they are complex.
- Abstraction is achieved 100% via *Interfaces*, not via *Abstract Classes* 'cause the methods in the abstract classes may or may not be     abstract.
- The direct *Multiple Inheritance* isn't possible in Java. It can be achieved via Interfaces only.
- There's no Operator Overloading in Java.

# **FAQs**
- A pure OOP language is that in which EVERY THING is treated as an object. Java isn't a pure OOP language 'cause it makes use of primitive data types, like int, char, double, etc. However, it tries to use wrapper classes, like Integer, Character, Double, etc.

- Constructor Chaining occurs when one constructor calls another constructor to reuse the setup logic. It happens in 2 ways:
  - 1. Within the same class using this(...)
    2. Across inheritance using super(...)