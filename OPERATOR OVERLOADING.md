# Exp.No:27  
## Operator Overloading

---

### AIM  
To write a Python program to perform division of two complex numbers using the binary '/' operator overloading. Class name: `Complex`, where the objects `Ob1 = Complex(10, 21)` and `Ob2 = Complex(2, 3)` represent complex numbers.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the Complex class**:
   - Define the constructor `__init__()` to accept two parameters: `real` and `imag` (representing the real and imaginary parts of the complex number).
   - Assign these values to `self.real` and `self.imag` respectively.
3. **Define the `__truediv__()` method** to perform the division of two complex numbers:
   - Calculate the real part of the result as the division of `self.real` by `other.real`.
   - Calculate the imaginary part of the result as the division of `self.imag` by `other.imag`.
   - Return a new Complex object with the calculated real and imaginary parts.
4. **Define the `__repr__()` method** to represent the complex number as a string.
   - Return a string formatted to display the real and imaginary parts with one decimal place using `f"{self.real:.1f}, {self.imag:.1f}"`.
5. **Create two objects of the Complex class**:
   - `Ob1 = Complex(10, 21)` represents the complex number `10 + 21i`.
   - `Ob2 = Complex(2, 3)` represents the complex number `2 + 3i`.
6. **Perform the division operation**: Use the `/` operator to divide `Ob1` by `Ob2`. This will call the `__truediv__()` method.
7. **Print the result**: Print the result of the division, which will be formatted by the `__repr__()` method.
8. **End the Program.**

---

### PROGRAM

```
class Complex:
    def __init__(self, real, imag):
        self.real = real
        self.imag = imag

    # Overloading the division operator '/'
    def __truediv__(self, other):
        # Calculating the denominator: (c^2 + d^2)
        denom = other.real**2 + other.imag**2
        
        # Calculating the real and imaginary parts of the result
        real_part = (self.real * other.real + self.imag * other.imag) / denom
        imag_part = (self.imag * other.real - self.real * other.imag) / denom
        
        # Returning a new Complex number as the result of division
        return Complex(real_part, imag_part)

    # To represent the complex number in a readable format
    def __str__(self):
        return f"{self.real} + {self.imag}i"

# Creating two complex numbers Ob1 and Ob2
Ob1 = Complex(10, 21)
Ob2 = Complex(2, 3)

# Performing division of Ob1 by Ob2
result = Ob1 / Ob2

# Displaying the result of the division
print(f"({Ob1}) / ({Ob2}) = {result}")

```

### OUTPUT
![image](https://github.com/user-attachments/assets/084822ae-3dae-4882-be9a-a82328061b24)


### RESULT
thus the program is executed successfully

