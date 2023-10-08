## Class_Object_CDLC(L1)

**Classes** in Python are a blueprint or template for creating objects. They define the structure and behavior of objects by specifying attributes (data members) and methods (functions) that the objects of the class will have. Classes allow you to create custom data types with their own characteristics and behaviors.

**Objects**, on the other hand, are instances of classes. They are concrete instances created from the class blueprint, with their own unique data values for the attributes. Objects can also invoke the methods defined in the class, allowing them to perform actions or operations related to their data.

## Syntax and Examples

1. **Class Definition:**
   ```python
   class MyClass:
   ```

2. **Creating an Object (Instance):**
   ```python
   my_object = MyClass()
   ```

3. **Attributes (Data Members) in a Class:**
   ```python
   class MyClass:
       attribute1 = "Hello"
       attribute2 = 42
   ```

4. **Accessing Class Attributes through an Object:**
   ```python
   print(my_object.attribute1)
   ```

5. **Methods (Functions) in a Class:**
   ```python
   class MyClass:
       def my_method(self):
           print("This is a method.")
   ```

6. **Calling a Method through an Object:**
   ```python
   my_object.my_method()
   ```

7. **Constructor Method (`__init__`):**
   ```python
   class MyClass:
       def __init__(self, param1, param2):
           self.param1 = param1
           self.param2 = param2
   ```

8. **Creating an Object with Constructor Arguments:**
   ```python
   my_object = MyClass("Value1", 123)
   ```

9. **Accessing Constructor Parameters through an Object:**
   ```python
   print(my_object.param1)
   ```

10. **Inheritance - Creating a Subclass:**
    ```python
    class MySubclass(MyClass):
        def my_sub_method(self):
            print("This is a subclass method.")
    ```

