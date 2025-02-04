**Day 5 \- Java Masters Course (1 hour)**

### **Ternary Operator (`?:`)**

**The ternary operator is a shorthand for `if-else` statements and provides a concise way to make decisions in Java. It follows the syntax:**

**java**

**Kopiuj**

**`variable = (condition) ? value_if_true : value_if_false;`**

**Example:**

**java**

**Kopiuj**

**`int num = 10;`**

**`String result = (num % 2 == 0) ? "Even" : "Odd";`**

**`System.out.println(result); // Output: Even`**

**This replaces a longer `if-else` statement with a single line.**

### **Operator Precedence**

**Operator precedence determines the order in which operators are evaluated in an expression. Operators with higher precedence are executed first.**

**Operator Precedence Table (from highest to lowest):**

| Precedence | Operators | Description |
| ----- | ----- | ----- |
| **1** | **`()`** | **Parentheses (highest)** |
| **2** | **`++`, `--`** | **Increment, Decrement** |
| **3** | **`*`, `/`, `%`** | **Multiplication, Division, Modulus** |
| **4** | **`+`, `-`** | **Addition, Subtraction** |
| **5** | **`<`, `<=`, `>`, `>=`** | **Relational Operators** |
| **6** | **`==`, `!=`** | **Equality Operators** |
| **7** | **`&&`** | **Logical AND** |
| **8** | **\`** |  |
| **9** | **`?:`** | **Ternary Operator** |
| **10** | **`=`, `+=`, `-=`, `*=` etc.** | **Assignment Operators (lowest)** |

**Example:**

**java**

**Kopiuj**

**`int result = 10 + 2 * 5;  // Multiplication happens first`**

**`System.out.println(result); // Output: 20`**

**To change precedence, use parentheses:**

**java**

**Kopiuj**

**`int result = (10 + 2) * 5;  // Parentheses force addition first`**

**`System.out.println(result); // Output: 60`**

### **Keywords in Java**

**Keywords are reserved words in Java that have a predefined meaning in the language. These cannot be used as variable names, method names, or identifiers.**

**Common Java Keywords:**

* **Data Types: `int`, `double`, `boolean`, `char`, `byte`, `float`, `long`, `short`**  
* **Control Flow: `if`, `else`, `switch`, `case`, `default`, `for`, `while`, `do`, `break`, `continue`**  
* **Class and Object Related: `class`, `interface`, `extends`, `implements`, `this`, `super`, `new`**  
* **Modifiers: `public`, `private`, `protected`, `static`, `final`, `abstract`, `synchronized`**  
* **Other Important Keywords: `return`, `void`, `try`, `catch`, `finally`, `throw`, `throws`, `import`, `package`**

### **Expressions in Java**

**An expression is any combination of variables, values, and operators that evaluates to a single value.**

**Examples:**

**java**

**Kopiuj**

**`int sum = 10 + 5;  // Arithmetic expression`**

**`boolean isValid = (sum > 10); // Boolean expression`**

**`String message = "Hello " + "World"; // String concatenation expression`**

### 

### **Summary**

**Today, I learned about the ternary operator, operator precedence, Java keywords, and expressions. Understanding operator precedence helps avoid logical errors, while mastering keywords and expressions is essential for writing effective Java programs.**

