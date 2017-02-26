Week 7 Refresher, Part 2
========================


In the second part of this refresher, you will have 30 minutes to make a couple
of the functions below. Don't spend time being stuck.  You have two options
if you aren't sure how to make something work or if there is a weird bug
that you aren't sure how to fix:

1. Look at the cookbook, see if you can find an example that fits what you want to do.
2. Ask me for help



Exercise 1
----------

Reminder of syntax

.. code-block:: python
    :linenos:
    
    def function_name():
        print("inside the function")
    
    print("going to call the function")
    function_name()
    print("just called the function")
    
    
Write a function which prints out your name and your favorite food. 
Name this function :code:`intro`.

Then, write code which calls this function. 

Goal:

    - function name: :code:`intro`
    - arguments: None
    - code inside function: print name and favorite food.
    - returns: Nothing


Exercise 2
----------

Write a function named :code:`madlibs`.  This function should take as input
four variables: noun1, noun2, and adjective. Inside the function, it should
have one of the following versions of a print statement. I have given you 3 version
because they are different ways of printing the same thing. You can use any of the 3.
You can change any of the words, if you want. 


.. code-block:: python
    :linenos:
    
    # version 1 
    print("Did you know that ", noun1, " are actually ", adjective, noun2)
    
    # version 2
    print("Did you know that {} are actually {} {}".format(noun1, adjective, noun2))
    
    # version 3
    print("Did you know that "+noun1+" are actually "+adjective+" "+noun2)
    

Goal:

    - function name: :code:`madlibs`
    - arguments: :code:`noun1, noun2, adjective`
    - code inside function: print statement from below
    - returns: Nothing    

Exercise 3
----------

Write a function named :code:`make_superhero`. The function should 
take 2 arguments, :code:`select_power`, and :code:`select_name`.  

Inside the function, you will have the following code. The function
should return back the :code:`result` variable from below. 

.. code-block:: python
    :linenos:
    
    ### put this at the top of your file
    import random
    
    
    ### code for inside the function
    
    powers = ['time travel', 'super strength', 'super intelligence']
    adjectives = ['Incredible', 'Unstoppable', 'Unflappable', 'Amazing', 'Scrumtrilescent', 'Purple', 'Bioluminescent']
    nouns = ['Bat', 'Wolf', 'Wolverine', 'Donkey', 'Spider', 'Monkey', 'Fighting', 
            'Alien', 'Baby', 'Dino', 'Computer']
    
    result = dict()
    
    if select_power: ## select_power should be true or false
        power = random.choice(powers)
        result['power'] = power
    else:
        result['power'] = 'unknown'
    
    if select_name:
        adjective = random.choice(adjectives)
        noun = random.choice(nouns)
        name = "The {} {}".format(adjective, noun)
        result['name'] = name
    else:
        result['name'] = 'unknown'
        
Goal:

    - function name: :code:`make_superhero`
    - arguments: :code:`select_power, select_name`
    - code inside function: the selection process from the code above
    - returns: :code:`result`
    
Exercise 4
----------

Revise the code from Exercise 3 so the :code:`select power` and :code:`select_name`
have default arguments of :code:`True` and :code:`True`.



When you get this far
---------------------

Please let me know.

For this bonus, you will make the following code more advanced. 

First, read through the code. 

.. code-block:: python
    :linenos:
    
    import random
    
    def make_monster():
        simple_monster = {'name': 'bugs', 
                          'health': 5}
        return simple_monster
    
    def make_hero():
        simple_hero = {'name': 'Super Coder',
                       'health': 10}
        return simple_hero
        
    
    def battle(hero, monster):
        print("A round of battle with hero and monster!")
        hero_alive = hero['health'] > 0
        monster_alive = monster['health'] > 0
        
        while hero_alive and monster_alive:
            print("Hero attacks!")
            amount = random.randint(1,3)
            monster['health'] -= amount
            
            print("Monster attacks!")
            amount = random.randint(0,1)
            hero['health'] -= amount
            
            hero_alive = hero['health'] > 0
            monster_alive = monster['health'] > 0
            
        print("Either the hero or the monster is dead!")
        print("If only there was an if statement here to figure out who...")
        
    hero = make_hero()
    monster = make_monster()
    battle(hero, monster)


In this code, there are three functions: :code:`make_monster`, :code:`make_hero`,
and :code:`battle`.  

Try to do as many of the following things:

1. Add arguments to :code:`make_monster` and :code:`make_hero` so that you can 
custom set the :code:`name`.

2. Change the code in :code:`make_monster` and :code:`make_hero` so the health
is from the :code:`random.randint(low,high)` function.

3. Add another property inside the :code:`monster` and :code:`hero` dictionaries
called :code:`power`. Then, inside the :code:`battle`, the :code:`hero` gets
their amount as :code:`random.randint(1, hero['power'])`.  Same pattern with the
:code:`monster`.