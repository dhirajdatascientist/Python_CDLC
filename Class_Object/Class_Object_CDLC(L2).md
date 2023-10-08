## Examples on Class and objects

1. **Creating a Class:**
   ```python
   class Dog:
       pass
   ```

2. **Creating an Object:**
   ```python
   my_dog = Dog()
   ```

3. **Adding Attributes to Objects:**
   ```python
   my_dog.name = "Buddy"
   my_dog.age = 3
   ```

4. **Defining a Constructor (Initializer) Method:**
   ```python
   class Dog:
       def __init__(self, name, age):
           self.name = name
           self.age = age

   my_dog = Dog("Buddy", 3)
   ```

5. **Accessing Object Attributes:**
   ```python
   print(my_dog.name)
   print(my_dog.age)
   ```

6. **Adding Methods to a Class:**
   ```python
   class Dog:
       def __init__(self, name, age):
           self.name = name
           self.age = age

       def bark(self):
           print(f"{self.name} says Woof!")

   my_dog = Dog("Buddy", 3)
   my_dog.bark()
   ```

7. **Creating Multiple Objects from the Same Class:**
   ```python
   dog1 = Dog("Buddy", 3)
   dog2 = Dog("Max", 2)
   ```

8. **Using Class Variables:**
   ```python
   class Dog:
       species = "Canis familiaris"

       def __init__(self, name, age):
           self.name = name
           self.age = age

   my_dog = Dog("Buddy", 3)
   print(f"{my_dog.name} is a {my_dog.species}")
   ```

9. **Inheritance - Creating a Subclass:**
   ```python
   class Labrador(Dog):
       def __init__(self, name, age, color):
           super().__init__(name, age)
           self.color = color

   my_labrador = Labrador("Max", 2, "Yellow")
   ```

10. **Using Methods in a Subclass:**
    ```python
    class Labrador(Dog):
        def __init__(self, name, age, color):
            super().__init__(name, age)
            self.color = color

        def fetch(self):
            print(f"{self.name} is fetching a ball!")

    my_labrador = Labrador("Max", 2, "Yellow")
    my_labrador.fetch()
    ```