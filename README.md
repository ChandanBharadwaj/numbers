
-----------------------------------------------------------------------------------------------------------------------------------------
select the correct option from below 4 options.
import java.lang.annotation.*;
public class Test {
	public Test() {}

	@Override
	public int hasCode() {
		return toString().hashCode();
	}

	public int hashCode() {
		return toString().hashCode();
	}
}

1. Compilation error because hasCode() is not found in parent class  == correct option
2. hashCode() can not be overriden
3. Code compiles successfully
4. Compilation error because @Override is a syntax error

----------------------------------------------------------------------------------------------------------------------------------
Which of the following best describes a directory service?
directory service = naming service + objects containing attributes
directory service = naming context + objects containing attributes == correct
directory service = binding context + names containing attributes
directory service = mapping service + maps contains key value pairs


-----------------------------------------------------------------------------------------------------------------------------------------
public class SystemFormat{

public static void main(String args[]){
Boolean b= null;
System.out.printf("%b %b", "false", b);
}
}

What is the output?
Select an option
1. false false
2. true false
3. false true
4. true true

OUTPUT: true false
---------------------------------------------------------------------------------------------------------------------------------------------------
Select an option
The members of the annotation must be defined with a syntax similar to interface method. Which of the following is a VALID method return type while defining the members of the annotation?
Integer
String
StringBuffer
Double
In Java, when defining members of an annotation, the return types of these members are restricted to specific types. The valid return types include:

- Primitive data types (e.g., `int`, `float`, `double`, etc.)
- `String`
- `Class`
- Enums
- Annotations
- Arrays of the above types

Given these constraints, let's evaluate the provided options:

1. **Integer**: This is not a valid return type because `Integer` is a wrapper class, not a primitive type.
2. **String**: This is a valid return type because `String` is allowed in annotation members.
3. **StringBuffer**: This is not a valid return type because `StringBuffer` is not among the allowed types.
4. **Double**: This is not a valid return type because `Double` is a wrapper class, not a primitive type.

Therefore, the correct answer is:

2. **String**

This is because `String` is explicitly mentioned as a valid return type for annotation members in Java.

----------------------------------------------------------------------------------------------------------------------------------------------
Which of the following should be inserted at xxxxxxxxxxxxxxxx so that a single worker thread is used to operate off an unbounded queue?

Select an option
ExecutorService objRef Executors.newSingleThreadExecutor:
ConcurrentObject objRef ConcurrentObject.getWorker Thread:
ConcurrentService objRef ConcurrentService.getFactoryImpl(ExecutorService):
ThreadFactory objRet-new ThreadFactory0.getWorker ThreadInstance

import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;

public class TestConcurrency1 {

	public static void main(String[] args) {
		// Insert correct code here
		//ExecutorService objRef Executors.newSingleThreadExecutor:
		//ConcurrentObject objRef ConcurrentObject.getWorker Thread:
		//ConcurrentService objRef ConcurrentService.getFactoryImpl(ExecutorService):
		//ThreadFactory objRet-new ThreadFactory0.getWorker ThreadInstance
		ExecutorService objRef= Executors.newSingleThreadExecutor();
		objRef.execute(new Runnable() {
		
		public void run() {
		System.out.println("Asynchronous task");
		}});
		
		objRef.shutdown();
	}
}

-------------------------------------------------------------------------------
import java.util.Scanner;

public class Scan2 {
	public static final String INPUT_STRING = "true boolean 9 java 7";
	public static void main(String[] args) {
		boolean b;
		String s, found = "";
		Scanner s1 = new Scanner(INPUT_STRING);
		s1.useDelimiter("\\d");
		while (b = s1.hasNext()) {
			s = s1.next();
			found += "s";
		}
		System.out.print("found=" + found);
	}
}

What is the output? = found=ss

found sssss
found-sss
found-ss
found-s

-------------------------------------------------------------------------------
Which one of the following is NOT true about the type of result set that you can specify in JDBC 2.0?

	1. TYPE FORWARD_ONLY is a scrollable result set, which means that you can navigate through it in a forward direction
	2. Any changes made to the TYPE_SCROLL_SENSITIVE result set while it's open are reflected in the database
	3. TYPE_SCROLL_INSENSITIVE is not a scrollable result set
	4. TYPE_SCROLL_SENSITIVE incorporates a bi-directional pointer.

Incorrect statement:
	1. TYPE_SCROLL INSENSITIVE is not a scrollable result set
Explanation:
In JDBC 2.0, there are three main types of result sets you can specify:
	1. TYPE_FORWARD_ONLY: This is the default type. You can only move the cursor forward one row at a time. It's not scrollable.
	2. TYPE_SCROLL_SENSITIVE: This type allows you to move the cursor forward, backward, and to specific rows. It's scrollable and reflects changes made to the underlying database by other connections (sensitive).
	3. TYPE_SCROLL_INSENSITIVE: This type also allows forward, backward, and specific row navigation (scrollable). However, it does not reflect changes made to the database by other connections (insensitive).
Therefore, option 3 is incorrect. TYPE_SCROLL_INSENSITIVE is indeed a scrollable result set, but it's insensitive to database modifications.

------------------------------------------------------------------------------------------------------------------------------------------

Select an option
The JMX technology defines standard connectors that enable you to access JMX agents from remote management applications. It is known as

	1. JMX connectors
	2. Remote connectors
	3. MBean connectors
	4. Management connectors

The JMX technology defines standard connectors (known as JMX connectors) that enable you to access JMX agents from remote management applications. JMX connectors using different protocols provide the same management interface.
-----------------------------------------------------------------------------------------------------------------------------------------------
Select an option
For every type of object, the Java virtual machine instantiates an immutable instance of

java.lang.Class
java.lang.Object
java.lang.Runtime
java.lang.Type

Out of the provided options, the closest answer is:
java.lang.Class
Here's why:
• java.lang.Class represents a class or interface at runtime. It provides information about the class structure, methods, fields, etc.
• java.lang.Class instances are immutable. Once a class is loaded by the JVM, its structure is fixed. The Class object reflects that structure and cannot be modified.
Explanation for other options:
• java.lang.Object: This is the root class for all Java objects. Objects of this type can be mutable or immutable depending on the specific class implementation.
• java.lang.Runtime: This class represents the runtime environment and provides methods for interacting with the system. It's a singleton object, meaning there's only one instance per JVM, but it's not necessarily immutable. Some methods might have side effects.
• java.lang.Type: This is a superclass for representing different kinds of types in Java. It can be used for both primitive types and reference types. Specific implementations like Class or primitive wrapper classes might have different mutability behavior.
Therefore, while java.lang.Class is the closest to being an immutable instance for every type of object, it's important to remember that immutability is determined by the class definition, not the JVM itself.
--------------------------------------------------------------------------------------------------------------------------------------------

