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
- list.insert(i, x): Insert an item ad a given index.
```
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu']
>>> 
>>> mylist.insert(1, "wed")
>>> mylist
['jack', 'wed', 'guido', 'irv', 'book', 'mon', 'thu']
>>> mylist.insert(3, "Sun")
>>> mylist
['jack', 'wed', 'guido', 'Sun', 'irv', 'book', 'mon', 'thu']
>>> 
```
- list.remove(x): Remove the item from given the value.
```
>>> mylist
['jack', 'wed', 'guido', 'Sun', 'irv', 'book', 'mon', 'thu']
>>> mylist.remove("Sun")
>>> mylist.remove("wed")
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu']
>>> 
```
- list.index(x): Return position of an item in the list by the zero-base index.
```
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu']
>>> mylist.index("irv")
2
>>> mylist.index("mon")
4
>>> 
```
- list.count(x): Return the number of times x appears in the list.
```
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu', 'book', 'book', 'mon']
>>> mylist.count("irv")
1
>>> mylist.count("book")
3
>>> mylist.count("mon")
2
>>> 
```
- list.pop(i): Remove the item from given the index. If no index is specified, list.pop() removes the last item in the list.
```
>>> mylist
['jack', 'guido', 'irv', 'book', 'mon', 'thu', 'abc']
>>> mylist.pop()
'abc'
>>> mylist.pop(3)
'book'
>>> mylist
['jack', 'guido', 'irv', 'mon', 'thu']
>>> 
```
- list.sort(*, key=None, reverse=False): Sort the items of the list.
```
(sort 1)
>>> mylist
['book', 'dance', 'apple', 'cook']
>>> mylist.sort()
>>> mylist
['apple', 'book', 'cook', 'dance']
>>> 
>>> mylist.sort(reverse=True)
>>> mylist
['dance', 'cook', 'book', 'apple']
>>> 
```
```
(sort 2: Using function)
>>> def cusFunc(e):
...     return len(e)
... 
>>> mylist = ["increse", "programming", "apple", "Std"]
>>> mylist.sort(key=cusFunc, reverse=True)
>>> mylist
['programming', 'increse', 'apple', 'Std']
>>> 
```
- 
