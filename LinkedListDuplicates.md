### Given a sorted linked list, write an algorithm to delete all duplicate numbers from the sorted linked list.

https://terriblewhiteboard.com/remove-duplicates-from-sorted-list-leetcode-83/


````
function removeDup(linkedList) {
  let current = linkedList.head
  while (current !== null && current.next !== null) {
    if (current.val === current.next.val) {
      current.next = current.next.next
      }
    else {
        current = current.next
    }
  }
  return head
}
````
