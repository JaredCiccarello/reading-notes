Ashley is a mom, goes to algebra class, and does CodeFellows full time.

flex box cheat sheet in repo

    CSS; Event Bubbling

If you forget where something is on a webpage
margin
border
padding

hover over this in the console

Flex box rules will sit on the parent element.

To find proof of life in CSS use:
border under main > section
main > section {
    border: 10px solid purple;
}

Main img will direct 

First thing to do when setting up a new CSS file: Find proof of life like a body tag.

EVENTS

click events will show a DOM event

an event is FIRED or RAISED
code is triggered

Event types:
click
submit

there are others defined by JavaScript

onChange
hover
on page load
on mouse over
on key release

event listener - code that is triggered when an even is FIRED

bind - bind or tether an event listener to an event

event handler - this is the code that runs in response to the event

Step 1: We need a DOM elemnt

let myContainer = document.getElementById

this grabs an element from our index.html

~10:09~
step 2: addEventListener () takes in 2 arguments
1 - an event as a string
2 - the name of a function we want to run

myContainer.addEventListener('click', handleClick);

must use from an events list that javascript knows. can't be random. Must be 'click'

addEventListener before you set the function

step 3 ~10:17~


~10:23~ This is telling us where the event occured.

let clickedElementId = event.target.id;
I want to get the id of the element I cliked on.

Next we next to make a window into the DOM
let results = document.getElementById('results')

create element
let pTag = document.createElementById
ptag.textContent = '${clickedElementId} was clicked';

results.appendChild(pTag)

    After ALL OF THIS we only need ONE eventListener

This process is called event bubbling





        FORMS

What elements will we need?
<input type="text" placeholder="kitten's name"


add an id

<input type="text" name="kittenName id = "nameOfKitten" placeholder="kitten's name">




~11:08~

We need a button
<button type="submit">Add a kitten</button>

Reminder: always check for proof of life

Two event types you'll be using are click and submit.

form.addEventListener('submit', )

when an event happens it passed through the call back function when it gets invoked. What passes through here? Event object that gets created.

~11:20~ 
Drill down to get the value that the username put into the form.
console.log(event.target.kittenName)
This is case sensitive.

~11:28~ Labels

Make sure to put comments

~11:50~ 

