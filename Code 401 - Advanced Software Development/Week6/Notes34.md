July 27, 2023

Whiteboard 

Problem Domain: Given a linked list of numbers, return a boolean of whether head to tail is ascending.

Could have: Floats, negatives, 

Floats are numbers that have decimals.

In: 1, 4, 6, 9
Out: 6, 5, 9, 9

LinkedList only knows its head.


Make sure to ask for a given test case.

Make sure you talk the whole time, think out loud!

Time: O(1)
This means instant look up


AGAIN! Read through the rubric! Ask all the questions necessary.

Ask for examples, input/outputs, 

Solution:
https://docs.google.com/spreadsheets/d/1X0CP30shv51zOGmyqjgHPmNnruOTUeMxYX8juWVXx7U/edit#gid=1813704304

def ascending:(LL)
  current=LL.head
  current2=current.next
  while current2 < current.next
    if current.val < current2
      current = current.next
      current2 = current.next
      if current2 is None:
        return True
    else: 
      return False

______________________________________________________________

Setup a new django account


This is all great and fine.


  DEPLOYMENTS: Vercel
When we do deployments
Most deployments will not let you use a database like SQLite

  (Mandatory)
https://www.elephantsql.com/
select free version

confirm new instance of database

docker compose run web python3 manage.py makemigrations
migrate

create superuser



When you run migrate, why is running so slowly? It's talking to elephantsql



You front end doesn't have to consume your API backend.



Video review:

One key takeaway: ElephanySQL
No credit card required.

  Creating new database
Create new instance
Keep naming simple
Default region
DOne



DCN = Nuke