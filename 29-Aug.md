# **split() in String**
- String provides a method named `split()` that basically helps split a single string value into different parts using certain delimiters and indexes - starting at 0.
- For an instance, we have:

```java
String data = "| Id | Description | Deadline | Status |";
```
- We can split the above *data* into different parts taking '|' as a delimiter as:

```java
String[] parts = data.split("\\|");
```
- This is what the string array will contain:
  - parts[0] = empty, because the line starts with '|'
  - parts[1] = id portion
  - parts[2] = description portion
  - parts[3] = deadline portion
  - parts[4] = status portion
  - parts[5] = empty, because the line starts with '|'

- Thus, the split() method can be used efficiently to access different string parts individually.