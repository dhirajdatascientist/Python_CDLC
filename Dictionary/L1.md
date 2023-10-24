## Dictionaries in Python (L1)

1. **What is a dictionary in Python?**
   - A dictionary in Python is an unordered collection of key-value pairs. It allows you to store and retrieve data using keys. Dictionaries are created using curly braces `{}` or the `dict()` constructor.

2. **How to create a dictionary?**
   - You can create a dictionary in Python by specifying key-value pairs within curly braces or using the `dict()` constructor:
     ```python
     my_dict = {'name': 'Alice', 'age': 30}
     ```

3. **Accessing values in a dictionary:**
   - Values in a dictionary are accessed by specifying the key within square brackets:
     ```python
     name = my_dict['name']  # Retrieves the value associated with the key 'name'
     ```

4. **Modifying values in a dictionary:**
   - You can change the value associated with a key by assigning a new value to it:
     ```python
     my_dict['age'] = 31  # Updates the age to 31
     ```

5. **Adding new key-value pairs:**
   - To add a new key-value pair to a dictionary, you can simply assign a value to a new key:
     ```python
     my_dict['city'] = 'New York'  # Adds a new key 'city' with the value 'New York'
     ```

6. **Removing key-value pairs:**
   - You can remove a key-value pair from a dictionary using the `del` statement:
     ```python
     del my_dict['age']  # Removes the key 'age' and its associated value
     ```

7. **Checking if a key exists:**
   - To check if a key exists in a dictionary, you can use the `in` keyword:
     ```python
     is_present = 'age' in my_dict  # Checks if 'age' is a key in the dictionary
     ```

8. **Iterating through a dictionary:**
   - You can use loops (e.g., `for` loop) to iterate through keys, values, or key-value pairs of a dictionary:
     ```python
     for key in my_dict:
         print(key, my_dict[key])
     ```

9. **Common use cases for dictionaries:**
   - Dictionaries are commonly used for storing and retrieving data that is organized by keys, such as configuration settings, database records, or JSON-like data.

10. **Dictionary comprehension:**
    - Dictionary comprehensions allow you to create dictionaries based on existing dictionaries or other iterable objects:
      ```python
      squared_dict = {key: value ** 2 for key, value in my_dict.items()}
      ```
