[Week 2 Exercises]

This week we had talked more about strings.  We also talked about input and converting types. 

To practice at home, we will first start with input.  We will look at how you can use it in different ways.


Input
-----

To get input from a user, you use the following syntax:

.. code-block:: python
   :linenos:
   
   name = input("Tell me your name: ")
   
Notice the following important things:

- :code:`input()` is the input function being used
- :code:`"Tell me your name: "` is a string literal and is only **shown** to the user. 
- :code:`name =` is the part of the code that **saves** the result of the input

Finish the following code.  You have to fill in the input commands for an adjective and a plant!

.. code-block:: python
    :linenos:
    
    animal = input("Choose an animal: ")
    color = input("Choose a color: ")
    adjective = 
    plant = 
    
    print("One day, a {} {} was eating a {} {}!".format(color, animal, adjective, plant))
    
    
    
Username Generator
^^^^^^^^^^^^^^^^^^

One thing we can do with input is use the strings to make new strings. 

In the following code, ask the user for their first and last name.  I have finished the first name part. 
Then, print out 6 types different types (patterns) of usernames they could have!  I have 
provided you with 2 different types.  Try do also do: 

1. first name then last initial
2. last name then first initial
3. first four letters of last name then first two letters of first name
4. first name then a period then the last name

.. code-block:: python
    :linenos:
    
    first_name = input("What is your first name? ")
    last_name = 
    
    username1 = first_name[0] + last_name
    username2 = first_name[0] + last_name[:5]
    username3 = ""
    username4 = ""
    username5 = ""
    username6 = ""
    
    print("Some possible usernames for you: ")
    print("\t 1. {}".format(username1))
    print("\t 2. {}".format(username2))
    print("\t 3. {}".format(username3))
    print("\t 4. {}".format(username4))
    print("\t 5. {}".format(username5))
    print("\t 6. {}".format(username6))
    
    
    
Converting types
----------------

Once you have input, it's really useful to use it as a number.  
But, the variable type that :code:`input` returns is a string type!

To convert it, we can do the following things:


.. code-block:: python
    :linenos:
    
    x = "3.5"
    
    x_float_version = float(x)
    
    y = "3"
    
    y_float_version = float(y)
    y_int_version = int(y)
    

To convert an input, you do the same thing, but this time the variable you 
are converting is just a variable made with the input function!

.. code-block:: python
    :linenos:
    
    some_number = input("What is a cool number? ")
    
    float_version = float(some_number)
    
    print("That number is {}".format(float_version))
    
    squared_version = float_version ** 2
    
    print("The square of {} is {}".format(float_version, squared_version))
    
    cubed_version = float_version ** 3

    print("The cube of {} is {}".format(float_version, cubed_version))

    squareroot_version = float_version ** 0.5
    
    print("The squareroot of {} is {}".format(float_version, squareroot_version))
    
    
Time since birth
^^^^^^^^^^^^^^^^

Using input, we can ask for all kinds of information.  
For this problem, ask the user for their birth year.  Then, print out 
the total years it has been since htey were born.  
Also print out how many months it has been, how many days it has been, and how many hours it has been.
It's ok to be approximate. You don't need to compute leap years or anything. Though,
technically it's just that every 4 years you add 1 day.  Floor division could work for that. 

.. code-block:: python
    :linenos:
    
    print("Welcome to your life calculator! This will compute how long you've been living.")
    
    # fill in this part
    # you have to use input and then convert the year to a float or int
    year_of_birth = 
    
    # years since born
    number_years = 2016 - year_of_birth
    print("It has been roughly {} years since you were born!".format(number_years))
    
    # months
    number_months
    print("It has been roughly {} months since you were born!".format(number_months))
    
    # days
    number_days
    print("It has been roughly {} days since you were born!".format(number_days))
    
    ## now you completely do these three
    
    # hours
    
    # minutes
    
    # seconds
    
    
Weight on Planets
^^^^^^^^^^^^^^^

If we know how much less gravity a planet has, then we can actually calculate our weight on that planet.

For example: Pluto has 5% of our gravity, which leads to this equation: weight_on_pluto = 0.05 * weight_on_earth
I have shown this in the code below. 

You should write the code for the other planets!  Instead of 0.05, you would use the following numbers:

- Mercury: 38% of our gravity, so 0.38
- Venus: 90% of our gravity, so 0.9
- The Moon: 16% of our gravity, so 0.16
- Mars: has 38% of our gravity, so 0.38
- Jupiter: has 236% of our gravity, so 2.36
- Saturn: has 108% of our gravity, so 1.08
- Uranus: has 80% of our gravity, so 0.8
- Nepture: has 112% of our gravity, so 1.12
- Pluto: has 5% of our gravity, so 0.05

.. code-block:: python
    :linenos:
    
    weight_on_earth = input("What is your weight on earth? ")
    # convert the weight to a float!!
    weight_on_earth = 
    
    weight_on_pluto = 0.05 * weight_on_earth
    print("You weight {} on Pluto!".format(weight_on_pluto))
