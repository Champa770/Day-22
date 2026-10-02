## Operators & Conditionals

**Arithmetic operators**

```jsx
let a = 10, b = 3;

console.log(a + b);   // 13 — addition
console.log(a - b);   // 7  — subtraction
console.log(a * b);   // 30 — multiplication
console.log(a / b);   // 3.333... — division
console.log(a % b);   // 1  — modulus (remainder after division)
console.log(a ** b);  // 1000 — exponent (10 to the power 3)
```

`%` (modulus) comes up constantly — e.g. checking even/odd: `num % 2 === 0`.

**Increment / decrement**

```jsx
let count = 5;
``````jsx
count++;   // count is now 6
count--;   // count is now 5 again
```

**Assignment operators — shorthand**

```jsx
let x = 10;
x += 5;   // same as x = x + 5  → 15
x -= 3;   // same as x = x - 3  → 12
x *= 2;   // same as x = x * 2  → 24
x /= 4;   // same as x = x / 4  → 6
```

---

**Comparison operators**

```jsx
console.log(5 == "5");    // true  — loose equality, converts types before comparing
console.log(5 === "5");   // false — strict equality, checks value AND type
console.log(5 != "5");    // false — loose not-equal
console.log(5 !== "5");   // true  — strict not-equal

console.log(10 > 5);    // true
console.log(10 < 5);    // false
console.log(10 >= 10);  // true
console.log(10 <= 9);   // false
```

**Always use `===` and `!==` — never `==`/`!=`**This is one of the most repeated JS best practices — `==` causes subtle bugs from unexpected type conversion. Strict equality (`===`) should be the default habit from day one.

---

**Logical operators**

```jsx
console.log(true && false);   // false — AND, both must be true
console.log(true || false);   // true  — OR, at least one must be true
console.log(!true);           // false — NOT, flips the boolean
```

Practical example:

```jsx
let age = 20;
let hasID = true;

if (age >= 18 && hasID) {
  console.log("Entry allowed");
}
```

---

**Conditionals — `if` / `else if` / `else`**Conditions are checked top to bottom — the first one that's `true` runs, the rest are skipped entirely.

**Truthy and falsy values — important concept**

Every value in JS is "truthy" or "falsy" when used in a condition, even if it's not an actual boolean.

```jsx
// Falsy values — only these:
false, 0, "", null, undefined, NaN

// Everything else is truthy, including:
"0"    // truthy — it's a non-empty string
[]     // truthy — empty array
{}     // truthy — empty object
```Conditions are checked top to bottom — the first one that's `true` runs, the rest are skipped entirely.

**Truthy and falsy values — important concept**

Every value in JS is "truthy" or "falsy" when used in a condition, even if it's not an actual boolean.

```jsx
// Falsy values — only these:
false, 0, "", null, undefined, NaN

// Everything else is truthy, including:
"0"    // truthy — it's a non-empty string
[]     // truthy — empty array
{}     // truthy — empty object
```# Day-22
js 2 Operators &amp; Conditionals
