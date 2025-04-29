# EX 1C Quick Sort
## DATE: 26.03.2025
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of integers.

## Algorithm
1. Start the program.
2. Input the number of elements n.
3. Initialize an empty list arr.
4. Read n integer values and append to arr.
5. Call quickSort(arr, 0, n-1) to sort the list.
6. Print the sorted list.
7. End the program.


## Program:
```
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: SATHYAA R
Register Number: 212223100052
```

```
def quickSort(a,st,en):
    if st<en:
        p=partition(a,st,en)
        quickSort(a,st,p-1)
        quickSort(a,p+1,en)
def partition(a,st,en):
    pivot=a[st]
    i=st
    j=en
    while True:
        while(i<=j and a[i]<=pivot):
            i=i+1
        while(i<=j and a[j]>=pivot):
            j=j-1
        if i<=j:
            a[i],a[j]=a[j],a[i]
        else:
            a[st],a[j]=a[j],a[st]
            return j
arr=[]
n=int(input())
for i in range(n):
    arr.append(int(input()))
quickSort(arr,0,len(arr)-1)
print("Sorted array is:")
for i in range(n):
    print(arr[i])
```

## Output:

![image](https://github.com/user-attachments/assets/463445d1-629d-4973-9ccb-24bb7d7eabf7)


## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
