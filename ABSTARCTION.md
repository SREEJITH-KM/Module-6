# Exp.No:28  
## Abstraction

---

### AIM  
To write a Python program to define the abstract base class named `Polygon` and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the `sides()` method.

---

### ALGORITHM

1. **Start the Program.**
2. **Import the ABC class** from the `abc` module to implement abstraction.
3. **Define the abstract base class Polygon**:
   - Inherit from `ABC` (Abstract Base Class).
   - Define an abstract method `sides()` with no implementation.
4. **Define the Triangle class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Triangle has 3 sides"`.
5. **Define the Pentagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Pentagon has 5 sides"`.
6. **Define the Hexagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Hexagon has 6 sides"`.
7. **Define the Square class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"I have 4 sides"`.
8. **Create an object `t` of the Triangle class** and call the `sides()` method to print the number of sides.
9. **Create an object `s` of the Square class** and call the `sides()` method to print the number of sides.
10. **Create an object `p` of the Pentagon class** and call the `sides()` method to print the number of sides.
11. **Create an object `k` of the Hexagon class** and call the `sides()` method to print the number of sides.
12. **End the Program.**

---

### PROGRAM

```
from abc import ABC, abstractmethod

# Abstract base class
class Polygon(ABC):
    @abstractmethod
    def sides(self):
        pass

# Subclass representing a Triangle
class Triangle(Polygon):
    def sides(self):
        return 3  # A triangle has 3 sides

# Subclass representing a Rectangle
class Rectangle(Polygon):
    def sides(self):
        return 4  # A rectangle has 4 sides

# Subclass representing a Square
class Square(Rectangle):  # Square is a type of Rectangle
    def sides(self):
        return 4  # A square has 4 sides

# Subclass representing a Pentagon
class Pentagon(Polygon):
    def sides(self):
        return 5  # A pentagon has 5 sides

# Create objects of the subclasses
triangle = Triangle()
rectangle = Rectangle()
square = Square()
pentagon = Pentagon()

# Call the sides() method
print(f"Triangle has {triangle.sides()} sides.")
print(f"Rectangle has {rectangle.sides()} sides.")
print(f"Square has {square.sides()} sides.")
print(f"Pentagon has {pentagon.sides()} sides.")



```

### OUTPUT
![image](https://github.com/user-attachments/assets/806f6c3e-3967-4e4a-9ed5-ef6b1aaec9f1)



### RESULT
thus the program is executed successfully
