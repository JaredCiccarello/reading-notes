
Quiz6
Question10
In modern browsers, localStorage data is stored in:
    The file system 

Question9
Consider the following JavaScript code and pick the statement that best describes the code:


function Dog (name, age) {
  this.name = name;
  this.age = age;
}
var ageDiff = function(dog1, dog2) {
  return Math.abs(dog1.age - dog2.age);
}
ageDiff(new Dog("Sparky", 12), new Dog("Molly", 8));
    The JavaScript engine will create two Dog objects, then pass them as arguments to function ageDiff 

Question 8
Consider the following JavaScript objects:


var john = new Object();
john.name = "John Doe";
john.age = 30;

var henry = {
  name: "Henry",
  age: 24
};

Which of the following statements best describes the two objects above?
    Both john and henry are valid objects and can have additional properties added to them 

Question7
Which of the following statements would evaluate as truthy, given the below variable definitions?

var dog = {
 breed: "Beagle",
 weight: 30,
 group: "Hound"
}
var key = "weight";
    A. dog[key] === 30

B. dog["weight"] == "30";

C. "weight" in dog

D. dog.weight

F. dog.hasOwnProperty('weight');
    A B C D & F

Question 6
Which of following statements are true about absolute positioning?

A. Absolute positioning lets you determine an element’s location by specifying a left, right, top, or bottom position in pixels, ems, or percentages

B. Adding the following CSS properties to an element will always make it show up on top left corner of an HTML page

     {
        position: absolute; 
        top: 0px;
        left: 0px;
     }
C. When using absolute positioning, an element is taken out of normal flow and is positioned in relation to the closest parent that is relatively positioned
    Absolute positioning lets you determine an element’s location by specifying a left, right, top, or bottom position in pixels, ems, or percentages
    When using absolute positioning, an element is taken out of normal flow and is positioned in relation to the closest parent that is relatively positioned

D. There is no difference between "position:absolute" and "position:fixed" CSS properties


Question 5
Which of the following best describes fixed positioning?
    The box is held in the same location even if the page is scrolled

Question4
Which of the following statements about the CSS float property are true?

A. The CSS "float" property affects the layout of elements in a page

B. Content flows down the right side of a left-floated box

C. Adding a "float" CSS property allows an element to be positioned outside its containing element

D. "float" CSS property can have pixel values such as "10px" or string values such as "left", "right"

E. "clear" CSS property can prevent content from trying to flow around or alongside a floated element
    The CSS "float" property affects the layout of elements in a page
    Content flows down the right side of a left-floated box
     "clear" CSS property can prevent content from trying to flow around or alongside a floated element

Question3
Consider the following CSS rule:
h1 { 
  border-width: 5px;
  border: dashed blue;
}

After adding the CSS properties listed above, at 100% zoom, what will be the computed width of the border around an <h1>?

Consider rendering it in your browser and checking it with the inspector.
    3px 

Question2
Consider the following HTML code:


<!DOCTYPE HTML>
<html>
  <head>
    <title>Movie Review</title>
  </head>
  <body>
    <div>
      <h1>Brief Review: <cite>John Doe</cite></h1>
      <p>Detailed Review by Alison</p>
    </div>
    <div>
      <h2>The Best Movie <em>EVER</em></h2>
      <p>The movie <cite>New Movie</cite> was the best action movie ever produced!!</p>
    </div>
   </body>
</html>
    cite {color: red} 

Question1
Your classmate has an account on GitHub, with a username of "naman14". She has a repository called "Timber". In order to download the "Timber" Git repository on your local machine for the first time, you would issue which of following Git commands?
    git clone https://github.com/naman14/Timber.git 





Quiz 5

Question10
Which of the following is/are true about JavaScript object properties?
     Variables declared inside constructor functions are locally scoped and cannot be directly accessed as properties

Question9
Which of the following are standard CSS pseudo-classes?
    Target
    :last-child
    :hover

Question8
Consider the following JavaScript code:

function helloCodeFellows(){ 
 // do some logic and return a valid value 
}
var testAlpha = helloCodeFellows();
var testBeta = helloCodeFellows;
What is the difference between variables testAlpha and testBeta?
    Variable testAlpha holds the return value from function helloCodeFellows whereas variable testBeta holds reference for function helloCodeFellows.



Question7
Given the following code what style should be applied to make the images stack vertically?

<section class=”isenguard”>
  <img class=”lotr” src=”orcsWithAxes.gif” alt=”Chopping Down Trees”>
  <img class=”lotr” src=”treeBeard.png” alt=”Stomping on Orcs”>
  <img class=”lotr” src=”riverDam.jpg” alt=”Dam breaking”>
</section>
    .lotr{display:block;} 

Question6
What property is used to change the text color of an element?
    color

Question5
In the following code which line shows the conflicting code from your working branch?

1    <<<<<<<<<<< HEAD
2    <h1>Code Fellows</h1>
3    ===========
4    <p>Code Fellows</p>
5    >>>>>>>>>>> master
    Line 2

Question4
A function __________ loads only when the interpreter reaches that line of code.
    Expression

Question3
What is the error in the following JavaScript code, assuming that there is a button in the corresponding HTML with an ID of "pugbomb":

var pugbombButton = document.getElementById('pugbomb');
pugbombButton.addEventListener('click', pugbombButtonHandler());

function pugbombButtonHandler() {
  alert('PUGBOMB!!!!');
}
    The handler function is being called inside of the event listener

Question2
The elements we need to put inside of a form are: input, button and _____?
    Label

Question1
A function ____________ loads before any code is executed.
    Decalaration





Quiz4

Question10
Invoke the wizardsOfMiddleEarth function.

function wizardsOfMiddleEarth() {
  this.gray = "Gandalf";
  this.white = "Saurumon";
  this.brown = "Radaghast"; 
  this.blue = ["Alatar", "Pallando"];
  return this.gray + this.white + this.brown + this.blue[0] + this.blue[1];
}
    wizardsOfMiddleEarth()

Question9
True/false: Javascript cannot be used to manipulate HTML elements; it is only used in web applications to solve arithmetic calculations.
    False

Question8
What does DOM stand for?
    Documen Object Model

Question7
True/false: Figuring out your problem domain should only be done after you start writing code; otherwise you do not know whether the code actually works.
    False

Question6
True/false: An object is a collection of properties and methods.
    True

Question5
What is the term we use for a function that is associated with (or, attached to) an object?
    A method

Question4
In the line of code

var turtle = newAnimal("Michelangelo",1);
"Michelangelo" and 1 are:
    Arguments 

Question3
var rabbit = {}; 
This line of code creates an object by using:
    Object literal notation 

Question2
When used inside of an object, this refers to:
    The object that it is used in 

Question1
What does Math.floor() do?
    Returns the largest integer less than or equal to a given number






Quiz3

Question10
What does the CSS property 'float' do?
    Allows you to take an element in normal flow and place it as for to the left or the right of the containing element as possible

Question9
What will be the result of the following JavaScript code?
let breakfast = ['banana',
                'chicken wing',
                'coffee',
                'eye of newt',
                'pancakes',
                'avocado',
                'fish biscuit',
                'pecan',
                'corn dog'];
let indexOne = 3;
let indexTwo = 4;
let indexThree = 6;
for (let i = indexOne; i < indexThree; i++) {
  console.log(breakfast[i]);
}
    The following items will log into the console: eye of newt, pancakes, avocado

Question8
What will be the result of the following JavaScript code:

let meows = true;
while (meows = true) {
  console.log('MEOW!');
  meow = false;
}
console.log('Sorry, no meowing allowed.');
    The code will cause an infinite loop and the console will log many many meows.

Question7
What type of CSS positioning takes an element out of normal flow and positions it in relation to its containing element?
    Absolute positioning 

Question6
In JavaScript, what is the difference between the "==" and "===" operators?
    "===" means strict equality: the two values being compared must be of the same data type and value to return true.

Question5
Check out the JavaScript code below:
let units = "years";
let davidAge = 65;
let johnAge = 40;
let ageDifference = davidAge - johnAge;
alert("The age difference is " + ageDifference + " " + units);
Why should we make a separate variable for the age difference?
    The code is more readable with an appropriately named variable, rather than including an arithmetic expression inside of parentheses inside of a concatenation.

Question4
    What type of CSS positioning is used to keep an element "stuck" to a permanent location in the browser window, even when scrolling?
    Fixed positioning 

Question3
In our guessing game we used a conditional (if/else statement) to check for what?
    If the guessed answer was equivalent to the stored answer.

Question2
What is the purpose of z-index in CSS positioning?
    In a layout with overlapping elements, determines which element sits on top 

Question 1
In JavaScript, the "=" operator is used for what purpose?
    To assign a value to a variable 







Quiz2

Question7
Assume you are on the main branch of a repository and need to make some edits to 'app.js' on a branch called hotfix. To create and switch to the branch you would enter 
 , then, after editing, you would enter 
 to stage the changes, followed by 
 to make a commit with message of "hotfix of app.js". Lastly, you would enter 
 to upload the branch to GitHub.
- git checkout -b hotfix
- git add app.js
- git commit -m "hotfix of app.js"
- git push origin hotfix

Question6
var movies = ["The Matrix", "Frozen"];
typeof(typeof(movies));
The code will produce valid results because both objects are invoked.
    The code will produce valid results as both typeof calls are invoked with valid JavaScript types.

Question5
Which of the following correctly lists the outside-in ordering of the components of the CSS “box model”?
    Margin, Border, Padding, Content.

Question4
Which of the following are true about HTML elements with inline display?
    1. The content of inline elements determines their default width.
    3. All HTML elements with inline display can be changed to block display.
    4. Inline elements flow within the text and do not start on a new line.

Question3
Please pick the statement that best describes the default display for the HTML elements listed below:

<span> This is an inline element
<div>
<h1>, <h2>, <h3>, <h3>, <h5>, <h6>
<ul>

    All listed elements, except <span>, are block elements by default

Question2
Assuming there are no other CSS declarations, and no inline CSS styles, what will the following CSS declaration do to the body element and other HTML elements inside the body tag?
body { 
color: white;
background-color: black; 
}
    Change background color of all HTML elements within body to black and change color of all text to white

Question1
HTML attributes and CSS declarations are examples of key-value pairs.
    True







Quiz1
Which is a correct example of concatenation in JavaScript?
    A: 'I brush my ' + bodyPart + ' in the morning'

What tag do you need to run JavaScript code in an html file?
    A: <script></script>

Which is not a data type?
    A: Which is not a data type?

What command would we use to create and switch to a new branch called debug in Git?
    A: git checkout -b debug

Which defines the structure of a webpage?
    A: <HTML>

When writing clean code, which should you avoid?
        A: Non-semantic variable names

What Unix command would create a new directory called thursday?
        A: mkdir thursday?

Which of these combinations evaluates to true?
        A: true && true
            true || true
            false || true
            true || false

Analyze this block of code. Will it run? If not, where is the error?
1: var gopher = 1;
2: if (gopher < 10) 
3:    console.log(gopher);
4: } else {
5:   console.log('potato');
6: }
        A: No - Line 2

Which is not an example of a JavaScript statement?
    A: 1 =! loneliestNumber