# QuickSort-Algorithm

Implementing QuickSort Algorithm.  Quicksort is an efficient algorithm for sorting values in a list. A single element, the pivot, is chosen from the list. All the remaining values are partitioned into two sub-lists containing the values smaller than and greater than the pivot element.  Ideally, this process of dividing the array will produce sub-lists of nearly equal length, otherwise, the runtime of the algorithm suffers.  When the dividing step returns sub-lists that have one or less elements, each sub-list is sorted. The sub-lists are recombined, or swaps are made in the original array, to produce a sorted list of values.



Quicksort is a divide-and-conquer algorithm that splits an unsorted data set into two partitions recursively and sorts the partitioned arrays in-place until there is only one element left in a partition.


To determine the elements that belong in a partition, we need a pivot element, pivot, that is sandwiched between the two partitions and its location called the pivotIndex.


The partition() function which groups and swaps the elements either to the left or right of the pivot element and returns the leftIndex that is the same as the pivotIndex is then implemented.


The quicksort() function which first calls partition() to determine the pivotIndex then recursively calls itself to sort the smaller partitions until there is only one element left in the partition is next implemented.


Quicksort has a **worst case runtime** of **O(N^2)**. This can happen when quicksort’s input data set comprises:

-pre-sorted numbers,

-backward-sorted numbers, or

-all similar elements along with a poorly chosen pivot element that produces a partition of zero or one element.




The **runtime** of quicksort is **O(N * log N)** if partition sizes are roughly equal.




**The pseudocode for our quicksort algorithm is as follows:**

```If there is more than one element left in the array:

  Find the pivot index through partitioning
  

  If the left pointer is less than the pivot index:
  
   Call quicksort() on the portion of the array between the left pointer and the pivot. 
    

  If the pivot index is less than the right pointer:
  
    Call quicksort() on the portion of the array between the pivot index and the right pointer.
    

Return the sorted array```





