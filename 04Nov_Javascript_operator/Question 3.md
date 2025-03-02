

### 1. **Unary Operators**
Unary operators work on a single operand (i.e., they perform an operation on one value). They typically perform operations such as incrementing, negating, or checking the type of a value.

- **Examples:**
  - `++` (Increment)
  - `--` (Decrement)
  - `+` (Unary plus, often used to convert a string to a number)
  - `-` (Unary negation, often used to convert a number to a negative value)
  - `typeof` (Returns the type of a variable)
  - `delete` (Deletes a property from an object)
  - `void` (Evaluates an expression and returns `undefined`)

**Example:**
```javascript
let a = 5;
console.log(++a);  // 6 (increments a by 1)
console.log(--a);  // 5 (decrements a by 1)

let b = '10';
console.log(+b);   // 10 (converts the string '10' to the number 10)

let obj = { name: "Alice" };
delete obj.name;  // deletes the 'name' property from the object
console.log(obj);  // {} (empty object)
```

---

### 2. **Binary Operators**
Binary operators operate on **two operands**. These are the most common operators in JavaScript and are used for a variety of tasks such as arithmetic, comparison, and logical operations.

- **Examples:**
  - Arithmetic operators: `+`, `-`, `*`, `/`, `%`, `**`
  - Comparison operators: `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=`
  - Logical operators: `&&` (AND), `||` (OR)
  - Assignment operators: `=`, `+=`, `-=`, `*=`, `/=`

**Example:**
```javascript
let x = 10, y = 5;
console.log(x + y);   // 15 (addition)
console.log(x - y);   // 5 (subtraction)
console.log(x * y);   // 50 (multiplication)
console.log(x / y);   // 2 (division)
console.log(x > y);   // true (comparison)
console.log(x && y);  // 5 (logical AND, returns the second operand if both are truthy)

let z = 2;
z += 3;  // z = z + 3
console.log(z); // 5 (assignment)
```

---

### 3. **Ternary Operator**
The ternary operator is a **conditional operator** that operates on **three operands**. It is a shorthand for an `if-else` statement. It evaluates a condition and returns one of two values depending on whether the condition is `true` or `false`.

- **Syntax:** 
  ```javascript
  condition ? expression1 : expression2;
  ```
  If the condition is true, `expression1` is executed; otherwise, `expression2` is executed.

- **Example:**
```javascript
let age = 18;
let canVote = (age >= 18) ? "Yes, you can vote" : "No, you're too young";
console.log(canVote);  // "Yes, you can vote"

let number = 0;
let result = (number > 0) ? "Positive" : (number < 0) ? "Negative" : "Zero";
console.log(result);   // "Zero"
```

In the second example, notice how you can use a **nested ternary operator** to handle multiple conditions in a compact form.

---

