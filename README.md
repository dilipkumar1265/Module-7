# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
```
def sum_digits(num,accumulator=0):

    if num==0:
        return accumulator
    if num>0:
        return sum_digits(num//10,accumulator+num%10)
    else:
        return "Not defined"
    

num= int(input())

print(sum_digits(num))
```


## OUTPUT
![image](https://github.com/user-attachments/assets/841a7e85-fe9f-4ea1-9794-992dd70eb898)



## RESULT
Program executed successfully.


# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:

ADD CODE HERE
```
def sum_digits(num): if num < 0 or int(num) != num: return 0 elif num == 0: return 0 else: return (num % 10) + sum_digits(num//10) num= int(input()) print(sum_digits(num))
```
## OUTPUT
![image](https://github.com/user-attachments/assets/bd449539-adc4-48c7-93a9-1e45a6f86af5)

## RESULT
Thus, the program has been executed successfully.


# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
l=[]
def SUM(n):
    if n==0:
        return 1
    dig=n%10
    l.append(dig)
    SUM(n//10)
n=int(input())
SUM(n)
print(sum(l))

## OUTPUT
![image](https://github.com/user-attachments/assets/7626a840-091a-4c89-ad05-5bc5f0545437)


## RESULT
Program successfully verified.


# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:

```
def series(x,n):
    if n==0:
        return 1
    return x**n+series(x,n-1)
x=int(input())
n=int(input())
result=series(x,n)
print(result)
```

## OUTPUT
![image](https://github.com/user-attachments/assets/ace5d972-8770-4f5e-8b8d-62149576aa56)


## RESULT
Program is successfully is verified.


# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:

```
def fact(i):
   if i==1 or i==0:
       return 1
   else:
       return i*fact(i-1)
def sine(x,n):
  if n==0:
    return x
  else:
    return(((((-1)**n)*pow(x,(2*n+1)))/fact(2*n+1)))+sine(x,n-1)
x=int(input())
n=int(input())
print(sine(x,n))
```

## OUTPUT
![image](https://github.com/user-attachments/assets/d7b8a05f-6e0e-4085-b025-35285ccffb11)


## RESULT
Program is successfully verified.
