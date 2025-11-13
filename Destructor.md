# Exp.No:22  
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

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A

class Student:
    def __init__(self):
        print("Constructor is called. Object created successfully.")

    def __del__(self):
        print("Destructor is called. Object destroyed successfully.")

# Creating object
s2 = Student()

# Deleting object
del s2

```

### OUTPUT
```
Constructor is called. Object created successfully.
Destructor is called. Object destroyed successfully.

```

### RESULT
Thus, the Python program using a destructor has been successfully executed.
