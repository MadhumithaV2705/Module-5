# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the Placement using multiple inheritance.

---

### ALGORITHM

1. **Begin the program.**
2. Define the `Student` class with an `__init__` method to initialize `name` and `student_id`, and a method `get_student_info()` to return student details.
3. Define the `Attendance` class that inherits from `Student`, with an `__init__` method to initialize `name`, `student_id`, and `attendance`, calling `super().__init__()` for the parent attributes.
4. Define a method `check_eligibility()` in `Attendance` to determine if the student’s attendance is greater than 80 and return the eligibility message.
5. Read `name`, `student_id`, and `attendance` from the user, create an `Attendance` object, call `check_eligibility()`, and print the result.
6. **Terminate the program.**


---

### PROGRAM
```
Reg.No: 212223060145
Name: Madhumitha V

class stu:
    def __init__(self, name):
        self.name=name
class att:
    def __init__(self, id):
        self.id=id
class placement(stu, att):
    def __init__(self, name, id, grade):
        stu.__init__(self, name)
        att.__init__(self, id)
        self.grade=grade
        
    def display(self):
        print(self.name)
        print(self.id)
        if self.grade > 90:
            print("Eligible for Placement")
        else:
            print("Not Eligible for Placement")
name=input()
id=int(input())
grade=int(input())
obj=placement(name, id, grade)
obj.display()

```

### OUTPUT
<img width="702" height="292" alt="image" src="https://github.com/user-attachments/assets/3d73a3a7-edb1-419f-aa6d-2e25e24153f8" />

### RESULT
Thus, program displays the student’s details and indicates whether they are eligible for placement based on attendance is verified successfully.



