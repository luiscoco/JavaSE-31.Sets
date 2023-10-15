# JavaSE-Sets

![image](https://github.com/luiscoco/JavaSE-31.Sets/assets/32194879/a8bcd4e8-3fd3-4fd2-b396-b3708c4bb36a)

In Java, a Set is a collection that does not allow duplicate elements. 

It models the mathematical set abstraction and is a part of the Java Collections Framework. 

There are several classes in Java that implement the Set interface, with HashSet, LinkedHashSet, and TreeSet being the most commonly used.

## 1. HashSet:

Uses a hash table for storage. Does not guarantee any specific order.

Offers constant time complexity for basic operations (add, remove, contains).

```java
Set<String> hashSet = new HashSet<>();
hashSet.add("apple");
hashSet.add("banana");
hashSet.add("orange");

System.out.println(hashSet); // Order not guaranteed
```

## 2. LinkedHashSet:

Maintains the order of insertion. Slower than HashSet but faster than TreeSet.

```java
Set<String> linkedHashSet = new LinkedHashSet<>();
linkedHashSet.add("apple");
linkedHashSet.add("banana");
linkedHashSet.add("orange");

System.out.println(linkedHashSet); // Order of insertion guaranteed
```

## 3. TreeSet:

Maintains natural ordering of elements (or order specified by a comparator).

Slower compared to HashSet and LinkedHashSet.

```java
Set<String> treeSet = new TreeSet<>();
treeSet.add("apple");
treeSet.add("banana");
treeSet.add("orange");

System.out.println(treeSet); // Natural ordering (lexicographical in this case)
```

Common operations on sets include adding elements (add), removing elements (remove), checking for the presence of an element (contains), and iterating over the elements.

```java
Set<String> fruits = new HashSet<>();
fruits.add("apple");
fruits.add("banana");
fruits.add("orange");

System.out.println(fruits.contains("apple")); // true

fruits.remove("banana");
System.out.println(fruits); // [apple, orange]
```

Remember, the choice of which set implementation to use depends on your specific requirements regarding ordering, speed, and whether duplicates are allowed.

