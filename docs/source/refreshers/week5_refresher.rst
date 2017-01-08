Week 5 Refresher
================

Refresher 1
-----------

Write down the variable type for all of the "x" variables. 
If it requires a calculation, write down the answer as well. 
Verify your answers using python. 
Remember that you can use "type(x)" in the iPython shell to figure out the variable type. 

.. code-block:: python
    :linenos:

    x = 10
    x = 5.2
    x = "5.5"
    x = False
    x = 10 / 2
    x = 10 % 3
    x = 5 + 4 % 3
    x = (5 + 4) % 3
    x = 10 < 38
    x = 10 == 10
    x = 57 % 2 == 0
    
    y = 30
    if y % 3 == 0:
        x = y // 3
    else:
        x = y + 1
        
Refresher 2
-----------

Finish the following code so that it tests for X being a modulo 2, 3, 4, 5, and 6.
    - be careful with the ordering of the tests
    - there should only be ONE :code:`if` statement. The rest should be :code:`elif`


.. code-block:: python
    :linenos:

    x = input("Give me any whole number: ")
    
    if x % 2 == 0:
        print("X is a multiple of 2!")
    
    
