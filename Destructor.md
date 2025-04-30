
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```python

# Name : Nidhish B
# Reg.No : 212223050032

class student:
    def __init__(self):
        print('''Inside Constructor
Object initialized
Hello, my name is Emma''')
    def __del__(self):
        print('''Inside destructor
Object destroyed''')

obj=student()
del obj
```

### OUTPUT

![image](https://github.com/user-attachments/assets/70156fb6-d579-4a94-bb44-c2d6821e117e)

### RESULT

The program successfully demonstrates the use of a constructor and a destructor in a Python class using the student class.
