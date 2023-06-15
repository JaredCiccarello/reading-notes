June 14, 2023

Exercise
Problem domain: Given a string a string, write a function that will return a new string with only one of each character in the new string.

  #Commissioner
  #Return: Comisoner

  A string is "iterable"
  iterable: Going over one item at a time
  strng is a reserved word in python
  lst is a reserved word in python

  This is a basic FOR LOOP in python
  def remove_char(string):
    for char in string:

  char is ???

  def remove_char(string):
    for char in string:
      print (char)

  remove_char("Commissioner")

  
  word = "commissioner"
    print(word[0])
    # remove_char(word)
  
  in terminal: python3 warmup.py
  we use warmup.py because of the filestructure. This is called "warmup"



    def remove_char(strng):
    new_string = ''
    for char in strng:
        if char not in new_string:
          new_string += char

  word = "commissioner"

  Here we want the string to be iterated over

  next we return new_string

      def remove_char(strng):
    new_string = ''
    for char in strng:
        if char not in new_string:
          new_string += char
      return new_string

  word = "commissioner"
  print (remove_char(word))
  print (remove_char('aggressiveness'))


  Again 
    for x in strng:
    is a FOR LOOP



  WHAT HAPPENS WHEN YOU GET STUCK IN A LAB?
Where do you go?

overAPI.com
This has a cheatsheet for python

w3schools.com

case
regex
files




  Lab 02 review

Length of the index divided by 2
Using insert method
// 2 force floor
Division operator that rounds down



TUPLE
Immutable: Cannot be changed

my_list = [1, 2, 3, 4]

for num in my_list:
  print(num)
my_list[0] = 100
for num in my_list:
  print(num)

my_tuple = (1, 2, 3, 4)
for num in my_tuple:
  print(num)
my_tuple[0] = 100

tuples do not allow you to reassign
If you wanted to edit the tuple, you would need to rewrite my_tuple with the new variables

my_tuple = (100, 2, 3, 4)

Is there a way to my a tuple mutable? Yes! Conversion!
similar to taking a string of age "10" and using INT to have the string be read.
int(age)

my_tuple = list(my_tuple)
print(my_tuple)
my_tuple[0] = 100
print(my_tuple)
my_tuple = tuple(my_tuple)

Sometimes you may need to make adjustments on the fly. You may need to fix bugs that have other bugs.

my_new_tuple = (1)
This will come up with a linter err on (1)

When you are dealing with a single item tuples, the linter does not recognize that the 1 is inside the parenths () without the comma.

my_new_tuple = (1,)
print(my_new_tuple)


word = "commissioner"

my_set = set(word)

terminal: python3 data.py

  SET METHOD
It WILL NOT return the same order because it iterates over all the entire word and returns individual characters of that word.

Game of Farkle: dice game. Possibly dealing with a pattern of numbers.

Dictionaries
These are VERY effecient.

Dictionaries are the SAME thing as Objects.
[]
.notations are a different way of accessing information




  Python syntax errors
print ("lets do something totally wrong")
print ("Too many parenthesis"))

If there are syntax errors the first line WILL NOT run.


print ("More wrongness. Do I get printed?")
print ("Who has ever"messed up" quotations marks?")

This can be fixed by
print ("Who has ever'messed up' quotations marks?")

Anytime you run into an error, stop and fix this error before moving forward.



  Logical Error
print("What happens now? Do you see me printed?")
value = 1/0
You won't get any linter errors.
If you run this code, the print will return the string even though value is an error. Why is this an error?

Here you can't divide by 0
When you run the code, it will tell you the error.


try:
  print("Divide by zero again", 1 / 0)
except ZeroDivisionError:
  print("Don't divide by zero silly.")

print("handled the exception above, carrying on")

This will find our error using except and then returning our except string.


try:
  print("Divide by zero again", 1 / "spam")
except ZeroDivisionError:
  print("Don't divide by zero silly.")

print("Total lie! The problem was not dividing by zero. It was a type error")

Running this code returns both strings of except/total-lie

We can handle multiple exceptions under except



try:
  spam = "nonsense" / 42
except ZeroDivisionError:
  print("Don't divide by zero silly.")

print("Total lie! The problem was not dividing by zero. It was a type error")


Except is a catchAll. We use ZeroDivisionError, which is built in python to use. 


https://docs.python.org/3/tutorial/errors.html
This site shows you the number of different errors that you may run into and how to deal with them using built in variables in python.



spam in here
but also some eggs

file = open('assests/spam.txt')
Terminal: Python3 fileio.py
This gives us an IO object in memory.

contents = file.read()
print(contents)
This will give us the information from the other file.

The problem. This file will be left open and actually leak memory.

print('Is the file closed: ', file.closed)
this returns a boolean, whether or not the file is closed. This is how we check. This will return false.


WITH
with open('assets/spam.txt') as file:
  print(file.read())

print ('Is the file closed: ', file.closed)
This will return a boolean of true.

file.read() shows the entire file contents

rb Read Binary

wb Write Binary

with open('assets/brain.jpg', 'rb') as file:
  contents = file.read()

with open('assets/brain.copy.jpg', 'wb') as file2:
  file2.write(contents)

This will copy the file of brain.jpg and make a new file brain.copy.jpg




Lab 03
Build out a game of MadLib

Play around with readline, in order to prevent running a test of an ENTIRE block of text.

pytest
comment out other tests
These are just STARTER tests, there should be other tests that you want to run.
You should be running MORE tests.

Inside the testing file, be sure to check the format.
You may need to import
You will always be creating a brand new virtual environment.
You have an option to bring in other libraries, not mandatory.





Code Challenge 03

Key feature: This is a sorted list. 

Do a binary search method. It splits the array in half. 

sequential search, searches from left to right.

There are additional stages of information.


STUDY TIPS

Putting 80-90 hours per week.


def BinarySearch(arr, target):
low = 0
high = len(arr)-1
#len(arr)-1 is how we get our last index, -1 helps us target the last index. If the array length is 10 then it would target is our 9th index.
#Defining two variables, high and low

while low <= high:
# While is set to make us iterate over our arr.
  mid = (low + high) // 2
# This cuts our arr in half. The //  divides and rounds down.
  if arr[mid] == key
    return mid
  elif: arr[mid] < key
# This cuts our arr and sets a new arr.
    low = mid + 1
# Whatever mid point, moving to the right of arr.
  else:
    high = mid -1
# Whatever high point, moving to the left of arr.

return -1