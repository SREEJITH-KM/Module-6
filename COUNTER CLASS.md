# Exp.No:30  
## COUNTER CLASS

---

### AIM  
To write a Python program to create a `Counter` class that can increment the value of a counter.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the `Counter` class.**
   - Initialize the `current` variable with 0.
3. **Define the `increment()` method** to increment the value of `current` by 1.
4. **Define the `value()` method** to return the current value of `current`.
5. **Define the `reset()` method** to reset the `current` value back to 0.
6. **Create a `counter` object** of the `Counter` class.
7. **Call the `increment()` method** three times to increment the counter.
8. **Call the `value()` method** and print the result to show the current counter value.
9. **End the program.**

---

### PROGRAM

```
class Counter:
    def __init__(self, start=0):
        """Initialize the counter with a starting value."""
        self.value = start

    def increment(self, amount=1):
        """Increment the counter by the specified amount (default is 1)."""
        self.value += amount

    def get_value(self):
        """Return the current value of the counter."""
        return self.value

# Create a Counter object
counter = Counter()

# Increment the counter by default amount (1)
counter.increment()

# Increment the counter by 5
counter.increment(5)

# Display the current counter value
print(f"The current counter value is: {counter.get_value()}")

```

### OUTPUT
![image](https://github.com/user-attachments/assets/49de850d-0446-43eb-9a23-25f5abb99512)


### RESULT
thus the program is executed successfully
