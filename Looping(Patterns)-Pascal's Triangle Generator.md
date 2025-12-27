<img width="201" height="225" alt="image" src="https://github.com/user-attachments/assets/fa50b453-308d-4b95-9a35-ab24875f5bd6" /><img width="201" height="225" alt="image" src="https://github.com/user-attachments/assets/599ab987-5626-45c6-9bee-a2fe45cded82" /># 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

def combination(a, b):
    return factorial(a) // (factorial(b) * factorial(a - b))

rows = int(input())

for i in range(rows):
    print(' ' * (rows - i - 1), end='')
    for j in range(i + 1):
        print(combination(i, j), end=' ')
    print()
```

## Sample Output
<img width="201" height="225" alt="image" src="https://github.com/user-attachments/assets/31434563-ccc2-4493-ab0e-a0712ee531ab" />

## Result
Thus, we were able to write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user
