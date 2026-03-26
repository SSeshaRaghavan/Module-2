# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
Add Code Here
```
#To write a Python program to convert the number 16 into its binary representation using built-in Python functions.
a = 16
print(bin(a))
```
## Output
<img width="562" height="265" alt="image" src="https://github.com/user-attachments/assets/deaec9fd-0a50-442c-994b-2b523ff57918" />

## Result
0b10000

# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program

Add code Here
```
#To write a Python program to convert the number 16 into its binary representation using built-in Python functions.
def result(a, b):
    print(a % b)

x = int(input())
y = int(input())
result(x, y)    
```
## Output
![Screenshot 2025-05-03 110534](https://github.com/user-attachments/assets/ece388f1-084c-412d-a91d-547ccc4b7606)
![image](https://github.com/user-attachments/assets/33006371-2d51-4464-9771-da39bd742596)

## Result
Thus, the program has been successfully executed.

# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
Add code here
```
#To write a Python program that defines a lambda function which takes two arguments a and b, and returns their sum.
a = int(input())
b = int(input())
f = lambda a, b: a + b
print(f(a, b))
```
## Output
<img width="461" height="186" alt="image" src="https://github.com/user-attachments/assets/5e10e779-fb56-43f0-bccf-881990362395" />

## Result
Thus, the program has been successfully executed.

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
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

def combination(n, k):
    return factorial(n) // (factorial(k) * factorial(n - k))

num_rows = int(input("Enter number of rows: "))

for i in range(num_rows):
    print(' ' * (num_rows - i - 1), end='')
    for j in range(i + 1):
        print(combination(i, j), end=' ')
    print()
```
## Sample Output
<img width="201" height="225" alt="image" src="https://github.com/user-attachments/assets/c602f210-4f95-4886-a1a3-16c5215a165c" />

## Result
Thus, the program has been successfully executed

## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if num == rev:
    print(f"{num} is a palindrome.")
else:
    print(f"{num} is not a palindrome.")
```
## Output
<img width="593" height="114" alt="image" src="https://github.com/user-attachments/assets/719d56c6-8c7f-4bfe-b9c6-1f09550e34fe" />

## Result
Thus, the program has been successfully executed.
