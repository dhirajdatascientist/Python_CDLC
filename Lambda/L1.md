## Lambda Functions in Python (L1)

1. **What is a lambda function in Python?**
   - A lambda function in Python is an anonymous and small, inline function that can take any number of arguments but can only have a single expression. It's defined using the `lambda` keyword, followed by the input parameters, a colon, and the expression to be evaluated.

2. **What is the syntax of a lambda function?**
   - The syntax of a lambda function is as follows:
     ```python
     lambda arguments: expression
     ```
     - `arguments` are the input parameters (like function arguments).
     - `expression` is a single expression that is evaluated and returned as the result.

3. **When and why should you use lambda functions?**
   - You should use lambda functions when you need a small, simple function for a short-lived purpose, especially as an argument to higher-order functions like `map()`, `filter()`, or `sorted()`.
   - They are useful for situations where creating a named function using `def` would be excessive or less readable.

4. **How do you define and use a lambda function?**
   - You define a lambda function using the `lambda` keyword, like this:
     ```python
     add = lambda x, y: x + y
     ```
     - You can then use the lambda function just like any other function:
       ```python
       result = add(3, 5)  # This will assign 8 to 'result'.
       ```

5. **Can lambda functions have multiple arguments?**
   - Yes, lambda functions can have multiple arguments. You specify these arguments after the `lambda` keyword, separated by commas.

6. **Can lambda functions have no arguments?**
   - Yes, lambda functions can have no arguments if you use an empty pair of parentheses. For example, `lambda: some_expression`.

7. **What are common use cases for lambda functions?**
   - Lambda functions are often used for simple transformations, filtering, or sorting of data in Python.
   - Common use cases include sorting a list of dictionaries by a specific key, filtering a list based on a condition, or performing a quick arithmetic operation on elements.

Here's an example of using a lambda function to sort a list of dictionaries by a specific key:

```python
data = [{'name': 'Alice', 'age': 30}, {'name': 'Bob', 'age': 25}, {'name': 'Charlie', 'age': 35}]
sorted_data = sorted(data, key=lambda x: x['age'])
print(sorted_data)
