# Linkify

`Linkify` is a Python library that converts arrays into linked lists. This library provides a simple way to create and manipulate linked lists using standard array data.

## Installation

You can install the `Linkify` library using pip:

```bash
pip install Linkify
```
## Usage
- Creating a Linked List from an Array

```
from Linkify import LinkedList

# Create a linked list from an array
arr = [1, 2, 3, 4, 5]
linked_list = LinkedList.from_array(arr)

# Display the linked list with arrows
print(linked_list.display())  # Output: 1 -> 2 -> 3 -> 4 -> 5
```
- Appending Elements

```
from Linkify import LinkedList

# Create an empty linked list
linked_list = LinkedList()

# Append elements
linked_list.append(10)
linked_list.append(20)

# Display the linked list
print(linked_list.display())  # Output: 10 -> 20
```
- Use Case

Imagine you are developing a task management system where tasks are frequently added and removed. Using a linked list for storing these tasks can be more efficient compared to arrays, especially for operations that involve frequent insertions and deletions.

```
from Linkify import LinkedList

# Initial list of tasks
tasks = ['Task 1', 'Task 2', 'Task 3']

# Convert the list of tasks to a linked list
task_list = LinkedList.from_array(tasks)

# Add a new task
task_list.append('Task 4')

# Display the updated task list
print(task_list.display())  # Output: Task 1 -> Task 2 -> Task 3 -> Task 4

# Suppose Task 1 is completed, you can remove it from the list (implementation needed)
# task_list.remove('Task 1')  # Assume you have implemented a remove method

# Display the list after removal
print(task_list.display())  # Output might be: Task 2 -> Task 3 -> Task 4
```
## License

This project is licensed under the MIT License - see the LICENSE file for details.

