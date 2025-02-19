**Day 10 \- Java Masters Course (1 Hour)**

### **Learning Objective: Method Overloading in Java**

**Today, I focused on method overloading, which allows multiple methods with the same name but different parameter lists. Overloading improves code reusability and makes methods more flexible.**

**I implemented two challenges to reinforce this concept:**

1. **Time Conversion (`getDurationString()`)**  
2. **Unit Conversion (`convertToCentimeters()`)**

---

### **1\. Time Conversion: `getDurationString()` Method Overloading**

#### **Concepts Covered:**

**✅ Method overloading (same method name, different parameters)**  
**✅ Integer division and modulus (`/` and `%`)**  
**✅ Nested method calls**

#### **Method Explanation:**

**The `getDurationString()` method converts seconds into a formatted duration (`hours, minutes, seconds`).**

* **One version takes seconds as input and calculates minutes.**  
* **Another version takes both seconds and minutes and calculates hours.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class Main {`**

    **`public static void main(String[] args) {`**

        **`System.out.println(getDurationString(3945)); // Test case`**

    **`}`**

    **`public static String getDurationString(int seconds) {`**

        **`if (seconds <= 0) {`**

            **`return "Invalid value. " + seconds + " must be a positive integer";`**

        **`}`**

        **`return getDurationString(seconds % 60, seconds / 60);`**

    **`}`**

    **`public static String getDurationString(int seconds, int minutes) {`**

        **`if (minutes < 0) {`**

            **`return "Invalid value";`**

        **`}`**

        **`int hours = minutes / 60;`**

        **`int remainingMinutes = minutes % 60;`**

        **`return hours + "h " + remainingMinutes + "m " + seconds + "s";`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(getDurationString(3945)); // Output: 1h 5m 45s`**

**`System.out.println(getDurationString(120));  // Output: 0h 2m 0s`**

**`System.out.println(getDurationString(-5));   // Output: Invalid value. -5 must be a positive integer`**

**Key Takeaways:**

* **The first method calls the second method, demonstrating method reuse.**  
* **Overloading helps simplify the logic, making it easier to handle different cases.**

---

### **2\. Unit Conversion: `convertToCentimeters()` Method Overloading**

#### **Concepts Covered:**

**✅ Method overloading**  
**✅ Mathematical operations (conversion factors)**  
**✅ Calling an overloaded method from another method**

#### **Method Explanation:**

**The `convertToCentimeters()` method converts height measurements from inches and feet to centimeters.**

* **One version converts inches to centimeters.**  
* **Another version converts feet and inches to inches, then calls the first method.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class Main {`**

    **`public static void main(String[] args) {`**

        **`System.out.println(convertToCentimeters(58));`**

        **`System.out.println(convertToCentimeters(88));`**

        **`System.out.println(convertToCentimeters(5, 8));`**

        **`System.out.println(convertToCentimeters(6, 3));`**

    **`}`**

    **`public static double convertToCentimeters(int heightInInches) {`**

        **`return heightInInches * 2.54;`**

    **`}`**

    **`public static double convertToCentimeters(int feet, int inches) {`**

        **`return convertToCentimeters((feet * 12) + inches);`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(convertToCentimeters(5, 8));  // Output: 172.72 cm (5 feet 8 inches)`**

**`System.out.println(convertToCentimeters(6, 3));  // Output: 190.5 cm (6 feet 3 inches)`**

**`System.out.println(convertToCentimeters(58));    // Output: 147.32 cm`**

**Key Takeaways:**

* **Method reuse: The second method calls the first method, improving efficiency.**  
* **Overloading makes the method flexible, allowing both inches-only and feet/inches conversions.**

---

### **Summary**

**Today’s challenges reinforced method overloading and method reuse in Java.**

* **The `getDurationString()` method demonstrated time formatting with multiple parameter variations.**  
* **The `convertToCentimeters()` method handled unit conversion, utilizing method calls within methods.**

**By overloading methods, I reduced code duplication and improved readability, making the code more efficient and reusable. 🚀**

