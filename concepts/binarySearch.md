# Binary Search

Binary search is an efficient algorithm for finding an item from a sorted list of items. It works by repeatedly dividing in half the portion of the list that could contain the item, until you've narrowed down the possible locations to just one.

## How Binary Search Works

1. **Start with the entire list**:
   - Determine the middle element of the list.
   - If the middle element is the target, you're done.
   - If the target is less than the middle element, repeat the search in the left half of the list.
   - If the target is greater than the middle element, repeat the search in the right half of the list.
2. **Repeat the process**:
   - Continue to divide the list in half until the target is found or the list cannot be divided further.

## Example

Suppose we have a sorted list `[1, 3, 5, 7, 9, 11, 13]` and we want to find the position of the number `7`.

1. **Initial list**: `[1, 3, 5, 7, 9, 11, 13]`
   - Middle element: `7` (target found!)

If the target was not `7`, we would decide which half to look at next and repeat the process.

## Python Implementation

```python
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    
    while left <= right:
        mid = (left + right) // 2
        
        # Check if target is present at mid
        if arr[mid] == target:
            return mid
        # If target is greater, ignore left half
        elif arr[mid] < target:
            left = mid + 1
        # If target is smaller, ignore right half
        else:
            right = mid - 1
    
    # Target is not present in array
    return -1
```