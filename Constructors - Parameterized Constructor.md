# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.
2. Define a class `employee` with an `__init__` method to initialize `id` and `name`.
3. Define a method `display()` to print the employee's ID and name.
4. Read the employee ID and name from the user.
5. Create an object `res` of the `employee` class using the provided inputs.
6. Call the method `res.display()` to display the employee details.
7. Terminate the program.
   
---

### PROGRAM

```
Reeg.No: 212223060145
Name: Madhumitha v

class employee:
    def __init__(self,id,name):
        self.id = id
        self.name = name
    def display(self):
        print("Hello my id is :",self.id)
        print("My name is :",self.name)
id = int(input())
name = input()
res = employee(id,name)
res.display()
```

### OUTPUT
<img width="622" height="176" alt="image" src="https://github.com/user-attachments/assets/2090ecf5-67da-49fa-8362-24a948c1f8ac" />

### RESULT
Thus,a Python code to create a class for a person with a parameterized constructor are verified.
