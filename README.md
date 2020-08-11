# codeprep
Collecting interview questions and answers.



## Java 

**Que :** How will you make sure that serilization, reflection or cloning doesnt affect Singleton design pattern ?

**Ans :** 

###### Reflection : 
We can declare class as Enum -

As enums don’t have any constructor so it is not possible for Reflection to utilize it. Enums have their by-default constructor, we can’t invoke them by ourself. JVM handles the creation and invocation of enum constructors internally. 


###### Serialization : 
readResolve() method needs to implemented.


###### Clonable :
we need to override the clone() method.


###### Reference : 
https://www.geeksforgeeks.org/prevent-singleton-pattern-reflection-serialization-cloning/
