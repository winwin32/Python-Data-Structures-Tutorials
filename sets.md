# Sets
## Introduction 
Sets are a slightly limited but much faster form of data structure.

**Baseline Knowledge and Setup**

Basic understanding of Python

Means of writing and compiling Python code

## Big O notation 
There is a measure programmers use to categorize how efficient their program is. They call it Big O notation. 

Big O notation is separated into several categories, each with a different processing speed and ability to manipulate data. 

You could compare these categories to businesses. If a small business has a few customers, it can always handle it. But if they are suddenly flooded with business, they will start to struggle. A large business however can handle anything from a few customers to a Black Friday mob. 

From most efficient to least efficient, the different Big O notations are: 

O(1), O(log n), O(n), O(n log n), O(n^2), O(2^n), O(n!)

It is important to understand that Big O notation doesn't measure an exact speed for each program. It abstracts it down to see a basic idea of how its resource demands can multiply. 

For a simple example, here we have a single variable. 

` x = 1 `

If we access this variable, the computer only needs to check one location to find it. 

`print(x)`

Output:

`1`

This is O(1). The program can easily find the information. Here is another example. 

```
myList = [1, 2, 3]

if(3 is in myList):
	print(“We found 3!”)
```

To find 3, the program has to traverse the entire list. That makes this O(n). n in this equation represents the length of the list, because the length of the program is entirely dependent on how long that list is. 

Big O notation is an abstract representation of how many resources a program could potentially require. This is especially useful in large programs. 

![alt text](o-complexity.png "Big O Notation")

https://www.digitalocean.com/community/tutorials/js-big-o-notation

## Comparing Sets and Lists
Sets are a lot like lists, but have two differences. They don't allow duplicate values, and they don't keep their data in a fixed order. 
If you tried to add 1 and then 1 again to a set, it wouldn't register the second value. 
And if you added 1, 2, 3 to a set, it might give you back 3, 1, 2 
These odd rules allow sets to be extremely fast at searching themselves for data. A set can find a stored value in O(1), whereas a list can't do faster than O(n). 
Because of this, we want to use sets whenever our data and purpose fits its specific rules.

To create a set, the syntax is as follows: 

`mySet = {}`

We can even create the set with some variables to start with. 
## Example
``` python
mySet = {1}

mySet.add(2)
mySet.add(3) 
mySet.add(1)

print(mySet)
```
Output: 
```
{1, 2, 3}
```
Notice how it didn't add another 1 to the set, because we already had one when it was created. 

Also, even though I added the variables in the order 2, 3, 1 it displayed them in the order 1, 2, 3. 

Because of this, we need the exact value of what we're looking for in a set, not just an index like a list. 
## Problem to Solve
We can remove a specfic item from a list with the following syntax: 

`mySet.remove("item")`

For this excercise, take the following data

`fruit = ["apple", "orange", "banana", "tomato", "carrot", "pasta", "orange", "oil", "dragonfruit", "banana", "apple"]`

Using a set, manipulate this data until it only shows fruit and does not have any duplicates. 
