Class 07 in repo has graphic table
Table graphic demo



<table>
    <thead>
    <tbody>
    <tfoot>
        <tr>



text content 
We give div text.

~9:29~
If we want td to be children of tr then we want

    Object literals have commas
    Constructor function have semicolons

objectLiteral = {
    name: riley,
}

Constructor Function = {
    name: riley;
}

prototypes are another type to do with constructor functions.

'seattle', 23, 65, 6.3
our numbers here are called arguments.

we invoke an argument with parameters

new command creates a new instance
    I.E. newStore

this.tableRender
^ is a called a method.

~9:48~
what code do I need to write individual functions for?



let numberArray = [
     0/0    0/1   0/2
    [1900, 1920, 1929],
     1/0    1/1    1/2
    [1894, 1921, 1965],
    [1925, 1946, 2014],
]

This is a nested array. Aka array inside of arrays.

First set of numbers is index 1

To only log 1920
console.log(numberArray[0][1]);
index 0 array 1

Logging all value of each array

for (let i = 0; i < numberArray.length; i++) {
    console.log(numberArray[i];)
}

This will log our numbers horizontally.

To log these numbers vertically you would need a second value.

 console.log(numberArray[i][i]);
 This still does not work

~10:17~
for (let i = 0; i < numberArray.length; i++) {
    for (let >> j << = 0; i < numberArray.length; j++) {
    console.log(`numberArray[${j}]${[i}]`);)
}
    console.log(`numberArray[${i}]${[i}]`);)
}


This will list the numbers from left to right all the way down.

We want the list to be from top to bottom then move to the next column.

We will need to map this out in order to see what's happening.

The internal for loop is considered the fast for loop.



Look at lab 6 stretch goals. They will be required to finish by the end of the week.

~10:34~
Utilize google fonts to find specific fonts.
Add in google links after your reset link.

~10:44~ Falls backs in CSS

~10:49~ inline block

~10:58~ Flex box

Place-hold.it
this command is for images

the last numbers in an place-hold.it/123-456/123 code are a number color code

Div's are for things that don't have a real meaning, such as decorative elements. Possible boarder shaping, or extra unlabeled items on a page for decorative featuring.

~11:40~

ul>li*4>a

This creates 4 li tags under ul parent.

click and select option to select the lines that you want to simultaneously change.

You may have a lot of warnings when you do a lighthouse review.

First thing you add to your CSS
* << universal selector

*{
    box-sizing: border-box;
}

margin: auto 
centers text
I think

~12:10~
Margin-top gives us space at the top of the page

~12:18~ Lorem Ipsum overflow auto
article section {
    overflow: auto
}

Finish up the header, style the button, and ACP!

~12:24~
Assets folder
shows all of the photos. We need 4 of them.



        HTML: Tables
<!DOCTYPE html>
<html>
  <head>
    <title>Adopt a Kitten</title>
    <link href="css/style.css" type="text/css" rel="stylesheet"/>
  </head>
  <body>
    <header>
      <h1>Adopt a Kitten</h1>
    </header>
    <main>
      <h2>Kittens Available for Adoption:</h2>
      <div id="kittenProfiles">
        <!-- generate this from js: -->
        <!-- <article>
          <h2></h2>
          <p></p>
          <ul>
            <li></li>
          </ul>
          <table>
            <tr>
              <th>
                Kids
              </th>
              <th>
                Dogs
              </th>
              <th>
                Other Cats
              </th>
            </tr>
            <tr>
              <td>
                true
              </td>
              <td>
                false
              </td>
              <td>
                true
              </td>
            </tr>
          </table>
          <img>
        </article> -->
      </div>
    </main>
    <footer>
    </footer>
    <script src="js/app.js"></script>
  </body>
</html>