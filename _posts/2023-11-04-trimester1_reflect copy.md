---
toc: false
comments: false
layout: post
title: Safe Computing
description: HW
type: tangibles
courses: { compsci: {week: 10} }
---

1. **PII in CompSci Projects:** PII includes personal data like names, addresses, SSNs. Safeguarding involves encryption, access control, and compliance with privacy laws for sensitive information storage.
2. **Good and Bad Passwords:** Good passwords are lengthy, diverse, and avoid common words. Bad passwords are short, predictable, and lack complexity. Two-factor authentication adds an extra layer of security.
3. **Symmetric & Asymmetric Encryption:** Symmetric uses one key for encryption and decryption, while asymmetric employs a key pair: public for encryption, private for decryption, enhancing security.
4. **AWS Encryption:** AWS Key Management Service (KMS) secures data in S3 by managing encryption keys, adding protection to stored information within an AWS deployment.
5. **Python Password Checker:**
```python
def check_password_strength(password): # Checks password strength criteria.
    # Define criteria for a strong password
    min_length = 8
    has_upper = any(char.isupper() for char in password)
    has_lower = any(char.islower() for char in password)
    has_digit = any(char.isdigit() for char in password)
    has_special = any(char in "!@#$%^&*()-_=+[]{};:'\"<>,.?/\\|`~" for char in password)
    # Check if password meets the criteria
    if len(password) >= min_length and has_upper and has_lower and has_digit and has_special:
        return "Strong password!"
    else:
        return "Weak password! Password should be 8+ characters with uppercase, lowercase, digit, and special characters."
# Get user input for password
user_password = input("Enter a password: ")
# Check the strength of the password
result = check_password_strength(user_password)
print(result)
```