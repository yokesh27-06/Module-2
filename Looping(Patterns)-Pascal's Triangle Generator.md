# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

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
def generate_pascals_triangle(n):
    for i in range(n):
        print(' ' * (n - i), end='')
        value = 1
        for j in range(i + 1):
            print(value, end=' ')
            value = value * (i - j) // (j + 1)
        print() 
rows = int(input("Enter the number of rows for Pascal's Triangle: "))
generate_pascals_triangle(rows)
```

## Sample Output
![image](https://github.com/user-attachments/assets/06566986-e93a-4f22-95a1-1a62d7b5bdde)


## Result
         program executed successfully
