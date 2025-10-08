# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```
marks = eval(input())
total = 0
total_marks = marks.copy()
for key,val in marks.items():
    total = sum(val)
    total_marks[key] = total
print(total_marks)
max = 0
topper = ''
for key,val in total_marks.items():
    if val>max:
        max = val
        topper = key
print("Topper is: ", topper, "with marks = ",max)
```

## OUTPUT
<img width="1230" height="147" alt="Screenshot 2025-10-08 143311" src="https://github.com/user-attachments/assets/8b67e08e-11c9-42d8-a92f-3dc2dc687e1c" />


## RESULT
Thus, the program has been successfully executed.
