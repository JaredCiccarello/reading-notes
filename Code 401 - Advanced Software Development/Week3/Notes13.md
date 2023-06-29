June 28, 2023
Roger's Roomba found fecal matter
_______________________________________________________
WarmUp1
Given a list, give a function that reverses the list
No internal methods.
Data inside the list does not matter

lst = [1, 2, 3, 4]

def reversed_lst(lst):
  reversed_lst = []
  for i in range(len(lst) - 1, -1, -1):
    reversed_lst.append(lst[i])
  return reversed_lst

my_list = [1, 2, 3, 4, 5]
reversed_list = reverse_list(my_list)
print(reversed_list)

SOLUTION
def reverse_list(lst):
    start = 0
    end = len(lst) - 1
    while start < end:
        # Swap elements at start and end positions
        lst[start], lst[end] = lst[end], lst[start]
        # Move the start and end positions towards the middle
        start += 1
        end -= 1
    return lst

Roger likes this method better
_______________________________________________________
WarmUp2

Reversing linkedlist
note: No need to write a Node/LinkedList Class!

REFER: Week1/Notes5

Current should be the NDDE 
Node only knows it's head

SOLUTION
def reverse_list(lst):
  prev = None
  currrent = lst.head
  while current is not None:
    next_node = current.next
    current.next = prev
    prev = current
    current = next_node

Method is part of a class.
Object.method this is how you invoke a method

This is the information that the method is receiving.
object.
____________________________________________________
Lab 12 review

Only needed 1 queue!

Cat and dog are just objects.
Creating two queue is too easy.


cat / dog / dog

these are Node's

dog2 / cat1 / dog1
are you a dog? Yes
move to end
dog1/ dog2 / cat1
Are you a dog? No
Are you the head? No
Take out of queue
dog1/ dog2
Are you a dog? Yes
Are you the head? No
Move to end
dog2 / dog1
Are you a dog? Yes
Are you the head? Yes
Fin~

________________________________________________
Code Challenge 13

This is not regex, this is a stack and queue

This explains why things would 
Only 3 brackets: (), {}, []

Hint: Look at a datastructure that is a string
Import stack and queue

_______________________________________________
Lab 13
Lots of ambiguity

We will select a kaggle data set. Something that we personally enjoy.

Notebook shows a way to validate your conclusions.
Tell us your story.

__________________________________________________
Salary notebook

salary = pd.read.csv(/kaggle/input/salaries/salary.csv)

test train split

X_train, X_test, y_train, y_test ??????????????????

X_train is looking for a reshape

y is dependent data
X is the independent data

This is typically how it's written, capital, non capital.

lm.score 
Shows how years of experience relates to salary.





Start thinking of midterm projects over the weekend.
Commented out code
Non executable code
naming conventions
live testing
These are all things that you will be graded on.

AFTER BOOTCAMP

Take a week off! Study for several hours, put some time aside for mass blasting resume, 