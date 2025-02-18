**Day 9 \- Java Masters Course (1 Hour)**

### **Challenge: Implementing Logical and Mathematical Methods**

**Today, I completed four coding challenges, implementing five Java methods. These challenges focused on logical operations, mathematical comparisons, and conditional statements, reinforcing key programming concepts.**

---

### **1\. `TeenNumberChecker` Class – Checking for Teen Numbers**

#### **Concepts Covered:**

**✅ Boolean logic (`true` / `false`)**  
**✅ Logical OR operator (`||`)**  
**✅ Method reuse (calling a method within another method)**

#### **Method Explanation:**

**The `hasTeen()` method checks if at least one of the three given numbers falls within the teen range (13-19). The method reuses `isTeen()`, which determines if a single number is a teen.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class TeenNumberChecker {`**

    **`public static boolean hasTeen(int num1, int num2, int num3) {`**

        **`return (isTeen(num1) || isTeen(num2) || isTeen(num3));`**

    **`}`**

    **`public static boolean isTeen(int num) {`**

        **`return num >= 13 && num <= 19;`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(hasTeen(12, 15, 22)); // Output: true`**

**`System.out.println(hasTeen(10, 25, 30)); // Output: false`**

---

### **2\. `EqualSumChecker` Class – Checking for Equal Sum**

#### **Concepts Covered:**

**✅ Arithmetic operations (`+`)**  
**✅ Boolean return values**  
**✅ Conditional logic**

#### **Method Explanation:**

**The `hasEqualSum()` method checks if the sum of two numbers equals the third number.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class EqualSumChecker {`**

    **`public static boolean hasEqualSum(int num1, int num2, int num3) {`**

        **`return num1 + num2 == num3;`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(hasEqualSum(5, 5, 10));  // Output: true`**

**`System.out.println(hasEqualSum(3, 6, 10));  // Output: false`**

---

### **3\. `DecimalComparator` Class – Comparing Decimal Values up to Three Places**

#### **Concepts Covered:**

**✅ Type casting (`double → long`)**  
**✅ Floating-point precision issues**  
**✅ Arithmetic operations (`* 1000`)**

#### **Method Explanation:**

**The `areEqualByThreeDecimalPlaces()` method compares two double values up to three decimal places by:**

1. **Multiplying each number by 1000 (shifting three decimal places).**  
2. **Casting the result to `long` to remove extra decimals.**  
3. **Comparing the integer values.**

#### **Implementation:**

**java**

**Kopiuj**

**`public class DecimalComparator {`**

    **`public static boolean areEqualByThreeDecimalPlaces(double num1, double num2) {`**

        **`long lng1 = (long) (num1 * 1000);`**

        **`long lng2 = (long) (num2 * 1000);`**

        **`return lng1 == lng2;`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(areEqualByThreeDecimalPlaces(3.176, 3.175)); // Output: false`**

**`System.out.println(areEqualByThreeDecimalPlaces(3.123, 3.123)); // Output: true`**

---

### **4\. `LeapYear` Class – Determining Leap Years**

#### **Concepts Covered:**

**✅ Nested conditional statements**  
**✅ Modulus operator (`%`)**  
**✅ Logical rules for leap years**

#### **Leap Year Rules:**

1. **A year is a leap year if it is divisible by 4\.**  
2. **Exception: If the year is divisible by 100, it is not a leap year unless…**  
3. **Exception to exception: If the year is divisible by 400, it is a leap year.**

#### **Method Implementation:**

**java**

**Kopiuj**

**`public class LeapYear {`**

    **`public static boolean isLeapYear(int year) {`**

        **`if (year < 1 || year > 9999) {`**

            **`return false;  // Invalid input range`**

        **`} else if (year % 4 == 0) {`**

            **`if (year % 100 == 0) {`**

                **`return year % 400 == 0; // Leap year only if divisible by 400`**

            **`} else {`**

                **`return true;`**

            **`}`**

        **`} else {`**

            **`return false;`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**java**

**Kopiuj**

**`System.out.println(isLeapYear(2020)); // Output: true`**

**`System.out.println(isLeapYear(1900)); // Output: false`**

**`System.out.println(isLeapYear(2000)); // Output: true`**

**`System.out.println(isLeapYear(2023)); // Output: false`**

---

### **Summary**

**Today’s challenges reinforced logical operations, arithmetic calculations, and method structuring in Java.**

* **`TeenNumberChecker` introduced method reuse and logical OR conditions.**  
* **`EqualSumChecker` demonstrated simple mathematical comparisons.**  
* **`DecimalComparator` tackled floating-point precision issues.**  
* **`LeapYear` involved nested conditionals and logical rules for real-world applications.**

**These challenges enhanced my problem-solving skills and deepened my understanding of boolean logic and mathematical operations in Java. 🚀**

