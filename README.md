# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:RUCHITRA THIYAGARAJ
RegisterNumber: 23000100
'''
def linearsearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array=eval(input())
k=eval(input())
n=len(array)
array.sort()
result=linearsearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:RUCHITRA THIYAGARAJ
RegisterNumber: 23000100
'''
def binarysearchiter(array,k,low,high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=binarysearchiter(array,k,0,len(array)-1)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: RUCHITRA THIYAGARAJ
RegisterNumber: 23000100
'''
def binarysearchiter(array,k,low,high):
    while high>=low:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=binarysearchiter(array,k,0,len(array)-1)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
## Sample Input and Output
![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/409e768d-877e-40b0-9634-989df781b7c4)
</BR>
</BR>
![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/a0324745-95d7-4ac6-a311-73d782e9d64b)
</br>
</br>
![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/47f1b2c0-4fbc-42c8-8f4f-dec2e9cff827)
</br>
</br>

![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/882f2910-bbba-4ef7-a47a-de05c55ce493)
</br>
</br>
![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/6c0f2be8-4081-47bb-ba9d-cd32b5917705)
</br>
</br>
![image](https://github.com/RuchitraThiyagaraj/Search-Algorithm/assets/154776996/c816a884-f2e5-41be-8c1a-3440ccfb5441)


## Result
Thus the linear search and binary search algorithm is implemented using python programming.
