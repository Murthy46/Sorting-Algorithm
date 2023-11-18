# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: sundaramurthy M
RegisterNumber: 23010238
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)




```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: sundaramurthy M
RegisterNumber: 23010238
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        item=nums[i]
        j=i-1
        while j>=0 and nums[j]>item:
            nums[j+1]=nums[j]
            j-=1        
        nums[j+1]=item
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)





```

## Output:
<img width="1440" alt="Screenshot 2023-11-18 at 9 57 00 AM" src="https://github.com/Murthy46/Sorting-Algorithm/assets/145112768/f879e2f1-2d9c-4fd7-809d-fa73ca2daeab">

<img width="1440" alt="Screenshot 2023-11-18 at 9 57 28 AM" src="https://github.com/Murthy46/Sorting-Algorithm/assets/145112768/51668799-e1e2-4825-9285-52f47d3feeda">


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
