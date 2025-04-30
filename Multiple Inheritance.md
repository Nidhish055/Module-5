# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the Exam using multiple inheritance. If attendance > 75, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 75, return a formatted string indicating the student is eligible for the exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM

```python
# Name : Nidhish B
# Reg No : 212223050032

class Person:  
    def __init__(self, personName, personAge):  
        self.name = personName  
        self.age = personAge  
  
    def showName(self):  
        print(self.name)  
  
    def showAge(self):  
        print(self.age)  
   
class Student:
    def __init__(self, studentpercent):  
        self.studentpercent = studentpercent  
  
    def getpercent(self):  
        return self.studentpercent  
  
  
class Resident(Person, Student):
    def __init__(self, name, age, percent):  
        Person.__init__(self, name, age)  
        Student.__init__(self, percent)  
  
  
name=input()
age=int(input())
percent=int(input())
resident1 = Resident(name, age, percent)  
resident1.showName()  
resident1.showAge()  
if resident1.getpercent() > 75:
    print("Eligible for Exam")
else:
    print("Not Eligible for Exam")

```

### OUTPUT
![image](https://github.com/user-attachments/assets/7c95865b-9590-4cfa-8927-373b627ed59c)

### RESULT
Thus the python program to get the name, attendance, and ID of a student and check if they are eligible for the Exam using multiple inheritance are verified.

