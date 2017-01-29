[Week 4]: Turtles and For Loops
=============================

`Turtles cheat sheet <https://github.com/Heroes-Academy/IntroPython_Fall2016/blob/master/code/week04/Turtles%20Cheat%20Sheet.pdf>`_

Agenda
------


1. Complete the refresher exercises: :doc:`Week 4 Refresher Exercises. <refreshers/week4_refresher>`
2. Listen to me tell you about for loops and turtles!
3. Work on the Week 4 exercises: :doc:`Week 4 Exercises <exercises/week4_for_turtles>`
4. Work on these at home (or in class, if you finish fast enough): :doc:`Week 4 Takehome Exercises <exercises/week4_takehome>`


Review
------

Terms you should know
*********************

1. :code:`for` loops
2. the :code:`loop variable`
3. :code:`range`


From Simple to Complex variables
********************************

There are two ideas you should combine in your head. The first is about simple variables.
Simple variables have a single type.  For example, a simple variable can be an integer or a string.

The other idea you should combine is code robots.
We talked about code robots in class.
Code robots have a very simple design: take an input, give an output.

Combining these ideas, we can talk about complex variables.
Complex variables can have multiple simple variables inside them.
They can also be several code robots in one.

Turtles are just this!  Turtles can have multiple variables, like color and shape.
They can also do multiple things.  You can have it go forward or have it turn!

Summary of Turtles
******************

Turtles are created from their factory.
::
    import turtle
    bob = turtle.Turtle()

Then, you can make it move and turn:
::
    bob.forward(100)
    bob.left(90)



There are many things you can do:
::
    bob.shape('turtle') # change the shape
    bob.stamp() # stamp the shape onto the board
    x=100
    y=100
    bob.goto(x,y) # go to this position
    bob.penup() # stop drawing when the turtle moves
    bob.pendown() # start drawing again



Lecture Slides
--------------

.. raw:: html

    <iframe src="https://docs.google.com/presentation/d/1-ymaDvE_wJEEkWyUo3aS_QflL4d-3nIxxESQP649KrQ/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
