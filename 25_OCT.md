#25 OCT 17
##SUPER CLASS
---------------

[CODE FELLOWS](https://codefellows.github.io/sea-python-401d7/lectures/intro_to_python_6_super_etc.html#super)

*.mro()* = method resolution order

When setting super in a function you call the class itself

EX:
====

instead of:

```class A(B):
    def __init__(self, *args, **kwargs)
        B.__init__(self, *args, **kwargs)
```

You can do:

```class A(B):
    def __init__(self, *args, **kwargs)
        super(A, self).__init__(*args, **kwargs)
        ...
```

##STATIC METHODS
------------------
Really no need - Just set globally

##PYTEST FIXTURES
-------------------
How to setup a fixture:
```
import pytest

@pytest.fixture
def the_fixture():
    print("this line runs")
    print("this line also runs")
    created_value = 5
    return created_value
```
