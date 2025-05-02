# Exp.No:29  
## Encapsulation

---

### AIM  
To write a Python program to create a class `Student` with the private members `name` and `age`, and add getter and setter methods to initialize and modify the `age` variable.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the `Student` class.**
   - Inside the `Student` class, define the `__init__` method to initialize `name` and the private member `__age`.
3. **Define a getter method** `get_age` to return the value of the private member `__age`.
4. **Define a setter method** `set_age` to set a new value to the private member `__age`.
5. **Create an object `stud`** of the `Student` class with the name 'Jessa' and age 14.
6. **Print the name and the age** of `stud` using the getter method.
7. **Use the setter method** `set_age` to change the age of `stud` to 16.
8. **Print the name and the updated age** of `stud` using the getter method.
9. **End the program.**

---

### PROGRAM

```
class Student:
    def __init__(self, name, age):
        """Initialize the Student with name and age."""
        self.name = name
        self._age = age  # Private variable with a leading underscore

    # Getter method for age
    def get_age(self):
        return self._age

    # Setter method for age
    def set_age(self, age):
        if age >= 0:
            self._age = age
        else:
            print("Age cannot be negative.")

    # Getter method for name (optional)
    def get_name(self):
        return self.name

    # Setter method for name (optional)
    def set_name(self, name):
        self.name = name

# Create a Student object
student = Student("Alice", 20)

# Get the name and age of the student
print(f"Student Name: {student.get_name()}")
print(f"Student Age: {student.get_age()}")

# Modify the age using the setter method
student.set_age(25)

# Try setting an invalid age
student.set_age(-5)

# Get the updated age of the student
print(f"Updated Student Age: {student.get_age()}")




```

### OUTPUT
class Student:
    def __init__(self, name, age):
        """Initialize the Student with name and age."""
        self.name = name
        self._age = age  # Private variable with a leading underscore

    # Getter method for age
    def get_age(self):
        return self._age

    # Setter method for age
    def set_age(self, age):
        if age >= 0:
            self._age = age
        else:
            print("Age cannot be negative.")

    # Getter method for name (optional)
    def get_name(self):
        return self.name

    # Setter method for name (optional)
    def set_name(self, name):
        self.name = name
### OUTPUT
![image](https://github.com/user-attachments/assets/bcb52821-a525-44e6-8d18-9d4b12a40a34)



### RESULT
thus the program is executed successfully


