# Variable
## way to using values to a variable

1. Basic assignment
Use the = operator.

```python
name = "Situ"
age = 24
height = 5.10
is_student = True
```

Here, = assigns the value on the right to the variable on the left.

2. Different ways to assign values
A. Single assignment
```python
x = 10
```



B. Multiple variables, multiple values
```python
a, b, c = 10, 20, 30
```



C. Multiple variables, same value
```python
a = b = c = 100
```



D. Unpacking a collection
```python
numbers = [10, 20, 30]
a, b, c = numbers
```



E. Assignment using an expression
```python
a = 10
b = 20
total = a + b
print(total)  # 30
```



F. Updating a variable
```python
x = 10x += 5   # x = x + 5
x -= 2   # x = x - 2
x *= 3   # x = x * 3
```



G. Taking input from the user
```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
```



Remember: input() returns a string, so use int() or float() when you need a number.

## Way to write variable

Case	Example	Common usage

Camel Case =	**studentName**    
Common in JavaScript

Pascal Case =	**StudentName**   
Common for class names

Snake Case =	**student_name**     
Recommended for Python variables

## Arithmetic operation with Assignment
Python code example

```python
x = 10x += 5
print(x)  # 15
x -= 3
print(x)  # 12
x *= 2
print(x)  # 24
x /= 4
print(x)  # 6.0
```



Remember: Each operation updates the value of x, so the next operation uses the updated value.

Special examples
```python
x = 17
x //= 5
print(x)  # 3
```



//= performs floor division.

```python
x = 17
x %= 5
print(x)  # 2
```



%= stores the remainder.

```python
x = 3x **= 3
print(x)  # 27
```



**= raises the variable to a power.