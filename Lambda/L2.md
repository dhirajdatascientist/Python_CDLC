## Lambda VS Traditional Function Examples

**1. Adding two numbers:**

Regular Function:
```python
def add(x, y):
    return x + y

result = add(3, 5)
```

Lambda Function:
```python
add = lambda x, y: x + y
result = add(3, 5)
```

**2. Squaring a number:**

Regular Function:
```python
def square(x):
    return x ** 2

result = square(4)
```

Lambda Function:
```python
square = lambda x: x ** 2
result = square(4)
```

**3. Checking if a number is even:**

Regular Function:
```python
def is_even(x):
    return x % 2 == 0

result = is_even(6)
```

Lambda Function:
```python
is_even = lambda x: x % 2 == 0
result = is_even(6)
```

**4. Reversing a string:**

Regular Function:
```python
def reverse_string(s):
    return s[::-1]

result = reverse_string("hello")
```

Lambda Function:
```python
reverse_string = lambda s: s[::-1]
result = reverse_string("hello")
```

**5. Calculating the square root:**

Regular Function:
```python
import math

def sqrt(x):
    return math.sqrt(x)

result = sqrt(25)
```

Lambda Function:
```python
import math

sqrt = lambda x: math.sqrt(x)
result = sqrt(25)
```

**6. Finding the maximum of two numbers:**

Regular Function:
```python
def max_of_two(x, y):
    return x if x > y else y

result = max_of_two(7, 3)
```

Lambda Function:
```python
max_of_two = lambda x, y: x if x > y else y
result = max_of_two(7, 3)
```

**7. Adding three numbers:**

Regular Function:
```python
def add_three(x, y, z):
    return x + y + z

result = add_three(2, 3, 4)
```

Lambda Function:
```python
add_three = lambda x, y, z: x + y + z
result = add_three(2, 3, 4)
```

**8. Checking if a string is a palindrome:**

Regular Function:
```python
def is_palindrome(s):
    return s == s[::-1]

result = is_palindrome("racecar")
```

Lambda Function:
```python
is_palindrome = lambda s: s == s[::-1]
result = is_palindrome("racecar")
```

**9. Generating a list of squares:**

Regular Function:
```python
def generate_squares(n):
    squares = []
    for i in range(n):
        squares.append(i ** 2)
    return squares

result = generate_squares(5)
```

Lambda Function:
```python
generate_squares = lambda n: [i ** 2 for i in range(n)]
result = generate_squares(5)
```

**10. Checking if a list contains an even number:**

Regular Function:
```python
def contains_even(lst):
    for num in lst:
        if num % 2 == 0:
            return True
    return False

result = contains_even([1, 3, 5, 4, 7])
```

Lambda Function:
```python
contains_even = lambda lst: any(num % 2 == 0 for num in lst)
result = contains_even([1, 3, 5, 4, 7])
```
