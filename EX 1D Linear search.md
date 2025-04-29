# EX 1D Linear search
## DATE: 25.02.2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.

## Algorithm
1. Start the program.
2. Input the number of elements x.
3. Initialize an empty list List.
4. Repeat x times:
   Read an element from the user and append it to List.
5. Input the value n to be searched.
6. Call the function search(List, n).
7. If the function returns True, print "Found". Else, print "Not Found".
8. End the program.


## Program:
```
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: SATHYAA R
Register Number: 212223100052
```

```
def search(List, n):
    for i in range(len(List)):
        if List[i]==n:
            return True
    return False
List = []
x=int(input())
for i in range(x):
    List.append(input())
n=input()
if search(List, n):
    print("Found")
else:
    print("Not Found")
```


## Output:

![image](https://github.com/user-attachments/assets/0ba21c01-f1e6-4289-bc97-5b2a79c13e32)


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
