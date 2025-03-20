# Patika.dev & Getir Java Spring Boot Bootcamp

---

---

## Homework 1 - Buğra Bilge Çelik

---

---

### Question 1:
#### Why do we need to use OOP? Can you give examples of major OOP languages?

### Answer 1:
![Alt metin](https://atlacademy.az/images/cache/f6/f6132f_opp-nedir.jpg)

Object-Oriented Programming (**OOP**) is a paradigm that revolutionized software development by structuring code around objects (**data and behavior**) rather than actions (**functions or procedures**). Here’s a breakdown of why OOP is essential in modern programming:

---

#### 1. Modularity: Organizing Complexity  
**Problem:** Large systems become unwieldy when code is scattered across functions or scripts.  

**OOP Solution:**  
- Breaks code into **objects** (self-contained units) that model real-world entities (e.g., a `User`, `Car`, or `BankAccount`).
- Example: A `Car` class can encapsulate **properties** (e.g., `color`, `speed`) and **methods** (e.g., `accelerate()`, `brake()`).

**Benefit:**  
✅ Easier to debug, test, and update individual components without disrupting the entire system.

---

#### 2. Reusability: Avoid Reinventing the Wheel  
**Problem:** Repetitive code leads to redundancy and maintenance nightmares.  

**OOP Solution:**  
- **Classes and Inheritance**: Define a **base class** (e.g., `Animal`) and create **subclasses** (e.g., `Dog`, `Cat`) that inherit shared properties/methods.
- **Libraries and Frameworks**: Reuse pre-built classes (e.g., Java’s `ArrayList`, Python’s Django models).

**Benefit:**  
✅ Faster development and consistency across projects.

---

#### 3. Encapsulation: Control Access to Data  
**Problem:** Global variables or exposed data can be modified accidentally, causing bugs.  

**OOP Solution:**  
- **Data Hiding**: Restrict direct access to an object’s data using `private`/`protected` modifiers.
- **Public Methods**: Expose controlled interfaces (e.g., `getBalance()` and `deposit()` for a `BankAccount`).

**Benefit:**  
✅ Prevents unintended side effects and ensures data integrity.

---

#### 4. Inheritance: Hierarchical Relationships  
**Problem:** Duplicating code for similar entities (e.g., different types of vehicles).  

**OOP Solution:**  
- Create a **hierarchy** where **child classes** inherit from a **parent** (e.g., `Vehicle → Car → ElectricCar`).
- Override or extend methods as needed (e.g., `ElectricCar` overrides `refuel()` to `charge()`).

**Benefit:**  
✅ Reduces redundancy and enforces logical structure.

---

#### 5. Polymorphism: Flexibility in Behavior  
**Problem:** Writing separate functions for similar actions on different objects.  

**OOP Solution:**  
- **Method Overriding**: A `Shape` class can have a `calculateArea()` method, overridden by `Circle` and `Rectangle` subclasses.
- **Interfaces/Abstract Classes**: Define a **contract** (e.g., `Drawable`) that multiple classes implement differently.

**Benefit:**  
✅ Code can interact with objects generically, simplifying scalability.

---

#### 6. Abstraction: Simplify Complexity  
**Problem:** Users don’t need to understand internal mechanics to use a system (e.g., driving a car without knowing engine details).  

**OOP Solution:**  
- **Abstract Classes**: Define high-level templates (e.g., `DatabaseConnection` with abstract `connect()` method).
- Hide implementation details (e.g., a `sendEmail()` method abstracts SMTP protocols).

**Benefit:**  
✅ Reduces cognitive load and isolates changes to internal code.

---

#### 7. Maintainability: Future-Proofing Code  
**Problem:** Updating monolithic codebases is error-prone and time-consuming.  

**OOP Solution:**  
- Isolate changes to specific **classes** (e.g., modifying `PaymentProcessor` logic doesn’t affect `ShoppingCart`).
- Follow principles like **SOLID** (e.g., **Single Responsibility Principle**).

**Benefit:**  
✅ Easier to fix bugs, add features, and adapt to new requirements.

---

#### 8. Collaboration: Team-Friendly Development  
**Problem:** Large teams risk conflicts when editing the same code.  

**OOP Solution:**  
- Divide work into **classes/modules** (e.g., one team works on `UserAuthentication`, another on `ProductCatalog`).
- Use **version control** (e.g., Git) to manage contributions.

**Benefit:**  
✅ Parallel development with minimal interference.
---

Object-Oriented Programming (**OOP**) is a programming paradigm that provides structure, efficiency, and scalability in software development. By emphasizing **modularity, reusability, encapsulation, inheritance, polymorphism, and abstraction**, OOP enables developers to build **maintainable, flexible, and collaborative** systems.  

In short, OOP helps us write **organized, reusable, and secure** code, making software development **faster, easier, and more robust**. 🎯🚀

---

#### Major OOP Languages  

Here are some widely used **object-oriented programming languages**:

1. **Java** – One of the most popular OOP languages, widely used in enterprise applications, Android development, and web services.
2. **C#** – A powerful OOP language used in Microsoft ecosystems, game development (Unity), and enterprise applications.
3. **Python** – Although it supports multiple paradigms, Python is heavily used in OOP for web development, data science, and automation.
4. **C++** – A multi-paradigm language that extends C with OOP capabilities, often used in game development and system programming.
5. **Ruby** – A dynamically typed OOP language famous for its simplicity and Rails framework in web development.
6. **Swift** – Apple's preferred language for developing iOS and macOS applications.
7. **Kotlin** – An OOP language designed as a modern alternative to Java for Android development.
8. **PHP** – A web-oriented language that has evolved to support OOP principles, commonly used in backend development.

Each of these languages follows OOP principles like **encapsulation, inheritance, polymorphism, and abstraction**, making them ideal choices for structured software development.

---

---

### Question 2:
#### What is the difference between an interface and abstract class?

### Answer 2:
Both interfaces and abstract classes are used to define blueprints for other classes, but they serve different purposes and have distinct characteristics.
#### 1. Definition and Purpose

##### **Abstract Class:**
- Can have both **abstract methods** (without implementation) and **concrete methods** (with implementation).
- Used to **share common state or behavior** among related classes.
- Can include **instance variables** and **constructors**.

##### **Interface:**
- Defines a **contract** that classes must implement.
- Can have **abstract methods**, **default methods** (Java 8+), and **static methods**.
- Used to define **what** a class can do **without specifying how**.
- Does **not allow instance variables** (only `static final` constants).

---

#### 2. Key Differences

![Alt metin](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhQ53bkHH0JXO6_lHV9ZuQWh9RACaObkTl0gZsBh5RuOqNzMnODGjG4YHeBVAA8Y-xeGK6IQ2KFEJnFnbBKBZvGxo3O4zXqDSe9iHVWAED-exhKgenpts6a4CMlReqZ26-RG-Uh8FvlXJM/s1600/Picture2.jpg)


---

#### 3. When to Use Which?

##### **Use an Abstract Class when:**
✅ You want to **share code or state** among related classes.  
✅ The class hierarchy follows an **"is-a" relationship** (e.g., a `Dog` is an `Animal`).  

📌 **Example:** A `Vehicle` class with common methods like `startEngine()`.

```java
abstract class Vehicle {
    void startEngine() { 
        System.out.println("Engine started"); 
    } // Concrete method

    abstract void move(); // Abstract method
}
Use an Interface when:
✅ You want to define a contract for unrelated classes.
✅ You need multiple inheritance (since a class can implement multiple interfaces).

📌 Example: A Drawable interface with a draw() method.


interface Drawable {
    void draw(); // Abstract method

    default void resize() { 
        System.out.println("Resizing..."); 
    } // Default method (Java 8+)
}
```
##### **Use an Interface when:**
✅ You want to define a contract for unrelated classes.
✅ You need multiple inheritance (since a class can implement multiple interfaces).

📌 **Example:** A Drawable interface with a draw() method.

```java
interface Drawable {
    void draw(); // Abstract method

    default void resize() { 
        System.out.println("Resizing..."); 
    } // Default method (Java 8+)
}
```
---

---

### Question 3:
#### Why we need equals and hashCode methods? When to override them?

### Answer 3:
We need equals() and hashCode() in Java for two main reasons:

- **equals():**
It is used to compare two objects for equality based on their content or specific fields (e.g., checking if two User objects have the same ID). The default equals() method in the Object class only checks if two references point to the same object in memory, which is often not useful for custom comparisons.

- **hashCode():**
It generates an integer hash code for an object, which is used by hash-based collections like HashMap or HashSet to store and retrieve objects efficiently. The default hashCode() method in the Object class is based on the object's memory address, which may not work well for custom equality checks.

**Why Both Are Needed Together:**
- Consistency Rule: If two objects are equal (according to equals()), their hash codes must also be the same. This ensures proper functioning in hash-based collections.

- Hash-Based Collections: Collections like HashMap and HashSet rely on hashCode() to quickly locate objects and equals() to confirm their equality.

**When to Override:**
- Override equals() when you want to compare objects based on their content instead of memory addresses.

- Override hashCode() whenever you override equals() to maintain consistency and ensure correct behavior in hash-based collections.
- We always need to override hashCode() when we override equals() method. If we don't override hashCode(), the default implementation in Object class will be used and it may lead to unexpected behavior in hash-based collections.

---

---

### Question 4:
#### What is diamond problem in Java? How can we fix it?

### Answer 4:

The diamond problem is a confusion that arises in multiple inheritance when a class inherits from two classes that both inherit from a common superclass. This creates ambiguity because the subclass doesn't know which method or behavior to use if both parent classes override the same method.

![Alt metin](https://cdn-media-1.freecodecamp.org/images/1*QVZomxLNxnRYhm9gGIfYyw.png)

**Example:**
```
// Parent Class1 
class Parent1 { 
    void fun() { System.out.println("Parent1"); } 
} 
  
// Parent Class2 
class Parent2 { 
    void fun() { System.out.println("Parent2"); } 
} 
  
// Inherting the Properties from 
// Both the classes 
class test extends Parent1, Parent2 { 
    // main function 
    public static void main(String[] args) 
    { 
        test t = new test(); 
        t.fun(); 
    } 
}
```

**Output:**

![Alt metin](https://media.geeksforgeeks.org/wp-content/uploads/20230829111448/diamond-768.png)

**Explanation:**

In above example we have seen that “test” class is extending two classes “Parent1 ” and “Parent2” and its calling function “fun()” which is defined in both parent classes so now here it got confused which definition it should inherit. 

**How Can We Fix It?:**

Although Diamond Problem is a serious issue but we can create a solution for it which is Interface. Interface are created by using interface keyword. It contains all methods by default as abstract we don’t need to declared as abstract ,compiler will do it implicitly. We can’t instantiate interface for this we have to use a class which will implement the interface and will write the definitions of its all functions.


Here below we will see , how can we implement multiple inheritance by interface.

```
// Interfaces Declared 
interface Parent1 { 
    void fun(); 
} 
  
// Interfaces Declared 
interface Parent2 { 
    void fun(); 
} 
  
// Inheritance using Interfaces 
class test implements Parent1, Parent2 { 
    public void fun() 
    { 
        System.out.println("fun function"); 
    } 
} 
  
// Driver Class 
class test1 { 
    // main function 
    public static void main(String[] args) 
    { 
        test t = new test(); 
        t.fun(); 
    } 
}
```

**Output:**

```
fun function
```

We are able to implement multiple inheritance through interface just because in case of interface we does not provide the definition of function and when class implement that function then it write definition of function only once.

---

---

### Question 5:
#### Why we need Garbage Collector? How does Garbage Collector run?

### Answer 5:

Garbage collection (GC) is essential in programming languages that use automatic memory management (such as Java, C#, and Python) to prevent memory leaks and optimize resource usage. Here’s why we need a garbage collector:

- **Automatic Memory Management:**

    In languages like C and C++, developers must manually allocate (malloc) and free (free) memory. If memory is not freed, it causes memory leaks.
    GC automates this process, ensuring memory no longer in use is reclaimed.


- **Prevention of Memory Leaks:**

    If objects are created but never deallocated, the program consumes more and more memory, leading to out-of-memory (OOM) errors.
    The garbage collector ensures unused objects are removed from memory.


- **Avoiding Dangling Pointers:**

    In languages without GC, accessing freed memory (dangling pointers) can cause crashes or undefined behavior.
    GC ensures objects remain in memory as long as they are needed.


- **Optimizing Memory Usage:**

    GC compacts memory by removing fragmented spaces, improving performance.


- **Improves Development Productivity:**

    Developers can focus on business logic instead of managing memory manually.

**How Does Garbage Collector Run?**

The Garbage Collector runs in the background as part of the Java Virtual Machine (JVM). Here's how it works:

1. **Identifying Unused Objects**

   - GC identifies objects that are no longer reachable (i.e., no references to them exist in the application).

   - It starts from root objects (e.g., static fields, active thread stacks) and traces all reachable objects. Objects not reachable are marked as garbage.

2. **Garbage Collection Algorithms**

    Java uses different algorithms for garbage collection, such as:

    - **Mark and Sweep**: Marks unused objects and sweeps them away.

    - **Generational GC**: Divides the heap into generations (Young, Old) and collects younger objects more frequently.

    - **G1 GC (Garbage-First)**: Divides the heap into regions and prioritizes garbage collection in the most filled regions.

3. **Phases of Garbage Collection**

    - **Minor GC**: Cleans up the Young Generation (short-lived objects).

    - **Major GC**: Cleans up the Old Generation (long-lived objects).

    - **Full GC**: Cleans up the entire heap (both Young and Old Generations).

4. **When Does GC Run?**

    GC runs automatically when:

    - The JVM detects that memory is running low.

    - The `System.gc()` method is called (though it’s just a suggestion to the JVM).

    It runs in a separate thread, so it doesn’t block the main application (most of the time).

---

---

### Question 6:
#### `static` keyword usage in Java

### Answer 6:

The static keyword in Java is used to define members (fields, methods, blocks, and nested classes) that belong to the class itself rather than to instances (objects) of the class. Here's a breakdown of its usage:

---
1. Static Variables (Class Variables)

    - A static variable is shared across all instances of the class.

    - It belongs to the class, not to any specific object.

    - Useful for storing data that is common to all objects (e.g., a counter for the number of objects created).

**Example:**
```java
class Counter {
    static int count = 0; // Static variable

    Counter() {
        count++; // Increment count for each object created
    }
}

public class Main {
    public static void main(String[] args) {
        Counter c1 = new Counter();
        Counter c2 = new Counter();
        System.out.println(Counter.count); // Output: 2
    }
}
```

2. Static Methods
    
    - A static method belongs to the class, not to any specific object.

   - It can be called using the class name without creating an instance.

   - Static methods can only access static members (variables or methods).

**Example:**
```java
class MathUtils {
    static int add(int a, int b) {
        return a + b;
    }
}

public class Main {
    public static void main(String[] args) {
        int result = MathUtils.add(5, 3); // Call static method
        System.out.println(result); // Output: 8
    }
}
```

3. Static Block

    - A static block is used to initialize static variables or perform one-time setup tasks.

    - It runs when the class is loaded into memory.

**Example:**
```java
class Database {
    static String connection;

    static {
        // Static block to initialize static variable
        connection = "Database connected!";
        System.out.println(connection);
    }
}

public class Main {
    public static void main(String[] args) {
        // Output: Database connected!
    }
}
```

4. Static Nested Classes

    - A static nested class is a nested class that is associated with the outer class, not with an instance of the outer class.

    - It can access only static members of the outer class.

**Example:**
```java
class Outer {
    static int x = 10;

    static class Inner {
        void display() {
            System.out.println("x = " + x); // Access static variable
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Outer.Inner inner = new Outer.Inner();
        inner.display(); // Output: x = 10
    }
}
```

5. Static Import

   - Static import allows you to access static members of a class directly without using the class name.

**Example:**
```java
import static java.lang.Math.*;

public class Main {
    public static void main(String[] args) {
        double result = sqrt(25); // Directly use sqrt() without Math.
        System.out.println(result); // Output: 5.0
    }
}
```

---

---

### Question 7:
#### What is the meaning of Immutability? Where, how and why to use?

### Answer 7:

Immutability means that an object's state cannot be changed after it is created. Once an immutable object is created, its data (fields or properties) remains constant throughout its lifetime.

**Where to Use Immutability**

- Thread Safety: Immutable objects are inherently thread-safe because their state cannot change.

- Caching: Immutable objects can be safely cached and reused.

- Functional Programming: Immutability is a key concept in functional programming, where data is not modified but transformed.

- Security: Immutable objects are safer to use in sensitive contexts (e.g., passwords, keys).

**How to Use Immutability**

1. Declare the class as final (to prevent subclassing).

2. Make all fields private and final (to prevent modification).

3. Do not provide setter methods (methods that modify fields).

4. Initialize all fields via a constructor.

5. Return copies of mutable objects (e.g., arrays or collections) instead of the original references.

**Example:**
```java
public final class ImmutablePerson {
    private final String name;
    private final int age;
    private final List<String> hobbies;

    public ImmutablePerson(String name, int age, List<String> hobbies) {
        this.name = name;
        this.age = age;
        this.hobbies = new ArrayList<>(hobbies); // Defensive copy
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public List<String> getHobbies() {
        return new ArrayList<>(hobbies); // Return a copy
    }
}
```

**Why Use Immutability?**

- Thread Safety: No need for synchronization in multi-threaded environments.

- Predictability: Immutable objects are easier to reason about because their state doesn't change.

- Avoid Side Effects: Prevents unintended changes to shared data.

- Caching and Reuse: Immutable objects can be safely shared and reused.

- Simpler Code: Reduces complexity by eliminating the need for defensive copies or synchronization.

---

---

### Question 8:
#### Composition and Aggregation means and differences?

### Answer 8:

Both composition and aggregation are types of association in object-oriented programming, where one class is related to another. They describe has-a relationships, but they differ in the strength of the relationship.

---
1. **Composition**
    
    - **Definition:** A strong "whole-part" relationship where the part cannot exist independently of the whole.
    
    - **Lifecycle:** The part is created and destroyed with the whole.
    
    - **Example:** A Car has an Engine. If the Car is destroyed, the Engine is also destroyed.
    
    - **Implementation:** Typically implemented using instance variables and final fields.

**Example:**
```java
class Engine {
    void start() {
        System.out.println("Engine started.");
    }
}

class Car {
    private final Engine engine; // Composition

    Car() {
        this.engine = new Engine(); // Engine is created with the Car
    }

    void start() {
        engine.start();
    }
}

public class Main {
    public static void main(String[] args) {
        Car car = new Car();
        car.start(); // Output: Engine started.
    }
}
```
---
2. **Aggregation**


- **Definition:** A weak "whole-part" relationship where the part can exist independently of the whole.

- **Lifecycle:** The part can exist before or after the whole.

- **Example:** A Department has Professors. If the Department is dissolved, the Professors still exist.

- **Implementation:** Typically implemented using instance variables and setter methods.

**Example:**
```java
class Professor {
    private String name;

    Professor(String name) {
        this.name = name;
    }

    void teach() {
        System.out.println(name + " is teaching.");
    }
}

class Department {
    private List<Professor> professors; // Aggregation

    Department(List<Professor> professors) {
        this.professors = professors;
    }

    void startClass() {
        for (Professor professor : professors) {
            professor.teach();
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Professor p1 = new Professor("Dr. Smith");
        Professor p2 = new Professor("Dr. Jones");
        List<Professor> professors = new ArrayList<>();
        professors.add(p1);
        professors.add(p2);

        Department department = new Department(professors);
        department.startClass();
        // Output:
        // Dr. Smith is teaching.
        // Dr. Jones is teaching.
    }
}
```
---
**Key Differences**

![Alt metin](https://www.theknowledgeacademy.com/_files/images/Differences_Between_Composition_and_Aggregation_UML.png)

---

---

### Question 9:
#### Cohesion and Coupling means and differences?

### Answer 9:

Cohesion and coupling are two fundamental concepts in software design that describe the quality and structure of a system. They are often discussed together because they are inversely related: high cohesion usually leads to low coupling, and vice versa.

---
1. **Cohesion**

- **Definition:** Cohesion refers to how closely the responsibilities of a module, class, or method are related to each other.

- **Goal:** High cohesion means that a module or class focuses on a single, well-defined task.

- **Benefits:**

  - Easier to understand, maintain, and reuse.

  - Reduces the risk of unintended side effects.

**Example of High Cohesion:**
```java
class Calculator {
    // All methods are related to mathematical operations
    int add(int a, int b) { return a + b; }
    int subtract(int a, int b) { return a - b; }
    int multiply(int a, int b) { return a * b; }
}
```

**Example of Low Cohesion:**
```java
class Utility {
    // Methods are unrelated
    int add(int a, int b) { return a + b; }
    void print(String message) { System.out.println(message); }
    void saveToFile(String data) { /* Save data to file */ }
}
```
---
2. **Coupling**
- **Definition:** Coupling refers to the degree of dependency between modules, classes, or components.
- **Goal:** Low coupling means that modules or classes are independent and interact with each other through well-defined interfaces.
- **Benefits:**

  - Easier to modify or replace one module without affecting others.

  - Improves flexibility and scalability.
  - Reduces the risk of cascading changes.

**Example of Low Coupling:**
```java
class EmailService {
    void sendEmail(String message) {
        System.out.println("Sending email: " + message);
    }
}

class UserNotifier {
    private EmailService emailService;

    UserNotifier(EmailService emailService) {
        this.emailService = emailService; // Dependency injected
    }

    void notifyUser(String message) {
        emailService.sendEmail(message);
    }
}
```
**Example of High Coupling:**
```java
class UserNotifier {
    private EmailService emailService = new EmailService(); // Tightly coupled

    void notifyUser(String message) {
        emailService.sendEmail(message);
    }
}
```
---
**Key Differences**

![Cohesion vs Coupling](https://www.baeldung.com/wp-content/uploads/sites/4/2021/05/comparison.png)

---

---

### Question 10:
#### Heap and Stack means and differences?

### Answer 10:

The heap and stack are two areas of memory used by Java programs to store data. They serve different purposes and have distinct characteristics.

---
1. **Stack**

- **Purpose:** Used for method execution and local variables.

- **Memory Allocation:** Memory is allocated and deallocated in a Last-In-First-Out (LIFO) order.

- **Scope:** Variables stored in the stack are local to a method and exist only during its execution.

- **Speed:** Faster access compared to the heap.

- **Size:** Fixed size (can be adjusted with JVM options, but limited).

- **Example:** Stores primitive data types (e.g., int, char) and references to objects.

```java
public void method() {
    int x = 10; // Stored in the stack
    String str = "Hello"; // Reference to the string object (stored in the heap)
}
```
---
2. **Heap**

- **Purpose:** Used for dynamic memory allocation (objects and their instance variables).
- **Memory Allocation:** Memory is allocated and deallocated in a random order.
- **Scope:** Objects stored in the heap are global and can be accessed from anywhere in the program.
- **Speed:** Slower access compared to the stack.
- **Size:** Larger and more flexible than the stack.
- **Example:** Stores objects (e.g., String, ArrayList) and their instance variables.

```java
public void method() {
    String str = new String("Hello"); // Object stored in the heap
}
```
---
**Key Differences**

| **Aspect**        | **Stack**                                    | **Heap**                                        |
|-------------------|-------------------------------------------|------------------------------------------------|
| **Purpose**      | Stores method execution and local variables. | Stores objects and their instance variables.   |
| **Memory Allocation** | LIFO (Last-In-First-Out).                | Random order.                                  |
| **Scope**        | Local to a method.                         | Global (accessible from anywhere).            |
| **Speed**        | Faster access.                             | Slower access.                                |
| **Size**         | Fixed size (limited).                     | Larger and more flexible.                     |
| **Example**      | Primitive types, method calls.            | Objects, instance variables.                  |

---

---

### Question 11:
#### What is Exception means and what are the types of Exceptions in Java?

### Answer 11:

An exception in Java is an event that disrupts the normal flow of a program. It occurs when an unexpected situation arises, such as dividing by zero, accessing an invalid array index, or trying to open a file that doesn't exist. Exceptions are used to handle errors and other exceptional events gracefully.

---
Types of Exceptions in Java
Java exceptions are divided into two main categories:

1. Checked Exceptions

2. Unchecked Exceptions

---

1. **Checked Exceptions**
- **Definition:** Exceptions that are checked at compile-time. The compiler ensures that these exceptions are either handled (using try-catch) or declared (using throws).
- **Purpose:** Used for situations that a program can anticipate and recover from (e.g., file I/O, database access).
- **Examples:**

  - IOException

  - SQLException

  - FileNotFoundException

**Example:**
```java
import java.io.FileInputStream;
import java.io.FileNotFoundException;

public class Main {
    public static void main(String[] args) {
        try {
            FileInputStream file = new FileInputStream("nonexistent.txt"); // Checked exception
        } catch (FileNotFoundException e) {
            System.out.println("File not found!");
        }
    }
}
```
2. **Unchecked Exceptions**
- **Definition:** Exceptions that are not checked at compile-time. They occur due to logical errors in the code (e.g., null pointer, division by zero).
- **Purpose:** Used for situations that are usually caused by programming errors and are not expected to be recovered from.
- **Examples:**
  - NullPointerException
  - ArithmeticException
  - ArrayIndexOutOfBoundsException

**Example:**
```java
public class Main {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3};
        System.out.println(numbers[5]); // Unchecked exception (ArrayIndexOutOfBoundsException)
    }
}
```

---

---

### Question 12:
#### How to summarize 'clean code' as short as possible?

### Answer 12:

Clean code is readable, simple, understandable, maintainable and crafted by adhering to DRY and SOLID principles, rigorous testing, and continuous refactoring to reduce complexity and enhance team collaboration.

---

---

### Question 13:
#### What is method of hiding in Java? 

### Answer 13:

In Java, method hiding occurs when a subclass defines a static method with the same signature as a static method in its superclass. This is not the same as method overriding, which applies to instance methods. Method hiding is specific to static methods and is based on the compile-time type of the reference, not the runtime object.

- When a subclass defines a static method with the same name, return type, and parameters as a static method in the superclass, the subclass method hides the superclass method.

- The method called depends on the reference type (not the actual object type).

**Example of Method Hiding**
```java
class Parent {
    static void display() {
        System.out.println("Parent's static method");
    }
}

class Child extends Parent {
    static void display() {
        System.out.println("Child's static method");
    }
}

public class Main {
    public static void main(String[] args) {
        Parent obj1 = new Parent();
        Parent obj2 = new Child(); // Reference type is Parent
        Child obj3 = new Child();

        obj1.display(); // Output: Parent's static method
        obj2.display(); // Output: Parent's static method (method hiding)
        obj3.display(); // Output: Child's static method
    }
}
```

---

---

### Question 14:
#### What is the difference between abstraction and polymorphism in Java? 

### Answer 14:
Abstraction simplifies complexity by hiding implementation details and focusing on what an object does, achieved through abstract classes and interfaces. Polymorphism, on the other hand, enables flexibility by allowing objects to behave differently based on their type, achieved through method overriding and overloading. While abstraction defines a blueprint, polymorphism brings dynamic behavior to the system. Together, they enhance code clarity, reusability, and scalability in Java.

---

| **Feature**       | **Abstraction**                              | **Polymorphism**                               |
|------------------|--------------------------------------------|----------------------------------------------|
| **Definition**   | Hides implementation details.              | Allows objects to take multiple forms.      |
| **Purpose**     | Simplifies complexity.                     | Provides flexibility and reusability.      |
| **How It’s Achieved** | Abstract classes and interfaces.        | Method overriding and overloading.         |
| **Focus**        | What an object does.                      | How an object behaves in different contexts. |
| **Example**      | `abstract void makeSound();`              | `Animal myAnimal = new Dog(); myAnimal.makeSound();` |
| **Use Case**     | Define a blueprint for classes.           | Enable dynamic behavior based on object type. |
