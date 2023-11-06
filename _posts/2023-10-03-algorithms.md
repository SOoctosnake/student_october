---
toc: true
comments: false
layout: post
title: Algorithm Homework
description: A simple game where you drag and drop shapes!
type: tangibles
courses: { compsci: {week: 7} }
---
# Algorithms

Definition: A finite set of instructions to accomplish a task

## Aspects of Algorithms:
Sequence: Follows a sequence of steps

Selection: choose different outcomes at steps based on a condition that is made

Iteration: Repetition of code segment if condition is met

## Problem #1: Write Python Code or Psuedo Code that is able to take a string as input and detect if its a palindrome

``` py
n = input() # main string
start_half = ""
end_half = ""
if len(n)%2 == 0:
    start_half = n[0:len(n)//2]
    end_half = n[len(n)//2:]
else:
    start_half = n[0:len(n)//2]
    end_half = n[len(n)//2+1:]
if start_half == end_half:
    print("This string is a palindrome")
else:
    print("This string is not a palindrome")

```

Problem #1 Explanation:
This Python code checks if a given input string 'n' is a palindrome by comparing its first half to its reversed second half. It handles even and odd-length strings and prints whether the string is a palindrome or not.

## Problem #2: Write Python Code or Psuedo Code that is able to take a string as input and detect if its a palindrome

``` py
def price_sort(car_prices):
    n = len(car_prices)

    for i in range(n):
        # Flag to optimize the sorting process
        swapped = False

        for j in range(0, n - i - 1):
            if car_prices[j] > car_prices[j + 1]:
                # Swap the elements if they are in the wrong order
                car_prices[j], car_prices[j + 1] = car_prices[j + 1], car_prices[j]
                swapped = True

        # If no two elements were swapped in the inner loop, the list is sorted
        if not swapped:
            break

# Example usage:
car_prices = [30000, 25000, 40000, 35000, 20000]
price_sort(car_prices)
print("Sorted Car Prices:", car_prices)
```

Problem #2 Explanation:
This Python program sorts a list of car prices using the Bubble Sort algorithm. It iterates through the list, comparing adjacent elements and swapping them if out of order, repeating until the list is sorted.

