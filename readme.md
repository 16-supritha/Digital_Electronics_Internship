# DIGITAL ELECTRONICS


## Table of Contents

- [What is Digital Electronics?](#what-is-digital-electronics)
- [Applications of Digital Electronics](#applications-of-digital-electronics)
- [Digital vs Analog Signals](#digital-vs-analog-signals)
- [Logic Levels](#logic-levels)
- [Number system](#Number-system)
- [Logic Gates](#Logic-Gates)
- [Integrated Circuits](#Integrated-Circuits)
- [Implementation of Logic Gatess](#Logic-Gates)
- [Implementationof HalfAdder](#Implementationof-Halfadder)
- [Implementationof FullAdder](#Implementationof-FullAdder)
- [Implementationof 2:1MUX ](#Implementationof-2:1mux)
 

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

## NUMBER SYSTEMS

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

    Example:    2F

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
 
 ## Logic Gates 


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


![XOR GATE](https://github.com/user-attachments/assets/facc735d-d181-4f0d-834e-216d475d24a7)


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


#  Logic Gates and Their IC Numbers 
---

## Logic Gate IC Reference Table

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

##  Notes

- **Quad** means the IC contains 4 identical gates.
- **Hex** means 6 gates (as in NOT gates).
- Most TTL logic gate ICs come in **14-pin Dual In-Line Packages (DIP)**.
- Vcc (power) is typically on pin 14 and GND on pin 7.

---

#  Applications of ICs with Logic Gates

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
![7408 and pin diagram](https://github.com/user-attachments/assets/46e792f0-858e-4bfd-85e6-6ed5101ea4e6)     

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
![OR PIN CONFIGURation](https://github.com/user-attachments/assets/30d68f18-a459-4b4a-8ace-84dceb1fbd4a)



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
 
 ![NOT GATE IC RESISE](https://github.com/user-attachments/assets/2a302768-ae95-43ca-8c58-5a7d3c7c139e)

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
![NAND GATE RESIZE](https://github.com/user-attachments/assets/cef89519-6658-4edc-8f5f-19aef6f36171)


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
![NOR GATE](https://github.com/user-attachments/assets/6f8e1b07-cf9a-4234-9cb8-f6697662d857)


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


--------------------------------------------------------------------------------
# 6. IC 7486 – Quad 2-Input XOR Gate
![XOR R](https://github.com/user-attachments/assets/af1c583c-2f12-455a-8cd7-aa9d664d464e)

![xor](https://github.com/user-attachments/assets/ac4feecb-5770-41f6-99c4-246b80abfa93)




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
![XOR PIN](https://github.com/user-attachments/assets/53af2a62-8ac8-4982-83f2-2f2a2540fb72)


![xnor](https://github.com/user-attachments/assets/c369e96a-2427-4b55-84f5-26d49f510c28)



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

## IMPLEMENTATION OF LOGIC GATES

 IMPLEMENTATION OF AND GATE USING NAND GATE 7400

![P](https://github.com/user-attachments/assets/c58d094c-9172-4e0b-bdee-0041170c18cb)

 Tinkercad Project Link

👉 [View  AND GATE USING NAND Gate 7400  Project on Tinkercad](https://www.tinkercad.com/things/2ikxvqCHHor-and-with-nand-gate)

-----------------------------------
# IMPLEMENTATION OF OR GATE  USING NAND GATE 7400

![O](https://github.com/user-attachments/assets/0d4d18b2-0881-46fb-8f07-4f5a5ebe29ad)


 Tinkercad Project Link:

👉 [View  OR GATE USING NAND GATE 7400 Circuit on Tinkercad](https://www.tinkercad.com/things/2SFUaJOht4N-or-with-nand)

-------------------------------------
# IMPLEMENTATION OF NOT GATE USING NAND GATE 7400

![N](https://github.com/user-attachments/assets/d093abae-7385-456e-92ef-84764d7887b4)


  Tinkercad Project Link :
  
👉 [View NOT GATE USING NAND 7400](https://www.tinkercad.com/things/2cgmEXES55h-not-with-nand)

-----------------------------------------------
#  IMPLEMENTATION OF AND GATE USING NOR GATE 7402

![DF](https://github.com/user-attachments/assets/3f6f6969-11a0-406a-9e87-7721cf2a5627)

 
 Tinkercad Project Link:

👉[View AND GATE USING NOR 7402](https://www.tinkercad.com/things/ifEgXWxR8pf-and-using-nor)
 
 -------------------------------------
#  IMPLEMENTATION OF OR GATE USING NOR GATE 7402


![fr](https://github.com/user-attachments/assets/df60b860-e837-4a31-8bc2-ea9535d76af7)


  Tinkercad Project Link:
  👉[View OR GATE USING NOR 7402](https://www.tinkercad.com/things/cleZgo1KQWd-or-with-nor)


--------------------------------------------
# IMPLEMENTATION OF NOT GATE USING NOR GATE 7402

![MM](https://github.com/user-attachments/assets/46e4dcfe-b6e8-47f7-b27d-da257d2ea06f)

Tinkercad Project Link:

👉 [View NOT GATE USING NOR GATE 7402](https://www.tinkercad.com/things/63mjcM1o9Tu-not-using-nor-gate)

-------------------------------------

## IMPLEMENTATION OF HALF ADDER

#Definition

A **Half Adder** is a combinational circuit that performs addition of two binary digits. It has two outputs:

![C](https://github.com/user-attachments/assets/a73838fe-63a7-4a23-b1e7-42f53ec21b52)  ![TT](https://github.com/user-attachments/assets/c65cf513-2452-452d-991e-6febc1a0d699)


#  Pinout Table

| S.No | Pin No (IC/Component)       | Connected To                                      |
|------|-----------------------------|---------------------------------------------------|
| 1    | 74HC00 (Left IC) Pin 14     | Vcc (+ve rail)                                    |
| 2    | 74HC00 (Left IC) Pin 7      | GND (-ve rail)                                    |
| 3    | 74HC00 (Right IC) Pin 14    | Vcc (+ve rail)                                    |
| 4    | 74HC00 (Right IC) Pin 7     | GND (-ve rail)                                    |
| 5    | DIP Switch Pin 1            | A input to 74HC00 Pin 1                           |
| 6    | DIP Switch Pin 2            | B input to 74HC00 Pin 2                           |
| 7    | A Input Line                | 74HC00 Pins 1, 5, 9 (varies for XOR structure)    |
| 8    | B Input Line                | 74HC00 Pins 2, 6, 10                              |
| 9    | 74HC00 (Left IC) Pin 3      | Internal XOR output line (to Right IC, SUM)       |
| 10   | 74HC00 (Right IC) Pin 3     | Connected to Green LED (SUM output)               |
| 11   | 74HC00 (Left IC) Pin 4      | Connected to Red LED (CARRY output)               |
| 12   | Red LED Cathode             | GND via 220Ω resistor                             |
| 13   | Green LED Cathode           | GND via 220Ω resistor                             |
| 14   | Red LED Anode               | From NAND output (CARRY)                          |
| 15   | Green LED Anode             | From NAND-XOR output (SUM)                        |
| 16   | Power Supply (+)            | Breadboard positive rail                          |
| 17   | Power Supply (–)            | Breadboard negative rail                          |

---

#  NAND Gate Implementation of Half Adder

### **SUM = A ⊕ B = (A NAND (A NAND B)) NAND (B NAND (A NAND B))**

### **CARRY = A · B = (A NAND B)' = A NAND B followed by NAND with itself**

---
![HALF](https://github.com/user-attachments/assets/a8464060-ddbc-4b29-a5fe-d2cd77c10db0)

Tinkercad Project Link:
👉 [View HALF ADDER ](https://www.tinkercad.com/things/1tYgP0O8NUE-half-adder)

-------------------------------------
## IMPLEMENTATION OF FULL ADDER USING NAND GATES

# Definition

A **Full Adder** is a combinational circuit that performs the addition of three binary bits:  
- A  
- B  
- Cin (Carry Input)

It produces two outputs:
- **SUM = A ⊕ B ⊕ Cin**
- **CARRY = (A·B) + (Cin·(A⊕B))**

---

![download](https://github.com/user-attachments/assets/cce25d29-f0ca-4872-866d-94be0a18afca)   

# Truth Table

| A | B | Cin | SUM | CARRY |
|---|---|-----|-----|--------|
| 0 | 0 |  0  |  0  |   0    |
| 0 | 0 |  1  |  1  |   0    |
| 0 | 1 |  0  |  1  |   0    |
| 0 | 1 |  1  |  0  |   1    |
| 1 | 0 |  0  |  1  |   0    |
| 1 | 0 |  1  |  0  |   1    |
| 1 | 1 |  0  |  0  |   1    |
| 1 | 1 |  1  |  1  |   1    |

---


#  Pinout Table

| S.No | Pin No (IC/Component)       | Connected To                                      |
|------|-----------------------------|---------------------------------------------------|
| 1    | 74HC86 Pin 14 (Vcc)         | Breadboard +ve rail                               |
| 2    | 74HC86 Pin 7 (GND)          | Breadboard –ve rail                               |
| 3    | 74HC08 Pin 14 (Vcc)         | Breadboard +ve rail                               |
| 4    | 74HC08 Pin 7 (GND)          | Breadboard –ve rail                               |
| 5    | 74HC32 Pin 14 (Vcc)         | Breadboard +ve rail                               |
| 6    | 74HC32 Pin 7 (GND)          | Breadboard –ve rail                               |
| 7    | DIP Switch 1                | Input A                                           |
| 8    | DIP Switch 2                | Input B                                           |
| 9    | DIP Switch 3                | Input Cin                                         |
| 10   | XOR Gate 1 Input (74HC86)   | A, B                                              |
| 11   | XOR Gate 1 Output           | Connected to XOR Gate 2 and AND gate              |
| 12   | XOR Gate 2 Input            | Cin and output of XOR 1                           |
| 13   | XOR Gate 2 Output           | Connected to SUM LED                              |
| 14   | AND Gate 1 Input (74HC08)   | A and B                                           |
| 15   | AND Gate 2 Input (74HC08)   | Cin and (A⊕B)                                     |
| 16   | OR Gate Input (74HC32)      | Output of both AND gates                          |
| 17   | OR Gate Output              | Connected to CARRY LED                            |
| 18   | SUM LED Cathode             | GND via resistor                                  |
| 19   | CARRY LED Cathode           | GND via resistor                                  |
| 20   | SUM LED Anode               | Output from XOR (SUM)                             |
| 21   | CARRY LED Anode             | Output from OR gate                               |
| 22   | Power Supply (+)            | Breadboard positive rail                          |
| 23   | Power Supply (–)            | Breadboard negative rail                          |

---
![CHJ](https://github.com/user-attachments/assets/44d7cbaf-77fc-4298-a591-b7663943c68f)

# Output
- **SUM** LED turns ON when A ⊕ B ⊕ Cin = 1
- **CARRY** LED turns ON when output carry is 1
  
 Tinkercad Project Link:

👉 [View FULL ADDER USING NAND GATE ](https://www.tinkercad.com/things/lDWqEUBlfJB-ful-adder)

-------------------------------------
## IMPLEMENTATION OF 2:1 MUX

# Definition

A 2:1 multiplexer  is a combinational logic circuit that selects one of two input signals and forwards it to a single output line. The selection is controlled by a single select input (S).

![mux](https://github.com/user-attachments/assets/492e0214-1d65-4a04-bcdf-af0b2a02cbc1)
![TT](https://github.com/user-attachments/assets/de95ca91-2fd7-41e7-bc18-1817c72bd742)

## Pin-Out Table

| S.No | Pin No (IC/Component)   | Connected To                                |
|------|-------------------------|---------------------------------------------|
| 1    | 74HC04 Pin 14 (Vcc)     | +ve Rail (Red)                              |
| 2    | 74HC04 Pin 7 (GND)      | -ve Rail (Black)                            |
| 3    | 74HC08 Pin 14 (Vcc)     | +ve Rail (Red)                              |
| 4    | 74HC08 Pin 7 (GND)      | -ve Rail (Black)                            |
| 5    | 74HC32 Pin 14 (Vcc)     | +ve Rail (Red)                              |
| 6    | 74HC32 Pin 7 (GND)      | -ve Rail (Black)                            |
| 7    | DIP Switch Pin 1        | 74HC04 Pin 1 (Input of NOT Gate)            |
| 8    | DIP Switch Pin 2        | 74HC08 Pin 1 (Input A of AND Gate)          |
| 9    | DIP Switch Pin 3        | 74HC08 Pin 2 (Input B of AND Gate)          |
| 10   | DIP Switch Pin 4        | 74HC32 Pin 5 (Input B of OR Gate)           |
| 11   | 74HC04 Pin 2 (Output)   | 74HC08 Pin 4 (Input B of second AND Gate)   |
| 12   | 74HC08 Pin 3 (Output)   | 74HC32 Pin 4 (Input A of OR Gate)           |
| 13   | 74HC32 Pin 6 (Output)   | LED Anode (Long leg)                        |
| 14   | LED Cathode (Short leg) | 330Ω Resistor                               |
| 15   | Resistor                | Ground Rail                                 |
| 16   | All ICs GND Pins        | Connected to Breadboard GND (-ve)           |
| 17   | All ICs Vcc Pins        | Connected to Breadboard Vcc (+ve)           |
| 18   | Power Supply (+ve)      | Breadboard Red Rail                         |
| 19   | Power Supply (-ve)      | Breadboard Black Rail                       |
---

![CC](https://github.com/user-attachments/assets/c287a3e4-a9b1-4622-a13d-d6f1156c3521)

 Tinkercad Project Link:
👉 [View 2:1 MUX](https://www.tinkercad.com/things/fmHQ6zkMW7Y-mux)
-------------------------------------


