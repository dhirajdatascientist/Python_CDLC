## Common Modules in Python (L2)

1. **What are modules in Python?**
   - Modules in Python are files containing Python definitions and statements designed to offer reusable functionality. Python offers a plethora of built-in modules that provide tools, methods, and functions to ease the development process.

2. **`math` module:**
   - Provides mathematical functions and constants:
     ```python
     import math
     print(math.sqrt(25))  # Outputs 5.0
     ```

3. **`datetime` module:**
   - Offers functions and classes to work with dates and times:
     ```python
     from datetime import datetime
     now = datetime.now()
     print(now)
     ```

4. **`os` module:**
   - Provides a way of using operating system dependent functionality, like reading or writing to the file system:
     ```python
     import os
     print(os.getcwd())  # Outputs the current working directory
     ```

5. **`sys` module:**
   - Grants access to some interpreter variables and functions directly related to the interpreter:
     ```python
     import sys
     sys.exit()  # Exits the script
     ```

6. **`re` module:**
   - Offers functions to work with regular expressions:
     ```python
     import re
     match = re.search('world', 'Hello world!')
     print(match.group())  # Outputs 'world'
     ```

7. **`json` module:**
   - Provides methods to encode and decode JSON data:
     ```python
     import json
     data = {'name': 'John', 'age': 30}
     json_str = json.dumps(data)
     ```

8. **`random` module:**
   - Contains functions to generate random numbers and choices:
     ```python
     import random
     print(random.randint(1, 10))  # Outputs a random integer between 1 and 10
     ```

9. **`collections` module:**
   - Implements several specialized container datatypes:
     ```python
     from collections import Counter
     count = Counter(['a', 'b', 'a', 'c', 'b', 'b', 'a'])
     print(count)  # Outputs Counter({'a': 3, 'b': 3, 'c': 1})
     ```

10. **`urllib` module:**
    - Provides a collection of modules to work with URLs:
      ```python
      from urllib.request import urlopen
      response = urlopen('https://www.example.com/')
      ```
