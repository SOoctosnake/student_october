---
toc: true
comments: false
layout: post
title: Binary Search Homework
description: What I learned
type: hacks
courses: { compsci: {week: 9} }
---
# Binary Search

## Problem #1: List Indexing and Procedures

```python
# Create a sample list of numbers
numbers = [5, 12, 8, 21, 10]

# Calculate the sum of the list using a list procedure (sum())
total = sum(numbers)

# Access the third element of the list using list indexing
third_element = numbers[2]

# Print the results
print(f"Sum of the numbers: {total}")
print(f"Third element of the list: {third_element}")
```

Problem #1 Explanation:
- We define a list of numbers.
- We use the `sum()` function to calculate the sum of the numbers in the list.
- We use list indexing (`numbers[2]`) to access the third element of the list.
- We print the calculated sum and the third element.

## Problem #2: Determine Worst Case Binary Search Iterations

```python
# Function to determine the worst case number of iterations for binary search
def worst_case_iterations(array_length):
    return int(math.log2(array_length))

# Import the math module for logarithm calculations
import math

# Call the function for an array of length 20 and print the result
array_length = 20
iterations = worst_case_iterations(array_length)
print(f"Worst case iterations for an array of length {array_length}: {iterations}")
```

Problem #2 Explanation:
- We define a function `worst_case_iterations` that calculates the worst-case number of iterations for a binary search based on the array's length.
- To determine the number of iterations, we use the logarithm to the base 2 of the array length, as binary search continually divides the list in half.
- We import the `math` module for logarithm calculations.
- We call the function for an array of length 20 and print the result.