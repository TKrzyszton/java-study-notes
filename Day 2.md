**Day 2 \- Java Masters Course (1 hour)**

Today, I continued working in `jshell`, focusing on expressions in Java and exploring primitive data types, including `byte`, `short`, `int`, and `long`. I learned about their **minimum and maximum value ranges**, as well as their **size and width in bits**, which are summarized in the table below:

| Data Type | Size (Bytes) | Width (Bits) | Minimum Value | Maximum Value |
| ----- | ----- | ----- | ----- | ----- |
| `byte` | 1 | 8 | \-128 | 127 |
| `short` | 2 | 16 | \-32,768 | 32,767 |
| `int` | 4 | 32 | \-2,147,483,648 | 2,147,483,647 |
| `long` | 8 | 64 | \-9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 |

### **Type Casting in Java**

I also learned about **casting**, which is the process of converting one data type into another. There are two types of casting:

1. **Implicit Casting (Widening Conversion)** – Automatically done by Java when converting a smaller data type into a larger one.  
2. **Explicit Casting (Narrowing Conversion)** – Manually done by the programmer when converting a larger data type into a smaller one, as data loss may occur.

**Example of Explicit Casting:**

java  
Kopiuj  
`int myInt = 100;`  
`byte myByte = (byte) myInt; // Explicit casting from int to byte`  
`System.out.println(myByte);`

### **Overflow and Underflow in Java**

I also explored **overflow** and **underflow**, which occur when a value exceeds the range of its assigned data type.

* **Overflow** happens when a value goes beyond the maximum limit of the data type, causing it to wrap around to the minimum value.  
* **Underflow** happens when a value goes below the minimum limit, wrapping around to the maximum value.

**Example of Overflow and Underflow:**

java  
Kopiuj  
`byte maxByte = 127;`  
`maxByte++; // Overflow occurs here`  
`System.out.println(maxByte); // Output: -128`

`byte minByte = -128;`  
`minByte--; // Underflow occurs here`  
`System.out.println(minByte); // Output: 127`

Today's session provided valuable insights into Java's primitive data types, type conversion, and potential pitfalls related to data type limits.

