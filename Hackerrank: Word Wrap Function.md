# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
```
def wrap(string, max_width):
    for i in range(0,len(string)+1,max_width):
        result = string[i:i+max_width]
        if len(result) == max_width:
            print(result)
        else:
            return(result)

string, max_width = input(), int(input())
```

## Sample Output
<img width="833" height="293" alt="image" src="https://github.com/user-attachments/assets/06db9a16-8d60-4821-aef2-6d5a9799ab31" />


## Result
The string has been successfully wrapped into lines.
