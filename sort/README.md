# Sorting Algorithms
Sorting algorithms is a process of organising a collection of data in an ascending or descending order. Sorting algorithms can be used as stand alone algorithms or as part of other algorithms like search algorithms. The binary search algorithm is a very efficient way to search large collections of data. Sorting is a pre-requisite for most searching algorithms.

**Internal vs. External Sorting**

Sorting algorithms can be classified into two types of algorithms: internal and external. Internal sorting algorithms require the full data set to fit into main memory whereas external sort is used when the full data set does not fit and have to reside on external storage during the sorting process.

**Stable vs. Unstable Sorting**

A stable sorting algorithm is when two objects with equal keys appear in the same order in the unsorted input array and the sorted output array. Examples of stable sorting algorithms are Insertion sort, Merge Sort and Bubble Sort.

An unstable sorting algorithm is when two objects with equal keys doesn't appear in the same order in the unsorted input array and the sorted output array. Examples of unstable sorting algorithms are Heap Sort and Quick Sort.

## Why Study Sorting Algorithms
The question always come up, why do we study sorting algorithms and why even care? The sorting algorithms are all very different to each other but with the same pre- and post-conditions. There are many ways to implement an algorithm to sort an array of integer values where the pre-condition and the post-conditions will be the exact same, but the behaviour and complexity of the algorithm is different. We would like to have a way to measure an algorithm to determine which is a good algorithm and which is best.

As we start to learn the different sorting algorithms, we should also learn techniques on how to measure the performance of algorithms.

The performance of algorithm is measured on the basis of following properties:

* **Time Complexity**: Time Complexity is the computational complexity that describes the amount of time it takes to run an algorithm.
* **Space Complexity**: Space Complexity is the computational complexity that describes the amount of memory space required by an algorithm.

## List of Sort Algorithms
The following algorithms are examples of internal sorting algorithms:

| Algorithm Name | Time Complexity: Best | Time Complexity: Average | Time Complexity: Worst | Space Complexity: Worst |
| --- | :---: | :---: | :---: | :---: |
| [Bubble Sort](BubbleSort.md) | Ω(n) | Θ(n<sup>2</sup>) | O(n<sup>2</sup>) | O(1) |
| [Bucket Sort](BucketSort.md) | Ω(n+k) | Θ(n+k) | O(n<sup>2</sup>) |  O(n) |
| [Counting Sort](CountingSort.md) | Ω(n+k) | Θ(n+k) | O(n+k) | O(k) |
| [Cube Sort](CubeSort.md) | Ω(n) | Θ(n log(n)) | O(n log(n)) | O(n) |
| [Heapsort](Heapsort.md) | Ω(n log(n)) | Θ(n log(n)) | O(n log(n)) | O(1) |
| [Insertion Sort](InsertionSort.md) | Ω(n) | Θ(n<sup>2</sup>) | O(n<sup>2</sup>) | O(1) |
| [Mergesort](Mergesort.md) | Ω(n log(n)) | Θ(n log(n)) | O(n log(n)) | O(n) |
| [Quicksort](Quicksort.md) | Ω(n log(n)) | Θ(n log(n)) | O(n<sup>2</sup> | O(n log(n)) |
| [Radix Sort](RadixSort.md) | Ω(nk) | Θ(nk) | O(nk) | O(n+k) |
| [Timsort](Timsort.md) | Ω(n) | Θ(n log(n)) | Θ(n log(n)) | O(n) |
| [Tree Sort](TreeSort.md) | Ω(n log(n))  | Θ(n log(n)) | O(n<sup>2</sup>) | O(n) |
| [Selection Sort](SelectionSort.md) | Ω(n<sup>2</sup>) | Θ(n<sup>2</sup>) | O(n<sup>2</sup>) | O(1) |
| [Shell Sort](ShellSort.md) | Ω(n log(n)) | Θ(n(log(n))<sup>2</sup>) | O(n(log(n))<sup>2</sup>) | O(1) |


## Conclusion
