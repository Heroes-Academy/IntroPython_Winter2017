Fors and Turtles!
================

`Link to turtle cheatsheet <https://github.com/Heroes-Academy/IntroPython_Fall2016/blob/master/code/week04/Turtles%20Cheat%20Sheet.pdf>`_

For this exercise, you will use a single turtle in more complex situations:

1. In a for loop using :code:`range`
2. In a for loop using :code:`range` and :code:`if` to change the colors
3. Fizz Buzz!  Read below for instructions =).

Basic turtle setup:

.. code-block:: python
    :linenos:

    ### first, import turtles
    import turtle

    ### then, create a turtle!
    bob = turtle.Turtle()
    bob.speed('fastest')

    ### do stuff with the turtle
    # for example, a triangle!
    for i in range(3):
        bob.forward(100)
        bob.left(120)

    ### end the code with the following, so python knows to keep the window open
    turtle.done()

Exercise 1
**********

.. code-block:: python
    :linenos:

    import turtle

    bob = turtle.Turtle()

    for i in range(500):
        bob.forward(i)
        bob.left(95)


Change the code so that each time around the :code:`for` loop, the turtle draws a triangle or a square.


Exercise 2
**********

.. code-block:: python
    :linenos:

    import turtle

    bob = turtle.Turtle()

    color1 = "#cc3333" ### you can use the internet to get more of these
    color2 = "#3333cc"

    for i in range(500):
        bob.forward(i)
        bob.left(95)

        if False:
            print("change colors here")

Change the code above so that the :code:`if` statement will change the turtle's color when :code:`i` is even.


Exercise 3
**********

Fizz Buzz!

Modify the code in Exercise 2 so that:

    - when :code:`i` is a multiple of 3
        - turn the turtle color1
        - make the turtle write "fizz"
    - when :code:`i` is a multiple of 5
        - turn the turtle color2
        - make the turtle write "buzz"
    - when :code:`i` is a multiple of both
        - turn the turtle color3
        - make the turtle write "fizz buzz"
    - else, make the turtle black and write nothing. 
    


Bonus Exercise 1
****************

You can "nest" loops inside each other:

.. code-block:: python
    :linenos:

    for i in range(5):
        for j in range(2):
            print(i,j)

Use a nested loop inside the turtle's for loop to do more interesting patterns.


Exercises that use a list
-------------------------

Exercise 1
****************

Lists let you store ordered sets of things.  There are a couple different ways to make a list.

.. code-block:: python
    :linenos:

    mylist = list()
    mylist.append(5)
    mylist.append(10)

    print(mylist)
    print(mylist[0])
    print(mylist[1:])

    mylist = [5, 10]

    print(mylist)
    print(mylist[0])
    print(mylist[1:])

You can use lists in for loops instead of range

.. code-block:: python
    :linenos:

    for item in mylist:
        print(item)


Do the following:
1. create a list with multiple turtles
::
    turtle_list = [turtle.Turtle()]
    turtle_list.append(turtle.Turtle())
2. use a second for loop inside the main for loop to make each turtle move
::
    for t in turtle_list:
        # code here
