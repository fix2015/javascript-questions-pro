## [Merge Two Sorted Linked Lists](#merge-two-sorted-linked-lists)

### Merge Two Sorted Linked Lists

To merge two sorted linked lists into one sorted linked list, use a two-pointer approach to traverse both lists and merge them in sorted order.

#### Algorithm:
1. Initialize two pointers, one for each list.
2. Compare the elements of both lists and append the smaller element to the merged list.
3. Once one list is exhausted, append the remaining elements from the other list.
4. Return the merged sorted list.

#### Example:
```javascript
function mergeLists(l1, l2) {
    let dummy = new ListNode(0);
    let current = dummy;
    while (l1 && l2) {
        if (l1.val < l2.val) {
            current.next = l1;
            l1 = l1.next;
        } else {
            current.next = l2;
            l2 = l2.next;
        }
        current = current.next;
    }
    current.next = l1 || l2;
    return dummy.next;
}

// Example usage
// Assuming ListNode is defined with val and next properties
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two linked lists.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Linked Lists](./theme/linked_lists), [Algorithm](./theme/algorithm)


