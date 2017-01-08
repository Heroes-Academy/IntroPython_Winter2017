Week 6: Functions Part 4
========================

You can use functions with turtles in really fun ways!


Make Turtle Function
--------------------

Our first turtle function will make a new turtle for us, and do all of the 
property changes that we want!

It should output the turtle. It can take inputs if you'd like (maybe for color, size, etc)

.. code-block:: python
    :linenos:
    
    def make_turtle():
        out_turtle = turtle.Turtle()
        ### CODE HERE
        ### modify properties like color, speed
        
        ### return the turtle back
        
    bob = make_turtle()
        


Turtle Spiral Function
----------------------

Our second turtle function will make a spiral using a :code:`for` loop! 

- **Input**: It should take as input :code:`turt`, which is the turtle that will do the loop. 
- **Input**: It should take as input :code:`num_times`: and that should be used for how many times
the :code:`for` loop  will run.
- **Input**: It should take as input :code:`angle`: and that should be used for what angle the
turtle will turn.
- **Bonus**: make these :code:`num_times` and :code:`angle` arguments be keyword arguments!
- **Output**: The function should return nothing!

.. code-block:: python
    :linenos:

    def spiral(turt, ______):
        ### your code goes here
        

Turtle Polygon Function
-----------------------

This turtle function should make a polygon using a :code:`for` loop!

- **Input**: It should take as input :code:`turt`
- **Input**: Take as input the :code:`num_sides` so that you can make any sided polygon
- **Output**: The function should return nothing

**important**: the angle that a turtle must turn for a polygon is :code:`360/num_sides`.


.. code-block:: python
    :linenos:

    def polygon(turt, ________):
        ### fill in the code here
        

Bonus: Turtles with Keyboard part 1
-----------------------------------

Now we will use functions to add interaction to our turtles!

I have written the first function below to make the turtle go **up**.  
You should write the rest for **left**, **right**, and **down**. 

**Vocabulary: this is called 'binding' the key to a function**


.. code-block:: python
    :linenos:
    
    screen = turtle.screen()
    
    bob = make_turtle()
    
    def move_bob():
        bob.forward(100)
        
    screen.onkey(move_bob, "space")
    screen.listen()
    


Bonus: Turtles with Keyboard part 2
-----------------------------------

Now that you can control your turtle, you should given it some extra skills!

Finishing writing the function below.  It will make it so that when you press "s", the 
turn will do the spiral function you wrote above!  

**Vocabulary: This is binding the key 's' to a function**

After that, write some other functions that make the turtle do things.  Some ideas:

1. Increase the turtle's size
2. Decrease the turtle's size
3. Make the turtle stamp
4. Make the turtle draw a circle, square, polygon, etc

.. code-block:: python
    :linenos: