#Java Arraylist (Part of Java Data Structures)
- An ArrayList is like a resizable array.
- Implements the List interface.
- To access the ArrayList, use: import java.util.ArrayList;
- To create an obj: ArrayList<DataType> objName = new ArrayList<DataType>();
- Can loop via the ArrayList using simple 'for' loop or 'for-each' loop as:
   for (int i = 0; i < theTrio.size(); i++) {
      System.out.println(theTrio.get(i));

  for (String i : theTrio) {
      System.out.println(i);

- To sort the ArrayList, use the sort() method from the Collections class.