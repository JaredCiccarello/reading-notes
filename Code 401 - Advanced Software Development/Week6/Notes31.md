July 24, 2023

MOTIVATION MOTIVATION MOTIVATION
Whiteboards is a process. Doing it with a professional is not helpful.
The 2/100 that do the whiteboard exactly as prescribed do well in the industry.
Whiteboards are NOT about coding.
Whiteboards are about the PROCESS.

Talk through the visual, in detail!


Instructors talk regularly about the industry. Instructors KNOW what is happening and is expected in the industry. If you can't trust the process than you won't be open to growth.

If it's not working for you, then develop a growth mindset. Again, trust the process. Sounds harsh, that's the game.


FANG companies are downsizing but, are still hiring.

What happened to the tech industry? Exponential growth.

Go look for how many jobs are available.
85% of jobs are filled through networking.

You can send out 200 resumes and still not get a response.

Anthony's brother has been in the industry for the last 5 years and is impressed with what we are doing.

Job: wants junior level to have 3 years.
THIS IS NOT JUNIOR LEVEL. That is mid or even senior.

Do not sacrifice your integrity for a job.


Want experience? Find someone that will let you build their website for free. That becomes industry experience.


There are students who NEVER touched coding after graduation. He went through nights course and did 301 twice.
There is a students who have spent 9 months looking.
There are TA's not getting jobs only because they aren't following the process.
  AFTER graduation: You can still reach out and get more suggestions down the road to get into the industry.

You get more than a CAP program. You get Roger.

Reminder: When Roger got his first job he got a mentor that would look at his code and say "Look at the documents and find similar code."
The point? Make sure you are finding ways to be autonmous.

Suggestion: Get good reps in.
Answer: You don't get as much learning from getting the answer right all the time. You learn from the struggle.

    The TRUTH?

Suggestion: Weekly feedback to help students with their thought process of problem solving.
  Response: You've already been taught the process. The solution is the whiteboard. 
  You only do whiteboards for CC rather than also doing that as a lab.
  The bad way is to start coding before you know where you're going to go.
  If you're still making bad habits. That's on you.
  You CAN sit down and go through a 1 on 1 with Roger to get help if you really need it.

Reminder: Roger claims he was a below average student.

Practice practice practice!
Go back to an old repo and redo it.


AGAIN! If you want 1 on 1 time for 15 min. YOU CAN SCHEDULE that time.
_____________________________________________________________________________

DJANGO!

Setup the basics of your website.




In models.py
add 
owner = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)
name = models.CharField(max_length=64)
created_at = models.DateTimeField(auto_now_add=True)
updated_at = models.DateTimeField(auto_now=True)

def __str__(self):
  return self.name

REMINDER: Anytime you change your models.py TYPE python3 manage.py makemigrations
THEN python3 manage.py migrate


a class method is an abstract from any individual instance.

ElephantSQL

When testing it would be a great idea to create another test for your app.

pip install djangorestframework
when adding this in INSTALLED_APPS: rest_framework


instead of doing a template, we are doing a serializer today.

We want JSON to display our data instead of using HTML.

GET CRUD WORKING
THEN
GET Docker working

