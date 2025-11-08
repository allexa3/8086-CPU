# 🧠 Intel 8086 Instruction Set Overview

This document lists **20 representative instructions** from the **Intel 8086 CPU architecture**, categorized into **Arithmetic**, **Logical**, **Data Transfer**, and **Jump/Control** instructions.  

Each table includes the **instruction mnemonic**, a brief **meaning**, an **example**, and a **description**.

---

## 🧮 Arithmetic Instructions

| Instruction | Meaning | Example | Description |
|--------------|----------|----------|--------------|
| **ADD** | Add | `ADD AX, BX` | AX ← AX + BX |
| **ADC** | Add with carry | `ADC AX, BX` | AX ← AX + BX + CF |
| **SUB** | Subtract | `SUB AX, BX` | AX ← AX − BX |
| **SBB** | Subtract with borrow | `SBB AX, BX` | AX ← AX − BX − CF |
| **INC** | Increment | `INC AX` | AX ← AX + 1 |
| **DEC** | Decrement | `DEC AX` | AX ← AX − 1 |
| **NEG** | Two’s complement | `NEG AL` | AL ← −AL |
| **CMP** | Compare | `CMP AX, BX` | Performs AX − BX, affects flags only |
| **MUL** | Unsigned multiply | `MUL BL` | AX ← AL × BL |
| **DIV** | Unsigned divide | `DIV BL` | AL ← AX ÷ BL; AH ← remainder |

---

## ⚙️ Logical Instructions

| Instruction | Meaning | Example | Description |
|--------------|----------|----------|--------------|
| **AND** | Bitwise AND | `AND AL, BL` | AL ← AL & BL |
| **OR** | Bitwise OR | `OR AL, BL` | AL ← AL \| BL |
| **XOR** | Bitwise XOR | `XOR AL, BL` | AL ← AL ⊕ BL |
| **NOT** | Bitwise NOT | `NOT AL` | AL ← ¬AL |
| **TEST** | Logical compare | `TEST AL, BL` | Performs AL & BL, affects flags only |

---

## 🔁 Data Transfer Instructions

| Instruction | Meaning | Example | Description |
|--------------|----------|----------|--------------|
| **MOV** | Move data | `MOV AX, BX` | AX ← BX |
| **XCHG** | Exchange | `XCHG AX, BX` | Swap AX and BX |
| **PUSH** | Push onto stack | `PUSH AX` | SP ← SP − 2; [SP] ← AX |
| **POP** | Pop from stack | `POP BX` | BX ← [SP]; SP ← SP + 2 |
| **LEA** | Load effective address | `LEA DX, [SI+8]` | DX ← address of (SI + 8) |

---

## 🧭 Jump and Control Instructions

| Instruction | Meaning | Example | Description |
|--------------|----------|----------|--------------|
| **JMP** | Unconditional jump | `JMP LABEL` | Jump to LABEL |
| **JE / JZ** | Jump if equal / zero | `JE LABEL` | Jump if ZF = 1 |
| **JNE / JNZ** | Jump if not equal / nonzero | `JNE LABEL` | Jump if ZF = 0 |
| **JC** | Jump if carry | `JC LABEL` | Jump if CF = 1 |
| **JNC** | Jump if not carry | `JNC LABEL` | Jump if CF = 0 |

---

## ✅ Summary

| Category | Number of Instructions | Examples |
|-----------|------------------------|-----------|
| **Arithmetic** | 10 | ADD, SUB, INC, DEC, CMP |
| **Logical** | 5 | AND, OR, XOR, NOT, TEST |
| **Data Transfer** | 5 | MOV, XCHG, PUSH, POP, LEA |
| **Jump/Control** | 5 | JMP, JE, JNE, JC, JNC |

---

**Total:** 25 representative 8086 instructions covering major functional groups.
