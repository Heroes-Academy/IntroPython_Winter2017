

For Loops
*********

The last thing we learned about is the ``for`` loop. ``for`` loops are great - they use indented lines to form a 'paragraph' (kind of like If statements!) and let you run the code in that paragraph over and over again, as many times as you want!

Say you wanted to print someone's name 10 times (kind of a ridiculous example). The loop would look like this:
::
	for i in range(10):
		print("Cinder")

That's it! If you execute this code in Python (easier to type it into PyCharm than the shell), it will print out "Cinder" ten times in a row.

Breaking it down:

- ``for`` is a special keyword - when Python sees it, it knows we'll be repeating some code
- ``i`` is just a variable, just like ``x`` or ``username``
- ``range(10)`` is the list of all numbers from 0 to 9

In the above For loop, Python will repeated the indented code 10 times, and each time, ``i`` will take a new value.

- First time through: ``i`` is ``0``
- Second time through: ``i`` is ``1``
- Third time through: ``i`` is ``2``

etc.

So you can also do something like this:
::
	for i in range(5):
		print(i)

This will print 0, 1, 2, 3, and 4, because the code will execute 5 times, and each time, ``i`` has a different value!

For loops can be tricky to wrap your head around. The best thing to do is to use the above two examples, copy them into PyCharm, and verify that they work.
Then try changing the number in range(), and also change around what happens in the indented text.
The best way to practice new coding techniques is to try it yourself

Trinkets
--------

1. Turtle Loops 1

.. raw:: html

    <iframe src="https://trinket.io/embed/python/eb7b608d56" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

2. Turtle Loops 2

.. raw:: html

    <iframe src="https://trinket.io/embed/python/fc826fce5d" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

3. Turtle Circles

.. raw:: html

    <iframe src="https://trinket.io/embed/python/6db31dcde4" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

4. Turtle Triangle Trick!

.. raw:: html

    <iframe src="https://trinket.io/embed/python/abd2f8c9d6" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

5. Two Turtles and Triangle Stamps

.. raw:: html

    <iframe src="https://trinket.io/embed/python/999e0b531e" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

6. Turtle Star!

.. raw:: html

	<iframe src="https://trinket.io/embed/python/59941a36dd" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>



Extra Turtle Challenge: Specific Coordinates
--------------------------------------------

Turtles are awesome because we can make them do many things.
Let's create the turtle first:

.. code-block:: python
   :linenos:

    import turtle
    bob = turtle.Turtle()
    bob.speed('fastest')

Now,  in the following, we can make the turtle go to very specific coordinates:

.. code-block:: python
   :linenos:

    bob.setpos(100,0)

Bob is now at x=100 and y=0.
In general, the syntax is ``setpos(x_coord,y_coord)``.

We can use this to make interesting things.
For example, if I want to make bob do a triangle without a for loop:

.. code-block:: python
   :linenos:

    bob.setpos(-100, 0)
    bob.setpos(0,100)
    bob.setpos(100,0)
    bob.setpos(-100, 0)

What's even cooler is that we can use variables to make this scalable:

.. code-block:: python
   :linenos:

    tri_size = 30
    bob.setpos(-1*tri_size, 0)
    bob.setpos(0, 1*tri_size)
    bob.setpos(1*tri_size, 0)
    bob.setpos(-1*tri_size, 0)

But this is a lot of code for something simple.
What if we could store all of the coordinates ahead of time and then
use a for loop to loop over the coordinates?

.. code-block:: python
   :linenos:

    tri_size = 130
    coords = [[-1, 0], [0, 1], [1, 0], [-1, 0]]
    for coord in coords:
        x = coord[0]
        y = coord[1]
        bob.setpos(x*tri_size, y*tri_size)


This triangle looks a little funny.
What if we wanted to have each side be the same length AND use the coords list?
What numbers would we have to change?

The Challenge
*************

Use a coordinate list like the one above to make your initials (first and last).
