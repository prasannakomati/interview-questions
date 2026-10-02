# ☕ Core Java Interview Questions & Answers

<p align="center">
  <strong>🚀 Core Java Interview Preparation</strong><br>
  <em>Simple explanations • Beginner-friendly answers • Quick revision</em>
</p>

---

## 📚 Table of Contents

1. [What is Java?](#1-what-is-java)
2. [Why is Java Platform-Independent?](#2-why-is-java-platform-independent)
3. [What is JVM?](#3-what-is-jvm)
4. [What is JRE?](#4-what-is-jre)
5. [What is JDK?](#5-what-is-jdk)
6. [What are Data Types in Java?](#6-what-are-data-types-in-java)
7. [What is a Variable?](#7-what-is-a-variable)
8. [What are Identifiers in Java?](#8-what-are-identifiers-in-java)
9. [What is a Class?](#9-what-is-a-class)
10. [What is an Object?](#10-what-is-an-object)
11. [What is a Constructor?](#11-what-is-a-constructor)
12. [What are the Types of Constructors?](#12-what-are-the-types-of-constructors)
13. [What is a Method?](#13-what-is-a-method)
14. [What is Method Overloading?](#14-what-is-method-overloading)
15. [What is Method Overriding?](#15-what-is-method-overriding)
16. [Overloading vs Overriding](#16-method-overloading-vs-method-overriding)
17. [What is the `main()` Method?](#17-what-is-the-main-method)
18. [Why is `main()` Static?](#18-why-is-main-static)
19. [What is `static` in Java?](#19-what-is-static-in-java)
20. [What is `final` in Java?](#20-what-is-final-in-java)

---

# ☕ Core Java Interview Questions & Answers — Part 2

<p align="center">
  <strong>💻 Java Fundamentals & Object-Oriented Programming</strong><br>
  <em>Simple answers • Code examples • Interview revision</em>
</p>

---

## 📚 Table of Contents

1. [Difference Between final, finally, and finalize()](#1-difference-between-final-finally-and-finalize)
2. [What are Access Modifiers?](#2-what-are-access-modifiers)
3. [Difference Between public, private, and protected](#3-difference-between-public-private-and-protected)
4. [What is Type Casting?](#4-what-is-type-casting)
5. [Implicit vs Explicit Casting](#5-implicit-vs-explicit-casting)
6. [What are Keywords in Java?](#6-what-are-keywords-in-java)
7. [What are Comments in Java?](#7-what-are-comments-in-java)
8. [What is a Package?](#8-what-is-a-package)
9. [What is the Use of import?](#9-what-is-the-use-of-import)
10. [What are Naming Conventions?](#10-what-are-naming-conventions-in-java)
11. [What is OOP?](#11-what-is-oop)
12. [What are the Four Pillars of OOP?](#12-what-are-the-four-pillars-of-oop)
13. [What is Encapsulation?](#13-what-is-encapsulation)
14. [What is Inheritance?](#14-what-is-inheritance)
15. [What is Polymorphism?](#15-what-is-polymorphism)
16. [What is Abstraction?](#16-what-is-abstraction)
17. [What is an Abstract Class?](#17-what-is-an-abstract-class)
18. [What is an Interface?](#18-what-is-an-interface)
19. [Abstract Class vs Interface](#19-abstract-class-vs-interface)

---


## 1. What is Java?

**Answer:** Java is a high-level, class-based, object-oriented programming language used to develop web applications, desktop applications, enterprise software, and Android applications.

**Example:**

```java
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

**Key points:**

* ☕ Developed by James Gosling's team at Sun Microsystems.
* 🔹 Object-oriented and strongly typed.
* 🔹 Supports platform-independent execution through the JVM.

---

## 2. Why is Java Platform-Independent?

**Answer:** Java is platform-independent because Java source code is compiled into **bytecode**, which can run on any compatible operating system with a Java Virtual Machine (JVM).

**How it works:**

```text
Java Source Code (.java)
          |
          ▼
     Java Compiler
          |
          ▼
      Bytecode (.class)
          |
          ▼
      JVM on the OS
          |
          ▼
       Program Runs
```

**Remember:** Write Once, Run Anywhere (WORA).

---

## 3. What is JVM?

**Answer:** JVM stands for **Java Virtual Machine**. It executes Java bytecode and provides the runtime environment needed to run Java programs.

**Main functions:**

* Executes bytecode.
* Manages memory.
* Performs garbage collection.
* Supports runtime security checks.

**Example:** The JVM allows compatible Java bytecode to run on Windows, Linux, and macOS.

---

## 4. What is JRE?

**Answer:** JRE stands for **Java Runtime Environment**. It provides the components needed to run Java applications, including the JVM and supporting runtime libraries.

**Remember:** JRE is for running Java applications, not for developing them with the full set of Java development tools.

---

## 5. What is JDK?

**Answer:** JDK stands for **Java Development Kit**. It provides the tools required to develop, compile, and run Java applications.

**It includes:**

* Java compiler (`javac`)
* Java launcher (`java`)
* Java libraries and development tools
* Runtime components

**Relationship:**

```text
JDK
 ├── Development Tools
 └── Runtime Components
      └── JVM
```

*Note: This is a simplified conceptual view; the exact packaging varies by Java version.*

---

## 6. What are Data Types in Java?

**Answer:** Data types specify the kind of value a variable can store.

Java has two main categories of data types.

### A. Primitive Data Types

| Data Type | Example             | Purpose                  |
| --------- | ------------------- | ------------------------ |
| `byte`    | `byte a = 10;`      | Small integer            |
| `short`   | `short a = 1000;`   | Short integer            |
| `int`     | `int a = 100;`      | Integer                  |
| `long`    | `long a = 10000L;`  | Large integer            |
| `float`   | `float a = 10.5f;`  | Decimal number           |
| `double`  | `double a = 20.55;` | Double-precision decimal |
| `char`    | `char a = 'A';`     | Single character         |
| `boolean` | `boolean a = true;` | True or false            |

### B. Non-Primitive (Reference) Types

Examples include:

* `String`
* Arrays
* Classes
* Interfaces
* Enums

---

## 7. What is a Variable?

**Answer:** A variable is a named storage location used to hold a value in a Java program.

**Example:**

```java
int age = 21;
String name = "Prasanna";
```

Here:

* `int` and `String` are types.
* `age` and `name` are variable names.
* `21` and `"Prasanna"` are values.

---

## 8. What are Identifiers in Java?

**Answer:** Identifiers are names used to identify program elements such as variables, methods, classes, and interfaces.

**Examples:**

```java
int studentAge = 20;

class StudentDetails {
    void displayName() {
        System.out.println("Prasanna");
    }
}
```

**Rules:**

* Can contain letters, digits, `_`, and `$`.
* Cannot start with a digit.
* Cannot be a Java keyword.
* Are case-sensitive.

**Valid:** `age`, `studentName`, `_count`

**Invalid:** `2name`, `class`, `student-name`

---

## 9. What is a Class?

**Answer:** A class is a blueprint used to create objects. It defines the fields and methods that its objects can have.

**Example:**

```java
class Student {
    int id;
    String name;

    void display() {
        System.out.println(id + " " + name);
    }
}
```

Here, `Student` is a class.

---

## 10. What is an Object?

**Answer:** An object is an instance of a class. It can have state (data) and behavior (methods).

**Example:**

```java
Student s1 = new Student();

s1.id = 101;
s1.name = "Prasanna";

s1.display();
```

Here, `s1` is a reference variable that refers to a `Student` object.

**Real-life example:** A `Car` class can describe cars, while individual cars are objects of that class.

---

## 11. What is a Constructor?

**Answer:** A constructor is a special class member used to initialize a newly created object.

**Key points:**

* Its name must match the class name.
* It has no return type, not even `void`.
* It runs when an object is created using `new`.

**Example:**

```java
class Student {
    String name;

    Student() {
        name = "Prasanna";
    }
}
```

---

## 12. What are the Types of Constructors?

Constructors are commonly classified into two types in beginner-level Java learning.

### A. No-Argument Constructor

A constructor that takes no parameters.

```java
class Student {
    Student() {
        System.out.println("Student created");
    }
}
```

### B. Parameterized Constructor

A constructor that accepts parameters.

```java
class Student {
    String name;

    Student(String studentName) {
        name = studentName;
    }
}
```

**Important:** If you do not declare any constructor, Java can provide a default constructor. If you declare a constructor yourself, Java does not automatically provide that default constructor.

---

## 13. What is a Method?

**Answer:** A method is a block of code that performs a particular task and can be called when needed.

**Example:**

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
}
```

**Calling the method:**

```java
Calculator c = new Calculator();

System.out.println(c.add(10, 20));
```

**Output:**

```text
30
```

---

## 14. What is Method Overloading?

**Answer:** Method overloading means defining multiple methods with the same name in the same class but with different parameter lists.

Parameters can differ in number, types, or order.

**Example:**

```java
class Calculator {

    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```

**Key point:** Changing only the return type does not create a valid overloaded method.

---

## 15. What is Method Overriding?

**Answer:** Method overriding occurs when a subclass provides its own implementation of an inherited instance method, using a compatible method signature.

**Example:**

```java
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
```

**Calling the overridden method:**

```java
Animal a = new Dog();
a.sound();
```

**Output:**

```text
Dog barks
```

**Key point:** Overriding supports runtime polymorphism.

---

## 16. Method Overloading vs Method Overriding

| Feature      | Overloading                                              | Overriding                                      |
| ------------ | -------------------------------------------------------- | ----------------------------------------------- |
| Meaning      | Same method name, different parameter lists              | Subclass redefines an inherited instance method |
| Classes      | Usually the same class                                   | Parent and child classes                        |
| Parameters   | Must differ                                              | Must match the method signature                 |
| Inheritance  | Not required                                             | Required                                        |
| Polymorphism | Compile-time                                             | Runtime                                         |
| Return type  | May differ when parameters differ, subject to Java rules | Must be compatible with the overridden method   |
| Example      | `add(int, int)` and `add(int, int, int)`                 | `Animal.sound()` and `Dog.sound()`              |

---

## 17. What is the `main()` Method?

**Answer:** The `main()` method is the conventional entry point used by the Java launcher to start a basic Java application.

**Syntax:**

```java
public static void main(String[] args) {
    System.out.println("Hello Java");
}
```

**Meaning:**

* `public` — accessible to the Java launcher.
* `static` — can be invoked without creating an instance of the class.
* `void` — returns no value.
* `main` — method name.
* `String[] args` — receives command-line arguments.

---

## 18. Why is `main()` Static?

**Answer:** The `main()` method is static so the Java launcher can invoke it without first creating an object of the class.

**Example:**

```java
class Demo {
    public static void main(String[] args) {
        System.out.println("Program started");
    }
}
```

If `main()` were an ordinary instance method, an object would be needed to call it. The conventional Java entry-point method avoids that requirement.

---

## 19. What is `static` in Java?

**Answer:** The `static` keyword declares a member that belongs to the class rather than to individual instances.

It can be used with fields, methods, initialization blocks, and nested classes.

**Example:**

```java
class Student {
    static String college = "VKR College";
    String name;
}
```

All `Student` objects share the same `college` field.

**Static method example:**

```java
class Demo {
    static void display() {
        System.out.println("Static method");
    }

    public static void main(String[] args) {
        Demo.display();
    }
}
```

**Remember:** A static method cannot directly access an instance field or instance method without an object reference.

---

## 20. What is `final` in Java?

**Answer:** The `final` keyword restricts certain kinds of changes in Java. Its meaning depends on where it is used.

### A. Final Variable

A final variable can be assigned only once.

```java
final int MAX_MARKS = 100;
```

### B. Final Method

A final method cannot be overridden in a subclass.

```java
class Parent {
    final void display() {
        System.out.println("Hello");
    }
}
```

### C. Final Class

A final class cannot be extended.

```java
final class Vehicle {
}
```

**Important:** A final reference variable cannot be reassigned to another object, but the referenced object's internal state may still be changed if the object is mutable.

---

## 🎯 Quick Revision

| Keyword / Concept | Remember                                                             |
| ----------------- | -------------------------------------------------------------------- |
| Java              | High-level, class-based programming language                         |
| JVM               | Executes Java bytecode                                               |
| JRE               | Runtime components for Java applications                             |
| JDK               | Development tools and runtime components                             |
| Variable          | Named storage for a value                                            |
| Identifier        | Name of a program element                                            |
| Class             | Blueprint for objects                                                |
| Object            | Instance of a class                                                  |
| Constructor       | Initializes a new object                                             |
| Method            | Performs a task                                                      |
| Overloading       | Same name, different parameters                                      |
| Overriding        | Subclass implementation of an inherited method                       |
| `main()`          | Conventional Java application entry point                            |
| `static`          | Class-level member                                                   |
| `final`           | Restricts reassignment, overriding, or inheritance, depending on use |

---


# ☕ Core Java Interview Questions & Answers — Part 2

<p align="center">
  <strong>💻 Java Fundamentals & Object-Oriented Programming</strong><br>
  <em>Simple answers • Code examples • Interview revision</em>
</p>

---

 

## 1. Difference Between `final`, `finally`, and `finalize()`

**Answer:** These three terms are different Java concepts.

| Term         | Meaning           | Purpose                                                                                                  |
| ------------ | ----------------- | -------------------------------------------------------------------------------------------------------- |
| `final`      | Keyword           | Restricts reassignment, overriding, or inheritance                                                       |
| `finally`    | Block             | Executes during normal or exceptional completion of a `try` statement, subject to abrupt JVM termination |
| `finalize()` | Deprecated method | Historically associated with object cleanup before garbage collection                                    |

### Example: `final`

```java
final int age = 21;
// age = 25; // Compilation error
```

### Example: `finally`

```java
try {
    System.out.println("Inside try");
} finally {
    System.out.println("Finally block");
}
```

### Example: `finalize()`

Historically, `finalize()` could be invoked by the garbage collector before reclaiming an object. However, **finalization is deprecated for removal** and is unreliable for resource management. Do not use it for new code.

Use `try-with-resources` for resources such as files and database connections.

---

## 2. What are Access Modifiers?

**Answer:** Access modifiers control where classes, methods, constructors, and fields can be accessed from.

Java has four access levels:

* `public`
* `protected`
* Default (package-private; no keyword)
* `private`

**Example:**

```java
public class Student {
    private int age;
    public String name;
    protected int marks;
    String college;
}
```

---

## 3. Difference Between `public`, `private`, and `protected`

| Modifier    | Same Class | Same Package | Subclass in Another Package  | Other Packages    |
| ----------- | ---------- | ------------ | ---------------------------- | ----------------- |
| `public`    | Yes        | Yes          | Yes                          | Yes               |
| `protected` | Yes        | Yes          | Yes, subject to access rules | No general access |
| Default     | Yes        | Yes          | No                           | No                |
| `private`   | Yes        | No           | No                           | No                |

**Remember:**

* `public` — accessible wherever the declaring type and its members are accessible.
* `private` — accessible only within the declaring top-level class or enclosing class's applicable scope.
* `protected` — accessible within the same package and through inheritance, subject to Java's cross-package access rules.
* Default — accessible within the same package.

**Important:** A top-level class can normally be declared `public` or package-private, not `private` or `protected`.

---

## 4. What is Type Casting?

**Answer:** Type casting is the process of converting a value from one data type to another.

Java supports conversions such as:

* `int` to `double`
* `double` to `int`
* `char` to `int`

**Example:**

```java
int number = 100;
double result = number;
```

Here, the integer value is converted into a `double`.

---

## 5. Implicit vs Explicit Casting

### A. Implicit Casting (Widening)

Java automatically converts a value to a compatible wider primitive type.

```java
int number = 100;
double result = number;

System.out.println(result);
```

**Output:**

```text
100.0
```

### B. Explicit Casting (Narrowing)

The programmer specifies the target type using a cast. Information may be lost.

```java
double price = 99.99;
int result = (int) price;

System.out.println(result);
```

**Output:**

```text
99
```

| Feature       | Implicit Casting                                       | Explicit Casting                   |
| ------------- | ------------------------------------------------------ | ---------------------------------- |
| Also called   | Widening conversion                                    | Narrowing conversion               |
| Conversion    | Usually to a wider compatible primitive type           | Often to a narrower primitive type |
| Cast required | No                                                     | Yes                                |
| Data loss     | Possible in some conversions, such as `int` to `float` | Possible                           |
| Example       | `int` → `double`                                       | `double` → `int`                   |

---

## 6. What are Keywords in Java?

**Answer:** Keywords are reserved words that have predefined meanings in Java. They cannot be used as ordinary identifiers.

**Examples:**

```java
class Student {
    public static void main(String[] args) {
        int age = 21;
        if (age >= 18) {
            System.out.println("Adult");
        }
    }
}
```

Keywords in this example include `class`, `public`, `static`, `void`, `int`, and `if`.

Other examples include `return`, `new`, `this`, `extends`, `implements`, `try`, and `final`.

**Note:** `true`, `false`, and `null` are literals, not keywords in the Java Language Specification's technical classification.

---

## 7. What are Comments in Java?

**Answer:** Comments are explanatory text in source code that the compiler does not treat as executable Java statements.

Java has three commonly used comment forms.

### A. Single-Line Comment

```java
// This is a single-line comment
int age = 21;
```

### B. Multi-Line Comment

```java
/*
 This is a multi-line comment.
 It can span multiple lines.
*/
```

### C. Documentation Comment

```java
/**
 * Displays a welcome message.
 */
void display() {
    System.out.println("Welcome");
}
```

Documentation comments can be processed by the `javadoc` tool to generate API documentation.

---

## 8. What is a Package?

**Answer:** A package groups related Java types, such as classes, interfaces, and enums, under a common namespace.

**Benefits:**

* Organizes code.
* Helps avoid naming conflicts.
* Supports package-level access control.
* Makes large projects easier to maintain.

**Example:**

```java
package com.example.student;

public class Student {
    public void display() {
        System.out.println("Student details");
    }
}
```

Here, `com.example.student` is the package name.

---

## 9. What is the Use of `import`?

**Answer:** The `import` statement allows a Java source file to refer to accessible types from another package by their simple names instead of repeatedly writing their fully qualified names.

**Without import:**

```java
java.util.Scanner sc =
    new java.util.Scanner(System.in);
```

**With import:**

```java
import java.util.Scanner;

class Demo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println(sc.nextLine());
        sc.close();
    }
}
```

**Remember:** `import` does not copy a class into your program or automatically import subpackages.

---

## 10. What are Naming Conventions in Java?

**Answer:** Naming conventions are commonly followed guidelines for choosing readable and consistent names for Java program elements.

| Element                | Convention               | Example               |
| ---------------------- | ------------------------ | --------------------- |
| Class                  | PascalCase               | `StudentDetails`      |
| Interface              | PascalCase               | `Runnable`            |
| Method                 | lowerCamelCase           | `calculateTotal()`    |
| Variable               | lowerCamelCase           | `studentName`         |
| Constant               | UPPER_SNAKE_CASE         | `MAX_VALUE`           |
| Package                | Lowercase                | `com.example.student` |
| Generic type parameter | Usually a capital letter | `T`, `E`, `K`, `V`    |

**Example:**

```java
class StudentDetails {
    static final int MAX_MARKS = 100;

    String studentName;

    void displayDetails() {
        System.out.println(studentName);
    }
}
```

These conventions improve readability but are not all mandatory compiler rules.

---

## 11. What is OOP?

**Answer:** OOP stands for **Object-Oriented Programming**. It is a programming approach that organizes software around objects containing data and behavior.

Java supports object-oriented programming through classes, objects, inheritance, polymorphism, encapsulation, and abstraction.

**Example:**

```java
class Car {
    String color;

    void drive() {
        System.out.println("Car is moving");
    }
}
```

Here, `Car` defines data (`color`) and behavior (`drive()`).

---

## 12. What are the Four Pillars of OOP?

The four commonly taught pillars of object-oriented programming are:

| Pillar        | Meaning                                                         |
| ------------- | --------------------------------------------------------------- |
| Encapsulation | Bundling data and methods together while controlling access     |
| Inheritance   | Creating a class based on another class                         |
| Polymorphism  | One interface or method call can have different implementations |
| Abstraction   | Hiding implementation details and exposing essential behavior   |

```text
          OOP
           |
   ┌───────┼────────┐
   |       |        |
Encapsulation     Inheritance
   |
Polymorphism
   |
Abstraction
```

---

## 13. What is Encapsulation?

**Answer:** Encapsulation is the practice of bundling data and related methods into a class while restricting direct access to internal state.

A common implementation uses `private` fields and public methods to control access.

**Example:**

```java
class Student {
    private int age;

    public void setAge(int age) {
        if (age > 0) {
            this.age = age;
        }
    }

    public int getAge() {
        return age;
    }
}
```

**Usage:**

```java
Student s = new Student();
s.setAge(21);

System.out.println(s.getAge());
```

**Output:**

```text
21
```

**Benefit:** The class controls how its internal data is accessed and updated.

---

## 14. What is Inheritance?

**Answer:** Inheritance allows a class to inherit accessible members from another class. It supports code reuse and method overriding.

**Example:**

```java
class Animal {
    void eat() {
        System.out.println("Animal eats");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Dog barks");
    }
}
```

**Usage:**

```java
Dog d = new Dog();
d.eat();
d.bark();
```

**Output:**

```text
Animal eats
Dog barks
```

Here, `Dog` is the subclass and `Animal` is the superclass.

---

## 15. What is Polymorphism?

**Answer:** Polymorphism means "many forms." In Java, it allows the same method name or method call to behave differently depending on the parameters or the actual object.

Two common forms are:

### A. Compile-Time Polymorphism

Achieved through method overloading.

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }
}
```

### B. Runtime Polymorphism

Achieved through method overriding and dynamic method dispatch.

```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}
```

```java
Animal a = new Dog();
a.sound();
```

**Output:**

```text
Bark
```

---

## 16. What is Abstraction?

**Answer:** Abstraction means exposing essential operations while hiding unnecessary implementation details.

In Java, abstraction is commonly achieved through abstract classes and interfaces.

**Real-life example:** When driving a car, you use the steering wheel and pedals without needing to understand every internal engine mechanism.

**Java example:**

```java
abstract class Shape {
    abstract double calculateArea();
}
```

The abstract class declares what the operation should do, while subclasses provide the implementation.

---

## 17. What is an Abstract Class?

**Answer:** An abstract class is a class declared with the `abstract` keyword. It cannot be instantiated directly and can contain both abstract methods and implemented methods.

**Example:**

```java
abstract class Animal {
    abstract void sound();

    void sleep() {
        System.out.println("Animal sleeps");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
```

**Usage:**

```java
Animal a = new Dog();
a.sound();
a.sleep();
```

**Key points:**

* Cannot be instantiated directly.
* Can contain abstract and concrete methods.
* Can have constructors and instance fields.
* A concrete subclass must implement inherited abstract methods unless it is also abstract.

---

## 18. What is an Interface?

**Answer:** An interface defines a contract that implementing classes agree to follow. It is declared using the `interface` keyword.

Interfaces can contain abstract methods, default methods, static methods, private helper methods, and constants.

**Example:**

```java
interface Printable {
    void print();
}

class Document implements Printable {
    @Override
    public void print() {
        System.out.println("Printing document");
    }
}
```

**Usage:**

```java
Printable p = new Document();
p.print();
```

**Output:**

```text
Printing document
```

**Key points:**

* A class uses `implements` to implement an interface.
* A class can implement multiple interfaces.
* Interface abstract methods are implicitly `public`.
* An implementing class must provide compatible public implementations of those methods unless the class is abstract.

---

## 19. Abstract Class vs Interface

| Feature              | Abstract Class                                       | Interface                                        |
| -------------------- | ---------------------------------------------------- | ------------------------------------------------ |
| Declaration          | `abstract class`                                     | `interface`                                      |
| Inheritance keyword  | `extends`                                            | `implements`                                     |
| Constructors         | Allowed                                              | Not allowed                                      |
| Instance fields      | Allowed                                              | Not allowed                                      |
| Constants            | Allowed                                              | Allowed (`public static final` by default)       |
| Abstract methods     | Allowed                                              | Allowed                                          |
| Concrete methods     | Allowed                                              | Default, static, and private methods are allowed |
| Multiple inheritance | A class can extend only one class                    | A class can implement multiple interfaces        |
| Main purpose         | Share state and implementation among related classes | Define a contract or capability                  |

### Example: Abstract Class

```java
abstract class Vehicle {
    int speed;

    abstract void start();

    void stop() {
        System.out.println("Vehicle stopped");
    }
}
```

### Example: Interface

```java
interface Flyable {
    void fly();
}

class Airplane implements Flyable {
    @Override
    public void fly() {
        System.out.println("Airplane is flying");
    }
}
```

**When to use each:**

* Use an **abstract class** when related classes need shared instance state or common implementation.
* Use an **interface** when different classes need to follow the same contract or provide the same capability.

---

## 🎯 Quick Revision

| Concept            | One-Line Answer                                                         |
| ------------------ | ----------------------------------------------------------------------- |
| `final`            | Restricts reassignment, overriding, or inheritance                      |
| `finally`          | Cleanup block associated with `try` and exception handling              |
| `finalize()`       | Deprecated object-finalization method                                   |
| Access modifiers   | Control accessibility                                                   |
| Type casting       | Converts a value from one type to another                               |
| Keywords           | Reserved words with predefined meanings                                 |
| Comments           | Explanatory text ignored as executable code                             |
| Package            | Groups related Java types                                               |
| `import`           | Allows use of accessible types by simple name                           |
| Naming conventions | Guidelines for readable names                                           |
| OOP                | Programming organized around objects                                    |
| Encapsulation      | Bundles data and methods and controls access                            |
| Inheritance        | Derives a class from another class                                      |
| Polymorphism       | Supports different implementations through a common method call or name |
| Abstraction        | Exposes essential behavior and hides implementation details             |
| Abstract class     | A class that cannot be instantiated directly                            |
| Interface          | A contract that classes can implement                                   |

---

## 💡 Interview Practice Checklist

* [ ] Explain `final`, `finally`, and `finalize()`.
* [ ] Compare all four access levels.
* [ ] Demonstrate widening and narrowing conversions.
* [ ] Explain the four pillars of OOP with examples.
* [ ] Write a program demonstrating encapsulation.
* [ ] Demonstrate inheritance and runtime polymorphism.
* [ ] Explain the difference between an abstract class and an interface.

**☕ Keep Learning, Keep Coding, and Keep Practising! 💻**




## 💡 Interview Preparation Tips

* ✅ Understand each definition in your own words.
* ✅ Practise writing the examples without copying.
* ✅ Learn the differences between JVM, JRE, and JDK.
* ✅ Be prepared to explain overloading and overriding with code.
* ✅ Run the examples in Eclipse and observe the output.

**Keep Learning, Keep Coding! ☕💻**

*Prepared for Core Java interview preparation — beginner level.*
