# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `userid`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.userid`.  
5. Print the `self.userid`.  
6. Prompt the user to enter their `name` (string) and `userid`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `userid` to the constructor.  
8. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A

class Person:
    def __init__(self, name, userid):
        self.name = name
        self.userid = userid
        print("User ID of the person:", self.userid)

name = input("Enter your name: ")
userid = input("Enter your User ID: ")
s1 = Person(name, userid)

```

### OUTPUT
```

Enter your name: Dinesh Kumar
Enter your User ID: 212223060057
User ID of the person: 212223060057

```

### RESULT
Thus, the Python program using a parameterized constructor has been successfully executed
