---
toc: true
comments: false
layout: post
title: Developing Algorithms Homework
description: What I learned
type: hacks
courses: { compsci: {week: 9} }
---
# Developing Algorithms

## Problem #1: Find the Median Test Grade of a Class

```python
# Function to calculate the median from a list of grades
def calculate_median(grades):
    sorted_grades = sorted(grades)
    n = len(sorted_grades)
    
    if n % 2 == 0:
        # For an even number of grades, take the average of the middle two grades
        median = (sorted_grades[n // 2 - 1] + sorted_grades[n // 2]) / 2
    else:
        # For an odd number of grades, the median is the middle grade
        median = sorted_grades[n // 2]
    
    return median

# Example usage:
grades = [90, 85, 78, 92, 88, 94]
median_grade = calculate_median(grades)
print(f"The median test grade is: {median_grade}")
```

Problem #1 Explanation:
This Python program calculates the median test grade of a class from a list of grades. It uses a function to sort the grades and determine the median based on whether the number of grades is even or odd.

## Problem #2: Create a Simple Game Using Random Numbers

```python
# Problem #2: Simple Number Guessing Game

import random

# Generate a random number between 1 and 100
secret_number = random.randint(1, 100)

attempts = 0
max_attempts = 10

print("Welcome to the Number Guessing Game!")
print("Try to guess the secret number between 1 and 100.")

while attempts < max_attempts:
    guess = int(input("Enter your guess: "))
    attempts += 1

    if guess < secret_number:
        print("Guess higher.")
    elif guess > secret_number:
        print("Guess lower.")
    else:
        print(f"Congratulations! You guessed the secret number {secret_number} in {attempts} attempts.")
        break
else:
    print(f"Sorry, you've reached the maximum number of attempts. The secret number was {secret_number}.")
```

Problem #2 Explanation:
This Python program creates a simple number guessing game. The computer selects a random number between 1 and 100, and the player has to guess it. The game provides feedback on whether to guess higher or lower and tracks the number of attempts, ending when the player guesses the correct number or exceeds the maximum allowed attempts.