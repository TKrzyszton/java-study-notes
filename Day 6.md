

**Day 6 \- Java Masters Course (1 Hour)**

### **1\. Statements, Whitespace, and Indentation**

#### **Statements vs. Expressions**

**Expression: A combination of variables, values, and operators that evaluates to a single value.**  
**Example:**  
**java**

**`int result = 10 + 5;  // Expression (evaluates to 15)`**

* 

**Statement: A complete command that performs an action and ends with a semicolon (`;`).**  
**Example:**

**`System.out.println("Hello, Java!");  // Statement`**

* 

#### **Whitespace in Java**

**Whitespace in Java improves code readability but has no effect on program execution.**

* **Vertical Whitespace: Used to separate sections of code (e.g., between methods or logical blocks).**  
* **Horizontal Whitespace: Used to improve readability within lines (e.g., around operators and keywords).**

**Example of Proper Whitespace Usage:**

**`int a = 5;  // Space before and after '='`**  
**`int b = 10;`**

**`if (a < b) {`**    
    **`System.out.println("a is smaller than b");`**    
**`}`**

#### **Indentation in Java**

**Indentation is used to visually structure code, making it easier to understand. Java follows a standard convention of 4 spaces per indentation level.**

**Example:**

**`if (true) {`**  
    **`System.out.println("This is inside an indented block.");`**  
**`}`**

---

### **2\. Code Blocks and If/Then/Else Control Statements**

**A code block in Java is enclosed within `{}` and groups multiple statements together.**

#### **Basic `if-else` Statement**

**`int age = 18;`**  
**`if (age >= 18) {`**  
    **`System.out.println("You are an adult.");`**  
**`} else {`**  
    **`System.out.println("You are a minor.");`**  
**`}`**

#### **`if-else if-else` Statement**

**Allows multiple conditions to be checked in sequence.**

**`int score = 85;`**  
**`if (score >= 90) {`**  
    **`System.out.println("Grade: A");`**  
**`} else if (score >= 80) {`**  
    **`System.out.println("Grade: B");`**  
**`} else if (score >= 70) {`**  
    **`System.out.println("Grade: C");`**  
**`} else {`**  
    **`System.out.println("Grade: F");`**  
**`}`**

---

### **3\. Methods in Java**

#### **Definition of a Method**

**A method is a reusable block of code that performs a specific task.**

#### **Method Structure**

**A method consists of:**

1. **Access Modifier (`public`, `private`, etc.)**  
2. **Return Type (`void` for no return, or a data type like `int`)**  
3. **Method Name**  
4. **Parameters (optional, enclosed in parentheses `()` )**  
5. **Method Body (enclosed in `{}` )**

#### **Example of a Simple Method**

**`public static void greet() {`**  
    **`System.out.println("Hello, Java!");`**  
**`}`**

#### **Executing a Method as a Statement**

**A method is executed (called) using its name followed by parentheses `()`.**

**`greet(); // Method call`**

#### **Method with Parameters**

**Methods can accept parameters to work with dynamic values.**

**`public static void greetUser(String name) {`**  
    **`System.out.println("Hello, " + name + "!");`**  
**`}`**

#### **Method with Parameters and Return Type**

**A method can return a value using the `return` keyword.**

**`public static int add(int a, int b) {`**  
    **`return a + b;`**  
**`}`**

**Calling the Method and Storing the Result:**

**`int sum = add(5, 10);`**  
**`System.out.println(sum); // Output: 15`**

---

### **Summary**

**Today, I covered statements vs. expressions, whitespace conventions, and proper indentation for clean code formatting. I also explored if/else control statements for decision-making and methods in Java, including defining, calling, and using parameters with return types.**

