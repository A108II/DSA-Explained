## Linked Lists

### Overview
- `Linked lists` are often compared to `arrays`.
- `Arrays` have `indexes` but `linked lists` do not.
- `Arrays` are stored in `contiguous places` in memory; `linked lists` are not.
- A `linked list` has a variable called `head` that `points` to the `first item`.
- A `linked list` may have another variable called `tail` that points to the `last item`.
- Each item in the `linked list` points to the `next` item, and the `last one` points to `null`.

### Linked Lists Big O

#### Adding and Removing Items from the End of a Linked List
- **Adding**: The last item will point to the newly added item, and the `tail` will point to the newly added item. The operation is constant time, so the big O is `O(1)`.
- **Removing (Popping)**: To ensure the `tail` points to the last item, you need to iterate through the list from `head` to find the second last item. The time complexity is `O(n)`.

#### Adding and Removing Items from the Beginning of a Linked List
- **Adding (Unshifting)**: Set the new node's `next` to point to the current `head`, and update the `head` to point to the new node. This is a constant-time operation, so the big O is `O(1)`.
- **Removing (Shifting)**: Update the `head` to point to `head.next` and remove the first node. This is also a constant-time operation, so the big O is `O(1)`.

#### Adding and Removing Items from the Middle of a Linked List
- **Adding (Inserting)**: Iterate through the list to find the position, set the new node's `next` to point to the current node at that position, and update the previous node to point to the new node. This requires traversal, so the big O is `O(n)`.
- **Removing**: Iterate through the list to find the node before the one to be removed, update its `next` to skip the node to be removed, and point to the subsequent node. This also requires traversal, so the big O is `O(n)`.

#### Finding an Item in a Linked List
- **Finding by Value or Index**: You need to iterate through the items to find the desired value or index. This operation has a time complexity of `O(n)`.

### Linked Lists Structure
- Each element in a linked list is called a `node`.
- A `node` consists of a `value` and a `next` property which points to the next node in the list.

### Representing a Linked List
- Example: A linked list with `Head -> 3 -> 8 -> 52 -> 4 -> null`.

### Linked List Operations

#### Constructor
- Initializes a linked list with a given value, setting both `head` and `tail` to the new node.

#### Push
- **Description**: Adds a node to the end of the linked list.
- **Big O**: `O(1)`.

#### Pop
- **Description**: Removes the last node of the linked list and updates the `tail`.
- **Big O**: `O(n)` (due to the need to iterate to find the second last node).

#### Unshift
- **Description**: Adds a new node to the beginning of the linked list.
- **Big O**: `O(1)`.

#### Shift
- **Description**: Removes the first node of the linked list and updates the `head`.
- **Big O**: `O(1)`.

#### Get
- **Description**: Retrieves a node at a specific index by iterating through the list.
- **Big O**: `O(n)`.

#### Set
- **Description**: Updates the value of a node at a specific index.
- **Big O**: `O(n)` (depends on the `get` operation).

#### Insert
- **Description**: Inserts a new node at a specific index by updating pointers.
- **Big O**: `O(n)`.

#### Remove
- **Description**: Removes a node at a specific index by updating pointers.
- **Big O**: `O(n)`.

#### Reverse
- **Description**: Reverses the linked list by reassigning pointers.
- **Big O**: `O(n)`.

- Check out the `Linked_List.md` file.
