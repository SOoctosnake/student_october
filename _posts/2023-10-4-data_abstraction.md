---
toc: true
comments: false
layout: post
title: Data Abstraction Homework
description: What I learned
type: tangibles
courses: { compsci: {week: 7} }
---
# Data Abstraction

## Variables 

Variables: an abstraction in a program that can hold a value

A variable can be thought of a holder from your program to use

Variables help you manage and organize your work with data



## Problem #1: Write a greeting using variables in python

``` py
user = input("Enter your name")
print("Hello ", user, " nice to meet you!")
```

Problem #1 Explanation:
This Python code takes the input of the user's name and print is with a greeting

## Problem #2: Print sum of num1Int and num2Int
```py
num1Int = 2
num2Int = 4
print(num1Int + num2Int)

```

Problem #2 Explanation:
Takes 2 variables and adds them in the print statement

## Problem #3: Print quotient of float1 and float2
```py

float1 = 4.6
float2 = 2.3
print(float1 / float2) 

```
Problem #3 Explanation:
Takes 2 variables and gets the quotient in the print statement


## Problem #4: Write a message with placeholders
```py
price_message = "{0} costs {1} dollars"

print(message.format("Banana", "1"))

print (message.format("Apple Vision Pro", "3500"))

print (message.format("Couch", "1000"))

```
Problem #4 Explanation:
Uses .format to add things to the place holders defined originally