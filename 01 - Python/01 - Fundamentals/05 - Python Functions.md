# Python Functions

## 1. Defining functions

Use `def` to define a reusable block of code.

```python
def greet():
    print("Hello")

greet()
```

- `def` defines the function.
    
- The function body is indented.
    
- Calling the function executes its body.
    

## 2. Parameters and arguments

- Parameters are variables in the function definition.
    
- Arguments are values passed when calling the function.
    

```python
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
```

## 3. return vs print

- `print()` displays a value.
    
- `return` sends a value back to the caller.
    
- A function without an explicit return statement returns `None`.
    

```python
def add(a, b):
    return a + b
```

Returning values makes functions reusable and easier to test.

## 4. Default arguments

Default values are used when an argument is omitted.

```python
def greet(name="Guest"):
    return f"Hello, {name}!"

print(greet())
print(greet("Kartik"))
```

Required parameters should generally appear before parameters with defaults.

## 5. Keyword arguments

Pass arguments by parameter name.

```python
def introduce(name, age):
    return f"{name} is {age}"

introduce(age=26, name="Kartik")
```

Positional arguments must come before keyword arguments when mixing the two.

## 6. *args

`*args` collects additional positional arguments into a tuple.

```python
def sum_all(*args):
    total = 0

    for number in args:
        total += number

    return total
```

## 7. **kwargs

`**kwargs` collects additional keyword arguments into a dictionary.

```python
def display_user(**kwargs):
    for key, value in kwargs.items():
        print(key, value)
```

## 8. Variable scope

- Local variables are defined inside a function.
    
- Global variables are defined outside functions.
    
- Use `global` to reassign a global variable inside a function.
    
- Prefer parameters and return values over modifying global state.
    

## 9. DSA example

```python
def find_max(numbers):
    if not numbers:
        return None

    maximum = numbers[0]

    for number in numbers:
        if number > maximum:
            maximum = number

    return maximum
```

Time complexity: O(n)  
Auxiliary space complexity: O(1)

## 10. Python vs JavaScript

|Python|JavaScript|
|---|---|
|`def`|`function`|
|`return`|`return`|
|`*args`|`...args`|
|`lambda x: x * 2`|`x => x * 2`|
|`**kwargs`|No direct equivalent|

## Key takeaways

- Use functions to organize and reuse code.
    
- Use `return` when the caller needs a result.
    
- Default arguments make parameters optional.
    
- `*args` collects positional arguments into a tuple.
    
- `**kwargs` collects keyword arguments into a dictionary.
    
- Understand local and global scope.
    
- Keep functions focused and easy to test.