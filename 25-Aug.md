# **String v/s StringBuffer in Java**
- String uses `String Constant Pool (SCP)` to store the String objects, which are immutable. 
- E.g.,
 ```java
        String str1 = "Sita"; 
        str1.concat("Ram"); // str1 = Sita 'cause String is immutable
        System.out.println(str1.concat("Ram")); //output = SitaRam 'cause there is an object reference now
 ```

 - Basically, from the above code, we can infer the object of an String isn't created unless assigned, and hence can't be referenced. 
 - Any modification like concat(), replace(), etc creates a new object in the SCP. 

 - On the other hand, StringBuffer uses a Heap memory  and  a Stack to store the objects and their references respectively. 
 - E.g.,
 ```java
    StringBuffer str2 = new StringBuffer("Dipaak");
    str2.append("Uni"); //output = DipaakUni 'cause StringBuffer is mutable
```

- Any modification in an object leads to its alteration without the need to create a new one. Hence, it is faster for multiple modifications.