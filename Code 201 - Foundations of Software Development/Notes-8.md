function (a, b)
    let sum1 = a + b;
    let stringer = `The sum of ${a} and ${b} is ${sum1}.`
    return [sum1, stringer];

a and b are parameters located inside of our function.

Return command: Ends the function.

/sum(4, 7) are called arguments.

let is a variable.

console.log just prints the strings.

If I have a value that I want to get out of a function. I need to save it to a variable so that I can reuse it.

Template Literal: 

~9:28~
Working on Question 3 for lab 5

let total = a + b;
let finalTotal = total + c;

This is how you would work with three different variables.

let finalTotal = sum(total[0], c);

This allows us to use only the sum function instead of the sum and the string.

sum (a,b)[0]

This drills down and only uses the sum.

let prod0 = multiply(a, b)[0]
let prod1 = mulitply(multiply(a, b)[0], c)[0];


Note: Ensure you're writing code that you can understand a month later. Either that or write notes that will help you understand each step as you do your code.

~9:50~ Question 4
let testArray = [2, 3, 4]

~10:15~

Objects

Why objects, what can they give us that we can't do with other dataTypes?

DataTypes: Number, string, array.

const axelArray = [
'axel',
6,
'yellow tabby',
true,
true
]

This doesn't tell us what this is referring to. So we will need a key to give us context.

In the real world, array is not robust enough. 

console.log(`my cat ${axelArray[0] is ${axelArray[1]} years old.`})
This does not give us enough context.

Objects help with this.


OBJECT
let axelObject = {
    // key: value,
    name: 'Axel',
    age: 6,
    breed: 'yellow tabby',
    spayedOrNeutered: true,
    vaccinated: true
}
console.log(axelObject)

This doesn't show 'name'

console.log(axelObject.name);
console.log(axelObject[`name`])

These both do the same thing by showing the object: name.

You can do the same thing for all the other objects.

~10:28~
a . will read elements seperately

~10:32~ This is a method

{} are used for object functions

Properties and keys are basically the same thing.

console is an object. Everything under javascript is an object.

For today's lab we will be writing object literals.

declare another method
about: function(){
  return `My cat ${axelObject.name} is ${axelObject.age} years old.`;
}

This feels redundant to keep using axelObject when we know we are in an object.

~10:41~
So we would replace `axelObject` with `this`
about: function(){
  return `My cat ${this.name} is ${this.age} years old.`;
}



Objects can show up in sneak ways.

`typeof document` will be read as an object.

Document Object Model or DOM

~10:44~ Reminder of how to add in images to HTML images/"name".jpeg alt="This text is for the specific image."

~10:50~ grab id for document
document.getElementById('name of id')


~11:09~ Window into the DOM
If I want to create new elements add them

3 steps for creating webpage:
1. Create element(Most important one)
2. give content: Other elements
3. append it to the DOM (add it to the page)

In this case it would be starting with an article.

document.createElement('content name')

~11:16~
step 3: append. Append it to the DOM
Take the parent variable, then we call .appendChild()

When creating additional elements

You'll want to create all the same elements that the article uses.
let h3 = document.createElement('h3');

Note, headline tags have text content. So give it text content.
h3.textContent = 'Jumper';
console.log(h3);

~11:28 - 11:36~
Reexplaining parent and child elements of variable and strings.

Parent is the direct parent in the DOM of the thing we want to add.

// img
let img = document.createElement('img')

image has content but, it does not have text content.

~11:44~ Setting up an image

~11:50~ nth child/Lab 6 part 1 explained

~12:07~ Lab 6 explained

~12:11~ step 1

let seattleObj = {
    name: 'seattle',
    min: 23,
    max: 65,
    avg: 6.3,
}


step 2
let seattleObj = {
    name: 'seattle',
    min: 23,
    max: 65,
    avg: 6.3,
    genereateRandomNumberOfCustomers: function(){
        return Math.floor(Math.random()) * (this.max - this.min + 1) + 
    }
}

Test for Min and Max value.

~12:19~

let hours = []

Step 3
let seattleObj = {
    name: 'seattle',
    min: 23,
    max: 65,
    avg: 6.3,
    genereateRandomNumberOfCustomers: function(){
        return Math.floor(Math.random() * (this.max - this.min + 1) + this.min);
        cookiesSoldEachHourArray: [],
        dailyTotal: 0,
    },
    calculateCookiesPerHour
}

console.log(seattleObj.generateRandomNumberOfCustomers())







