## Examples

1. **Hello World Function:**
   ```python
   def say_hello():
       print("Hello, World!")

   say_hello()
   ```

2. **Addition Function:**
   ```python
   def add_numbers(a, b):
       return a + b

   result = add_numbers(5, 3)
   print(result)
   ```

3. **Square Function:**
   ```python
   def square(number):
       return number ** 2

   squared = square(4)
   print(squared)
   ```

4. **Check Even or Odd Function:**
   ```python
   def is_even(number):
       if number % 2 == 0:
           return True
       else:
           return False

   print(is_even(7))
   ```

5. **Max Function:**
   ```python
   def find_max(numbers):
       return max(numbers)

   numbers = [2, 9, 5, 1, 7]
   max_num = find_max(numbers)
   print(max_num)
   ```

6. **Factorial Function:**
   ```python
   def factorial(n):
       if n == 0:
           return 1
       else:
           return n * factorial(n-1)

   print(factorial(5))
   ```

7. **Concatenate Strings Function:**
   ```python
   def concatenate_strings(str1, str2):
       return str1 + " " + str2

   result = concatenate_strings("Hello", "World")
   print(result)
   ```

8. **Reverse String Function:**
   ```python
   def reverse_string(string):
       return string[::-1]

   reversed_str = reverse_string("Python")
   print(reversed_str)
   ```

9. **List Length Function:**
   ```python
   def list_length(lst):
       return len(lst)

   my_list = [1, 2, 3, 4, 5]
   length = list_length(my_list)
   print(length)
   ```

10. **Sum of List Function:**
    ```python
    def sum_list(lst):
        return sum(lst)

    my_list = [1, 2, 3, 4, 5]
    total = sum_list(my_list)
    print(total)
    ```