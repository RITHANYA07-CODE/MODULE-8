# 🔍 Hackerrank:Python Program to Validate Mobile Numbers Using Regular Expressions

This Python program checks whether a given string is a valid mobile number. A valid mobile number is defined as a 10-digit number starting with 7, 8, or 9.
---

## 🎯 Aim

To write a Python program that checks whether each input string is a valid mobile number using Python's regular expressions.
---

## 🧠 Algorithm

1. Start the program.
2. Input the number of test cases num.
3. For each test case:

  (i) Input a string n.
  
  (ii) Compile a regular expression pattern to match a 10-digit number starting with 7, 8, or 9.
  
  (iii) Use re.match() to check if the string matches the pattern.
  
  (iv) If it matches, print "YES".
  
  (v) Else, print "NO".

4. End the program.

---

## 💻  Program
```
import re
num=int(input())
for i in range(num):
    n=input()
    p=re.compile("[7|8|9]\d{9}")
    if re.match(p,n):
        print("YES")
    else:
        print("NO")
```

## Output
<img width="456" height="193" alt="image" src="https://github.com/user-attachments/assets/7bd0d60c-6f33-4dd9-ab90-2487952bf320" />


## Result
The program correctly identifies whether a given input string is a valid mobile number.
