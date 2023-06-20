June 15, 2023

You are right where you are supposed to be with struggling.

You can only submit until up to the beginning of the next week.

Keep working and the grades will come, don't worry about grades you've got 10 weeks.

Whiteboard is going to be different each time. Just keep practicing, 60% of people fail the first time.
Print out the whiteboard, this will help.




Code Challenge 04
Mock interview Whiteboard

Code is is only 8 points out of possible 45

DO NOT go straight into coding first.
The whiteboard is made to help you figure out what you're supposed to do.

TRY to do the whiteboard without resources.

You can try whiteboard your labs.

36 out of 45

SOME interviews will be easier but, it's important that you learn the industry standard.




Lab 03 Review

pytest website


~47min~ 
Warm up

.venv : You do this by .... standby

-------------------------------
test_warmup2.py file
****************
  import pytest

def test_add_values_one_two():
  actual = add_values(1, 2)
  expected = 3
  assert = actual expected

warmup2.py
**********
def add_values(num1, num2)
  pass
return num1 + num2

Doing this will result in a passed test!
----------------------------------------

Next we
def test_add_values_one_two_fail():
  actual = add_values(1, 2)
  expected = 6
  assert actual != expected

  This test, tests for false positive

    VENV SHORTCUT
# VENV Alias
alias vi="python3 -m venv .venv"
alias vs="source ./.venv/bin/activate && python -m pip install -U pip"
alias ve="deactivate"





~1hr 15~ CLASSES

Make sure you check your test. Is the file path at the top correct? 
From star_wars the folder .star_wars the file
no need to add the py

What is a class? It's an object constructor


????????????????????

Dry out code
Remember to write your code 

Method: Function that is inside of a class

Self is a way to identify

????????????????



Getting good with TDD (Test Driven Development)
Companies usually don't have a TDD team or have a small TDD team. TDD is tedious and hard to master.






Here is how you fix testing for modules

Execute the command for modules
python3 -m folder.name_of_file

Notice the . notation here

Regularly you would test using
python3 star_wars/star_wars




Jedi class
sithlord class

When testing for sithlord class, make sure you IMPORT the class into test

Grouping classes
import star_wars.star_wars

You wouldn't want to send over the entire group of classes, this is a security issue. If you only need 8 classes you wouldn't want to import all 30.
This also becomes a processing issue. If there are 200 classes, it will take longer to load and become ineffecient.




No dunder init
JediMaster
SithLord



MRO. This is an inheritance.
This is a way for python to "bubbleup"
This is an inheriting from a parent.


pytest.fixture autouse
resets everytime a test runs


Two ways to overwrite print
1. Dunder str def __str__(self):
  You use this to prevent the print from showing the object itself to the user
  
  return f"{self.name} is in the House!"
  This will default to the dunder str

2. Dunder repr def __repr__(self):
    return f"JediMaster('{self.name}')"
    What command do you need to 


Lightning talks






After class Review:

cd ~
code .
Then
    VENV SHORTCUT
# VENV Alias
alias vi="python3 -m venv .venv"
alias vs="source ./.venv/bin/activate && python -m pip install -U pip"
alias ve="deactivate"