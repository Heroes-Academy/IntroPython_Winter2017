Week 4 Refresher
================

Let's refresh your memory!
First, read the reminders about syntax.
Then, complete the exercises!


Reminders
---------

Basic Variables and Operations
******************************

There are four basic variable types

.. code-block:: python
    :linenos:

    x = 5     # int
    x = 5.0   # float
    x = "5"   # str
    x = True  # bool

You can convert between types

.. code-block:: python
    :linenos:

    y = "5"       # a string variable
    x = int(y)    # convert to integer
    x = float(y)  # convert to float
    z = str(x)    # convert the float to string. does this equal "5" or "5.0"

There are 7 math operator types

.. code-block:: python
    :linenos:

    x = 10
    y = 2
    x + y
    x - y
    x * y
    x / y
    x // y
    x ** y
    x % y

There are shortcuts for math operators.  The following pairs of statements have the same result.

.. code-block:: python
    :linenos:

    x = 5
    y = 3
    # x = x + y
    x += y

    x = 5
    y = 3
    # x = x - y
    x -= y

    x = 5
    y = 3
    # x = x * y
    x *= y

    x = 5
    y = 3
    # x = x / y
    x /= y

    x = 5
    y = 3
    # x = x // y
    x //= y

    x = 5
    y = 3
    # x = x ** y
    x **= y

    x = 5
    y = 3
    # x = x % y
    x %= y

Booleans and Comparisons
************************

There are boolean variables

.. code-block:: python
    :linenos:

    x = True
    x = False

Variables can be compared to create boolean variables

.. code-block:: python
    :linenos:

    x = 42
    y = 41
    x == y
    x != y
    x > y
    x >= y
    x < y
    x <= y

Boolean variables can be combined using the special boolean keywords

.. code-block:: python
    :linenos:

    x = True
    y = False
    z1 = x and y
    z2 = x or y
    z3 = (x and y) or (not x and not y)
    z4 = (not x and y) or (x and not y)

Code blocks let you group code.  In python, they are created with 4 spaces.
In pycharm and most python editors, hitting tab will just add 4 spaces.
:code:`if` statements use code blocks.

.. code-block:: python
    :linenos:

    x = 10
    y = 9
    if x > y:
        print("X is bigger!")

:code:`if` statements can be expanded using :code:`elif`.  
:code:`elif` will only be used if the first :code:`if` is false.
(hidden question: What needs to be put into the placeholder to make the above code work?)

.. code-block:: python
    :linenos:

    x = "3"
    # placeholder
    if x == 1:
        print("x is 1")
    elif x == 2:
        print("x is 2")
    elif x == 3:
        print("x is 3")
    else:
        print("I'm not sure what x is")


Getting Input from Users
************************

You can use the :code:`input` to get information from the user.
Try the following.  What is missing?

.. code-block:: python
    :linenos:

    print("My Menu: ")
    print("\t 1. Option 1")
    print("\t 2. Option 2")
    print("\t 3. Option 3")
    x = input("What option do you choose?")
    # placeholder
    if x == 1:
        print("x is 1")
    elif x == 2:
        print("x is 2")
    elif x == 3:
        print("x is 3")
    else:
        print("I'm not sure what x is")

