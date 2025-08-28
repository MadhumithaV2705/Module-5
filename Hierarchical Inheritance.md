# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. Define a base class `Details` with methods to initialize and get basic details.
3. Define derived classes `employee` and `doc` that inherit from `Details`, with methods to get and display their specific details.
4. Create objects of `employee` and `doc`, call their input and display methods.
5. **Terminate the program.**


---

### PROGRAM
```
Reg.No: 212223060145
Name: Madhumitha V

class Details:
    def __init__(self):
        self.id=0
        self.name=''
        self.gender=''
    def get_details(self):
        self.id=int(input())
        self.name=input()
        self.gender=input()
        
class employee(Details): #Inheritance
    def __init__(self):
        super().__init__()
        self.com=''
        self.dept=''
    def get_emp(self):
        self.get_details()
        self.com=input()
        self.dept=input()
    def display_employee(self):
        print("Employee Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Company: ", self.com)
        print("Department: ", self.dept)

class doc(Details): #Inheritance
    def __init__(self):
        super().__init__()
        self.hospital=''
        self.department=''
    def get_doc(self):
        self.get_details()
        self.hospital=input()
        self.department=input()
    def display(self):
        print("\nDoctor Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)


emp=employee()
emp.get_emp()
emp.display_employee()
d=doc()
d.get_doc()
d.display()

```

### OUTPUT  
<img width="882" height="439" alt="image" src="https://github.com/user-attachments/assets/b2bf3a24-1537-4972-81f7-9aa03be92f07" />

### RESULT
Thus , a Python program to get the employee and doctor details and display them using hierarchical inheritance are verified.
