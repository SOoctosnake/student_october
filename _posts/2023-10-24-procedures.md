---
toc: true
comments: false
layout: post
title: Procedures Homework
description: What I learned
type: hacks
courses: { compsci: {week: 10} }
---
# Procedures


## Problem #1: Procedural Abstraction

```python
# Function to calculate the square of a number
def calculate_square(number):
    return number ** 2

# Example usage:
number = 5
square = calculate_square(number)
print(f"The square of {number} is {square}")
```

Problem #1 Explanation:
This Python function, `calculate_square`, demonstrates procedural abstraction by taking a parameter (a number), performing a specific task (calculating the square), and returning the result.

## Problem #2: Summing Machine

```python
# Function to calculate the sum of two numbers
def summing_machine(first_number, second_number):
    return first_number + second_number

# Calculate the sum of 7 and 5 using the function
result = summing_machine(7, 5)
print(f"The sum of 7 and 5 is {result}")
```

Problem #2 Explanation:
This Python function, `summing_machine`, calculates the sum of two numbers by taking them as parameters and returning the result. We use the function to find the sum of 7 and 5 and print the result.