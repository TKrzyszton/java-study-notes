**Day 13 \- Java Masters Course (1 Hour)**

### **Learning Objective: For Loops in Java**

**Today, I focused on for loops and their practical applications in Java. I implemented several challenges using loop structures, covering:**

1. **Summing numbers divisible by 3 and 5 (`sumChallenge()`)**  
2. **Basic loop iteration (`printCounter()`)**  
3. **Finding prime numbers (`isPrime()`)**  
4. **Calculating interest rates (`calculateInterest()`)**

**These exercises helped reinforce loop logic, conditional checks, and method efficiency.**

---

## **1\. Summing Numbers Divisible by 3 and 5 – `sumChallenge()`**

### **Concepts Covered:**

**✅ Looping through a range (1–1000)**  
**✅ Using conditional checks (`% 3 && % 5`)**  
**✅ Maintaining a counter for matches**

### **Method Explanation:**

**The `sumChallenge()` method loops from `1` to `1000` and sums all numbers divisible by both 3 and 5\. It also counts how many numbers matched the condition.**

### **Implementation:**

**`public static void sumChallenge() {`**

    **`int sum3and5 = 0;`**

    **`int countOfMatches = 0;`**

    **`for (int i = 1; i <= 1000; i++) {`**

        **`if (i % 3 == 0 && i % 5 == 0) {`**

            **`sum3and5 += i;`**

            **`countOfMatches++;`**

        **`}`**

    **`}`**

    **`System.out.println("Sum = " + sum3and5 + ", Count = " + countOfMatches);`**

**`}`**

### **Example Usage:**

**`sumChallenge();`** 

**`// Output: Sum = 234168, Count = 67`**

### **Key Takeaways:**

* **Using a single loop to accumulate both sum and count improves efficiency.**  
* **Using `countOfMatches++` eliminates the need for an additional `if` block.**

---

## **2\. Basic Loop Iteration – `printCounter()`**

### **Concepts Covered:**

**✅ Simple `for` loop execution**  
**✅ Loop increment (`counter++`)**

### **Method Explanation:**

**The `printCounter()` method prints numbers from 1 to 5 using a simple `for` loop.**

### **Implementation:**

**`public static void printCounter() {`**

    **`for (int counter = 1; counter <= 5; counter++) {`**

        **`System.out.println(counter);`**

    **`}`**

**`}`**

### **Example Usage:**

**`printCounter();`**

**`// Output:`**

**`// 1`**

**`// 2`**

**`// 3`**

**`// 4`**

**`// 5`**

### **Key Takeaways:**

* **For loops are ideal for simple, sequential iterations.**

---

## **3\. Finding Prime Numbers – `isPrime()`**

### **Concepts Covered:**

**✅ Checking for prime numbers using a loop**  
**✅ Breaking execution after finding a set count**

### **Method Explanation:**

* **The `isPrime()` method determines if a number is prime.**  
* **The loop runs from `2` to `n-1`, checking if `n` is divisible by any number.**  
* **The `printPrimeNumbers()` method prints the first 3 prime numbers found between `1–1000`.**

### **Implementation:**

**`public static boolean isPrime(int number) {`**

    **`if (number <= 2) return number == 2;`**

    **`for (int divisor = 2; divisor < number; divisor++) {`**

        **`if (number % divisor == 0) return false;`**

    **`}`**

    **`return true;`**

**`}`**

**`public static void printPrimeNumbers() {`**

    **`int counter = 0;`**

    **`for (int number = 1; number <= 1000; number++) {`**

        **`if (isPrime(number)) {`**

            **`System.out.println(number + " is a prime number");`**

            **`counter++;`**

            **`if (counter == 3) break; // Stop after 3 prime numbers`**

        **`}`**

    **`}`**

**`}`**

### **Example Usage:**

**`printPrimeNumbers();`** 

**`// Output:`**

**`// 2 is a prime number`**

**`// 3 is a prime number`**

**`// 5 is a prime number`**

### **Key Takeaways:**

* **Breaking out of the loop (`break`) when the count reaches 3 avoids unnecessary iterations.**  
* **Using `isPrime()` as a helper method makes the code modular and reusable.**

---

## **4\. Interest Rate Calculation – `calculateInterest()`**

### **Concepts Covered:**

**✅ Incrementing loop values (`rate += 0.25`)**  
**✅ Breaking loop execution based on a condition (`if (interestAmount > 8.5) break;`)**

### **Method Explanation:**

* **`calculateInterest()` computes interest on a principal amount using a given rate.**  
* **`printInterestRates()` loops through interest rates from `7.5%` to `10%`, stopping when interest exceeds `8.5`.**

### **Implementation:**

**`public static double calculateInterest(double amount, double interestRate) {`**

    **`return amount * (interestRate / 100);`**

**`}`**

**`public static void printInterestRates() {`**

    **`for (double rate = 7.5; rate <= 10; rate += 0.25) {`**

        **`double interestAmount = calculateInterest(100.00, rate);`**

        **`if (interestAmount > 8.5) break;`**

        **`System.out.println("Rate: " + rate + "% - Interest: " + interestAmount);`**

    **`}`**

**`}`**

### **Example Usage:**

**`printInterestRates();`**

**`// Output:`**

**`// Rate: 7.5% - Interest: 7.5`**

**`// Rate: 7.75% - Interest: 7.75`**

**`// Rate: 8.0% - Interest: 8.0`**

**`// Rate: 8.25% - Interest: 8.25`**

### **Key Takeaways:**

* **Using increment steps (`+= 0.25`) allows finer control over loop iteration.**  
* **Breaking execution when a threshold is met (`> 8.5`) optimizes performance.**

---

## **Final Cleaned-Up Version of Code**

**`public class Main {`**

    **`public static void main(String[] args) {`**

        **`sumChallenge();`**

        **`printCounter();`**

        **`printPrimeNumbers();`**

        **`printInterestRates();`**

    **`}`**

    **`public static void sumChallenge() {`**

        **`int sum3and5 = 0, countOfMatches = 0;`**

        **`for (int i = 1; i <= 1000; i++) {`**

            **`if (i % 3 == 0 && i % 5 == 0) {`**

                **`sum3and5 += i;`**

                **`countOfMatches++;`**

            **`}`**

        **`}`**

        **`System.out.println("Sum = " + sum3and5 + ", Count = " + countOfMatches);`**

    **`}`**

    **`public static void printCounter() {`**

        **`for (int counter = 1; counter <= 5; counter++) {`**

            **`System.out.println(counter);`**

        **`}`**

    **`}`**

    **`public static boolean isPrime(int number) {`**

        **`if (number <= 2) return number == 2;`**

        **`for (int divisor = 2; divisor < number; divisor++) {`**

            **`if (number % divisor == 0) return false;`**

        **`}`**

        **`return true;`**

    **`}`**

    **`public static void printPrimeNumbers() {`**

        **`int counter = 0;`**

        **`for (int number = 1; number <= 1000; number++) {`**

            **`if (isPrime(number)) {`**

                **`System.out.println(number + " is a prime number");`**

                **`counter++;`**

                **`if (counter == 3) break;`**

            **`}`**

        **`}`**

    **`}`**

    **`public static double calculateInterest(double amount, double interestRate) {`**

        **`return amount * (interestRate / 100);`**

    **`}`**

    **`public static void printInterestRates() {`**

        **`for (double rate = 7.5; rate <= 10; rate += 0.25) {`**

            **`double interestAmount = calculateInterest(100.00, rate);`**

            **`if (interestAmount > 8.5) break;`**

            **`System.out.println("Rate: " + rate + "% - Interest: " + interestAmount);`**

        **`}`**

    **`}`**

**`}`**

---

## **Summary**

**Today's practice with for loops helped improve:**  
**✅ Loop optimization using `break` conditions**  
**✅ Using helper methods to keep code modular**  
**✅ Efficiently handling number operations (summing, primes, interest calculation)**

**Mastering loops is crucial for writing efficient and clean Java code\! 🚀**

