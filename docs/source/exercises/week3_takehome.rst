Week 3: Take home exercises
===========================


What is your favorite color?
****************************

1. Get input from the user using the input function
2. Check to see if it’s a specific color 
3. Is the string the user provided equal to the string “blue” or the string “red”?
    - If it is, tell the user something about it
        + print out “{} is a super cool color!”
    - Else, tell the user something different
        + print out “{} is an ok color”


Menu Options
************

1. Print at least 2 options to the user
2. Each option should have a number at the front.
    - For example:  
::
    An Awesome Menu
    1. Tell a Joke
    2. Play a Game
3. Get the input choice from the user 
    - “What menu item do you want?”
4. Check to see if that choice is equal to one of the options
    - If it is, do that option
    - If it isn't, print an error message


Bonus
*****

1. Make your menu two-levels.  This requires a "nested if".  
2. Use random to have a dice roll be one of the options. 

.. code-block:: python
    :linenos:
    
    import random
    
    random_number = random.randint(0, 6) # a random number between 0 and 6 (includes 0, doesn't include 6)
    random_number = random.randint(1, 7) # a random number between 1 and 7 (includes 1, doesn't include 7)
    




