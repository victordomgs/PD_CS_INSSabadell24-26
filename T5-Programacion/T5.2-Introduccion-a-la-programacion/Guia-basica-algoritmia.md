<h1 align="center">Guía básica de algoritmia
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:

[1. Basic Syntax and Fundamental Concepts](#1-basic-syntax-and-fundamental-concepts)  
  - [1.1. Variable Declaration](#11-variable-declaration)  
  - [1.2. Operators](#12-operators)  
    - [1.2.1. Arithmetic Operators](#121-arithmetic-operators)  
    - [1.2.2. Comparison Operators](#122-comparison-operators)  
    - [1.2.3. Logical Operators](#123-logical-operators)  
  - [1.3. Input and Output](#13-input-and-output)  
[2. Conditional Statements](#2-conditional-statements)  
[3. Loops](#3-loops)  
  - [3.1. WHILE Loop](#31-while-loop)  
  - [3.2. FOR Loop](#32-for-loop)  
[4. Arrays and Matrices](#4-arrays-and-matrices)  
  - [4.1. One-dimensional Arrays](#41-one-dimensional-arrays)  
  - [4.2. Two-dimensional Arrays](#42-two-dimensional-arrays)  

---

## 1. Basic Syntax and Fundamental Concepts

### 1.1. Variable Declaration

```plaintext
variable ← initial_value
```

**Examples:**
```plaintext
count ← 0
name ← "Alice"
active ← true
```

### 1.2. Operators

#### 1.2.1. Arithmetic Operators

| Operation         | Symbol | Example         |
|------------------|--------|-----------------|
| Addition          | `+`    | `x ← a + b`     |
| Subtraction       | `-`    | `x ← a - b`     |
| Multiplication    | `*`    | `x ← a * b`     |
| Division          | `/`    | `x ← a / b`     |
| Modulo            | `mod`  | `r ← a mod b`   |

#### 1.2.2. Comparison Operators

| Comparison     | Symbol | Example              |
|----------------|--------|----------------------|
| Equal          | `=`    | `if x = 10 then`     |
| Not equal      | `≠`    | `if x ≠ 10 then`     |
| Greater than   | `>`    | `if x > 10 then`     |
| Less than      | `<`    | `if x < 10 then`     |
| Greater or eq. | `≥`    | `if x ≥ 10 then`     |
| Less or eq.    | `≤`    | `if x ≤ 10 then`     |

#### 1.2.3. Logical Operators

| Operator | Example                          |
|----------|----------------------------------|
| `and`    | `if x > 0 and x < 10 then`       |
| `or`     | `if x < 0 or x > 100 then`       |
| `not`    | `if not active then`            |

### 1.3. Input and Output

**Input:**
```plaintext
input variable
```

**Output:**
```plaintext
output value
```

---

## 2. Conditional Statements

### IF Statement

```plaintext
if condition then
   statements
end if
```

### IF...ELSE Statement

```plaintext
if condition then
   statements_if_true
else
   statements_if_false
end if
```

**Example:**
```plaintext
if grade ≥ 5 then
   output "Passed"
else
   output "Failed"
end if
```

---

## 3. Loops

### 3.1. WHILE Loop

```plaintext
loop while condition
   statements
end loop
```

**Example:**
```plaintext
count ← 0
loop while count < 5
   output count
   count ← count + 1
end loop
```

### 3.2. FOR Loop

```plaintext
for i ← start to end
   statements
end for
```

**Example:**
```plaintext
for i ← 1 to 10
   output i
end for
```

---

## 4. Arrays and Matrices

### 4.1. One-dimensional Arrays

**Declaration:**
```plaintext
arr ← [0, 0, 0, 0, 0]
```

**Access:**
```plaintext
arr[index] ← value
output arr[index]
```

### 4.2. Two-dimensional Arrays

**Declaration:**
```plaintext
matrix ← [[0, 0], [0, 0]]
```

**Access:**
```plaintext
matrix[row][column] ← value
output matrix[row][column]
```
