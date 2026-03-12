# 4-Bit ALU with Flags

A **4-bit Arithmetic Logic Unit (ALU)** capable of performing arithmetic and logical operations on two 4-bit inputs.  
This ALU also generates **status flags** that indicate the result condition after an operation.

The project demonstrates the basic working principle of an ALU used in computer processors.

---

# 📌 Features

- 4-bit input operands
- Arithmetic operations
- Logical operations
- Status flag generation
- Simple and easy to simulate
- Useful for learning **Digital Electronics and Computer Architecture**

---

# 🧠 Supported Operations

| Select (S2 S1 S0) | Operation |
|------------------|-----------|
| 000 | A + B |
| 001 | A - B |
| 010 | A AND B |
| 011 | A OR B |
| 100 | A XOR B |
| 101 | NOT A |
| 110 | Increment A |
| 111 | Decrement A |

---

# 📥 Inputs

| Input | Size | Description |
|------|------|-------------|
| A | 4-bit | First operand |
| B | 4-bit | Second operand |
| S | 3-bit | Operation select |

---

# 📤 Outputs

| Output | Size | Description |
|-------|------|-------------|
| Result | 4-bit | Operation result |
| Carry | 1-bit | Carry/Borrow flag |
| Zero | 1-bit | Result equals zero |
| Sign | 1-bit | Indicates negative result |
| Overflow | 1-bit | Arithmetic overflow |

---

# 🚩 ALU Flags

## Carry Flag (C)
- Set to **1** when a carry occurs in addition  
- Set to **1** when a borrow occurs in subtraction

## Zero Flag (Z)
- Set to **1** if the result is **0000**
- Indicates that the operation result is zero

## Sign Flag (S)
- Represents the **most significant bit (MSB)** of the result
- Indicates **negative numbers in signed operations**

## Overflow Flag (V)
- Set when **signed arithmetic overflow** occurs
- Happens when result exceeds the representable range

---

# 🏗️ ALU Block Diagram

```
        +-----------------------+
A ----->|                       |
        |                       |
B ----->|        4-bit ALU      |-----> Result[3:0]
        |                       |
S ----->|                       |-----> Carry
        |                       |-----> Zero
        |                       |-----> Sign
        +-----------------------+-----> Overflow
```

---

# 📊 Example

Example operation:

```
A = 0111 (7)
B = 0001 (1)
S = 000
```

Operation performed:

```
A + B
```

Output:

```
Result = 1000
Carry = 0
Zero = 0
Sign = 1
Overflow = 1
```

---
# 🔧 Tools Used

- Digital Logic Design
- Verilog / VHDL / Logisim
- Simulation tools:
  - Vivado

---

# 🎯 Learning Objectives

- Understand **ALU architecture**
- Learn **flag generation**
- Practice **HDL based digital design**
- Perform **hardware simulation**

---
