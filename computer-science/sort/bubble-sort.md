A comparison based sorting algorithm
- It iterates left to right comparing every couplet, moving the smaller element to the left.
- It repeats this process until it no longer moves and element to the left.

What you need to know:
- While it is very simple to implement, it is the least efficient of these three sorting methods.
- Know that it moves one space to the right comparing two elements at a time and moving the smaller on to left.

Big O efficiency:
- Best Case Sort: Merge Sort: O(n)
- Average Case Sort: Merge Sort: O(n^2)
- Worst Case Sort: Merge Sort: O(n^2)

```
for (int i = 0; i < data.Length; i++)
   for (int j = 0; j < data.Length - 1; j++)
      if (data[j] > data[j + 1])
      {
         tmp = data[j];
         data[j] = data[j + 1];
         data[j + 1] = tmp;
      }
```
