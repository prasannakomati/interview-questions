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

## 💡 Interview Preparation Tips

* ✅ Understand each definition in your own words.
* ✅ Practise writing the examples without copying.
* ✅ Learn the differences between JVM, JRE, and JDK.
* ✅ Be prepared to explain overloading and overriding with code.
* ✅ Run the examples in Eclipse and observe the output.

**Keep Learning, Keep Coding! ☕💻**

*Prepared for Core Java interview preparation — beginner level.*
