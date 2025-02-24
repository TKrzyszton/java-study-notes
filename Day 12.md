**Day 12 \- Java Masters Course (1 Hour)**

### **Learning Objective: Switch Statements (Traditional & Enhanced)**

**Today, I explored switch statements in Java, including traditional switch cases and the enhanced switch expression (Java 14+). I implemented four methods that apply switch logic to solve different challenges.**

**The challenges covered:**

1. **NATO Phonetic Alphabet (`NATO()`)**  
2. **Printing the Day of the Week (`printDayOfTheWeek()`)**  
3. **Determining the Number of Days in a Month (`getDaysInMonth()`)**  
4. **Printing a Number in Words (`printNumberInWord()`)**

---

## **1\. NATO Phonetic Alphabet – `NATO()`**

### **Concepts Covered:**

**✅ Traditional switch statement**  
**✅ Character matching (`char`)**  
**✅ Using `default` for unmatched cases**

### **Method Explanation:**

**The `NATO()` method converts a character (A–E) into its corresponding NATO phonetic alphabet representation.**

* **If the input matches one of the defined cases, it prints the associated word.**  
* **If the character is not found, it prints `"Not found"`.**

### **Implementation:**

**java**  
**KopiujEdytuj**  
**`public static void NATO(char value) {`**  
    **`switch (value) {`**  
        **`case 'A':`**  
            **`System.out.println("Able");`**  
            **`break;`**  
        **`case 'B':`**  
            **`System.out.println("Baker");`**  
            **`break;`**  
        **`case 'C':`**  
            **`System.out.println("Charlie");`**  
            **`break;`**  
        **`case 'D':`**  
            **`System.out.println("Dog");`**  
            **`break;`**  
        **`case 'E':`**  
            **`System.out.println("Easy");`**  
            **`break;`**  
        **`default:`**  
            **`System.out.println("Not found");`**  
    **`}`**  
**`}`**

### **Example Usage:**

**java**  
**KopiujEdytuj**  
**`NATO('A'); // Output: Able`**  
**`NATO('C'); // Output: Charlie`**  
**`NATO('X'); // Output: Not found`**

### **Key Takeaways:**

* **Each `case` represents a character, followed by a break statement to prevent fall-through.**  
* **The `default` case handles all unexpected inputs.**

---

## **2\. Printing the Day of the Week – `printDayOfTheWeek()`**

### **Concepts Covered:**

**✅ Enhanced switch expressions (Java 14+)**  
**✅ Returning a value from a switch**  
**✅ Improved readability with `->` syntax**

### **Method Explanation:**

**The `printDayOfTheWeek()` method converts an integer (0–6) into the corresponding weekday name using an enhanced switch expression.**

### **Implementation:**

**java**  
**KopiujEdytuj**  
**`public static void printDayOfTheWeek(int number) {`**  
    **`String dayOfWeek = switch (number) {`**  
        **`case 0 -> "Monday";`**  
        **`case 1 -> "Tuesday";`**  
        **`case 2 -> "Wednesday";`**  
        **`case 3 -> "Thursday";`**  
        **`case 4 -> "Friday";`**  
        **`case 5 -> "Saturday";`**  
        **`case 6 -> "Sunday";`**  
        **`default -> "Invalid Day";`**  
    **`};`**  
    **`System.out.println(dayOfWeek);`**  
**`}`**

### **Example Usage:**

**java**  
**KopiujEdytuj**  
**`printDayOfTheWeek(3); // Output: Thursday`**  
**`printDayOfTheWeek(6); // Output: Sunday`**  
**`printDayOfTheWeek(10); // Output: Invalid Day`**

### **Key Takeaways:**

* **Enhanced switch expressions make the code more concise and readable.**  
* **Arrow syntax (`->`) eliminates the need for break statements.**

---

## **3\. Determining the Number of Days in a Month – `getDaysInMonth()`**

### **Concepts Covered:**

**✅ Nested switch statements**  
**✅ Calling another method inside a switch (`isLeapYear()`)**  
**✅ Validating inputs before processing**

### **Method Explanation:**

**The `getDaysInMonth()` method:**

* **Takes month and year as inputs.**  
* **Uses switch cases to return the correct number of days for the month.**  
* **February (Month 2\) is checked for leap years using the `isLeapYear()` method.**  
* **If inputs are invalid, it returns `-1`.**

### **Implementation:**

**java**  
**KopiujEdytuj**  
**`public class NumberOfDaysInMonth {`**  
    **`public static boolean isLeapYear(int year) {`**  
        **`if (year < 1 || year >= 9999) {`**  
            **`return false;`**  
        **`} else if (year % 4 == 0) {`**  
            **`if (year % 100 == 0) {`**  
                **`return year % 400 == 0;`**  
            **`} else {`**  
                **`return true;`**  
            **`}`**  
        **`} else {`**  
            **`return false;`**  
        **`}`**  
    **`}`**

    **`public static int getDaysInMonth(int month, int year) {`**  
        **`if (year < 1 || year >= 9999) {`**  
            **`return -1;`**  
        **`}`**

        **`switch (month) {`**  
            **`case 1, 3, 5, 7, 8, 10, 12:`**  
                **`return 31;`**  
            **`case 4, 6, 9, 11:`**  
                **`return 30;`**  
            **`case 2:`**  
                **`return isLeapYear(year) ? 29 : 28;`**  
            **`default:`**  
                **`return -1;`**  
        **`}`**  
    **`}`**  
**`}`**

### **Example Usage:**

**java**  
**KopiujEdytuj**  
**`System.out.println(getDaysInMonth(2, 2024)); // Output: 29 (Leap Year)`**  
**`System.out.println(getDaysInMonth(4, 2023)); // Output: 30`**  
**`System.out.println(getDaysInMonth(13, 2023)); // Output: -1 (Invalid month)`**

### **Key Takeaways:**

* **Leap year validation is done using `isLeapYear()`.**  
* **Comma-separated case values (`case 1, 3, 5...:`) improve readability.**  
* **The method ensures input validation before execution.**

---

## **4\. Printing a Number in Words – `printNumberInWord()`**

### **Concepts Covered:**

**✅ Using `switch` to map numbers to words**  
**✅ Handling numbers outside the defined range (`default`)**

### **Method Explanation:**

**The `printNumberInWord()` method converts an integer (0–9) into its word representation.**

* **If the number is outside this range, it prints `"OTHER"`.**

### **Implementation:**

**java**  
**KopiujEdytuj**  
**`public class NumberInWord {`**  
    **`public static void printNumberInWord(int number) {`**  
        **`switch (number) {`**  
            **`case 0 -> System.out.println("ZERO");`**  
            **`case 1 -> System.out.println("ONE");`**  
            **`case 2 -> System.out.println("TWO");`**  
            **`case 3 -> System.out.println("THREE");`**  
            **`case 4 -> System.out.println("FOUR");`**  
            **`case 5 -> System.out.println("FIVE");`**  
            **`case 6 -> System.out.println("SIX");`**  
            **`case 7 -> System.out.println("SEVEN");`**  
            **`case 8 -> System.out.println("EIGHT");`**  
            **`case 9 -> System.out.println("NINE");`**  
            **`default -> System.out.println("OTHER");`**  
        **`}`**  
    **`}`**  
**`}`**

### **Example Usage:**

**java**  
**KopiujEdytuj**  
**`printNumberInWord(5); // Output: FIVE`**  
**`printNumberInWord(9); // Output: NINE`**  
**`printNumberInWord(15); // Output: OTHER`**

### **Key Takeaways:**

* **Enhanced switch syntax simplifies the code.**  
* **Using `default` ensures all unexpected inputs are handled.**

---

## **Summary**

**Today’s challenges reinforced traditional and enhanced switch statements, improving my ability to:**

* **Use `switch` for efficient decision-making.**  
* **Leverage enhanced switch expressions (`->`) for cleaner code.**  
* **Validate and process inputs efficiently.**

**These exercises provided real-world examples where `switch` statements simplify logic compared to multiple `if-else` conditions. 🚀**

