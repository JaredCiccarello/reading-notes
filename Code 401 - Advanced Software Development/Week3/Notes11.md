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
ChatGPT's:
Let's go through the code line by line:
import random: This line imports the built-in random module from Python. It allows us to generate random numbers and make random choices.
suits = ('Hearts', 'Diamonds', 'Spades', 'Clubs'): This line creates a tuple named suits that contains four elements representing the different suits of playing cards.
card_names = ('Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine', 'Ten', 'Jack', 'Queen', 'King', 'Ace'): This line creates a tuple named card_names that contains thirteen elements representing the names of the cards in a deck.
values = {'Two': 2, 'Three': 3, 'Four': 4, 'Five': 5, 'Six': 6, 'Seven': 7, 'Eight': 8, 'Nine': 9, 'Ten': 10, 'Jack': 10, 'Queen': 10, 'King': 10, 'Ace': 11}: This line creates a dictionary named values that maps each card name to its corresponding value in the game. For example, 'Two' maps to 2, 'Three' maps to 3, and so on.
class Card:: This line starts the definition of a class named Card. A class is a blueprint for creating objects with certain properties (attributes) and behaviors (methods).
def __init__(self, suit, value):: This line defines the initialization method (__init__) for the Card class. It takes three parameters: self (a reference to the current instance of the class), suit, and value.
self.suit = suit: This line assigns the value of the suit parameter to the suit attribute of the Card object.
self.value = value: This line assigns the value of the value parameter to the value attribute of the Card object.
def __str__(self):: This line defines the string representation method (__str__) for the Card class. It specifies what should be returned when we convert a Card object to a string.
return f'{self.value} of {self.suit}': This line returns a formatted string representation of the Card object. It combines the value and suit attributes to create a string like 'Two of Hearts'.
class Deck:: This line starts the definition of a class named Deck.
def __init__(self):: This line defines the initialization method (__init__) for the Deck class. It takes one parameter: self.
self.deck = []: This line creates an empty list named deck as an attribute of the Deck object.
self.dealt = []: This line creates an empty list named dealt as an attribute of the Deck object.
for suit in suits:: This line starts a loop that iterates over each suit in the suits tuple.
for card in card_names:: This line starts a nested loop that iterates over each card name in the card_names tuple.
self.deck.append(Card(suit, card)): This line creates a Card object with the current suit and card values and appends it to the deck list.
def __str__(self):: This line defines the string representation method (__str__) for the Deck class.
return f'{[value for value in self.deck if print(value)]}': This line returns a string representation of the Deck object. It uses a list comprehension to iterate over the deck list and prints each card's string representation. The printed values are included in the final string representation.
def deal(self):: This line defines a method named deal for the Deck class.
single_card = self.deck.pop(random.randrange(len(self.deck))): This line selects a random index within the range of the deck list's length using random.randrange(). It then removes and returns the card at that index using pop(). The selected card is assigned to the single_card variable.
self.dealt.append(single_card): This line adds the selected card (single_card) to the dealt list.
return single_card: This line returns the selected card to the caller.
Overall, this code defines two classes, Card and Deck, which represent individual cards and a deck of cards, respectively. The Card class has attributes for the suit and value of the card, along with methods for initialization and string representation. The Deck class has attributes for the deck and dealt cards, along with methods for initialization, string representation, and dealing a card from the deck.
Mine:
# explain this code line by line then put it into an AI and see how close you were
# importing the built in module random from Python
import random
# setting suits = to different suites as classes
suits = ('Hearts', 'Diamonds', 'Spades', 'Clubs')
# setting card_names to the face values of the cards as a string
card_names = ('Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine', 'Ten', 'Jack', 'Queen', 'King', 'Ace')
# creating a dictionary called values that is setting the card_names strings to integers
values = {'Two': 2, 'Three': 3, 'Four': 4, 'Five': 5, 'Six': 6, 'Seven': 7, 'Eight': 8, 'Nine': 9, 'Ten': 10,
          'Jack': 10, 'Queen': 10, 'King': 10, 'Ace': 11}
# creating a class card ('factory') that has a method that initializes(def __init__) with 3 arguements- self suit and value- setting self.suit to suit and self.value to value
class Card:
    def __init__(self, suit, value):
        self.suit = suit
        self.value = value
# setting a method of string to return template literal of value with the suits
    def __str__(self):
        return f'{self.value} of {self.suit}'
#new class of Deck
class Deck:
#creating a method inside of Deck that inits with arg of self- self.deck and self.dealt is = to an empty list
#for suit in suits is a for loop that.. for every card in card_names will append to the self.deck
    def __init__(self):
        self.deck = []
        self.dealt = []
        for suit in suits:
            for card in card_names:
                self.deck.append(Card(suit, card))
#creating a method for a string to return a template literal that will return the value in self.deck if called- the value is in a for loop that will print the value
    def __str__(self):
        return f'{[value for value in self.deck if print(value)]}'
#method that deals- a single_card is assigned the value of self.deck.pop and given the argument that it will be random and is a random range in the length of the deck, then it will append itself to single_card and return the value
    def deal(self):
        single_card = self.deck.pop(random.randrange(len(self.deck)))
        self.dealt.append(single_card)
        return single_card


DATA SCIENCE
Data Scientist: People often get a doctorate

Kim Damalas and Adam Owada LOVE data science. Kim did data science in the military.



NumPy
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