
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.
2. Define a class named 'details'.
3. Inside the class, define a parameterized constructor (__init__) that takes 'name' and 'userid' as parameters.
4. Assign these parameters to instance variables self.name and self.userid.
5. Define a method 'view()' that prints the userid.
6. Prompt the user to input name and userid.
7. Create an object of the class 'details' using the inputs.
8. Call the 'view()' method on the object to display the userid.
9. End the program.


---

### PROGRAM

```python

# Name: Nidhish B
# Reg No: 212223050032

class details:
    def __init__(self,name,userid):
        self.name=name
        self.userid=userid
    def view(self):
        print(f"{self.userid}")
name=input()
userid=input()
obj=details(name,userid)
obj.view()

```

### OUTPUT

![image](https://github.com/user-attachments/assets/41868920-9f5a-45c6-b2d8-7ea22db241d7)


### RESULT

The Python program successfully uses a parameterized constructor to initialize and print the userid of a person.

