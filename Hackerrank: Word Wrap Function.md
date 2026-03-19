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
    wrapped_lines = []  # list to store each line
    for i in range(0, len(string), max_width):
        part = string[i:i+max_width]
        wrapped_lines.append(part)
    return '\n'.join(wrapped_lines)  
string, max_width = input(), int(input())
print(wrap(string, max_width))
```


## Sample Output
<img width="833" height="293" alt="image" src="https://github.com/user-attachments/assets/f2c1b7e0-bf2e-4100-8bf9-08ee0b2967ab" />

## Result
Thus, the Python program defines a function that wraps a long string into multiple lines is executed successfully.
