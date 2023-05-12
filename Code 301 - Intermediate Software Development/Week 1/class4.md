May 11, 2023

Parent/Child?

~9:09~ Challenge 3 Review

Question 1: 

Map is like forEach, having a callback function arr[i]

Callback function does: 

let num = [i]

Each time the loop runs I'm reassigning num to = arr at [i]

An array was created even though there was no return value.

return num; keeps returning num value

This is all what you will see with filter.


~9:20~ difference about filter

We are going through each item in the array and we are going to do stuff to the array.

reminder for loop for {i = 0; i < arr.length; i++>}

~9:23~ This does the same thing as this

Filtered array and a for loop filter

math that has a remainder %modula

% division after the remainder has taken place
It's purpose is to find the remainder after dividing the number by 2. If 1 is left over after dividing by 2.

    Example: 12 % 5 = 2

Once we have created a let we must always have a RETURN value.




~9:37~ LAB REVIEW: Displaying modal once clicked on

isModalDisplaying: true;
This would make the modal to display early before we can render content inside

We use modal to create a boolean value for if the modal is displaying or not.

Next we need a method for an eventhandler to change the value of isModelDisplaying: handleModalOpen

Next we need a method for an eventhandler to change the value of isModelDisplaying: handleModalCase

STATE is a method on app.js

Once invoke the Click event HandleModalOpen on hornedBeast.js, the method fires on app.js

Where else do we have to send this value from state? SelectedBeast.js will hold our modal in order to isolate single cards of beasts that are clicked on.

Next we need to find a way to close the modal.

handleCloseModal will do this for us. 

REMEMBER TO ADD PROPS to anything that is getting passed from PARENT to CHILD files

Next we need to make sure the modal has content being displayed inside of it.

this.props.handleModalOpen(beastInfo) this data 


~10:10~ 
This.setState will only work the component that it is in.

If setState is in app we call setState, that will change the state of the App only.

SelectedBeast Component ??????


~10:20~ 

addHearts
Can only be accessed inside main using this.props.handleShowModal

AGAIN props is essential for properties to be read outside of the parent.

What do parenthesis do with a function? invokes the function

(words) inside of a parenthesis is considered an argument

if I want to find beast inside this.props.beast, we can console.log our page and look into our objects.

~10:25~ Lab review End

??????

props means parent


~10:31~ Today's Code challenge 4

numArr = []

Using numArr will move the first integer

    ~1:37~ This is good practice to break the code down

const strArr sorts capital letters first


in order to get around this issue ~10:40~

ADVICE: be careful of the wording, the code challenges aren't as hard as they sound. Use the examples from class in order to give you hints, it should be what you need to solve these issues.

~10:43~ Review end





~10:45~ Today's Lab Review

Filter beasts by the number of horns that they have

    To make a new react project we will need to: npx create-react app FileName. This creates a brand new local repo

~10:50~
What 4 files should I remove?
— Remove unnecessary files
 App.test.js
 Logo.svg
 reportWebVitals.js
 setUpTest.js
— Remove code for reportWebVitals in index.js
— Change App.js to class based component) and remove use of logo

~10:55~

    Always remember when making class component
    1. Declare class component
    2. render and return
    3. Export


    class App extends React.Component
    render() {
        return (
            <h1>Forms in React<h1>

    export default App;

{} declaring an object like this will identify that specific object from another file.

We wouldn't import ALL of bootstrap in order to avoid causing a lag in processing speed. However if we had multiple lines of bootstrap imported, we may for simplicity sake just import all of the bootstrap code.

~11:05~ Bootstrap's version of UL

invoke map data.map()

then create a name for the ????

let data = [1, 2, 3, 4, 5, 6, 7, 8, 9]

{num} Why is num being put in this syntax?
When I'm writing in JSX (looks like HTML) "num" is a javascript variable. I want the value read as a javascript value.

writing just num will write only num instead of the values associated to num.

Comments look like {/* */} when writing in JSX

~11:12~ We got the numbers to display

Must import bootstrap CSS to avoid the data displaying plainly.

~11:28~ This will fix that particular error message
using key={idx}


~11:32~ Form and screen readers

What do we need to get a form? Label and input
In react we need a self closing tag <input/>

Check is this works with screen readers: Highlight the tag name in the browser and the form section should highlight. If not then the id and for are not working together.
How do we get the label and input to work together? Must have for and id with the same name.
However, using for in javascript will define for as a for loop
but, we are in JSX so we need to write htmlFor

~11:39~ labels

When dealing with forms what do we need to have at the beginning? event.preventDefault();
This will be used when you implement handleSubmit event.

Where do we look to find information that was added to our input? Target
event.target.nameFirst.value

how do we put something into state? setState updates state
We do this because ????

~11:55~ Data displays as an empty string?

That's because it takes time for setState to process. It can't immediately be put to use.

~12:02~ put a value in state

rawData: data,
fitleredData: data,

We want to change this to have odd or even numbers.

let newData = this.state.rawData.filter(num) => num % 2 === 0)
            It WORKS!

this.setState({filteredData: newData})

Why is it important that we run filter on the raw data? Because the filtered data would already be filtered, so we need the raw data to be the only thing that's filtered.


~12:17~ Bootstrap button

form.Label
form.Select

This part is trickier inputs become form.control
instead of form.Input

Form.Group
That will take two elements and make them siblings and make them work with screen readers.

controlID is how we access the values via our event handlers

FINAL NOTE: Always assume you need to submit your deployed link and your github link when doing submissions.