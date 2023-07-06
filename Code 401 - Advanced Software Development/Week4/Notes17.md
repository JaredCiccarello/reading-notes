July 5, 2023: MOTIVATION MOTIVATION MOTIVATION

cryptography
Web scraping

Whiteboard process slowly getting together.
Code maturity: You may NEVER get to FULL maturity but, over time you will get better and better.

YOU will not remember every little thing, make sure you look things up and go over the material.

It's okay to go back and reference things.
Your cup is FULL, what you're taking away is a background knowledge NOT a 

How long are the videos up? up to 6 months

If you go back to your first weeks whiteboard, you will remember more than you think. However, with the caveate that you will NEED to practice.
___________________________________________
Serverless functions

Spelling issues
Setup mistakes

JB tellez likes giving out lots of code, Roger Huba likes making you work for your code.

Friday: Project prep all day
Midterm project: You can and is encouraged to use chatGPT API.

midterm project is 25% of your overall grade.
Guy gets kicked out of 401 for intentionally trying to sabotage team and throwing a tantrum for not liking a project idea.

What are your menus?
What is your data flow like?
What is your database?

These are the questions you should ask before starting your project.

Code Challenge 18 Today only

Serverless: 
When creating a function that only spits out "hello world" that is a serverless function. It's not apart of any other application.

"A single function that lives on the internet and does not use any other application."

Serverless is a different type of service offered on the internet.
____________________________________________
Lab 18: Ceaser Cypher

Decrypt method.

Crack function. Without access to key.


3 functions:
Encrypt
Decrypt
Crack


  ENCRYPT
Base 10 system of 0-9
Input: 101, 11
outpute 212, 212

Lab is based on shfit of 26. ABC's

def encrypt():

function must take in something.
def encrypt(plain_text, shift):

Need a dictionary or list with stored plain text?
Maybe a string instead?
Look through and move by the shift.

for char in plain_text:
    print(char)

python3 cipher.py

We need to increase char by the number of the shift.
char += shift ??? This will not work. char needs to be changed before shifting.

num = int(char)
this converts our string of characters into integers and assign it a variable.

encrypted_str = ''
This will take our variable and ???

encrypted_str = ''
for char in plain_text:
  num = int(char)
  new_num = num + potato
  encrypted_string += str(new_num)
return encrypted_string

What are we missing? num + shift
Will simply give all the integers as a return. We want this to go through all the integers of 0-9 and return a number each time.

shifting by 1 or shifting by 11
Difference is 10!
This matters because this is a base 10 cypher

We will need a while loop

while potato > 10
  shifted_key = potato % 10

Modular %: Returns the remainder

Modular essentially serves the same function as: 
while potato < 10:
  potato = potato /10

So we don't need to write it out.

However we still don't have the modular giving us the right output


this is the broken down version of the code

for char in plain_text:
  num = int(char)
  new_num = (num + potato) % 10
  encrypted_string += str(new_num)
return encrypted_string

we can break this down further by:

for char in plain_text:
  new_num = (int(char) + potato) % 10
  encrypted_string += str(new_num)
return encrypted_string


  DECRYPT
We simply take the encrypt function and:

def decrypt(encoded, shift):
  return encrypt(encoded, -shift)

That's it!
_______________________________________

NTL = Natural Language Toolkit

word_list
name_list

come from NTL

def find_word(sentence):
  for word in sentence.split():
    if word in word_list:
      print(f'{word} It is here')
    else:
      print(f'{word} Nope, not here')

sentence: 'The quick brown fox jumped over the lazily sleeping dog'

Here we take a function find_word and pass in a sentence.
if word is found in our word_list, then we print the word and say 'it is here' and vice versa.
____________________________________________
Code Challenge 17
Read: Tree's AGAIN
It will give you the breakdown of breadth-first search

____________________________________________

Project
Do your own adventure games
Buy stuff from command line
Remove duplicates



.git init creates a root repository