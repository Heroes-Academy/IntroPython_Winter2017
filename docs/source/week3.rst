[Week 3]: Booleans, If-Elif-Else
================================


:doc:`Refresh your knowledge from Week 2! <refreshers/week3_refresher>`
and if you finish quickly, :doc:`an extra challenge <exercises/week3_extrachallenge>`.

Exercises
---------

1. :doc:`In class: Booleans <exercises/week3_booleans>`
2. :doc:`In class: If-Elif-Else Statements <exercises/week3_ifs>`
3. :doc:`Week 3 Takehome Exercises <exercises/week3_takehome>`

Terms
-----

You should know the following terms!

1. Boolean values (True and False)
2. Boolean Algebra (and, or, not)
3. Code blocks (4 spaces!)
4. Conditional operators (!=, ==, >, <, >=, <=)
5. Conditional Statements (If, elif, else)

Extra Review
------------

Booleans
********
Booleans are variables that can have a value of ``True`` or ``False``.
You can set Boolean variables in code with something like ``x = True``, or you can use **comparison operators.**

These are the comparison operators we discussed:

- < less than
- > greater than
- <= less than or equal to
- >= greater than or equal to
- == equal to (remember, in Python, "equal to" uses two equals signs, because one equals sign is just used for making a variable)
- != not equal to

Comparison operators compare the values of two different variables, and will evaluate to either True or False.
For example, ``5 > 3`` will evaluate to ``True``, but ``10 == 9`` will evaluate to ``False``.
You can use these to make Boolean variables as well.

Booleans can also be combined using the ``and`` and ``or`` keywords.
If ``x`` and ``y`` are Booleans, the expression ``x and y`` will only be ``True`` if both ``x`` and ``y`` are ``True``.
``x or y`` will only be ``True`` if at least one of them is ``True``.
And of course, ``not x`` will just be the opposite of ``x``.

We practiced evaluating Booleans using cards and complex conditions: :code:`(suit == hearts and not number <= 5)`.

If Statements
*************

``if`` statements are comprised of two ingredients: a condition (which must evaluate or be a boolean), and some code.
Python checks if the condition is True; if it is, the code will be executed.
But if the condition is False, Python will just ignore the code and move on.

If statements kind of resemble a paragraph - the condition goes at the top, and the accompanying code is all indented by 4 spaces.
::
	if <condition>:
		do some code
		do some more code
	back to normal code

The computer knows when the ``if`` statement paragraph ends because the indentation stops.
That's the only way it will know!

If-Elif-Else
************

More complex types of ``if`` Statements: ``if-else``, and ``if-elif-else`` structures.

It helps to think of the three of them like this:

- An ``if`` statement gives the computer one option: if ``<condition>`` is True, then do something. That's all.
- An ``if-else`` statement gives the computer two options: if ``<condition>`` is True, then do something. If ``<condition>`` is False, do some other thing!
- An ``if-elif-else`` statement gives the computer several options, where you can say "Check all of these conditions until you find one that's True."

Each kind of statement is indented in the same way - with 4 spaces. Here's an example of each:

If Statement:
::
	if x == 5:
		print("x is 5!")

If-Else Statement:
::
	if x == "Penny":
		print("Your name is Penny!")
	else:
		print("Looks like your name isn't Penny!")

If-Elif-Else Statement:
::
	if age == 50:
		print("You're really old!")
	elif age == 20:
		print("You're kind of young!")
	elif age == 10:
		print("You're a kid!")
	else:
		print("I wonder how old you are?")

You can put in however many  "elif" portions you want. The computer will just go through each of the conditions, one after another, until it finds one that's True.
Then, it will skip the rest of the paragraph. And if none of the conditions are True, it will do whatever is written under the "else" section.


Lecture Slides
--------------

.. raw:: html

    <iframe src="https://docs.google.com/presentation/d/1tjpvWrhVX4e_gsURvMK6TqGiaevVJyKow5zxLD6YyA0/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

