### Navigation
* [Queues][1]

* [Sets][2]

* [Trees][3]

[1]: https://github.com/winwin32/Python-Data-Structures-Tutorials/blob/main/queues.md

[2]: https://github.com/winwin32/Python-Data-Structures-Tutorials/blob/main/sets.md

[3]: https://github.com/winwin32/Python-Data-Structures-Tutorials/blob/main/tree.md

## Introduction
Imagine a line at DisneyLand. Each person enters the line at the back, and leaves when it’s their turn to get on the ride everyone is waiting for. Cutting in the line is not allowed. 

Queues work the same way. As information is added, it goes to the back of the queue and it can’t exit the queue until all the items in front of it move out of the queue. It follows the First In First Out structure, or FIFO. 

**Baseline Knowledge and Setup**

Basic understanding of Python

Means of writing and compiling Python code

**Why should you care?**

In many cases, queues can make your program process faster than if you used other data structures. In small programs, this is difficult to notice. But once you work on huge programs with thousands of lines of code, the difference can be significant. 

## Lists in Python
A list in Python does not need to follow the queue structure, but it can be used to simulate a queue. 
You can create a list with this syntax. 

`my_queue = []`

## Append, Pop and FIFO
We can add or subtract items from our queue with two commands. The first is “append”, which adds an item to the front of the list. You will need to include the item you want to add to the list in parentheses. This is the syntax.

`my_queue.append(number)`

Second is “pop”, which removes the last item from the list, and returns the value. This is the syntax.

`my_queue.pop()`

With only these two commands, we can turn our list into a queue. 

## Example
``` python
num1 = 1
num2 = 2
num3 = 3

my_queue = []

my_queue.append(num1)
my_queue.append(num2)
my_queue.append(num3)

print(my_queue.pop())
print(my_queue.pop())
print(my_queue.pop())

Output: 
1
2
3
```

Here is all the methods you can use to implement a queue and their speeds according to Big O notation.

|Method|Speed|
|-|-|
| my_queue.pop() | O(1)
| my_queue.pop(#) | O(n)
| my_queue.append() | O(1)

## Problem to Solve
In this problem, we have an empty queue and some loose variables. 
Starting with the following code, use the correct combination of "append" and "pop" to display the information in the right order. 

**Hint:** *Remember to print your "pop" commands*

``` python
var1 = "e"
var2 = "f"
var3 = "a"
var4 = "c"
var5 = "d"
var6 = "b"

queue = []

#Start your code here. 
```
