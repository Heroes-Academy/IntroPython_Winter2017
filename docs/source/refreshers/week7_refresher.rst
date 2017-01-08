Week 7 Refresher
================

This week you will only have one problem to solve for the refresher.
Use the cookbook to help you solve it.
I have given you little code here so that you can connect the way I describe code to the code itself better.

Nested :code:`for` loops
----------------

Sometimes in Computer Science, having loops that are inside other loops are really useful.
When this happens, we can refer to the loops as layers.  Think of it like an onion.

Requirements:

1. Write two :code:`for` loops, one inside the other.
    - The outer :code:`for` loop should start at 1 and go to 20.
    - The inner :code:`for` loop should start at 1 and go to 10.
2. Before both :code:`for` loops, create an empty :code:`list`.
3. Inside the inner :code:`for` loop, multiply the two loop variables.
    - if you aren't sure what I mean by "loop variable", check the cookbook.
4. Check if the resulting number is inside the list yet.
    - If you aren't sure what I mean by "is inside", check the :code:`list` part of the cookbook
5. If the result is not in the :code:`list`, then add it to the :code:`list`.
6. After both loops are finished, print out the length of the :code:`list`.

Things to observe:

1. What happens if you change the sizes of the loops?  For instance, if you make the 20 number into 200?  Do you notice anything about the speed of the code?

2. I have written about :code:`set`s in the cookbook.  Use a :code:`set` instead of a :code:`list`. Is it faster?

3. Count how much faster it is.  Do this using the :code:`time` module. This is also in the cookbook.

