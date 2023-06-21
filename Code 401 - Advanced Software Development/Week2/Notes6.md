June 20, 2023

    # File Name: random.py
    # Import the library random.
    import random

    # Create a list to get a random number from
    number_list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]

    # Declare a variable and assign it the return of a random value from number_list
    random_number = random.choice(number_list)

    # Print the random number
    print(random_number)

    # Is there anything wrong with this code? Yes, naming.

This code runs properly.
Choice is a method in python.
This is trying to import local first.

python random1.py

Circular import error. Look at the files you are importing.
This is looking at the file random.
Looks at local first, then bubbles up to 'built ins'.
Look up MRO. <-- Very deep information.


TRAVERSE: Memorizing is your friend

ll: [1] -> [2] -> None
current = self.head
output = ''
while current: 
    output += f'{{ {current.value} }}-> '
    current = current.next
  output += 'None' (This is the doc string)
MUST return output

TRAVERSE: No but, really


node = Node(value)

if the LinkList is not empty we need to insert the new Node.

LL: [3] -> [1] -> [2] -> None
LL: [1] -> [2] -> None

The rest of the LL stays in tact, in the first LL. We simply change [3] to [1] and keep the rest the same. So we do not need a traversal for this one.

~58 min~ This is what we were looking for on friday.


LinkedLists are the FOUNDATION for all of our other data structures. LinkedLists are your new best friend.



Code Challenge 06

append
insert
insert after

Whiteboard
write code
provided test passing

Code Challenges worked in teams





FARKLE

Don't worry about round 2

Version 1 TODAY
Version 2 Tomorrow
Version 3 Next day


pytest -k version_1
This runs things in your repo marked with version_1

return [random.randint(1, 6) for _ in range (num_dice)]
We want a tuple list from this code.

return Tuple[random.randint(1, 6) for _ in range (num_dice)]

@staticmethod
def function_name(num_dice)

staticmethod is necessary to prevent using (self, num_dice)


