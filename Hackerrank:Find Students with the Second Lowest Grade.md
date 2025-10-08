# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program

```
n = int(input())
arr = list(map(int, input().split()))
arr.sort()
large=arr[-1]
arr.reverse()
for i in range(len(arr)-1):
    if arr[i+1]<arr[i]:
        print(arr[i+1])
        break
```

## Output
<img width="511" height="173" alt="image" src="https://github.com/user-attachments/assets/c1dee613-44d3-4c5f-b77d-20cf49f9776b" />

## Result
The students with the second lowest grade have been successfully identified.

