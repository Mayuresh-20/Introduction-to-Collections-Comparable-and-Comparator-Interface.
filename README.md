# Introduction-to-Collections-Comparable-and-Comparator-Interface.

Java Arrays
Normally, an array is a collection of similar type of elements which has contiguous memory location.

Java array is an object which contains elements of a similar data type. Additionally, The elements of an array are stored in a contiguous memory location. It is a data structure where we store similar elements. We can store only a fixed set of elements in a Java array.

Array in Java is index-based, the first element of the array is stored at the 0th index, 2nd element is stored on 1st index and so on.

In Java, array is an object of a dynamically generated class. Java array inherits the Object class, and implements the Serializable as well as Cloneable interfaces. We can store primitive values or objects in an array in Java. 

![image](https://user-images.githubusercontent.com/91977965/136513374-9a688713-b133-4f41-8613-cad667e239c7.png)

Advantages
Code Optimization: It makes the code optimized, we can retrieve or sort the data efficiently.
Random access: We can get any data located at an index position.
Disadvantages
Size Limit: We can store only the fixed size of elements in the array. It doesn't grow its size at runtime. To solve this problem, collection framework is used in Java which grows automatically.
Types of Array in java
There are two types of array.

Single Dimensional Array
Multidimensional Array

//Java Program to illustrate how to declare, instantiate, initialize  
//and traverse the Java array.  
class Testarray{  
public static void main(String args[]){  
int a[]=new int[5];//declaration and instantiation  
a[0]=10;//initialization  
a[1]=20;  
a[2]=70;  
a[3]=40;  
a[4]=50;  
//traversing array  
for(int i=0;i<a.length;i++)//length is the property of array  
System.out.println(a[i]);  
}}

Output:

10
20
70
40
50


What is Java Collections Framework?
Collections are like containers that group multiple items in a single unit. For example, a jar of chocolates, a list of names, etc.

Collections are used in every programming language and when Java arrived, it also came with few Collection classes – Vector, Stack, Hashtable, Array.

Java 1.2 provided Collections Framework that is the architecture to represent and manipulate Collections in java in a standard way. Java Collections Framework consists of the following parts:

1. Interfaces
Java Collections Framework interfaces provides the abstract data type to represent collection.

java.util.Collection is the root interface of Collections Framework. It is on the top of the Collections framework hierarchy. It contains some important methods such as size(), iterator(), add(), remove(), clear() that every Collection class must implement.

Some other important interfaces are java.util.List, java.util.Set, java.util.Queue and java.util.Map. The Map is the only interface that doesn’t inherit from the Collection interface but it’s part of the Collections framework. All the collections framework interfaces are present in java.util package.

2. Implementation Classes
Java Collections framework provides implementation classes for core collection interfaces. We can use them to create different types of collections in the Java program.

Some important collection classes are ArrayList, LinkedList, HashMap, TreeMap, HashSet, and TreeSet. These classes solve most of our programming needs but if we need some special collection class, we can extend them to create our custom collection class.

Java 1.5 came up with thread-safe collection classes that allowed us to modify Collections while iterating over them. Some of them are CopyOnWriteArrayList, ConcurrentHashMap, CopyOnWriteArraySet. These classes are in java.util.concurrent package.

All the collection classes are present in java.util and java.util.concurrent package.

3. Algorithms
Algorithms are useful methods to provide some common functionalities such as searching, sorting and shuffling.

Collections Framework Class Diagram
Below class diagram shows Collections Framework hierarchy. For simplicity, I have included only commonly used interfaces and classes.
