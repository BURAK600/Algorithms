# Quick Sort

Like Merge Sort, QuickSort is a Divide and Conquer algorithm. It picks an element as pivot and partitions the given array around the picked pivot.

---

### There are many different versions of quickSort that pick pivot in different ways. 
- Always pick first element as pivot.
- Always pick last element as pivot (implemented below)
- Pick a random element as pivot.
- Pick median as pivot.

---

The key process in quickSort is partition(). Target of partitions is, given an array and an element x of array as pivot, put x at its correct position in sorted 
array and put all smaller elements (smaller than x) before x, and put all greater elements (greater than x) after x. All this should be done in linear time.

## How Merge sort Works?
![How Merge sort Works?](https://www.techiedelight.com/wp-content/uploads/Quicksort.png)

---

## Time Complexity of Merge Sort

- ### Worst case
The worst case in quicksort occurs when the partition gives a 1 : n-1 split every time. Graphically, this looks like:

![Quick Sort Worst Case](https://www.cs.dartmouth.edu/~thc/cs5-F96/quicksort_worse.gif)

- ### Best case
The best case occurs when we have an even split all the time. The tree looks exactly like the recursion tree that we got for merge sort:

![Quick Sort Average Case](https://www.cs.dartmouth.edu/~thc/cs5-F96/merge_tree.gif)

And as you have probably guessed by now, the running time is the same, which is O(n log2 n)

- ### Average case
For the average case, I will use the graceful art of handwaving. Let's just say that most splits are not too far from even. 
Given this, the analysis exceeds the scope of this course, but it turns out to be O(n log2 n).

---
# Difference Between  Quicksort and Merge Sort

 |**Basis for comparison**|**Quick Sort**| **Merge Sort** |
|----------|:-------------:|------:|
| **Worst case complexity**| O(n2) | O(nlogn)|
| **Average case complexity** |  O(nlogn) |  O(nlogn) |
|**Speed of execution** | It work faster than other sorting algorithms for small data set  |It has a consistent speed on any size of data |
| **Efficiency**| Inefficient for larger arrays | More efficient in case of larger array size or datasets|
| **Preferred for** | for Arrays | for Linked Lists |
| **Locality of reference** | Quicksort exhibits good cache locality and this makes quicksort faster than merge sort (in many cases like in virtual memory environment)| 	poor |
| **Additional storage space requirement** | Merge sort is not in place because it requires additional memory space to store the auxiliary arrays. | The quick sort is in place as it doesn’t require any additional storage. |





