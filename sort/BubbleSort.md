# Sort Algorithm: BubbleSort

## Overview
Bubble sort is sometimes referred to as sinking sort. The bubble sort algorithm repeatedly steps through the list and compare each adjacent item. The pair of values gets swapped if they are in the wrong order. The algorithm gets its name from the way smaller or larger elements "bubble" to the top of the list.

## Algorithm Classification

| Classification | Value|
| --- | --- |
| Data structure | Array |
| Worst Case | O(n<sup>2</sup>) |
| Average Case | O(n<sup>2</sup>) |
| Best Case | O(n) |

## Pseudocode



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



## Conclusion
