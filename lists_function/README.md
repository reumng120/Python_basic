# This article will describes how to use the lists function.

## Architecture
![alt text](https://github.com/reumng120/Python_basic/blob/main/lists_function/lists_function.png?raw=true)

## Functions
- list.append(x): Add an item to the end of the list.
```
>>> mylist = ['jack', 'guido', 'irv']
>>> mylist.append("book")
>>> mylist
['jack', 'guido', 'irv', 'book']
>>> 
```
- list.extend(x): Extend the list by appending the items from the iterable.
```
(Spilit the character into list.)
>>> mylist.extend("Monday")
>>> mylist
['jack', 'guido', 'irv', 'book', 'M', 'o', 'n', 'd', 'a', 'y']
```
```
(Using list to extend the list.)
>>> mylist.extend(["mon", "thu"])
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu']
>>>
```
- 
