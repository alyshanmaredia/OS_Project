DESCRIPTION:
A process is an executing instance of an application and a thread is a path of execution within a process. The same methodology will be applied to implement some sorting structures to better understand their time complexities. E.g. Merge Sort, Quick Sort, etc.




HOW WE STARTED:
First of all we decided which sorting algorithms to use. We chose Bubble, Insertion, Merge, Quick and Heap sorts. After that we implemented their individual functions. Then we divided process and threads amongst us two and started working on the implementations.






PROBLEMS FACED:
In Merge, Quick and Heap sort the array was being divided into processes but then it wasn’t merging into one sorted array.

SOLUTION TO PROBLEM:
For the processes to communicate with each other, we used the concept of shared memory so that they can share the same array and sort it.







THE ACTUAL WORKING OF THE PROJECT (Methodology):
Firstly, all 5-sorting algorithms are implemented using threads and process techniques. In Process, the function fork() is used to create parent and child process which then access the different sub parts of the main array and sort them. After that every subarray is merged into one. 
In Threads, 4 individual threads are created to divide the main array into 4 equal parts. Each thread then performs the sorting, and then the threads are joined to display the sorted arrays.
During each sorting algorithm, its time complexity is also calculated which we used to make the following line graphs depicting the difference between time taken by processes and threads to complete a task.





EXPLANATION OF OUR SOURCE CODE:
We have implemented 5 sorting algorithms, Bubble, Insertion, Merge, Quick and Heap sort. We created a menu driven program, which gives us the option to select between process and threads as a choice to do the sorting through switch case. Then we have to select the respective sorting. Each sorting algorithm is implemented 2 times, one using the concept of process and other through threads. Other than these some other functions are: 

1) Display
The function displays the unsorted/sorted array.

2) Swap
This function swaps the two instances of an array.

3) Combine
This function merges the sub arrays in case of sorting through threads.



PROJECT ASPECTS in CURRENT/FUTURE TECHNOLOGY: 
These concepts of sorting through processes and threads can help us understand the time complexities of each sorting algorithm in different environments and also which approach is better while working on an OS. Knowing the better approach can result in faster working of systems and different software.
