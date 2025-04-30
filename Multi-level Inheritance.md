
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and location of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.
2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_location`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_location` to `self.person_location`.
3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_location`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_location`.
4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_location`.
5. Prompt the user to enter `name` (string), `age` (integer), and `person_location` (integer).
6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_location` to the constructor.
7. Call the `show_details` method on the `person` object and print the result.
8. Terminate the program.

---

### PROGRAM

```python

#Name : Nidhish B
#Reg No : 212223050032

class Parent:
   def __init__(self,name):
     self.name = name
   def getName(self):
     return self.name
class Child(Parent):
   def __init__(self,name,age):
     Parent.__init__(self,name)
     self.age = age
   def getAge(self):
     return self.age
class Grandchild(Child):
   def __init__(self,name,age,location):
     Child.__init__(self,name,age)
     self.location=location
   def getLocation(self):
     return self.location
name=input()
age=int(input())
loc=input()
gc = Grandchild(name,age,loc)
print(gc.getName(), gc.getAge(), gc.getLocation())

```

### OUTPUT
![image](https://github.com/user-attachments/assets/16e8aef1-e885-44c9-9dbd-e72df5fa173b)

### RESULT
Thus the python program to get the name, age, and location of a person and display them using multilevel inheritance are verified.
