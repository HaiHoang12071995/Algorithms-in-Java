# Sort Algorithm: Bubble Sort

## Overview
Bubble sort is sometimes referred to as sinking sort. The bubble sort algorithm repeatedly steps through the list and compare each adjacent item. The pair of values gets swapped if they are in the wrong order. The algorithm gets its name from the way smaller or larger elements "bubble" to the top of the list.

## Algorithm Classification
The following table contains information about the analysis of the BubbleSort algorithm. It defines the worst, average and best cases in terms of time complexity and also the worst case in space complexity.

| Classification | Value|
| --- | --- |
| Class | Sorting Algorithm |
| Data Structure | Array |
| Time Complexity: Worst | O(n<sup>2</sup>) |
| Time Complexity: Average | O(n<sup>2</sup>) |
| TimeComplexity: Best | O(n) |
| Space Complexity: Worst | O(1) |

Please use the following [link][0] for an explanation on Big-O notation and what is good, fair and bad.

## Pseudocode
The following is the pseudocode for the BubbleSort algorithm.
```
BUBBLESORT(int [] t, int n)
  int i,j,p
  for i = n downto 2 do
    for j = 1 to i-1 do
      if t[j]>t[j+1]then
        p= t[j]
        t[j]= t[j+1]
        t[j+1]= p
      end if
    end for
  end for
```

## BubbleSort In Java
The BubbleSort class implements the BubbleSort algorithm for sorting an array of integers.

```java
public final class BubbleSort {

    public void sort(int[] collection) {
      if (collection != null) {
        bubbleSort(collection);
      } else {
        throw new IllegalArgumentException("Input parameter for array to sort is null.");
      }
    }

    private void bubbleSort(int[] collection) {
          int n = collection.length;
          for (int i = 0; i < n-1; i++) {
              for (int j = 0; j < n-i-1; j++) {
                  if (collection[j] > collection[j+1]) {
                      swap(collection, j, j+1);
                  }
              }
          }
    }

    private void swap(int[] collection, int x, int y) {
      int temp = collection[x];
      collection[x] = collection[y];
      collection[y] = temp;
    }

}
```
### Sample Code (GitHub)
* The details of the BubbleSort class can be viewed [here][1].
* The details of the BubbleSort JUnit Test class can be viewed [here][2].

## BubbleSort In Java (Recursive)
The BubbleSort class implements the BubbleSort algorithm for sorting an array of integers. The following is the recursive implementation of the BubbleSort algorithm in Java.

```java
public final class BubbleSortRecursive {

    public void sort(int[] collection) {
    	if (collection != null) {
    		bubbleSort(collection, collection.length);
    	} else {
    		throw new IllegalArgumentException("Input parameter for array to sort is null.");
    	}
    }

    private void bubbleSort(int[] collection, int arrayLength) {
          if (arrayLength == 1) {
              return;
          }

          for (int i=0; i < arrayLength-1; i++) {
              if (collection[i] > collection[i+1]) {
              		swap(collection, i, i+1);
              }
          }

          bubbleSort(collection, arrayLength-1);
    }

    private void swap(int[] collection, int x, int y) {
    	int temp = collection[x];
    	collection[x] = collection[y];
    	collection[y] = temp;
    }

}
```
### Sample Code (GitHub)
* The details of the BubbleSortRecursive class can be viewed [here][3].
* The details of the BubbleSortRecursive JUnit Test class can be viewed [here][4].

## Conclusion
The BubbleSort algorithm forms part of a larger group of sorting algorithms. Learning through experience is the reason I created this post about the implementation of the BubbleSort algorithm in Java. I have learned a lot about how others have solved the BubbleSort algorithm in other languages including different implementations in Java.

Learning how to solve difference problems and algorithms with certain techniques, one starts to develop certain pattern recognition abilities which will help you in future when similar problems arise.

[0]: http://www.bigocheatsheet.com/img/big-o-cheat-sheet-poster.png
[1]: https://github.com/Code2Bits/Algorithms-in-Java/blob/master/sort/src/main/java/com/code2bits/algorithm/sort/BubbleSort.java
[2]: https://github.com/Code2Bits/Algorithms-in-Java/blob/master/sort/src/test/java/com/code2bits/algorithm/sort/BubbleSortTest.java
[3]: https://github.com/Code2Bits/Algorithms-in-Java/blob/master/sort/src/main/java/com/code2bits/algorithm/sort/BubbleSortRecursive.java
[4]: https://github.com/Code2Bits/Algorithms-in-Java/blob/master/sort/src/test/java/com/code2bits/algorithm/sort/BubbleSortRecursiveTest.java
