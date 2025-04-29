# EX 1A Reverse a String
## DATE: 21.03.2025
## AIM:
To write a program to convert the given decimal number to binary number using recursive function.

## Algorithm
1. Start the program.
2. Input the decimal number num.
3. Check if num is 0:
If yes, print "0" and end.
4. Define a recursive function dec_to_bin(n)
5. If n == 0, return an empty string ""
6. Else:
   Call dec_to_bin(n // 2) recursively
   Append str(n % 2) to the result
   Return the combined string
7. Call dec_to_bin(num) and store the result.
8. Print the result
9. End the program.
  

## Program:
```
Program to implement Reverse a String
Developed by: SATHYAA R
Register Number: 212223100052
```

```
def dec_to_bin(n):
    if n == 0:
        return ""
    else:
        return dec_to_bin(n // 2) + str(n % 2)

num = int(input())
if num != 0:
    result = dec_to_bin(num)
else:
    result = "0"
print(result)
```


## Output:

![image](https://github.com/user-attachments/assets/cae5751e-6f44-4ac1-b0b0-a245c1d1fe28)


## Result:
The program successfully convert the given decimal number to binary number using recursive function. 
