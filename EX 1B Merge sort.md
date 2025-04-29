# EX 1B Merge Sort
## DATE: 04.03.2025
## AIM:
To write a python program to sort the first half of the list using merge sort with float values.

## Algorithm
1. Start the program.
2. Input the size of the list n.
3. Initialize an empty list arr.
4. Read n float values from the user and append them to arr
5. Print the original array
6. Call mergeSort(arr, 0, (n // 2) - 1) to sort only the first half of the list using merge sort.
7. Print the array after sorting the first half (the second half remains unchanged).
8. End the program.

## Program:
```
Program to implement Merge Sort
Developed by: SATHYAA R
Register Number: 212223100052
```

```
def merge(arr, l, m, r):
    n1=m-l+1
    n2=r-m
    L=[0]*(n1)
    R=[0]*(n2)
    for i in range(n1):
        L[i]=arr[l+i]
    for j in range(n2):
        R[j]=arr[m+1+j]
    i=0
    j=0
    k=l
    while i<n1 and j<n2:
        if L[i]<=R[j]:
            arr[k]=L[i]
            i+=1
        else:
            arr[k]=R[j]
            j+=1
        k+=1
    while i<n1:
        arr[k]=L[i]
        i+=1
        k+=1
    while j<n2:
        arr[k]=R[j]
        j+=1
        k+=1
def mergeSort(arr, l, r):
    if l<r:
        m=l+(r-l)//2
        mergeSort(arr, l, m)
        merge(arr, l, m, r)
arr=[]
n=int(input())
for i in range(n):
    arr.append(float(input()))
print("Original array:")
for i in range(n):
    print("%.1f" % arr[i], end=" ")
mergeSort(arr, 0, (n//2)-1)
print("\nSorted first half and unchanged second half:")
for i in range(n):
    print("%.1f" % arr[i], end=" ")
```

## Output:

![image](https://github.com/user-attachments/assets/3ac6d97b-b092-425c-b99c-57a99b4a4174)


## Result:
The program successfully sorts the first half of the given array using merge sort with float values, where only the first half is sorted, and the second half remains unchanged.
