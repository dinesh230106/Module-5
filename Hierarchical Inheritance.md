# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
# Reg.No: 212223060057
# Name: DINESH KUMAR A

class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_details(self):
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)

class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_details(self):
        print("Employee Object")
        super().display_details()
        print("Company: ", self.company)
        print("Department: ", self.department)

class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_details(self):
        print("Doctor Object")
        super().display_details()
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

emp_id = input()
emp_name = input()
emp_gender = input()
emp_company = input()
emp_department = input()

doc_id = input()
doc_name = input()
doc_gender = input()
doc_hospital = input()
doc_department = input()

employee = Employee(emp_id, emp_name, emp_gender, emp_company, emp_department)
doctor = Doctor(doc_id, doc_name, doc_gender, doc_hospital, doc_department)

employee.display_details()
print()
doctor.display_details()

```

### OUTPUT  
<img width="505" height="336" alt="image" src="https://github.com/user-attachments/assets/91c0d234-5dd7-42dd-b37a-b973659464bf" />


### RESULT
Thus, the Python program to display employee and doctor details using Hierarchical Inheritance has been successfully executed.
