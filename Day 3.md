**Day 3 \- Java Masters Course (2 hours)**

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

