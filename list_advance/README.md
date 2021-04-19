# Advance to use list

## List Comprehensions
There is a simple way to create a list of math function.
```
>>> mylist = []
>>> for x in range(5):
...     mylist.append((x + x) * x)
... 
>>> mylist
[0, 2, 8, 18, 32]
```
A variable named x that still exists after the loop completes. There are two ways can avoid the side effect.
```
>>> mylist = list(map(lambda x: (x+x)*x, range(5)))
>>> mylist
[0, 2, 8, 18, 32]
```
and
```
>>> mylist = [(x+x)*x for x in range(5)]
>>> mylist
[0, 2, 8, 18, 32]
```
## Set()
The set is an unordered collection with no duplicate elements. It also support the mathematical oprations like, union, intersection, difference, and symmetric difference.

```
(With no duplicate element)
>>> mylist = ["book", "apple", "Jon", "apple", "cycle"]
>>> non_duplicate = set(mylist)
>>> non_duplicate
{'book', 'Jon', 'cycle', 'apple'}
```
Mathematical oprations
```
>> a = set("abcd")
>>> b = set("cdef")
>>> a
{'c', 'b', 'd', 'a'}
>>> b
{'e', 'c', 'd', 'f'}
```
letter in a but not in b
```
>>> a - b
{'b', 'a'}
```
letter in a or b or both
```
>>> a | b
{'e', 'd', 'f', 'a', 'c', 'b'}
```
letter in both a and b
```
>>> a & b
{'c', 'd'}
```
letter in a or b but not both
```
>>> a ^ b
{'e', 'f', 'a', 'b'}
```

