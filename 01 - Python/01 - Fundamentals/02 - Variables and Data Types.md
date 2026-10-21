# Python Fundamentals — 02: Variables and Data Types

## 1. Variables
A variable is a name that refers to an object.

```python
age = 26
age = "twenty-six"
```

Python is dynamically typed. A variable can refer to objects of different types during execution.

## 2. Basic data types

| Type | Description | Example |
|---|---|---|
| int | Whole numbers | 10, -5, 0 |
| float | Floating-point numbers | 3.14, 10.0 |
| str | Text | "Kartik" |
| bool | Truth values | True, False |
| NoneType | Absence of a value | None |

Use type(value) to inspect a value's type and isinstance(value, type) to check its type.

## 3. Strings
Strings can use single or double quotes.

```python
name = "Kartik"
print(f"Hello, {name}")
```

f-strings are a convenient way to format strings using variables and expressions inside curly braces.

Strings are immutable.

## 4. Type conversion

| Function | Example |
|---|---|
| int() | int("25") |
| float() | float("3.14") |
| str() | str(25) |
| bool() | bool(1) |

input() returns a string. Convert it when numeric input is needed.

Invalid conversions can raise ValueError.

## 5. Truthiness
Falsy values include:
- False
- None
- 0
- 0.0
- Empty strings
- Empty collections

Non-empty strings are truthy, even when their contents are "False" or "0".

## 6. Mutable vs immutable
Immutable objects cannot be changed after creation.
Examples: int, float, str, bool, NoneType.

Mutable objects can be modified in place. Lists and dictionaries are examples.

Reassigning a variable is not the same as mutating an object.

## 7. Python vs JavaScript

| Python | JavaScript |
|---|---|
| int and float | number |
| str | string |
| bool | boolean |
| None | null (rough equivalent) |
| type() | typeof |
| int() | Number() / parseInt() |

Python's / operator performs true division and returns a float.

## 8. Interview questions
1. What does dynamically typed mean?
2. What is the difference between int and float?
3. Why does bool("False") return True?
4. What is the difference between None and False?
5. What is the difference between mutability and reassignment?
6. Why can 0.1 + 0.2 produce a precision artifact?

## 9. My doubts and learnings
Add explanations for any questions that arise during practice.

## 10. Practice
- [ ] Identify the types of different values.
- [ ] Convert strings to numbers.
- [ ] Use f-strings.
- [ ] Explain truthiness.
- [ ] Explain mutable vs immutable values.