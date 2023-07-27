July 26, 2023

given 3 ll whose node val are single digits 0-9 give a function that will give sum of num rep by ll
can assume ll will have at least 1 node in it

def sum_ll_streamlines(ll1, ll2, ll3):

(Class github)


  BRUTE FORCE METHOD
def sum_ll(ll1, ll2, ll3):
  current1 = ll1.head
  current1 = ll2.head
  current1 = ll3.head
  num1 = '123'
  num1 = '234'
  num1 = '345'
  while current1:
    num1 += str(current1.value)
    current1 = current1.next
  while current1:
    num2 += str(current2.value)
    current2 = current2.next
  while current1:
    num3 += str(current3.value)
    current3 = current3.next

return int(num1) + int(num2) + int(num3)

_________________________________________________________

Docker compose down.



There's ways to stop all running container
Docker Container stop
  (Look in class repo for more details)



Authentication
What would you need to authenticate?

Changing a password
Buying beer with ID

Balance between effectiveness and efficiency.

Going to a bar and getting a stamp. If someone under 21 got a stamp for people only 21 and older, then it's not very efficient.


JSON web tokens is our way of doing things.
  The reading differs slightly but, has most of the same ideas.

Bearer token uses:
base 64 halo payload signature.

doc -d
gives us access to our docker data

http :8000/api/v1/things/ 'Authorization bearer: ssdfsdf'





pip3 install gunicorn

pip3 freeze > requirements.txt


PostgresSQL

Gunicorn
whitenoise

Do research for places you can do deployments.

DON'T FORGET THE LIBRARY 5 minute preview INTRODUCTION