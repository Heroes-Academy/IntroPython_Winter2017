Week 7 Refresher, Part 1
========================


For all of the following examples, please write down the order of the print
statements on a sheet of paper. 


Example 1
^^^^^^^^^

.. code-block:: python
    :linenos:
    
    print("a")

    def some_function():
        print("b")
    
    print("c")
    some_function()
    print("d")
    

Example 2
^^^^^^^^^

.. code-block:: python
    :linenos:
    
    print("a")

    def get_potatoes(number_potatoes):
        if number_potatoes > 5:
            print("b")
        else:
            print("c")
        print("d")
    
    print("e")
    get_potatoes(5)
    print("f")
    

Example 3
^^^^^^^^^

.. code-block:: python
    :linenos:
    
    print("a")

    def bake_bread(number_loafs):
        print("b")
        if number_loafs > 3:
            return "c"
        print("d")
        
        return "e"
        
        print("f")
        
        
    print("g")
    result = bake_bread(6)
    print(result)
    print("h")
    
    
    
    
    
When you get here
^^^^^^^^^^^^^^^^^

First, tell me that you got here. Stuff after this is bonus.

To stay busy and practice while others finish, look at the following code.
It will run, but you should make things better.

First, in the function :code:`spiral`, you should change the arguments
:code:`num_times` and :code:`angle` so that they are default arguments
in the same way :code:`color` is in the function :code:`make_turtle`.

Then, make your own function in :code:`run_version1`.   You should add
some arguments to this function so you can change things freely.
     
.. code-block:: python
    :linenos:
    
    import turtle
    
    def make_turtle(color='blue'):
        turt = turtle.Turtle()
        turt.color(color)
        turt.speed("fastest")
        return turt
    
    def spiral(turt, num_times, angle):
        for i in range(num_times):
            turt.forward(i)
            turt.left(angle)
        
    
    def run_version1(turt):
        print("fill in a design here")
        
    
    theo = make_turtle("red")
    george = make_turtle()
    
    print("Doing a spiral!")
    spiral(theo, 100, 30)
    
    print("First design!")
    run_version1(george)