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

- Digital Electronics is a field of electronics involving digital signals that use binary values (0 and 1) to represent information. It forms the basis of all modern computing devices, utilizing logic gates and circuits to perform operations.

- Unlike analog electronics, where signals vary continuously, digital systems work with discrete voltage levels which makes them less susceptible to noise and easier to process.

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

## LOGIC LEVELS

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

Example:  1011₂  = (1 × 2³) + (0 × 2²) + (1 × 2¹) + (1 × 2⁰)
 = 8 + 0 + 2 + 1
 = 11₁₀
= **11 (Decimal)**

---

### Decimal (Base 10)
- **Digits**: 0–9  
- **Each position** = power of 10
- Example:  253₁₀ =  (2 × 10²) + (5 × 10¹) + (3 × 10⁰) 
     = 200 + 50 + 3 = 253 = **253 (Decimal)**

---

### Octal (Base 8)
- **Digits**: 0–7  
- **Each position** = power of 8  

Example:  145 = (1×8^2) + (4×8^1) + (5×8^0) 
= 64 + 32 + 5 
= **101 (Decimal)**

---

### Hexadecimal (Base 16)
- **Digits**: 0–9 and A–F  
- **Each position** = power of 16  

Example:  2F 
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

**Example:**  1101
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

**Example:**   2F
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

![and gate](https://github.com/user-attachments/assets/d807fc51-a1e3-4cd2-b872-26ac0104780a)




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

**Symbol:**


![or gate](https://github.com/user-attachments/assets/8acd2c27-f26b-4537-b789-4adba20d26b7)

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


![not gate](https://github.com/user-attachments/assets/4bcdbf38-3e0a-484b-a8b0-c2167dc52dc5)


**Truth Table:**

| A | NOT  |
|---|----------|
| 0 | 1        |
| 1 | 0        |

---

## 4. XOR Gate (Exclusive OR)  
**Function:** The output is TRUE (1) if the inputs are **different**. The output is FALSE (0) if the inputs are the same.  

**Symbol:**


![exor gate](https://github.com/user-attachments/assets/27a5e193-affe-4ca7-adc5-3a5b62bd7b77)


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


![nand gate](https://github.com/user-attachments/assets/82f95ac1-8af3-4bdf-881f-89d3e1e9a326)


 
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

![nor gate](https://github.com/user-attachments/assets/f5d9ed37-da60-4f2d-a1e1-1d0d149ccd48)

  
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

![xnor gate](https://github.com/user-attachments/assets/98a3237d-8e56-4e42-89b4-2a08e5dd07d4)


 
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


# 🔌 Logic Gates and Their IC Numbers 
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

| Logic Gate | IC Number | Application                | Description of Use                                     |
|------------|-----------|----------------------------|--------------------------------------------------------|
| AND        | 7408      | Password Verification      | All conditions must be true to unlock a system.        |
| OR         | 7432      | Alarm Systems              | Triggers alarm if any of multiple inputs are high.     |
| NOT        | 7404      | Inverter Circuits          | Used to reverse input logic (e.g., for control logic). |
| NAND       | 7400      | Burglar Alarm Trigger      | Output goes low only when all sensors are active.      |
| NOR        | 7402      | Memory Cell Reset Circuits | Resets system when all inputs are low.                 |
| XOR        | 7486      | Parity Generators/Checkers | Checks for even or odd parity in data transmission.    |
| XNOR       | 74266     | Digital Comparators        | Compares binary numbers bit by bit.                    |

# 1.IC 7408 – Quad 2-Input AND Gate
![7408 and pin diagram](https://github.com/user-attachments/assets/46e792f0-858e-4bfd-85e6-6ed5101ea4e6)     ![pin 7408](https://github.com/user-attachments/assets/5f0363d4-d4ab-473d-ad98-0c13ccec1872)

![and gate ic](https://github.com/user-attachments/assets/bee93829-bf61-466d-9e49-960943e861df)

👉 [Open  AND in Tinkercad](https://www.tinkercad.com/things/88w3ni0Cg88-and-gate-ic-7408)

## Pin Description

| Pin No. | Pin Label | Direction | Function                       |
|---------|-----------|-----------|--------------------------------|
| 1       | A1        | Input     | 1st input of AND gate 1        |
| 2       | B1        | Input     | 2nd input of AND gate 1        |
| 3       | Y1        | Output    | Output of AND gate 1           |
| 4       | A2        | Input     | 1st input of AND gate 2        |
| 5       | B2        | Input     | 2nd input of AND gate 2        |
| 6       | Y2        | Output    | Output of AND gate 2           |
| 7       | GND       | Power     | Ground (0V)                    |
| 8       | Y3        | Output    | Output of AND gate 3           |
| 9       | A3        | Input     | 1st input of AND gate 3        |
| 10      | B3        | Input     | 2nd input of AND gate 3        |
| 11      | Y4        | Output    | Output of AND gate 4           |
| 12      | A4        | Input     | 1st input of AND gate 4        |
| 13      | B4        | Input     | 2nd input of AND gate 4        |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)  |

----------------------------------------------
# 2. IC 7432 – Quad 2-Input OR Gate
![7432](https://github.com/user-attachments/assets/bd5aaca8-44b9-4bbb-a374-310c04ab1604)    ![7432 pin diagram](https://github.com/user-attachments/assets/84bf016f-4897-48ba-b026-89adc1f24d7a)


![or circuit](https://github.com/user-attachments/assets/9e61463e-64db-4b42-9ceb-9e0c1bfe0f68)

### 🔸 OR Gate using IC 7432
👉 [Open OR Gate Circuit in Tinkercad](https://www.tinkercad.com/things/9nPagTCFV95-or-gate-ic-7432)
## Pin Description

| Pin No. | Pin Label | Direction | Function                       |
|---------|-----------|-----------|--------------------------------|
| 1       | A1        | Input     | 1st input of OR gate 1         |
| 2       | B1        | Input     | 2nd input of OR gate 1         |
| 3       | Y1        | Output    | Output of OR gate 1            |
| 4       | A2        | Input     | 1st input of OR gate 2         |
| 5       | B2        | Input     | 2nd input of OR gate 2         |
| 6       | Y2        | Output    | Output of OR gate 2            |
| 7       | GND       | Power     | Ground (0V)                    |
| 8       | Y3        | Output    | Output of OR gate 3            |
| 9       | A3        | Input     | 1st input of OR gate 3         |
| 10      | B3        | Input     | 2nd input of OR gate 3         |
| 11      | Y4        | Output    | Output of OR gate 4            |
| 12      | A4        | Input     | 1st input of OR gate 4         |
| 13      | B4        | Input     | 2nd input of OR gate 4         |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)  |
----------------------------------------------
# 3. IC 7404 – Hex Inverter (NOT Gate)
 ![7404 ic pin](https://github.com/user-attachments/assets/798e2325-8b51-4304-9926-8cdaddfefe65)   ![7404](https://github.com/user-attachments/assets/a6aa0fe0-ebb3-4a49-bdc6-63b2190957dd)
 
 ![7404 circuit](https://github.com/user-attachments/assets/aee8a5d2-fc78-402c-92f6-6bcc7a13293e)
 
 ### 🔸 NOT Gate using IC 7404  
 
  [Open NOT GATE in Tinkercad](
 ## Pin Description

| Pin No. | Pin Label | Direction | Function                        |
|---------|-----------|-----------|---------------------------------|
| 1       | A1        | Input     | Input of inverter 1             |
| 2       | Y1        | Output    | Output of inverter 1            |
| 3       | A2        | Input     | Input of inverter 2             |
| 4       | Y2        | Output    | Output of inverter 2            |
| 5       | A3        | Input     | Input of inverter 3             |
| 6       | Y3        | Output    | Output of inverter 3            |
| 7       | GND       | Power     | Ground (0V)                     |
| 8       | Y4        | Output    | Output of inverter 4            |
| 9       | A4        | Input     | Input of inverter 4             |
| 10      | Y5        | Output    | Output of inverter 5            |
| 11      | A5        | Input     | Input of inverter 5             |
| 12      | Y6        | Output    | Output of inverter 6            |
| 13      | A6        | Input     | Input of inverter 6             |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)   |

----------------------------------------------------------------------
# 4. IC 7400 – Quad 2-Input NAND Gate
![7400 both](https://github.com/user-attachments/assets/06f1be00-a996-4d60-8134-d51e6d276105)

![circuit](https://github.com/user-attachments/assets/fee9c3de-25bc-4523-b40d-0a1a06cc1537)

### 🔸 NAND Gate using IC 7400  
👉 [Open NAND GATE in Tinkercad](https://www.tinkercad.com/things/4oQlEQfwRKP-nand-gate-ic-7400)
## Pin Description

| Pin No. | Pin Label | Direction | Function                       |
|---------|-----------|-----------|--------------------------------|
| 1       | A1        | Input     | 1st input of NAND gate 1       |
| 2       | B1        | Input     | 2nd input of NAND gate 1       |
| 3       | Y1        | Output    | Output of NAND gate 1          |
| 4       | A2        | Input     | 1st input of NAND gate 2       |
| 5       | B2        | Input     | 2nd input of NAND gate 2       |
| 6       | Y2        | Output    | Output of NAND gate 2          |
| 7       | GND       | Power     | Ground (0V)                    |
| 8       | Y3        | Output    | Output of NAND gate 3          |
| 9       | A3        | Input     | 1st input of NAND gate 3       |
| 10      | B3        | Input     | 2nd input of NAND gate 3       |
| 11      | Y4        | Output    | Output of NAND gate 4          |
| 12      | A4        | Input     | 1st input of NAND gate 4       |
| 13      | B4        | Input     | 2nd input of NAND gate 4       |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)  |
------------------------------------------------------------------------------
  
# 5. IC 7402 – Quad 2-Input NOR Gate
![7402](https://github.com/user-attachments/assets/82951dd5-a65a-4141-8b04-b1125c242da3)

![7402 circuit](https://github.com/user-attachments/assets/ec2c5349-45ab-4466-866f-97fe8ed34829)

### 🔹 NOR Gate using IC 7402  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/6eAb1UnugPH-nor-gate-ic-7402)


## Pin Description

| Pin No. | Pin Label | Direction | Function                       |
|---------|-----------|-----------|--------------------------------|
| 1       | Y1        | Output    | Output of NOR gate 1           |
| 2       | A1        | Input     | 1st input of NOR gate 1        |
| 3       | B1        | Input     | 2nd input of NOR gate 1        |
| 4       | Y2        | Output    | Output of NOR gate 2           |
| 5       | A2        | Input     | 1st input of NOR gate 2        |
| 6       | B2        | Input     | 2nd input of NOR gate 2        |
| 7       | GND       | Power     | Ground (0V)                    |
| 8       | A3        | Input     | 1st input of NOR gate 3        |
| 9       | B3        | Input     | 2nd input of NOR gate 3        |
| 10      | Y3        | Output    | Output of NOR gate 3           |
| 11      | A4        | Input     | 1st input of NOR gate 4        |
| 12      | B4        | Input     | 2nd input of NOR gate 4        |
| 13      | Y4        | Output    | Output of NOR gate 4           |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)  |

✅ Note: The pin order is slightly different in 7402 compared to 7400/7408/7432 — outputs come first in the pin sequence.
--------------------------------------------------------------------------------
# 6. IC 7486 – Quad 2-Input XOR Gate
![7486 pin](https://github.com/user-attachments/assets/c3faa97d-cf61-481c-8902-0c987c936398)

![XOR IC 7486](https://github.com/user-attachments/assets/ba25a292-ecce-4b62-a0bf-81f8f705b999)

### 🔹 XOR Gate using IC 7486  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/2tIHfi7LytI-xor-ic-7486)


## Pin Description

| Pin No. | Pin Label | Direction | Function                       |
|---------|-----------|-----------|--------------------------------|
| 1       | A1        | Input     | 1st input of XOR gate 1        |
| 2       | B1        | Input     | 2nd input of XOR gate 1        |
| 3       | Y1        | Output    | Output of XOR gate 1           |
| 4       | A2        | Input     | 1st input of XOR gate 2        |
| 5       | B2        | Input     | 2nd input of XOR gate 2        |
| 6       | Y2        | Output    | Output of XOR gate 2           |
| 7       | GND       | Power     | Ground (0V)                    |
| 8       | Y3        | Output    | Output of XOR gate 3           |
| 9       | A3        | Input     | 1st input of XOR gate 3        |
| 10      | B3        | Input     | 2nd input of XOR gate 3        |
| 11      | Y4        | Output    | Output of XOR gate 4           |
| 12      | A4        | Input     | 1st input of XOR gate 4        |
| 13      | B4        | Input     | 2nd input of XOR gate 4        |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)  |
--------------------------------------------------------

# 7.  IC 74266 – Quad 2-Input XNOR Gate
![74266](https://github.com/user-attachments/assets/4caf12ad-191d-415d-87c4-ba3946c3e7d0)

![XNOR gate IC 74266](https://github.com/user-attachments/assets/7539347a-1be6-4f59-a054-fd67189b9c6c)

 ### 🔹 XNOR Gate  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/7g94kDrrNwn-xnor-gate-ic-74266)

## Pin Description

| Pin No. | Pin Label | Direction | Function                              |
|---------|-----------|-----------|---------------------------------------|
| 1       | A1        | Input     | 1st input of XNOR gate 1              |
| 2       | B1        | Input     | 2nd input of XNOR gate 1              |
| 3       | Y1        | Output    | Output of XNOR gate 1 (open collector)|
| 4       | A2        | Input     | 1st input of XNOR gate 2              |
| 5       | B2        | Input     | 2nd input of XNOR gate 2              |
| 6       | Y2        | Output    | Output of XNOR gate 2 (open collector)|
| 7       | GND       | Power     | Ground (0V)                           |
| 8       | Y3        | Output    | Output of XNOR gate 3 (open collector)|
| 9       | A3        | Input     | 1st input of XNOR gate 3              |
| 10      | B3        | Input     | 2nd input of XNOR gate 3              |
| 11      | Y4        | Output    | Output of XNOR gate 4 (open collector)|
| 12      | A4        | Input     | 1st input of XNOR gate 4              |
| 13      | B4        | Input     | 2nd input of XNOR gate 4              |
| 14      | Vcc       | Power     | Positive supply voltage (+5V)         |
--------------------------------------------------------









