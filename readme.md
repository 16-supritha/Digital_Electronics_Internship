# DIGITAL ELECTRONICS


## Table of Contents

- [What is Digital Electronics?](#what-is-digital-electronics)
- [Applications of Digital Electronics](#applications-of-digital-electronics)
- [Digital vs Analog Signals](#digital-vs-analog-signals)
- [Logic Levels](#logic-levels)
- [Number system](#Number-system)
- [Logic Gates](#Logic-Gates)
- [Integrated Circuits](#Integrated-Circuits) 

---

## What is Digital Electronics?

**Digital Electronics** is a field of electronics involving digital signals that use binary values (0 and 1) to represent information. It forms the basis of all modern computing devices, utilizing logic gates and circuits to perform operations.

Unlike analog electronics, where signals vary continuously, digital systems work with discrete voltage levels which makes them less susceptible to noise and easier to process.

---

## Applications of Digital Electronics

Digital electronics play a crucial role in various industries and applications:

- **Computing Devices:** Microprocessors, RAM, ROM, and hard drives
- **Communication Systems:** Mobile phones, satellites, and networking equipment
- **Consumer Electronics:** Smart TVs, cameras, and home automation systems
- **Automotive Systems:** Electronic control units, ABS, and infotainment
- **Medical Equipment:** MRI scanners, digital thermometers, ECG monitors
- **Industrial Automation:** PLCs, robotics, and smart control systems

---

## Digital vs Analog Signals

| Feature              | Digital Signal         | Analog Signal          |
|----------------------|------------------------|------------------------|
| Signal Type          | Discrete               | Continuous             |
| Noise Immunity       | High                   | Low                    |
| Data Representation  | Binary (0 and 1)       | Infinite values        |
| Transmission Quality | Less signal degradation| Prone to distortion    |
| Processing           | Simple & Efficient     | Complex                |
| Examples             | Computer data, logic circuits | Audio signals, sensors |

---

## Logic Levels

Logic levels refer to voltage ranges used to represent digital values:

- **Logic 0 (Low):** Typically 0V
- **Logic 1 (High):** Typically 3.3V, 5V, or other depending on the logic family

# Number Systems 

---

## 1. What Are Number Systems?

"A number system in digital electronics is a method of representing numbers using a specific set of symbols or digits". It defines how numbers are expressed and processed in digital circuits. The commonly used number systems are:

- **Binary (Base 2)** - Uses 0 and 1  
- **Decimal (Base 10)** - Our everyday system; uses 0 to 9  
- **Octal (Base 8)** - Uses 0 to 7  
- **Hexadecimal (Base 16)** - Uses 0 to 9 and A to F (A=10, B=11, ..., F=15)

---

## 2. Number Systems Explained

### Binary (Base 2)
- **Digits**: 0, 1  
- **Each position** = power of 2  

Example:  1011₂ 
 = (1 × 2³) + (0 × 2²) + (1 × 2¹) + (1 × 2⁰)
 = 8 + 0 + 2 + 1
 = 11₁₀
= **11 (Decimal)**

---

### Decimal (Base 10)
- **Digits**: 0–9  
- **Each position** = power of 10
- Example:  
253₁₀ =  (2 × 10²) + (5 × 10¹) + (3 × 10⁰) 
     = 200 + 50 + 3
     = 253
= **253 (Decimal)**

---

### Octal (Base 8)
- **Digits**: 0–7  
- **Each position** = power of 8  

Example:  
145 = (1×8^2) + (4×8^1) + (5×8^0) 
= 64 + 32 + 5 
= **101 (Decimal)**

---

### Hexadecimal (Base 16)
- **Digits**: 0–9 and A–F  
- **Each position** = power of 16  

Example:  
2F 
2 -> = (2×16^1) + 
E -> = (15×16^0) 
= 32 + 15 
= **47 (Decimal)**

---



## 3. Conversions Between Number Systems

---

### A. Binary to Decimal

**Steps:**
1. Write the binary number.
2. Multiply each digit by 2ⁿ (where n is the position from right, starting at 0).
3. Add the results.

**Example:**  
1101
     = (1 × 2³)  + (1 × 2²) + (0 × 2¹)  + (1 × 2⁰)  
     = 8 + 4 + 0 + 1  
     = **13 (Decimal)**

---

### B. Decimal to Binary

**Steps:**
1. Divide the number by 2.
2. Record the remainder.
3. Repeat until the quotient is 0.
4. Read the remainders from bottom to top.

**Example:** 13  
13 ÷ 2 = 6 remainder **1**  
6 ÷ 2 = 3 remainder **0**  
3 ÷ 2 = 1 remainder **1**  
1 ÷ 2 = 0 remainder **1**  

**Binary:** 1101

---

### C. Decimal to Hexadecimal

**Steps:**
1. Divide the number by 16.
2. Write down the remainder.
3. Repeat until the quotient is 0.
4. Read from bottom to top and convert numbers > 9 into letters A–F.

**Example:** 254  
254 ÷ 16 = 15 remainder **14 (E)**  
15 ÷ 16 = 0 remainder **15 (F)**  

**Hexadecimal:** FE

---

### D. Hexadecimal to Decimal

**Steps:**
1. Convert each hex digit to decimal.
2. Multiply each by 16ⁿ (n starts from 0 on the right).
3. Add the results.

**Example:** 1A  
= (1 × 16¹)  + (10 × 16⁰)  
= 16 + 10  
= **26 (Decimal)**

---

### E. Binary to Hexadecimal

**Steps:**
1. Group binary digits into 4 from the right.
2. Convert each group to hex.

**Example:** 11010110  
→ 1101 | 0110  
→ D | 6  

**Hexadecimal:** D6

---

### F. Hexadecimal to Binary

**Steps:**
1. Convert each hex digit to 4-bit binary.

**Example:**   `2F`
2 = (2×16^1)
F = (15×16^0)
= 32 + 15
= **47 (Decimal)**
---

### G. Decimal to Octal

**Steps:**
1. Divide the decimal number by 8.
2. Write down the remainder.
3. Repeat until quotient is 0.
4. Read from bottom to top.

**Example:** 100  
100 ÷ 8 = 12 remainder **4**  
12 ÷ 8 = 1 remainder **4**  
1 ÷ 8 = 0 remainder **1**  

**Octal:** 144

---

### H. Octal to Decimal

**Steps:**
1. Multiply each digit by 8ⁿ (n starts from 0 on the right).
2. Add the results.

**Example:** 145  
= (1 × 8²)  
+ (4 × 8¹)  
+ (5 × 8⁰)  
= 64 + 32 + 5  
= **101 (Decimal)**

---

### I. Binary to Octal

**Steps:**
1. Group binary digits in 3s from the right.
2. Convert each group to octal.

**Example:** 101101  
→ 000 | 101 | 101  
→ 0 | 5 | 5  

**Octal:** 55

---

### J. Octal to Binary

**Steps:**
1. Convert each octal digit to 3-bit binary.

**Example:** 74  
7 = 111  
4 = 100  

**Binary:** 111100

---
## Importance of Number Systems in Digital Systems

- Digital devices (like computers) only understand two states: ON and OFF. These are represented using 1 and 0, which is **binary**.
- Number systems allow us to **store, process, and communicate** data efficiently in digital circuits.
- **Octal and Hexadecimal** make it easier for humans to read and write large binary numbers.
- Using number systems helps in **designing hardware** and **writing software** for digital systems.
 
 # Logic Gates 


---

## 1. AND Gate

**Function:**
The AND gate outputs HIGH (1) only when all its inputs are HIGH. It performs a logical multiplication operation.

**Symbol:**

![AND GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/c41067a7a1ebaf9435de0413a5973ff03d7fc40d/and%20gate.png)



**Boolean Function:**
Output = A * B


**Truth Table:**
|  INP A |  INP B | Output Y |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   0    |
| 1 | 0 |   0    |
| 1 | 1 |   1    |

**Applications:**
- Digital circuits
- Multiplication operations in ALUs
- Input validation

---


## 2. OR Gate  
**Function:** The output is TRUE (1) if **at least one** input is TRUE (1). The output is FALSE (0) only if both inputs are FALSE (0).    
**Truth Table:**

| A | B | OR  |
|---|---|----------|
| 0 | 0 | 0        |
| 0 | 1 | 1        |
| 1 | 0 | 1        |
| 1 | 1 | 1        |

---

## 3. NOT Gate (Inverter)  
**Function:** The output is the inverse of the input. If the input is TRUE (1), output is FALSE (0), and vice versa.

**Symbol:**
![NOT GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/e701caeb201c96f3b3fb8b66ec95545766695da1/not%20gate.png)

**Truth Table:**

| A | NOT  |
|---|----------|
| 0 | 1        |
| 1 | 0        |

---

## 4. XOR Gate (Exclusive OR)  
**Function:** The output is TRUE (1) if the inputs are **different**. The output is FALSE (0) if the inputs are the same.  

**Symbol:**


![XOR GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/5b126d9ba7a2eb0ed8ae24e09a3b4826f879e2b2/Jmxzy.jpg)

**Truth Table:**

| A | B | XOR |
|---|---|-----------|
| 0 | 0 | 0         |
| 0 | 1 | 1         |
| 1 | 0 | 1         |
| 1 | 1 | 0         |

---

## 5. NAND Gate (NOT AND)  
**Function:** The output is FALSE (0) only if both inputs are TRUE (1). Otherwise, the output is TRUE (1). It is the inverse of the AND gate.  

**Symbol:**
![NAND GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/97908bcd529cb80b9ac613d8dd354ce6bad034ac/1280px-Nand-gate-en.svg.png)


 
**Truth Table:**

| A | B | NAND |
|---|---|---------------|
| 0 | 0 | 1             |
| 0 | 1 | 1             |
| 1 | 0 | 1             |
| 1 | 1 | 0             |

---

## 6. NOR Gate (NOT OR)  
**Function:** The output is TRUE (1) only if **both** inputs are FALSE (0). Otherwise, the output is FALSE (0). It is the inverse of the OR gate.  

**Symbol:**

![NOT GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/b4eb3036b6893aa215ab404a1773c95645748c36/Eaazs.png)

  
**Truth Table:**

| A | B | NOR |
|---|---|--------------|
| 0 | 0 | 1            |
| 0 | 1 | 0            |
| 1 | 0 | 0            |
| 1 | 1 | 0            |

---

## 7. XNOR Gate (Exclusive NOR)  
**Function:** The output is TRUE (1) if the inputs are **the same**. The output is FALSE (0) if the inputs are different. It is the inverse of the XOR gate. 
**Symbol:**

![XNOR GATE](https://github.com/16-supritha/Digital_Electronics_Internship/blob/d51eadfd5e5d07c08aefb0d9bd49b8cc67bc1f21/Logic-gate-xnor-us.png)

 
**Truth Table:**

| A | B | XNOR  |
|---|---|------------|
| 0 | 0 | 1          |
| 0 | 1 | 0          |
| 1 | 0 | 0          |
| 1 | 1 | 1          |

---
# INTEGRATED CIRCUITS

# What is an IC?

An **Integrated Circuit (IC)** is a small chip that contains many electronic components like transistors and resistors on a single semiconductor.  
It performs specific functions such as logic operations, amplification, or memory storage in compact electronic systems.


# 🔌 Logic Gates and Their IC Numbers (TTL Series)

This document provides a reference table of basic logic gates, their standard IC numbers, descriptions, the number of gates inside each IC, and total pin count.

---

## 📋 Logic Gate IC Reference Table

| Logic Gate | IC Number | Description                         | Gates per IC | Pin Count |
|------------|-----------|-------------------------------------|--------------|-----------|
| AND        | 7408      | Quad 2-input AND gates              | 4            | 14        |
| OR         | 7432      | Quad 2-input OR gates               | 4            | 14        |
| NOT        | 7404      | Hex inverters (NOT gates)           | 6            | 14        |
| NAND       | 7400      | Quad 2-input NAND gates             | 4            | 14        |
| NOR        | 7402      | Quad 2-input NOR gates              | 4            | 14        |
| XOR        | 7486      | Quad 2-input XOR gates              | 4            | 14        |
| XNOR       | 74266     | Quad 2-input XNOR gates (open drain)| 4            | 14        |

---

## 🧠 Notes

- **Quad** means the IC contains 4 identical gates.
- **Hex** means 6 gates (as in NOT gates).
- Most TTL logic gate ICs come in **14-pin Dual In-Line Packages (DIP)**.
- Vcc (power) is typically on pin 14 and GND on pin 7.

---

# 🧩 Applications of ICs with Logic Gates

This table shows how basic logic gates (using TTL ICs) are used in real-world digital circuits and systems.

| Logic Gate | IC Number | Application                | Description of Use                                     |
|------------|-----------|----------------------------|--------------------------------------------------------|
| AND        | 7408      | Password Verification      | All conditions must be true to unlock a system.        |
| OR         | 7432      | Alarm Systems              | Triggers alarm if any of multiple inputs are high.     |
| NOT        | 7404      | Inverter Circuits          | Used to reverse input logic (e.g., for control logic). |
| NAND       | 7400      | Burglar Alarm Trigger      | Output goes low only when all sensors are active.      |
| NOR        | 7402      | Memory Cell Reset Circuits | Resets system when all inputs are low.                 |
| XOR        | 7486      | Parity Generators/Checkers | Checks for even or odd parity in data transmission.    |
| XNOR       | 74266     | Digital Comparators        | Compares binary numbers bit by bit.                    |



![not gate](https://github.com/user-attachments/assets/7fb4b7ab-97cd-4b47-bd8a-62b947cc04f5)
