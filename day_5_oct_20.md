# DAY 5 : 20 OCT 17

## LISTS
### Sorting Lists
-------------------
#### Given a list
people = [{'name': 'Nick', 'amt': 500}, {'name': 'Bob', 'amt': 700}, {'name': 'Dan', 'amt': 50}, {'name': 'Adrienne', 'amt': 50000}, {'name': 'Chelsea', 'amt': -88} ]

#### Lambda is an anonymous function (similar lexical arrow function)
sorted(people, key=lambda person: person['amt'])

#### Expected Output
[{'amt': -88, 'name': 'Chelsea'},
 {'amt': 50, 'name': 'Dan'},
 {'amt': 500, 'name': 'Nick'},
 {'amt': 700, 'name': 'Bob'},
 {'amt': 50000, 'name': 'Adrienne'}]

### Converting to list
-----------------------
In [1]: list('abcdefg')
Out[2]: ['a', 'b', 'c', 'd', 'e', 'f', 'g']

#### Tuple
In [1]: list((1, 2, 3))
Out[2]: [1, 2, 3]

### Lists
-----------
[ [] ] * 5
Out[5]: [[], [], [], [], []]

In [1]: foor = _

In [2]: foor[0].append(5)

In [3]: foor
Out[4]: [[5], [5], [5], [5], [5]]

This happens becuase when a list is multiplied, all the lists hold the same id.
You need to long hand lists to append to a specific list inside a list.

foor = [[], [], []]

Each list is there own idea because it was manually put in and not manipulated by a math operator that creates duplicated id's

#### Mutating lists
.extend : adds one lists content and appends it to another list(at the end)
.pop : removes and returns  item
.remove : removes with no return value (if not in list - value error)


### Collections Package
------------------------
In[1]: import collections

In[2]: c = collections.Counter('flerg the blerg because glerg the merg')
Out[2]:
Counter({' ': 6,
         'a': 1,
         'b': 2,
         'c': 1,
         'e': 8,
         'f': 1,
         'g': 5,
         'h': 2,
         'l': 3,
         'm': 1,
         'r': 4,
         's': 1,
         't': 2,
         'u': 1})

### Exeception Handling
-------------------------
#### Example
try:
    # do a thing
except KeyError:
    # do something else
except NameError:
    # do something else

### Testing with Tox
----------------------
Tox allows you to test both Python 2 and Python 3

#### Installing
pip install tox (inside the virtual environment)

#### Using Tox
create a tox.ini file

Inside the tox.ins

[tox]
envlist = py27, py36

[testenv]
commands = py.test --cov --cov-report term-missing
deps =
    pytest
    pytest-cov





