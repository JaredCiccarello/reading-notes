July 21, 2023


Make sure to edit your own template and build it from the ground up. Using DjangoX may not help. Building a template from the ground up and then changing the repo to a template to be used later will help you to figure out not only how to make your own but, also what's going on in your code.

Update your djangoX project to use later on.
__________________________________
Hash Map

What is a hash table?

It's like a bucket, which will be our list.

0, 1, 2, 3, 4



Roger: 111 -
Logan: 222 -
Sarah: 333 -
Slava: 444 -

We are going to take the value of our key value pairs and return an index of 4


Roger: 111 - 4
Logan: 222 - 0
Sarah: 333 - 2
Slava: 444 - 4

We are going to take the value of our key value pairs and return an index of 4

You can do this with a list, a set, all types.

This moves values from our 4 position and then ???

When you set a password, it goes through a hash map

md5hashgenerator.com

  This uses an old method of hashing. It's no longer used because it can be easily hacked.

  When you create a password here, it starts with a bcdc
  hash passcode. This is storing your password using a key identifier. When looking for your password it compares these hash passcodes with what's stored. It's not actually looking at your password but, at the hashcode associated with it.

This is how companies get around a security risk.

There is something called SALTING. It adds random text to the end of your hash.

You use hashmaps in dictionaries.


It's important to note: You will not be using other custom variation of hashmap.


"""
"""

MUST add doc strings into ALL of your code. This is where you explain what is happening with your code. Do NOT forget to add doc strings.

"""
Parameters: Key, Value
Returns: Nothing
"""

Simple explanations are acceptable.


class Hashtable():
  def __init__(self):
    pass

  def hash(self):
    pass


if __name__ == '__main__':
  Hashtable()

  def hash(self, key):
    """
    hash
    Arguments: key
    Returns: Index in the collection for that key
    :return:
    """
    index = 0
    return index

What is one thing that's required? The size.

class Hashtable():
  def __init__(self, size=1024):
    self._size = size


Adding an underscore to size, means this is a fixed size.

The other thing we need to do is create our bucket.

  def __init__(self, size=1024):
    self._size = size
    self._buckets = size * [None]

So what is actually happening here? It's creating a list that has a size of 10, with None in each index.

sum = 0
for ch in key:  
  total += orc(ch)
primed = total * 19
index = primed % self.size
return index

This is going to return an index of the range of our hash table.

ord = returns the asky value of a given character. Converts each character into some number.

Take in a key of super and then goes through the word with each letter.
# super
# ^
# total = 0 + 115 + 117 + 112 + 101 = 559 * 19 = 10,621
Roger says this is 10,640
sum = 0
for ch in key:  
  total += orc(ch)
primed = total * 19
index = primed % self.size
return index

We pull these numbers from the ASCII table.
https://www.cs.cmu.edu/~pattis/15-1XX/common/handouts/ascii.html

10,621 is divided by 10

The remainder 

If we took the word jump (lowercase)
106 + 117 + 109 + 112 = 444
Roger says this is 446

The algorithm that we use to return the index.

Do NOT run this through chatGPT. This will return a very specific signature. Meaning it gives a very unique solution that can be seen right away.

Struggling? Read through the reading.
Still don't understand? Whiteboard it out.
Still having trouble?

Partner Power hour: Debugging VSCode.

Career coaching prep needed before workshop. Will potentially go for 3 hours.

___________________________

CAREER COURSE

Last time seeing Kristen.

Steps to find employment:
Job Search
Network
Resume

Technical Interview: Whiteboard
Personal Interviews
Job Offer
Negotiate!

GTM Strategy

Unlocking behavorial interview
Why do companies use this?
The best prediction of future behavior, is past behavior.
What is it?
A conversation about past experiences.
How do you unlock it?
Practice and be prepared. STAR method.
Situation
Task
Action Result

What are some common questions?
Strengths/Weaknesses
How you fit at the company.
(Throw in your personal pitch here)
You went above and beyond
You disagreedw ith a manager
You had a chance to take the lead
You had to work with someone difficult
You experienced a failure/mistake/challenge

Why are you here?
Motivation/plans/readon for making a move

When researching companies:
Upward mobility, What are they doing that interest you?
What charities do they support?

Keep in mind, your scenarios of how YOU handled a situation. Not simply what happened.




Interview Review

Don't start with a negative spin, toxic work environment.
Make sure when giving experiences, give a positive spin.
Give more information about WHY software engineering.
Work on what your personal weakness is. Don't bring in your technical expertise. 
Technical questions: Keep it simple bro. Or I have an idea of what I think this means.
