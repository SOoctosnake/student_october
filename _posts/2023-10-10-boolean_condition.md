---
toc: true
comments: false
layout: post
title: Boolean and Conditions Homework
description: What I learned
type: hacks
courses: { compsci: {week: 8} }
---
# Boolean and Conditions


## Problem #1: Voter Eligibility Check

```python
# Ask for citizenship and age input from the user
is_citizen = input("Are you a citizen? (yes/no): ").strip().lower() == "yes"
age = int(input("Enter your age: "))

# Check eligibility based on citizenship and age criteria
if is_citizen and age >= 18:
    print("You are eligible to vote.")
else:
    print("You are not eligible to vote.")
```

Problem #1 Explanation:
This Python program checks a user's eligibility to vote. It asks for citizenship and age, then determines eligibility based on the criteria that the user must be a citizen and 18 or older.


## Problem #2: Calculate Employee Bonus

```python
# Ask the user for their salary and years of service
salary = float(input("Enter your salary: $"))
years_of service = int(input("Enter your years of service: "))

# Check if the employee is eligible for a bonus
if years_of_service > 5:
    bonus_percentage = 5  # 5% bonus
    bonus_amount = (bonus_percentage / 100) * salary
    print(f"You are eligible for a {bonus_percentage}% bonus of ${bonus_amount:.2f}.")
else:
    print("You are not eligible for a bonus.")
```

Problem #2 Explanation:
This Python program calculates and prints the net bonus amount for an employee based on their salary and years of service. If the employee has more than 5 years of service, they receive a 5% bonus.

I apologize for the previous responses. Here's the solution in the specified format:

## Problem #3: Grade Classification

```python
# Ask the user to enter their marks
marks = float(input("Enter your marks: "))

# Determine the grade based on the provided rules
if marks < 25:
    grade = "F"
elif marks >= 25 and marks < 45:
    grade = "E"
elif marks >= 45 and marks < 50:
    grade = "D"
elif marks >= 50 and marks < 60:
    grade = "C"
elif marks >= 60 and marks <= 80:
    grade = "B"
else:
    grade = "A"

# Print the corresponding grade
print(f"Your grade is: {grade}")
```

Problem #3 Explanation:
This Python program takes a user's input for marks and calculates the corresponding grade based on the provided grading rules. It then prints the determined grade for the input marks.