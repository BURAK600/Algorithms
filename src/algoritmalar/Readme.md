# Merge Algorithm

Merge Sort is a Divide and Conquer algorithm. It divides the input array into two halves, calls itself for the two halves, and then it merges the two sorted halves. The merge() function is used for merging two halves. The merge(arr, l, m, r) is a key process that assumes that arr[l..m] and arr[m+1..r] are sorted and merges the two sorted sub-arrays into one. 

---

## How Merge sort Works?
![How Merge sort Works?](https://i0.wp.com/furkanalniak.com/wp-content/uploads/2017/08/merge.jpg?w=554)


---

## Time Complexity of Merge Sort
Merge Sort is a recursive algorithm and time complexity can be expressed as following recurrence relation.

- *** T(n) = 2T(n/2) + O(n)

The solution of the above recurrence is O(nLogn). The list of size N is divided into a max of Logn parts, and the merging of all sublists into a single list takes O(N) time, the worst-case run time of this algorithm is O(nLogn)

- Best Case Time Complexity: O(n*log n)

- Worst Case Time Complexity: O(n*log n)

- Average Time Complexity: O(n*log n)

The time complexity of MergeSort is O(n*Log n) in all the 3 cases (worst, average and best) as the mergesort always divides the array into two halves and takes linear time to merge two halves.


