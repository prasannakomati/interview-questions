

# Java Fundamentals – Interview Questions and Answers

**Topic:** Core Java Fundamentals  
**Level:** Beginner  
**Purpose:** Interview Preparation and Revision

---

## 1. Introduction to Java

### Q1. What is Java?
**Answer:**  
Java is a high-level, object-oriented, and platform-independent programming language used to develop desktop, web, mobile, and enterprise applications.

### Q2. Who developed Java?
**Answer:**  
Java was developed by James Gosling and his team at Sun Microsystems.

### Q3. When was Java released?
**Answer:**  
Java was officially released in 1995.

### Q4. Why is Java popular?
**Answer:**  
Java is popular because it is platform-independent, object-oriented, secure, robust, and supports multithreading.

### Q5. Where is Java used?
**Answer:**  
Java is used in:
- Web applications
- Enterprise applications
- Android development
- Banking applications
- Desktop applications
- Cloud-based applications

### Q6. Is Java a purely object-oriented programming language?
**Answer:**  
No. Java is not purely object-oriented because it supports primitive data types such as `int`, `char`, `boolean`, and `double`.

---

## 2. Computer and Programming Language

### Q7. What is a computer?
**Answer:**  
A computer is an electronic device that accepts data as input, processes the data, and produces useful information as output.

**Example:**
- Input: Two numbers
- Processing: Addition
- Output: Sum of the numbers

### Q8. What is a programming language?
**Answer:**  
A programming language is a language used to write instructions that tell a computer what to do.

**Examples:** Java, Python, C, and C++.

### Q9. What is a program?
**Answer:**  
A program is a set of instructions written to perform a particular task.

**Example:**
```java
System.out.println("Hello World");
```

This statement displays `Hello World` on the screen.

### Q10. Why do we need programming languages?
**Answer:**  
Computers work using machine instructions. Programming languages help humans write instructions in a form that can be translated into instructions the computer can execute.

### Q11. What is the difference between a programming language and a program?
**Answer:**

| Programming Language | Program |
|---|---|
| Used to write instructions. | A set of written instructions. |
| Example: Java. | Example: A calculator program. |

---

## 3. High-Level and Low-Level Languages

### Q12. What is a high-level programming language?
**Answer:**  
A high-level programming language uses instructions that are relatively easy for humans to read and understand.

**Examples:** Java, Python, and C++.

### Q13. What is a low-level programming language?
**Answer:**  
A low-level programming language is closer to the instructions and operations of computer hardware.

**Examples:** Machine language and assembly language.

### Q14. What is machine language?
**Answer:**  
Machine language consists of binary instructions represented using `0` and `1`. The processor executes machine instructions.

**Example (illustrative binary):**
```text
10110000 01100001
```

The meaning of a binary instruction depends on the processor's instruction set.

### Q15. What is assembly language?
**Answer:**  
Assembly language uses short symbolic instructions called mnemonics to represent machine instructions.

**Example (illustrative):**
```asm
MOV AX, 5
```

The exact syntax depends on the processor architecture and assembler.

### Q16. What is the difference between high-level and low-level languages?

| High-Level Language | Low-Level Language |
|---|---|
| Easier for humans to understand. | Closer to hardware instructions. |
| Generally easier to develop and maintain. | Often requires hardware-specific knowledge. |
| Example: Java. | Examples: Assembly and machine language. |
| Requires translation into executable instructions. | Machine code is directly executed by the processor. |

---

## 4. History and Features of Java

### Q17. What was the original name of Java?
**Answer:**  
Java was originally called **Oak**. It was later renamed Java.

### Q18. What are the main features of Java?
**Answer:**

1. **Simple:** Java avoids many complex features found in some other languages.
2. **Object-oriented:** Java supports classes and objects.
3. **Platform-independent:** Java bytecode can run on compatible JVM implementations.
4. **Portable:** Java provides consistent behavior across supported platforms.
5. **Secure:** Java includes features such as bytecode verification and runtime security mechanisms.
6. **Robust:** Java provides exception handling and automatic memory management.
7. **Multithreaded:** Java supports running multiple threads.
8. **Architecture-neutral:** Java bytecode is not tied to one processor architecture.
9. **High-performance:** JIT compilation can improve execution speed.
10. **Distributed:** Java supports network-based application development.

### Q19. What does platform-independent mean?
**Answer:**  
Platform-independent means Java bytecode can run on different operating systems when a compatible JVM is available.

**Example:** A compiled Java program can run on Windows and Linux without recompiling the source code, provided the required runtime and dependencies are compatible.

### Q20. What is the meaning of "Write Once, Run Anywhere"?
**Answer:**  
It means Java source code can be compiled into bytecode once and that bytecode can run on different platforms with compatible JVMs.

### Q21. Is Java compiled or interpreted?
**Answer:**  
Java uses both compilation and runtime execution techniques. The Java compiler converts source code into bytecode, and the JVM interprets or compiles bytecode into native machine instructions.

---

## 5. JDK, JRE, and JVM

### Q22. What is the JVM?
**Answer:**  
JVM stands for **Java Virtual Machine**. It loads and executes Java bytecode.

### Q23. What is the JRE?
**Answer:**  
JRE stands for **Java Runtime Environment**. Traditionally, it refers to the JVM and the libraries and components needed to run Java applications.

### Q24. What is the JDK?
**Answer:**  
JDK stands for **Java Development Kit**. It contains development tools such as the Java compiler and the tools needed to develop Java applications.

### Q25. What is the difference between JDK, JRE, and JVM?

| JDK | JRE | JVM |
|---|---|---|
| Used to develop Java applications. | Traditionally used to run Java applications. | Executes Java bytecode. |
| Includes development tools. | Includes runtime components. | Part of the runtime environment. |
| Contains the Java compiler (`javac`). | Provides libraries needed at runtime. | Loads, verifies, and executes bytecode. |

**Note:** Modern JDK distributions commonly do not provide a separate JRE installation. You can use a JDK to compile and run Java programs.

### Q26. What is the Java compiler?
**Answer:**  
The Java compiler, `javac`, converts Java source code (`.java`) into bytecode (`.class`).

### Q27. What is bytecode?
**Answer:**  
Bytecode is the intermediate instruction format generated by the Java compiler. The JVM executes it.

---

## 6. How Java Works: Compilation and Execution

### Q28. Explain the execution process of a Java program.
**Answer:**

The Java program follows these steps:

1. Write source code in a `.java` file.
2. Compile the source code using `javac`.
3. The compiler generates a `.class` file containing bytecode.
4. The JVM loads the required classes.
5. The JVM verifies and executes the bytecode.
6. The program produces output.

**Flow:**

```text
Java Source Code
     Main.java
         |
         v
Java Compiler (javac)
         |
         v
Bytecode (Main.class)
         |
         v
         JVM
         |
         v
Program Output
```

### Q29. What is the extension of a Java source file?
**Answer:**  
The extension is `.java`.

**Example:** `Main.java`

### Q30. What is the extension of a compiled Java class file?
**Answer:**  
The extension is `.class`.

**Example:** `Main.class`

### Q31. How do you compile a Java program using the command line?
**Answer:**
```bash
javac Main.java
```

This generates `Main.class` if compilation succeeds.

### Q32. How do you run a compiled Java program?
**Answer:**
```bash
java Main
```

Use the class name without the `.class` extension.

### Q33. What is the difference between compilation and execution?
**Answer:**

- **Compilation:** Converts Java source code into bytecode and checks for compilation errors.
- **Execution:** Runs the compiled program through the JVM.

### Q34. What happens if a Java program contains a syntax error?
**Answer:**  
The compiler reports a compilation error, and the program cannot be compiled successfully until the error is corrected.

---

## 7. Installing JDK and Setting Up Eclipse

### Q35. What is the JDK installation used for?
**Answer:**  
The JDK provides the tools needed to compile and run Java programs and develop Java applications.

### Q36. What is Eclipse?
**Answer:**  
Eclipse IDE is a software development environment that provides tools for writing, compiling, debugging, and managing Java projects.

### Q37. What is an IDE?
**Answer:**  
IDE stands for **Integrated Development Environment**. It combines tools such as a code editor, compiler integration, and debugger in one application.

**Examples:** Eclipse, IntelliJ IDEA, and NetBeans.

### Q38. How can you check whether Java is installed?
**Answer:**  
Open Command Prompt or a terminal and execute:

```bash
java -version
```

To check the compiler:

```bash
javac -version
```

### Q39. What is the PATH environment variable?
**Answer:**  
`PATH` tells the operating system where to find executable commands such as `java` and `javac`.

### Q40. What is JAVA_HOME?
**Answer:**  
`JAVA_HOME` is an environment variable commonly used to identify the JDK installation directory. Some development tools use it to locate Java.

### Q41. What is the difference between a text editor and an IDE?
**Answer:**

| Text Editor | IDE |
|---|---|
| Mainly used to write and edit code. | Provides tools for the development workflow. |
| May require separate compilation commands. | Usually integrates compilation and debugging tools. |
| Example: Notepad. | Example: Eclipse. |

---

## 8. First Java Program

### Q42. Write your first Java program.
**Answer:**

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

**Output:**
```text
Hello World
```

### Q43. Why do we use `public class Main`?
**Answer:**  
`public` is an access modifier, and `class` declares a class. `Main` is the class name.

When a public top-level class is declared, its source file normally uses the same name. In this example, the file is `Main.java`.

### Q44. What is a class in Java?
**Answer:**  
A class is a blueprint used to define objects, including their data and behavior.

### Q45. What is a statement in Java?
**Answer:**  
A statement is an instruction that performs an action.

**Example:**
```java
int age = 21;
```

### Q46. Why do we use semicolons in Java?
**Answer:**  
A semicolon (`;`) marks the end of most Java statements.

**Example:**
```java
System.out.println("Hello");
```

---

## 9. The `main()` Method and `System.out.println()`

### Q47. What is the `main()` method?
**Answer:**  
The `main()` method is a standard entry point used to launch a conventional Java application.

### Q48. Explain `public static void main(String[] args)`.
**Answer:**

```java
public static void main(String[] args)
```

- **public:** Allows the launcher to access the method.
- **static:** Allows the method to be invoked without creating an instance of the class.
- **void:** The method does not return a value.
- **main:** The method name recognized by the conventional Java launcher.
- **String[] args:** An array of strings containing command-line arguments.

### Q49. What is `System.out.println()`?
**Answer:**  
`System.out.println()` prints a value to the standard output, usually the console, and moves to a new line.

**Example:**
```java
System.out.println("Java");
System.out.println("Programming");
```

**Output:**
```text
Java
Programming
```

### Q50. What is the difference between `print()` and `println()`?
**Answer:**

| `print()` | `println()` |
|---|---|
| Prints without automatically moving to a new line. | Prints and then moves to a new line. |
| Output continues on the same line. | The next output starts on another line. |

**Example:**
```java
System.out.print("Hello ");
System.out.print("Java");
```

**Output:**
```text
Hello Java
```

### Q51. What is `System.out`?
**Answer:**  
`System.out` is the standard output stream, typically connected to the console.

### Q52. Can we execute a Java program without a `main()` method?
**Answer:**  
For a conventional Java application launched with the standard `java` launcher, an appropriate entry-point method is required. Some special execution environments and newer Java features have different rules.

---

## 10. Comments in Java

### Q53. What is a comment in Java?
**Answer:**  
A comment is text written in source code to explain the code. The compiler ignores ordinary comments.

### Q54. What are the types of comments in Java?
**Answer:**  
Java has three commonly used comment forms:

**1. Single-line comment**
```java
// This is a single-line comment
```

**2. Multi-line comment**
```java
/*
 This is a
 multi-line comment
*/
```

**3. Documentation comment**
```java
/**
 * This method displays a message.
 */
```

Documentation comments can be processed by the `javadoc` tool.

### Q55. Why are comments used?
**Answer:**  
Comments explain the purpose or behavior of code and make it easier for developers to understand and maintain.

### Q56. Are comments executed by the JVM?
**Answer:**  
No. Ordinary source-code comments do not become executable instructions in the compiled class file.

---

## 11. Keywords and Identifiers

### Q57. What is a keyword in Java?
**Answer:**  
A keyword is a reserved word with a predefined meaning in the Java language.

**Examples:**
```java
class
public
static
void
int
if
else
return
```

### Q58. Can we use a keyword as a variable name?
**Answer:**  
No. A Java keyword cannot be used as an ordinary identifier.

**Invalid example:**
```java
int class = 10;
```

### Q59. What is an identifier in Java?
**Answer:**  
An identifier is a name given to a program element, such as a variable, method, class, or interface.

**Examples:**
```java
int age = 21;

class Student {
}
```

Here, `age` and `Student` are identifiers.

### Q60. What are the rules for identifiers in Java?
**Answer:**

1. Identifiers can contain letters, digits, underscores (`_`), and dollar signs (`$`).
2. They cannot start with a digit.
3. They cannot be Java keywords.
4. Identifiers are case-sensitive.
5. Spaces are not allowed.

**Valid identifiers:**
```java
studentName
age
_marks
$amount
```

**Invalid identifiers:**
```java
2student
student name
class
```

### Q61. Is Java case-sensitive?
**Answer:**  
Yes. Java treats uppercase and lowercase letters as different characters.

**Example:**
```java
int age = 20;
int Age = 25;
```

Here, `age` and `Age` are two different variables.

---

## 12. Data Types in Java

### Q62. What is a data type?
**Answer:**  
A data type specifies the kind of value a variable can store and determines the operations that can be performed on that value.

### Q63. What are the types of data types in Java?
**Answer:**  
Java data types are commonly classified into two categories:

1. Primitive data types
2. Reference types (non-primitive types)

### Q64. What are primitive data types in Java?
**Answer:**  
Java has eight primitive data types.

| Data Type | Example | Purpose |
|---|---|---|
| `byte` | `byte a = 10;` | Small integer |
| `short` | `short a = 100;` | Short integer |
| `int` | `int age = 21;` | Integer |
| `long` | `long n = 1000L;` | Large integer |
| `float` | `float x = 10.5f;` | Single-precision decimal |
| `double` | `double x = 20.5;` | Double-precision decimal |
| `char` | `char grade = 'A';` | Single UTF-16 code unit |
| `boolean` | `boolean valid = true;` | Logical value |

### Q65. What is the difference between primitive and reference types?
**Answer:**

| Primitive Types | Reference Types |
|---|---|
| Represent primitive values. | Represent references to objects or arrays, or can have the value `null`. |
| Examples: `int`, `char`, `boolean`. | Examples: `String`, arrays, classes. |
| Have fixed primitive types and ranges, where applicable. | Their behavior depends on the referenced type. |

### Q66. What is a variable?
**Answer:**  
A variable is a named storage location used to hold a value during program execution.

**Example:**
```java
int age = 21;
```

### Q67. What is the difference between declaration and initialization?
**Answer:**

- **Declaration:** Introduces a variable and its type.
- **Initialization:** Gives the variable its initial value.

**Example:**
```java
int age;      // Declaration
age = 21;     // Initialization
```

Both can be done together:
```java
int age = 21;
```

### Q68. What is the default value of a variable in Java?
**Answer:**  
Instance variables and static variables receive default values. Local variables do not receive automatic default values and must be assigned before they are read.

Common default values for fields:

| Type | Default Value |
|---|---|
| Integer types | `0` |
| `float` | `0.0f` |
| `double` | `0.0d` |
| `char` | `'\u0000'` |
| `boolean` | `false` |
| Reference types | `null` |

### Q69. What is the size of an `int` in Java?
**Answer:**  
A Java `int` is a 32-bit signed integer. Its range is:

```text
-2,147,483,648 to 2,147,483,647
```

### Q70. What is the difference between `float` and `double`?
**Answer:**  
Both store floating-point values. `float` uses 32 bits, while `double` uses 64 bits and generally provides greater precision.

### Q71. What is the difference between `char` and `String`?
**Answer:**

- `char` is a primitive type that stores one UTF-16 code unit.
- `String` is a reference type used to represent a sequence of characters.

**Example:**
```java
char grade = 'A';
String name = "Prasanna";
```

### Q72. Is `String` a primitive data type?
**Answer:**  
No. `String` is a class in Java, not a primitive data type.

---

## 13. Basic Coding Interview Questions

### Q73. Write a Java program to print your name.
**Answer:**
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Prasanna Komati");
    }
}
```

### Q74. Write a Java program to print your name and age.
**Answer:**
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Name: Prasanna Komati");
        System.out.println("Age: 21");
    }
}
```

### Q75. Write a Java program to declare variables of different types.
**Answer:**
```java
public class Main {
    public static void main(String[] args) {
        int age = 21;
        double percentage = 85.5;
        char grade = 'A';
        boolean passed = true;
        String name = "Prasanna";

        System.out.println(name);
        System.out.println(age);
        System.out.println(percentage);
        System.out.println(grade);
        System.out.println(passed);
    }
}
```

### Q76. What is the output of this program?
**Question:**
```java
public class Main {
    public static void main(String[] args) {
        System.out.print("Java ");
        System.out.println("Developer");
        System.out.println("Welcome");
    }
}
```

**Answer:**
```text
Java Developer
Welcome
```

### Q77. Identify the error in this program.
**Question:**
```java
public class Main {
    public static void main(String[] args) {
        int age = 21
        System.out.println(age);
    }
}
```

**Answer:**  
The semicolon (`;`) is missing after `int age = 21`.

**Correct statement:**
```java
int age = 21;
```

---

## 14. Quick Revision Questions

Try answering these questions without looking at the answers.

1. What is Java?
2. Who developed Java?
3. What was the original name of Java?
4. What is platform independence?
5. What is the JVM?
6. What is the JDK?
7. What is the JRE?
8. What is bytecode?
9. What does the Java compiler do?
10. What is the difference between compilation and execution?
11. What is an IDE?
12. What is the purpose of the `main()` method?
13. What does `static` mean in the main method?
14. What is the difference between `print()` and `println()`?
15. What are comments?
16. What is a keyword?
17. What is an identifier?
18. Is Java case-sensitive?
19. How many primitive data types does Java have?
20. Is `String` a primitive data type?
21. What is the difference between `int` and `double`?
22. What is the difference between a local variable and an instance variable?
23. What is the purpose of `javac`?
24. Which command runs a compiled Java class?
25. Why is Java called platform-independent?

---

## 15. Important Commands

| Purpose | Command |
|---|---|
| Check Java version | `java -version` |
| Check compiler version | `javac -version` |
| Compile a program | `javac Main.java` |
| Run a program | `java Main` |
| Generate documentation | `javadoc Main.java` |

---

## Interview Preparation Tips

- Understand each concept instead of memorizing only the definition.
- Practice writing the first Java program without copying.
- Learn the difference between JDK, JRE, and JVM.
- Practice compiling and running Java programs using the command line.
- Explain concepts using simple real-world examples.
- Practice the quick revision questions before interviews.

**Next Topic:** Java Operators and Expressions.
