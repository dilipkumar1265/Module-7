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
