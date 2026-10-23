# Datatype
**Numeric types**

Python has three built-in numeric types.
```python
a = 10          # int
b = 10.5        # float
c = 2 + 3j      # complex

print(type(a))  # <class 'int'>
print(type(b))  # <class 'float'>
print(type(c))  # <class 'complex'>
```
**Boolean type (bool)**

Represents logical truth values.
```python
is_student = True
is_working = False

print(type(is_student))  # <class 'bool'>
print(10 > 5)            # True
print(10 < 5)            # False
```

**String type (str)**

Stores text inside single, double, or triple quotes.

```python
name = "Situ"
language = 'Python'
message = """Welcome to Python"""

print(type(name))  # <class 'str'>
print(name)        # Situ
```


**Sequence types**

**A. List (list)**
An ordered, mutable collection that allows duplicate values.
```python
numbers = [10, 20, 30, 20]
numbers[0] = 100
print(numbers)  # [100, 20, 30, 20]
```



**B. Tuple (tuple)**
An ordered, immutable collection that allows duplicates.
```python
coordinates = (10, 20, 30)
print(coordinates[0])  # 10print(type(coordinates))  # <class 'tuple'>
```



**C. Range (range)**
Represents a sequence of integers, commonly used in loops.
```python
numbers = range(1, 5)
print(list(numbers))  # [1, 2, 3, 4]
```
**Mapping type (dict)**
Stores data as key-value pairs. Dictionaries are mutable.

```python
student = {
    "name": "Situ",
    "age": 24,
    "course": "MCA"
}

print(student["name"])  # Situ
print(type(student))    # <class 'dict'>
```
**Set types**

**A. Set (set)**
An unordered collection of unique elements.
```python
numbers = {10, 20, 30, 20}
print(numbers)  # {10, 20, 30}
```



Duplicate values are automatically removed. The printed order is not guaranteed.

**B. Frozen set (frozenset)**
An immutable set.
```python
numbers = frozenset([10, 20, 30])
print(numbers)
print(type(numbers))  # <class 'frozenset'>
```



You cannot add or remove elements from a frozenset.

**Binary types**

These types are useful when working with binary data, files, and networking.

```python
a = bytes([65, 66, 67])
b = bytearray([65, 66, 67])
c = memoryview(bytes([65, 66, 67]))

print(a)       # b'ABC'
print(type(b)) # <class 'bytearray'>
print(type(c)) # <class 'memoryview'>
```

**None type (NoneType)**
Represents the absence of a value.

```python
result = None

print(result)       # None
print(type(result)) # <class 'NoneType'>
```


# Operator

## Arithmetic Operators
Used to perform mathematical calculations.
```python
a = 10b = 3print(a + b)   # 13  
Additionprint(a - b)   # 7   
Subtractionprint(a * b)   # 30  
Multiplicationprint(a / b)   # 3.333... 
Divisionprint(a // b)  # 3   
Floor divisionprint(a % b)   # 1   
Modulus (remainder)
print(a ** b)  # 1000 Exponentiation
```



## Comparison Operators
Compare two values and return True or False.

```python
print(5 == 5)   # True  Equal
print(5 != 3)   # True  Not equal
print(5 > 3)    # True  Greater than
print(5 < 3)    # False Less than
print(5 >= 5)   # True  Greater than or equal
print(3 <= 5)   # True  Less than or equal
```



also shows these Python comparisons:
```python
print(1 == 2)       # False
print(1.0 == 1)     # True
print('A' == 'a')   # False
print(True == 1)    # True
print(False == 0)   # True
```



Why? Python considers 1.0 equal to 1, and True equal to 1, while False equals 0. String comparisons are case-sensitive.
## Assignment Operators
Assign or update variable values.

```python
x = 10x += 5     # x = x + 5  -> 15
x -= 2     # x = x - 2  -> 13
x *= 2     # x = x * 2  -> 26
x /= 2     # x = x / 2  -> 13.0
x //= 3    # x = x // 3 -> 4.0
x %= 3     # x = x % 3  -> 1.0
x **= 2    # x = x ** 2 -> 1.0print(x)
```



Other assignment forms include &=, |=, ^=, >>=, and <<= for bitwise operations.
## Logical Operators
Combine or reverse conditions.
```python
x = 10
print(x > 5 and x < 20)  # True
print(x < 5 or x == 10)  # True
print(not x > 5)         # False
```



- and — True when both conditions are true.
- or — True when at least one condition is true.
- not — Reverses the truth value.
## Bitwise Operators
Operate on the binary bits of integers.
```python
a = 5  # Binary: 0101
b = 3  # Binary: 0011
print(a & b)   # 1  AND
print(a | b)   # 7  OR
print(a ^ b)   # 6  XOR
print(~a)      # -6 NOT
print(a << 1)  # 10 Left shift
print(a >> 1)  # 2  Right shift
```



## Membership Operators
Check whether a value exists in a sequence or collection.
```python
fruits = ["apple", "banana", "mango"]
print("apple" in fruits)       # Trueprint("grapes" not in fruits)  # True
```



- in — Checks whether an item exists.
- not in — Checks whether an item does not exist.
## Identity Operators
Check whether two variables refer to the same object, not merely whether their values are equal.

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]
print(a is b)      # Trueprint(a is c)      # Falseprint(a == c)      # Trueprint(a is not c)  # True
```



Remember: == compares values; is compares object identity.