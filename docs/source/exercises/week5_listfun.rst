List Exercises
==============

Lists are an extremely powerful way of managing multiple variables at once!

Exercise 1: Basic List
----------------------

.. code-block:: python
    :linenos:
    
    students = list()
    students.append('John')
    students.append('Jenna')
    students.append('Rachael')
    students.append('Isabel')
    
    num_students = len(students)
    
    print("There are {} students!".format(num_students))
    print("The first student is {}".format(students[0]))

Modify the above code to finish printing out each student.


Exercise 2: Adding to the list
------------------------------

.. code-block:: python
    :linenos:

    fav_things = list()
    
    num_things = len(fav_things)
    print("I have {} favorite things!".format(num_things))
    
Modify the above code by adding in your favorite things!  You can change the variable name
and the print statement if you want to do movies, books, pets, etc instead of "things".


Exercise 3: Looping over a list
-------------------------------

.. code-block:: python
    :linenos:

    fav_things = list()
    
    num_things = len(fav_things)
    print("I have {} favorite things!".format(num_things))

    if num_things > 0:
        print(fav_things[0])
        
        for i in range(num_things):
            print(i)
            
Take a look at the above code.  Indexing into :code:`fav_things` allows me to print the first item. 
The :code:`for` loop allows me to loop over the exact integers that can index into :code:`fav_things`.

Modify the code so that :code:`fav_things` is being indexed inside the loop and printed out.

Exercise 3 part 2
-----------------

You can also use a for loop to loop over each of the things. 

.. code-block:: python
    :linenos:
    
    test = ['this', 'is', 'cool']
    for item in test:
        print(item)
        
Use this style of loop to print out your favorite things.


Exercise 4: Looping with While
------------------------------
        
A while loop will keep doing things until you tell it to stop!

.. code-block:: python
    :linenos:
    
    done = False
    
    while not done:
        print("Inside my loop!")
        print("Exit?")
        choice = input("[yes/no] > ")
        
        if choice == "yes":
            done = True
    

Make a while loop which let's you exit as the previous code.  
But inside the loop, ask for the user for their favorite things. 
Then, add these favorite things to a list!

This is basically the same code as before, you are just using :code:`append` to add new things. 
The only difference is now it is inside the :code:`while`.

After the :code:`while` loop finishes, use a :code:`for` loop to 
print the list!

Exercise 5: Higher or Lower
---------------------------

Play the guessing game using a while loop.

1. The computer selects a number
2. The user has to guess until they are right
3. The computer tells the user higher or lower
4. The computer counts how many guesses it took

To guess a random number, you can use the :code:`random` package

At the top of your code, put: 

.. code-block:: python
    :linenos:

    import random
    
Then, when you want to select the number, do:

.. code-block:: python
    :linenos:

    low = 0
    high = 100
    correct_number = random.randint(low, high)


Now, the game should look like the following (you have to write the rest of the code):

.. code-block:: python
    :linenos:
    
    low = 0
    high = 100
    correct_number = random.randint(low, high)
    
    guess = -1
    
    while guess != correct_number:
        print("Fill out the code here!")
        
        
Important: Do not run the code above without editing it!  
You will enter into an infite loop. 
If you do end up doing this, either "Ctrl-C" or the red stop button will stop it. 


Bonus Exercise
--------------

Generate random sentences.  An example of how to generate adjective-nouns is below!

You can play with generating different "patterns" of sentences:

1. You are a ADJECTIVE NOUN. 
    - this is the example below
2. NOUN tried to VERB.
    - Euclid tried to sleep.
3. NOUN is ADJECTIVE. 
    - Cheese is stinky. 
    
How complex can you make it?

.. code-block:: python
    :linenos:

	import random
	adjectives = ["super", "silly", "evil", "furry"]
	nouns = ["rabbit", "tortiose", "gorilla"]
	keep_going = True
	while keep_going:
        pick1 = random.choice(adjectives)
        pick2 = random.choice(nouns)
        print("you are a {} {}".format(pick1, pick2))
        answer = input("Keep going? (yes/no) ")
        keep_going = answer == "yes"
        # alternate version:
        # keep_going = (input("Keep going? (yes/no) ") == "yes")
        # alternate version:
        # if answer == "yes":
        #    keep_going = True
        # else:
        #    keep_going = False
        # why is the way I did it a good way to do it? 
	print("goodbye!")
