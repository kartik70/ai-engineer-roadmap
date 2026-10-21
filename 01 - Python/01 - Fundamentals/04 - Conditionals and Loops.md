# Conditionals and Loops

## 1. Conditional statements

Conditionals allow a program to execute different code depending on whether a condition is true or false.

```python
age = 20

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

- `if`: executes when the condition is true.
    
- `elif`: checks another condition if previous conditions were false.
    
- `else`: executes if no previous condition was true.
    
- Python uses indentation to define code blocks.
    

## 2. Comparison and logical operators

|Operator|Meaning|
|---|---|
|`==`|Equal|
|`!=`|Not equal|
|`>`|Greater than|
|`<`|Less than|
|`>=`|Greater than or equal|
|`<=`|Less than or equal|
|`and`|Both conditions must be true|
|`or`|At least one condition must be true|
|`not`|Reverses a boolean|

Python uses `and`, `or`, and `not`, unlike JavaScript's `&&`, `||`, and `!`.

Python supports chained comparisons:

```python
if 18 <= age <= 60:
    print("Within range")
```

## 3. For loops

A `for` loop iterates over an iterable, such as a list, string, tuple, or range.

```python
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
```

## 4. range()

`range()` generates a sequence of integers.

```python
range(stop)
range(start, stop)
range(start, stop, step)
```

The stop value is excluded.

```python
for i in range(2, 10, 2):
    print(i)
```

Output: `2, 4, 6, 8`

## 5. enumerate()

Use `enumerate()` to iterate over both the index and value of a collection.

```python
fruits = ["apple", "banana", "mango"]

for index, fruit in enumerate(fruits, start=1):
    print(index, fruit)
```

## 6. While loops

A `while` loop repeats as long as its condition is true.

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

Ensure the condition eventually becomes false to avoid an infinite loop.

## 7. break and continue

- `break`: exits the loop immediately.
    
- `continue`: skips the rest of the current iteration.
    

```python
for number in range(1, 6):
    if number == 3:
        continue
    print(number)
```

## 8. Choosing a loop

- Use `for` to iterate over a collection or sequence.
    
- Use `while` when repetition depends on a condition.
    

## 9. DSA connection: Linear search

```python
numbers = [3, 7, 12, 5, 20]

for number in numbers:
    if number > 10:
        print(number)
        break
```

This finds the first number greater than 10. Worst-case time complexity: O(n).

## 10. Python vs JavaScript

|Python|JavaScript|
|---|---|
|`elif`|`else if`|
|`and`|`&&`|
|`or`|`|
|`not`|`!`|
|`True`|`true`|
|`False`|`false`|
|`for i in range(5)`|`for (let i = 0; i < 5; i++)`|

## Key takeaways

- Indentation defines Python code blocks.
    
- `if`, `elif`, and `else` control decisions.
    
- `for` iterates over sequences and collections.
    
- `range()` excludes the stop value.
    
- `while` repeats while a condition remains true.
    
- `break` exits a loop; `continue` skips an iteration.
    
- Linear search has O(n) worst-case time complexity.