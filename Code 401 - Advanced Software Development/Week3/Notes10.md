June 26, 2023

Tammy Do said you're the best class for not qutting and grouping up together.
Don't give up!
Quitting means the true end.
Keep going.
Everyone is on a different path!
Most people think they are not smart enough for this. Don't give up.

How much of this do you think you'll memorize when you constantly have new information being thrown at you? Keep studying, keep pushing. It's a lot of information but, you'll get there.



Looping

Roger is not familiar with Pylance because he does not use VSCode, he used PYCHARM.

He likes a try-except error better. 

??? THAT'S WHY TARGETERROR CAN BE IN THE CLASS OF PASS ???

When you run into a targeterror
here's how we WANT to handle this.

Running a try-except in a targeterror class, you're asking for it to run it again.

Example: If you had a LinkedList with no HEAD. Then you want to concatenate the value of HEAD. Your try-except block will raise an exception to continue to move on.

WHAT ARE YOU TRYING TO TEST? 



STACK AND QUEUE
Reminder: Class is factory that creates instances.
A class, with errors, is a brand new instance everytime.

LinkedList knows: Where the head is
queue knows: It's front and rear
stack knows: The top

Queue is it's own instance in memory

What are the properties that the queue has: What it is instantiated with. Typically front and rear. What is in the __init__.


Properties are: Actually values that are assigned to it.
Stack: Assigning a top
LinkedList: Assigning a head.
What does a Node know? Value and next

Front and rear.

__init__ builds it in memory

MEMORIZE
Queue
take from a queue dequeue and add to a queue enqueue. 

Stack
Take from a stack pop and add to a stack push.




Code Challenge 11
Implement a queue, using two stacks

A queue, gives us First in, first out. What goes in, goes in exactly the same order.

I want to make a stack of a lineup. When I put something in a stack, will the first thing be Logan? No.

Logan, Andrew, Anthony, Jared
Moving to a new stack
Jared, Anthony, Andrew, Logam

Jared                         Logan
Anthony                       Andrew
Andrew  Moving to new Stack   Anthony
Logan                         Jared


You may be traversing a binary tree with a stack or queue.

Utilizing data structure to do something with another data structure.




Black-Jack: Explain line by line

# We import random, which is a method that
import random
suits = ('Hearts', 'Diamonds', 'Spades', 'Clubs')
card_names = ('Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine', 'Ten', 'Jack', 'Queen', 'King', 'Ace')
values = {'Two': 2, 'Three': 3, 'Four': 4, 'Five': 5, 'Six': 6, 'Seven': 7, 'Eight': 8, 'Nine': 9, 'Ten': 10,
          'Jack': 10, 'Queen': 10, 'King': 10, 'Ace': 11}


class Card:
    def __init__(self, suit, value):
        self.suit = suit
        self.value = value

    def __str__(self):
        return f'{self.value} of {self.suit}'


class Deck:
    def __init__(self):
        self.deck = []
        self.dealt = []
        for suit in suits:
            for card in card_names:
                self.deck.append(Card(suit, card))

    def __str__(self):
        return f'{[value for value in self.deck if print(value)]}'

    def deal(self):
        single_card = self.deck.pop(random.randrange(len(self.deck)))
        self.dealt.append(single_card)
        return single_card


DATA SCIENCE
Data Scientist: People often get a doctorate

Kim Damalas and Adam Owada LOVE data science. Kim did data science in the military.



NumbPy
Python lists, mutable.

We can create an empty list. We don't need to know the length of the list.

NumbPyArr are built are strict type optimization. You neeed to know what data type.
These are NOT mutable. They make them alot more efficient to work with.

arrays = lists in python

Python 

Python is like taking a jack hammer to get the job done.

NumbPy was written in C. It is not user friendly to code in C.





Lab class 11
Creating a chess board.
Red square and blue square
Determine if the red queen is under attack by the blue queen

RGB format: Red/Green/Blue
Using this we can create any color that we want to.

KAGGLE
We are going to be coding in Kaggle today, which is a seperate notebook


V IMPORTANT: When you are done. Share, public. Make sure you save!

PYTHON VERSION
import sys
print (sys.version)
You'll get an error
You need to re-run the code

VARIABLE ASSIGNMENTS
message = "Python is Fun"

run file
Restart and clear all cell outputs





Import numbpy as np 
import pandas as pd

We can call these whatever

Each cell has some sort of heading
IT is a requirement

We are going to be creating a matrix
A matrix is just an array of arrays

grid = np.
we need a matrix because we want something that is long

Prepopulate an 8 by 8 grid with zero's.

Must re-run code when you make a change to it!



IPNBY
Interactive Python NoteBook