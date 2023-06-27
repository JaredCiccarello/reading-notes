June 22, 2023

Problem domain: Take a tuple and then square

def transformation(2ple)
  new_list = list(2ple)
  squared_list = [x ** 2 for x in new_list]
    return squared_list


whiteboard

Make sure to give a personal pitch
Ask for simple examples
Make sure to do visualization



    > Given a 2 linked lists, write a function that returns the sum of the number represented by the 2 linked lists.

    Sample Data
    1 -> 2 -> 5 -> None:  This would be 125
    3 -> 7 -> 5 -> None:  This would be 375

    Would return the sime of 125 and 375
    return 500

    Possible solution:
    def sum_ll(ll1, ll2)
        current1 = ll1.head
        curret2 = ll2.head
        value1 = ''
        value2 = ''
        while current1 or current2:
            if current1:
                value1 += str(current1.value)
                current1 = current1.next
            if current2:
            value2 += str(current2.value)
            current2 = current2.next
        return int(value1) + int(value2)




If you create function

def main {}
  name = input("Please Enter your name: ")
  while True:
  input (f'{name})
    if input == "q"
      break

This code will not work because input is not being identified anywhere.

Once you exit the terminal using "ctrl c" you get an ugly error message saying "Keyboard interrupted"

We fix this error by:
def quit_game(message):
  exit(message)

__name__ == '__main__':
  try: 
    main()
  except KeyboardInterrupt:
    quit_game('keyboard interrupt detected')

make sure to import sys
from sys import exit
from system library
we import the exit method



Imports are important because, it looks at imports from the root of your project. When you import as a module.
When you import as a script, it imports from where the file is. So if you, when you write it as a script, where is your game?






advanced sim

validate keeper

MAIN FOCUS: Setting aside scoring dice


python -m ten_thousand.game
This will run your game as a module
BUT executes it as a script

IF you run as a script, your imports will not work

we run it under a dunder main


