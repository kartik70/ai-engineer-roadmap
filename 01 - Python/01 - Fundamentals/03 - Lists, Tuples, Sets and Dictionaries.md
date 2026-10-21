# Python Fundamentals — 03: Collections

## 1. Lists
- Ordered, mutable collection.
- Allows duplicate values.
- Similar to JavaScript arrays.

```python
numbers = [10, 20, 30]
numbers.append(40)
numbers.insert(1, 15)
numbers.remove(20)
```

Useful methods:
- append(x): add one item to the end
- extend(iterable): add items from an iterable
- insert(i, x): insert at an index
- remove(x): remove first matching value
- pop(i): remove and return an item
- sort(): sort in place
- reverse(): reverse in place

Slicing:
```python
numbers = [10, 20, 30, 40, 50]
numbers[1:4]  # [20, 30, 40]
numbers[::-1] # reversed copy
```

Slicing creates a new list and takes O(k) time and space for k selected elements.

List comprehension:
```python
squares = [n*n for n in range(5)]
evens = [n for n in range(10) if n % 2 == 0]
```

## 2. Tuples
- Ordered, immutable collection.
- Allows duplicates.
- Supports indexing and unpacking.
- Useful for fixed groups of values and returning multiple values.

```python
coordinates = (10, 20)
x, y = coordinates
```

A tuple can contain mutable objects. Those inner objects can still be modified.

## 3. Sets
- Unordered collection of unique, hashable elements.
- Mutable.
- Useful for deduplication and fast membership checks.

```python
numbers = {1, 2, 2, 3}
numbers.add(4)
numbers.discard(10)
```

Set operations:
- a | b: union
- a & b: intersection
- a - b: difference
- a ^ b: symmetric difference

Membership lookup is O(1) on average.

## 4. Dictionaries
- Mutable mapping of keys to values.
- Preserves insertion order.
- Keys must be hashable.
- Similar to JavaScript objects or Maps.

```python
user = {"name": "Kartik", "age": 26}
user["role"] = "Developer"
age = user.get("age", 0)
```

Useful methods:
- keys()
- values()
- items()
- get()
- pop()
- update()
- clear()

Average dictionary lookup, insertion, and deletion are O(1).

## 5. Collection comparison

| Feature | List | Tuple | Set | Dict |
|---|---|---|---|---|
| Ordered | Yes | Yes | No | Yes |
| Mutable | Yes | No | Yes | Yes |
| Duplicates | Yes | Yes | No | Keys unique |
| Indexing | Yes | Yes | No | Key-based |
| Average lookup | O(n) | O(n) | O(1) | O(1) |

## 6. DSA patterns

### Duplicate detection
Use a set to track previously seen values. Average O(n) time.

### Frequency counting
Use a dictionary to count occurrences. Average O(n) time.

```python
frequency = {}
for n in numbers:
    frequency[n] = frequency.get(n, 0) + 1
```

## 7. Interview questions
1. List vs tuple: what is the difference?
2. Why are sets useful for duplicate detection?
3. What is the difference between append() and extend()?
4. Why use dict.get() instead of direct indexing?
5. What makes a dictionary key hashable?
6. What is the average time complexity of dictionary lookup?
7. What is the difference between mutating and reassigning a collection?

## 8. My doubts and learnings
Add questions and answers from the tutorial here.

## 9. Practice
- [ ] Perform list insertions and deletions.
- [ ] Remove duplicates using a set.
- [ ] Count frequencies using a dictionary.
- [ ] Explain the time complexity of common operations.