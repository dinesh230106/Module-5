# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

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
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A

class Student:
    def __init__(self, name, student_id):
        self.name = name
        self.student_id = student_id

class Record:
    def __init__(self, attendance):
        self.attendance = attendance

class Eligibility(Student, Record):
    def __init__(self, name, student_id, attendance):
        Student.__init__(self, name, student_id)
        Record.__init__(self, attendance)

    def check_eligibility(self):
        print("\n--- Student Details ---")
        print("Name:", self.name)
        print("Student ID:", self.student_id)
        print("Attendance:", self.attendance, "%")
        if self.attendance > 80:
            print("Result: Eligible for next module.")
        else:
            print("Result: Not eligible for next module.")

# Getting input from user
name = input("Enter Student Name: ")
student_id = int(input("Enter Student ID: "))
attendance = int(input("Enter Attendance Percentage: "))

# Creating object
student = Eligibility(name, student_id, attendance)

# Checking eligibility
student.check_eligibility()

```

### OUTPUT
```

Enter Student Name: Karthik
Enter Student ID: 102
Enter Attendance Percentage: 85

--- Student Details ---
Name: Karthik
Student ID: 102
Attendance: 85 %
Result: Eligible for next module.

```


### RESULT
Thus, the Python program to check a student’s eligibility for the next module using Multiple Inheritance has been successfully executed.




