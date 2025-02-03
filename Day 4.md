**Day 4 \- Java Masters Course (1 hour)**

**Today, I expanded my knowledge of Java data types, focusing on floating-point types (`double`, `float`), character (`char`), and boolean (`boolean`). I also explored operators, expressions, and Java statements.**

### **Floating-Point Data Types (`double` vs. `float`)**

**I learned about the two primary floating-point data types in Java:**

* **`double` (64-bit, more precise, commonly used in Java)**  
* **`float` (32-bit, less precise, requires an `f` suffix for literals)**

**Example:**

**java**

**Kopiuj**

**`double myDouble = 5.99;`**

**`float myFloat = 5.99f;`**

**The `double` type is preferred for most mathematical computations due to its higher precision.**

### **Character (`char`) and Boolean (`boolean`)**

* **The `char` type represents a single character and is enclosed in single quotes (`'A'`).**  
* **The `boolean` type holds only two possible values: `true` or `false`.**

**Example:**

**java**

**Kopiuj**

**`char myChar = 'A';`**

**`boolean isJavaFun = true;`**

### **Unicode and Decimal Values of Symbols**

**Java uses Unicode to represent characters, allowing for a vast range of symbols. Each character has a corresponding decimal value.**

**Examples:**

**java**

**Kopiuj**

**`char mySymbol = '\u0041'; // Unicode for 'A'`**

**`System.out.println(mySymbol); // Output: A`**

**`char mySymbol2 = 36; // Decimal for '$'`**

**`System.out.println(mySymbol2); // Output: $`**

### **Primitive Data Types Recap**

**At this point, I have covered all eight primitive data types in Java:**

* **Integer types: `byte`, `short`, `int`, `long`**  
* **Floating-point types: `float`, `double`**  
* **Character type: `char`**  
* **Boolean type: `boolean`**

### **String Data Type**

**Although `String` is not a primitive type, it is a fundamental part of Java, used to store text sequences. Strings are enclosed in double quotes (`" "`) and provide powerful built-in methods.**

**Example:**

**java**

**Kopiuj**

**`String myString = "Hello, Java!";`**

**`System.out.println(myString);`**

### **Operators, Operands, and Expressions**

**I explored basic mathematical operators:**

* **Addition (`+`)**  
* **Subtraction (`-`)**  
* **Multiplication (`*`)**  
* **Division (`/`)**  
* **Modulus (`%`) (returns the remainder of a division)**

**Example:**

**java**

**Kopiuj**

**`int sum = 10 + 5;  // 15`**

**`int remainder = 10 % 3; // 1`**

### **Java Statements and Code Blocks `{}`**

**Java statements are individual instructions executed by the program. Multiple statements can be grouped within `{}` to create a block of code, often used in loops and conditionals.**

**Example:**

**java**

**Kopiuj**

**`if (true) {`**

    **`System.out.println("This is inside a block.");`**

**`}`**

### **Abbreviating Operators (Shorthand Notation)**

**Java allows shorthand operators to simplify expressions:**

* **`+=` (addition assignment)**  
* **`-=` (subtraction assignment)**  
* **`*=` (multiplication assignment)**  
* **`/=` (division assignment)**

**Example:**

**java**

**Kopiuj**

**`int x = 10;`**

**`x += 5;  // Equivalent to: x = x + 5;`**

**`System.out.println(x); // Output: 15`**

### **Summary**

**Today, I reinforced my understanding of primitive data types, explored Unicode representations, and practiced mathematical operations in Java. I also learned how to structure statements using `{}` and efficiently update variables using shorthand operators.**

**4o**

##### **Powiedziałeś(-aś):**

**Make a professional note: InteliJJ \- installing, differences betwen jshell and ide InteliJJ \- connecting intelijj with JDK, change your theme to dracula, some things in settings InteliJ \- creating new project with upper camel case, ''Hello World' InteliJJ \- creating first java class FirstClass and by intelijj shortcut psvm first statement (?) which prints Hello World by System.out.print function keywords public as access modifier class \- defining the class what is method main method static, void \- are gonna be discucces later system.out.print with ln suffix to render in a new line if statements assigning a value true/false to boolean variable building if statement and printing if its true building if statements with code blocks logical operators like \==, \!=, \>,\<,\>=, \<= logical AND operator example logical OR operator example Assignment operator vs equals to operator**

###### **ChatGPT powiedział:**

**ChatGPT**

**Day 4 \- Java Masters Course (1 Hour)**

### **Installing IntelliJ IDEA and Differences Between JShell and an IDE**

**Today, I installed IntelliJ IDEA, a professional Integrated Development Environment (IDE) for Java development. I explored its differences from `jshell`:**

* **JShell is an interactive REPL (Read-Eval-Print Loop) tool for testing small Java snippets.**  
* **IntelliJ IDEA is a full-featured IDE that provides project management, debugging, code assistance, and more.**

### **Setting Up IntelliJ IDEA**

* **Connected IntelliJ with JDK (Java Development Kit).**  
* **Customized the IDE by switching the theme to Dracula for better visibility.**  
* **Explored key settings to improve the development experience.**

### **Creating a New Java Project**

* **Followed UpperCamelCase naming convention when creating a new Java project.**  
* **Wrote a "Hello World" program using IntelliJ IDEA.**

### **Creating and Running the First Java Class**

* **Created the first Java class named `FirstClass` following Java's naming conventions.**  
* **Used IntelliJ's shortcut (`psvm`) to generate the `main` method quickly.**

**Wrote the first statement:**  
**java**  
**Kopiuj**  
**`System.out.println("Hello, World!");`**

*   
  * **`System.out.print` prints text, and adding `ln` (`println`) moves the output to a new line.**

### **Understanding Key Java Concepts**

#### **Access Modifier \- `public`**

* **`public` is an access modifier that allows a method or class to be accessible from anywhere in the program.**

#### **Class Definition**

* **A `class` is a blueprint for objects, defining their behavior and properties.**

#### **Methods in Java**

* **A method is a block of code designed to perform a specific task.**  
* **The `main` method (`public static void main(String[] args)`) serves as the entry point of a Java program.**

#### **Introduction to `static` and `void`**

* **These keywords will be discussed in detail later, but for now:**  
  * **`static` allows a method to be called without creating an object.**  
  * **`void` indicates that a method does not return a value.**

### **Conditional Statements: `if` Statements**

#### **Assigning a Boolean Value**

**A `boolean` variable can hold either `true` or `false`.**  
**java**  
**Kopiuj**  
**`boolean isJavaFun = true;`**

* 

#### **Building an `if` Statement**

**An `if` statement executes a block of code only if a condition is true.**  
**java**  
**Kopiuj**  
**`if (isJavaFun) {`**

    **`System.out.println("Java is fun!");`**

**`}`**

* 

#### **Using Code Blocks in `if` Statements**

* **`{}` defines a block of code to execute when the condition is met.**

### **Logical and Comparison Operators**

#### **Comparison Operators (`==`, `!=`, `>`, `<`, `>=`, `<=`)**

**Used to compare values:**  
**java**  
**Kopiuj**  
**`int a = 10, b = 20;`**

**`System.out.println(a < b);  // true`**

**`System.out.println(a == b); // false`**

* 

#### **Logical AND (`&&`)**

**Returns `true` only if both conditions are met:**  
**java**  
**Kopiuj**  
**`if (a > 5 && b > 15) {`**

    **`System.out.println("Both conditions are true.");`**

**`}`**

* 

#### **Logical OR (`||`)**

**Returns `true` if at least one condition is met:**  
**java**  
**Kopiuj**  
**`if (a > 15 || b > 15) {`**

    **`System.out.println("At least one condition is true.");`**

**`}`**

* 

### **Assignment Operator (`=`) vs. Equals (`==`)**

* **`=` is the assignment operator (used to assign a value to a variable).**  
* **`==` is the equality operator (used to compare two values).**

**Example:**

**java**

**Kopiuj**

**`int x = 5;    // Assigning value`**

**`boolean result = (x == 5);  // Comparing values`**

### **Summary**

**Today's session focused on setting up IntelliJ IDEA, writing the first Java class, and understanding key programming concepts such as conditional statements, logical operators, and the difference between assignment and equality operators.**

