Week 3: Boolean Exercises
=========================

Syntax Information
------------------

.. code-block:: python
    :linenos:
    
    var1 = True
    var2 = False
    
    False and False     # is False
    True and False      # is False
    False and True      # is False
    True and True       # is True
    
    False or False      # is False
    True or False       # is True
    False or True       # is True
    True or True        # is True
    
    not False           # is True
    not True            # is False
    
    5 == 5              # is True
    5 != 4              # is True
    4 == 5              # is False
    4 <  5              # is True
    4 <= 5              # is True
    5 <= 5              # is True
    5 <  5              # is False
    4 >  5              # is False
    6 >= 6              # is True
    
    
    
Practice
--------

Write down the results for the items

.. code-block:: python
    :linenos:
    
    var1 = False
    var2 = True
    
    
    item1 = var1 and var2
    item2 = (not var1) and var2
    item3 = var2 and (not var1)
    item4 = item3 or (not item1)
    
.. 
    item1 = False
    item2 = True
    item3 = True
    item4 = True

For this one, write down the truth table for all values that var1 and var2 can have.

.. code-block:: python
    :linenos:
    
    item5 = (not var1 and var2) or (var1 and not var2)
    
    
Making Booleans
---------------

You can make booleans with the comparison operators


.. code-block:: python
    :linenos:

    x = 5
    y = "awesome!"
    
    # Here we have parenthesis to show which part is the comparison
    item1 = (x==5)
    item2 = (x>3)
    
    # technically we don't need the parenthesis!
    # you can keep using them if you want
    item3 = x % 2 == 0
    item4 = y[0] == "a"
    item5 = y[-1] == "!"
    
    # remember, you can use to say "not"
    item6 = y != "awesome!"
    
    # I am using parenthesis here to group a math operation together:
    item7 = (x-2) != 3
    
