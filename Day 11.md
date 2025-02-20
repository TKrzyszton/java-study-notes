**Day 11 \- Java Masters Course (1 Hour)**

### **Learning Objective: Implementing Methods with Conditional Logic and Mathematical Operations**

**Today, I implemented four Java methods to reinforce concepts such as boolean logic, conditional statements, arithmetic calculations, and method overloading.**

**The challenges covered:**

1. **Checking if a cat is playing (`isCatPlaying()`)**  
2. **Comparing three integers (`printEqual()`)**  
3. **Converting minutes into years and days (`printYearsAndDays()`)**  
4. **Calculating area for circles and rectangles (`area()`)**

---

### **1\. Checking if a Cat is Playing – `isCatPlaying()`**

#### **Concepts Covered:**

**✅ Boolean conditions (`true` / `false`)**  
**✅ Logical operators (`&&`, `||`)**  
**✅ Conditional statements (`if-else`)**

#### **Method Explanation:**

**The method determines if a cat is playing based on the temperature and whether it is summer.**

* **If not summer, the cat plays between 25°C and 35°C.**  
* **If summer, the cat plays between 25°C and 45°C.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class PlayingCat {`**

    **`public static boolean isCatPlaying(boolean summer, int temperature) {`**

        **`if (!summer && temperature >= 25 && temperature <= 35) {`**

            **`return true;`**

        **`} else if (summer && temperature >= 25 && temperature <= 45) {`**

            **`return true;`**

        **`} else {`**

            **`return false;`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(isCatPlaying(true, 40));  // Output: true`**

**`System.out.println(isCatPlaying(false, 36)); // Output: false`**

**`System.out.println(isCatPlaying(true, 20));  // Output: false`**

**Key Takeaways:**

* **The logical conditions determine the temperature range based on the summer flag.**  
* **The use of boolean expressions simplifies decision-making.**

---

### **2\. Comparing Three Integers – `printEqual()`**

#### **Concepts Covered:**

**✅ Integer comparison (`==`, `!=`)**  
**✅ Conditional statements (`if-else`)**  
**✅ Handling invalid input**

#### **Method Explanation:**

**The method compares three numbers and prints whether they are:**

1. **All equal**  
2. **All different**  
3. **Neither all equal nor all different**  
4. **Invalid (if any number is negative)**

#### **Implementation:**

**java**

**Kopiuj**

**`public class IntEqualityPrinter {`**

    **`public static void printEqual(int num1, int num2, int num3) {`**

        **`if (num1 < 0 || num2 < 0 || num3 < 0) {`**

            **`System.out.println("Invalid Value");`**

        **`} else if (num1 == num2 && num2 == num3) {`**

            **`System.out.println("All numbers are equal");`**

        **`} else if (num1 != num2 && num2 != num3 && num1 != num3) {`**

            **`System.out.println("All numbers are different");`**

        **`} else {`**

            **`System.out.println("Neither all are equal or different");`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`printEqual(1, 1, 1);  // Output: All numbers are equal`**

**`printEqual(1, 2, 3);  // Output: All numbers are different`**

**`printEqual(1, 1, 2);  // Output: Neither all are equal or different`**

**`printEqual(-1, 2, 3); // Output: Invalid Value`**

**Key Takeaways:**

* **The method validates inputs before processing.**  
* **Logical conditions determine equality or inequality.**

---

### **3\. Converting Minutes to Years and Days – `printYearsAndDays()`**

#### **Concepts Covered:**

**✅ Arithmetic calculations (`/`, `%`)**  
**✅ Integer division and modulus**  
**✅ Handling large numbers (`long` type)**

#### **Method Explanation:**

**The method converts minutes into years and days, using the following calculations:**

* **1 hour \= 60 minutes**  
* **1 day \= 24 hours**  
* **1 year \= 365 days**

#### **Implementation:**

**java**

**Kopiuj**

**`public class MinutesToYearsDaysCalculator {`**

    **`public static void printYearsAndDays(long minutes) {`**

        **`if (minutes < 0) {`**

            **`System.out.println("Invalid Value");`**

        **`} else {`**

            **`long hours = minutes / 60;`**

            **`long days = hours / 24;`**

            **`long years = days / 365;`**

            **`long remainingDays = days % 365;`**

            **`System.out.println(minutes + " min = " + years + " y and " + remainingDays + " d");`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`printYearsAndDays(525600); // Output: 525600 min = 1 y and 0 d`**

**`printYearsAndDays(1051200); // Output: 1051200 min = 2 y and 0 d`**

**`printYearsAndDays(-500); // Output: Invalid Value`**

**Key Takeaways:**

* **Integer division is used to calculate years and days.**  
* **The method ensures negative values are handled properly.**

---

### **4\. Calculating Area – `area()` (Method Overloading)**

#### **Concepts Covered:**

**✅ Method overloading**  
**✅ Arithmetic calculations (`Math.PI`, `*`)**  
**✅ Input validation**

#### **Method Explanation:**

**The overloaded `area()` method calculates:**

* **Circle area if given radius.**  
* **Rectangle area if given two dimensions (`width × height`).**  
* **Returns \-1.0 for invalid inputs (negative values).**

#### **Implementation:**

**java**

**Kopiuj**

**`public class AreaCalculator {`**

    **`public static double area(double radius) {`**

        **`if (radius < 0) {`**

            **`return -1.0;`**

        **`}`**

        **`return Math.PI * (radius * radius);`**

    **`}`**

    **`public static double area(double x, double y) {`**

        **`if (x < 0 || y < 0) {`**

            **`return -1.0;`**

        **`}`**

        **`return x * y;`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(area(5.0));   // Output: 78.5398 (Circle with radius 5)`**

**`System.out.println(area(4.0, 5.0)); // Output: 20.0 (Rectangle 4x5)`**

**`System.out.println(area(-3.0));  // Output: -1.0 (Invalid input)`**

**`System.out.println(area(2.5, -1.0)); // Output: -1.0 (Invalid input)`**

**Key Takeaways:**

* **Overloaded methods handle different types of inputs.**  
* **Validation checks prevent negative values.**  
* **`Math.PI` is used for accurate circle area calculations.**

---

### **Summary**

**Today’s challenges reinforced boolean logic, conditional statements, integer division, and method overloading:**

* **`isCatPlaying()`: Used boolean logic to determine if a cat plays based on temperature and season.**  
* **`printEqual()`: Compared three integers and categorized them.**  
* **`printYearsAndDays()`: Converted minutes to years and days with integer division.**  
* **`area()`: Overloaded methods for circle and rectangle area calculations, handling invalid inputs.**

**These exercises strengthened my understanding of decision-making in Java and improved my problem-solving skills. 🚀**

