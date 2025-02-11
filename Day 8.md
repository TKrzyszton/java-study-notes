**Day 8 \- Java Masters Course (1 Hour)**

### **Challenge: Implementing Methods for Real-World Scenarios**

**Today, I worked on three method-based challenges, each reinforcing key Java concepts such as conditional statements, return types, method calls, and mathematical operations.**

---

### **1\. `BarkingDog` Class – Should Wake Up?**

#### **Concepts Covered:**

**✅ Boolean logic (`true` / `false`)**  
**✅ Conditional statements (`if-else`)**  
**✅ Validating input range**

#### **Method Explanation:**

**The `shouldWakeUp()` method determines whether a dog’s barking requires waking up based on the time of day.**

#### **Implementation:**

**`public class BarkingDog {`**

    **`public static boolean shouldWakeUp(boolean barking, int hourOfDay) {`**

        **`if (hourOfDay < 0 || hourOfDay > 23) {`**

            **`return false; // Invalid hour range`**

        **`} else if (!barking) {`**

            **`return false; // No barking, no need to wake up`**

        **`} else if (hourOfDay < 8 || hourOfDay > 22) {`**

            **`return true; // Barking during quiet hours (before 8 AM or after 10 PM)`**

        **`} else {`**

            **`return false; // Barking but not during quiet hours`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**`System.out.println(shouldWakeUp(true, 7));  // Output: true`**

**`System.out.println(shouldWakeUp(false, 3)); // Output: false`**

**`System.out.println(shouldWakeUp(true, 12)); // Output: false`**

**`System.out.println(shouldWakeUp(true, 23)); // Output: true`**

---

### **2\. `MegaBytesConverter` Class – Converting KB to MB**

#### **Concepts Covered:**

**✅ Mathematical operations (`division`, `modulus`)**  
**✅ Handling invalid inputs**  
**✅ String concatenation for readable output**

#### **Method Explanation:**

**The `printMegaBytesAndKiloBytes()` method converts a given number of kilobytes (`KB`) into megabytes (`MB`) and remaining kilobytes (`KB`).**

#### **Implementation:**

**`public class MegaBytesConverter {`**

    **`public static void printMegaBytesAndKiloBytes(int kiloBytes) {`**

        **`if (kiloBytes < 0) {`**

            **`System.out.print("Invalid Value"); // Handles negative input`**

        **`} else {`**

            **`System.out.print(kiloBytes + " KB = " + kiloBytes / 1024 + " MB and " + kiloBytes % 1024 + " KB");`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**`printMegaBytesAndKiloBytes(5000); // Output: 5000 KB = 4 MB and 872 KB`**

**`printMegaBytesAndKiloBytes(-1);   // Output: Invalid Value`**

---

### **3\. `SpeedConverter` Class – Kilometers per Hour to Miles per Hour**

#### **Concepts Covered:**

**✅ Method returning a value**  
**✅ Calling a method within another method**  
**✅ Rounding numbers (`Math.round()`)**

#### **Method Explanation:**

* **The `toMilesPerHour()` method converts kilometers per hour (km/h) to miles per hour (mi/h).**  
* **The `printConversion()` method calls `toMilesPerHour()` and prints a formatted conversion statement.**

#### **Implementation:**

**`public class SpeedConverter {`**

    **`public static long toMilesPerHour(double kilometersPerHour) {`**

        **`if (kilometersPerHour < 0) {`**

            **`return -1; // Invalid value case`**

        **`}`**

        **`return Math.round(kilometersPerHour / 1.609); // Conversion formula`**

    **`}`**

    **`public static void printConversion(double kilometersPerHour) {`**

        **`if (kilometersPerHour < 0) {`**

            **`System.out.print("Invalid Value");`**

        **`} else {`**

            **`System.out.print(kilometersPerHour + " km/h = " + toMilesPerHour(kilometersPerHour) + " mi/h");`**

        **`}`**

    **`}`**

**`}`**

#### **Example Usage:**

**`printConversion(100); // Output: 100 km/h = 62 mi/h`**

**`printConversion(-5);  // Output: Invalid Value`**

---

### **Summary**

**Today’s challenges reinforced conditional logic, mathematical operations, and method execution.**

* **The `BarkingDog` method introduced boolean logic and if statements.**  
* **The `MegaBytesConverter` method demonstrated integer division and modulus operations.**  
* **The `SpeedConverter` method used method calls within methods and applied rounding functions for precise calculations.**

**These challenges provided real-world problem-solving experience and strengthened my understanding of method structure and logic handling in Java. 🚀**

