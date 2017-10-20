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
