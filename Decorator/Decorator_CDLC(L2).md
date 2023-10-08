1. **Basic Function Decorator:**
   ```python
   def my_decorator(func):
       def wrapper():
           print("Something is happening before the function is called.")
           func()
           print("Something is happening after the function is called.")
       return wrapper

   @my_decorator
   def say_hello():
       print("Hello!")

   say_hello()
   ```

2. **Function Repeater Decorator:**
   ```python
   def repeater_decorator(func):
       def wrapper():
           func()
           func()
       return wrapper

   @repeater_decorator
   def say_hello():
       print("Hello!")

   say_hello()
   ```

3. **Function Greeting Decorator:**
   ```python
   def greeting_decorator(func):
       def wrapper(name):
           print(f"Hello, {name}!")
           func(name)
           print(f"Goodbye, {name}!")
       return wrapper

   @greeting_decorator
   def say_hello(name):
       print(f"Hi, {name}!")

   say_hello("Alice")
   ```
4. **Function Divider Decorator:**
```python
def divider_decorator(func):
    def wrapper(a, b):
        if b == 0:
            print("Division by zero is not allowed.")
            return None
        else:
            return func(a, b)
    return wrapper

@divider_decorator
def divide(a, b):
    return a / b

result = divide(6, 2)
```
