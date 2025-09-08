# Experiment-7
## Write a python program for sorting and inspect for failures. 
## Algorithm:
Start the program.
2. Get the number of elements from user
3. Get the elements to be sorted
4. Traverse the array and sort the elements one by one
5. Print the sorted array
6. Stop the program. 
# Program:
```
n = int(input("Enter the number of elements: "))
arr = []

try:
    for i in range(n):
        a = float(input("Enter the element: "))
        arr.append(a)

    # Bubble sort (corrected)
    for i in range(n):
        for j in range(n - i - 1):
            if arr[j] > arr[j + 1]:  # Compare adjacent elements
                temp = arr[j]
                arr[j] = arr[j + 1]
                arr[j + 1] = temp

    print("The array after sorting: ", end="")
    for i in range(n):
        print(arr[i], end=" ")

except ValueError:
    print("Enter a valid number")
```
# Result
<img width="529" height="147" alt="image" src="https://github.com/user-attachments/assets/55aeae7e-d71a-4302-be23-4701feed9e3a" />

# Output
Thus the python program for sorting and inspect for failures is executed successfully.
