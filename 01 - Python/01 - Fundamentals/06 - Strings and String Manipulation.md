# Strings and String Manipulation

## 1. What is a string?

A string (`str`) is an immutable sequence of Unicode characters.

```python
name = "Kartik"
message = 'Hello'
multiline = """Hello
Python"""
```

## 2. String indexing

Indexing starts at 0. Negative indexes count from the end.

```python
word = "Python"

print(word[0])   # P
print(word[-1])  # n
```

## 3. String slicing

Syntax: `string[start:stop:step]`

- Start is inclusive.
    
- Stop is exclusive.
    
- Step controls the increment.
    

```python
word = "Python"

print(word[0:3])  # Pyt
print(word[:4])   # Pyth
print(word[2:])   # thon
print(word[::-1]) # nohtyP
```

Slicing creates a new string. A slice of length k takes O(k) time and space.

## 4. Common string methods

|Method|Purpose|
|---|---|
|`lower()`|Convert to lowercase|
|`upper()`|Convert to uppercase|
|`capitalize()`|Capitalize first character|
|`title()`|Capitalize each word|
|`strip()`|Remove surrounding whitespace|
|`replace(old, new)`|Replace occurrences|
|`find(sub)`|Find first occurrence; -1 if missing|
|`count(sub)`|Count occurrences|
|`startswith(prefix)`|Check prefix|
|`endswith(suffix)`|Check suffix|

Most string methods return new strings rather than modifying the original.

## 5. String immutability

Strings cannot be modified in place.

```python
word = "Python"
# word[0] = "J"  # TypeError

word = "J" + word[1:]
print(word)  # Jython
```

## 6. f-strings

Use f-strings to insert variables and expressions into strings.

```python
name = "Kartik"
age = 26

print(f"My name is {name}, age {age}")
print(f"Price: {123.456:.2f}")
```

## 7. split() and join()

`split()` divides a string into a list.

```python
text = "apple,banana,mango"
fruits = text.split(",")
```

`join()` combines an iterable of strings.

```python
words = ["Python", "is", "useful"]
sentence = " ".join(words)
```

## 8. Common DSA examples

### Reverse a string

```python
def reverse_string(text):
    return text[::-1]
```

### Count vowels

```python
def count_vowels(text):
    vowels = "aeiou"
    count = 0

    for char in text.lower():
        if char in vowels:
            count += 1

    return count
```

### Check palindrome

```python
def is_palindrome(text):
    return text == text[::-1]
```

These solutions use slicing and iteration. Later, two-pointer techniques can solve some of these problems without creating reversed copies.

## 9. Python vs JavaScript

|Python|JavaScript|
|---|---|
|`len(s)`|`s.length`|
|`s.lower()`|`s.toLowerCase()`|
|`s.upper()`|`s.toUpperCase()`|
|`s.strip()`|`s.trim()`|
|`s.split(",")`|`s.split(",")`|
|`",".join(items)`|`items.join(",")`|
|`"x" in s`|`s.includes("x")`|

Both languages have immutable strings.

## Key takeaways

- Strings are immutable sequences of characters.
    
- Python supports positive and negative indexing.
    
- Slicing extracts a portion of a string.
    
- `split()` converts a string to a list.
    
- `join()` combines strings.
    
- f-strings make formatting readable.
    
- String reversal and palindrome checking are common interview problems.