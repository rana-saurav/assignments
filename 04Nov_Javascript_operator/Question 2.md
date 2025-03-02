In JavaScript, operators can be categorized based on their functionality. These categories help us understand their specific use cases and the kind of operations they perform. 

### 1. **Arithmetic Operators**
These operators are used to perform mathematical calculations.

- **Examples:**
  - `+` (Addition)
  - `-` (Subtraction)
  - `*` (Multiplication)
  - `/` (Division)
  - `%` (Modulo, remainder after division)
  - `**` (Exponentiation)

**Example:**
```javascript
let a = 5, b = 3;
console.log(a + b); // 8
console.log(a - b); // 2
console.log(a * b); // 15
console.log(a / b); // 1.666...
console.log(a % b); // 2 (remainder of 5 divided by 3)
console.log(a ** b); // 125 (5 raised to the power of 3)
```

---

### 2. **Assignment Operators**
These operators are used to assign values to variables.

- **Examples:**
  - `=` (Simple assignment)
  - `+=` (Add and assign)
  - `-=` (Subtract and assign)
  - `*=` (Multiply and assign)
  - `/=` (Divide and assign)
  - `%=` (Modulo and assign)
  - `**=` (Exponentiation and assign)

**Example:**
```javascript
let x = 5;
x += 3; // x = x + 3 → 8
x *= 2; // x = x * 2 → 16
x /= 4; // x = x / 4 → 4
```

---

### 3. **Comparison Operators**
These operators are used to compare two values or expressions. They return a boolean value (`true` or `false`).

- **Examples:**
  - `==` (Equal to)
  - `===` (Strict equal to)
  - `!=` (Not equal to)
  - `!==` (Strict not equal to)
  - `>` (Greater than)
  - `<` (Less than)
  - `>=` (Greater than or equal to)
  - `<=` (Less than or equal to)

**Example:**
```javascript
console.log(5 == '5');  // true (loose comparison, type conversion)
console.log(5 === '5'); // false (strict comparison, no type conversion)
console.log(10 > 5);    // true
console.log(4 <= 3);    // false
```

---

### 4. **Logical Operators**
These operators are used to combine multiple boolean expressions and return a boolean result.

- **Examples:**
  - `&&` (Logical AND)
  - `||` (Logical OR)
  - `!` (Logical NOT)

**Example:**
```javascript
console.log(true && false); // false
console.log(true || false); // true
console.log(!true);         // false
```

---

### 5. **Unary Operators**
Unary operators operate on a single operand and perform various operations like incrementing, negating, or determining the type of a value.

- **Examples:**
  - `++` (Increment)
  - `--` (Decrement)
  - `+` (Unary plus)
  - `-` (Unary negation)
  - `typeof` (Returns the type of a variable)
  - `delete` (Deletes a property from an object)
  - `void` (Evaluates an expression and returns `undefined`)

**Example:**
```javascript
let a = 5;
a++;   // 6
a--;   // 5
console.log(typeof a);  // "number"
```

---

### 6. **Bitwise Operators**
These operators perform operations on binary numbers (bits). They are often used for low-level programming and performance optimizations.

- **Examples:**
  - `&` (Bitwise AND)
  - `|` (Bitwise OR)
  - `^` (Bitwise XOR)
  - `~` (Bitwise NOT)
  - `<<` (Left shift)
  - `>>` (Right shift)
  - `>>>` (Unsigned right shift)

**Example:**
```javascript
let a = 5;  // binary: 0101
let b = 3;  // binary: 0011

console.log(a & b); // 1 (binary: 0001)
console.log(a | b); // 7 (binary: 0111)
console.log(a ^ b); // 6 (binary: 0110)
console.log(~a);    // -6 (bitwise NOT)
```

---

### 7. **Conditional (Ternary) Operator**
The ternary operator is a shorthand for `if-else` statements. It takes three operands and evaluates the condition.

- **Example:**
  ```javascript
  let age = 18;
  let isAdult = (age >= 18) ? "Yes" : "No";
  console.log(isAdult); // "Yes"
  ```

---

### 8. **Nullish Coalescing Operator (`??`)**
This operator returns the right-hand operand when the left-hand operand is `null` or `undefined`, otherwise it returns the left-hand operand. It’s useful for handling `null` or `undefined` values without affecting other falsy values like `0` or `false`.

- **Example:**
  ```javascript
  let name = null;
  let defaultName = name ?? "Guest"; // "Guest"
  
  let age = 0;
  let defaultAge = age ?? 25; // 0 (since age is not null or undefined)
  ```

---

### 9. **Optional Chaining Operator (`?.`)**
This operator allows you to safely access properties or methods of an object that may be `null` or `undefined`, without throwing an error.

- **Example:**
  ```javascript
  let user = { profile: { name: "Alice" } };
  console.log(user?.profile?.name);  // "Alice"
  console.log(user?.profile?.age);   // undefined (doesn't throw an error)
  ```

---

### 10. **Spread (`...`) and Rest (`...`) Operators**
Both the spread and rest operators are represented by `...`, but they serve different purposes depending on context.

- **Spread Operator**: Expands elements of an iterable (e.g., arrays or objects).
- **Rest Operator**: Collects multiple elements into a single array or object.

**Example (Spread):**
```javascript
let arr = [1, 2, 3];
let newArr = [...arr, 4]; // [1, 2, 3, 4]
```

**Example (Rest):**
```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

console.log(sum(1, 2, 3)); // 6
```

---

### 11. **Comma Operator (`,`)**
The comma operator allows multiple expressions to be evaluated in a single statement, but only the result of the last expression is returned.

- **Example:**
  ```javascript
  let x = (1, 2, 3); // x = 3
  console.log(x); // 3
  ```

---

