Class 7: Review



~9:04~

create new branches
lab 6: branch 'object literals'
lab 6 pt. 1: object constructors

THIS refers to the object itself.
let seattle
seattle would be THIS.

~9:51~ Memorize this formula






// We need a 'Constructor function'
// Object constructors

// this refers to the object that WILL be created
function Student(name, pronouns){
  this.studentName = name;
  this.pronouns = pronouns;
  this.codeClass = 201;
  this.onLine = true;
  this.introduce = function(){
    console.log(`Hello, my name is ${this.name}`)
  }

}
// create instances of Student
let juan = new Student ('Juan');
let sara = new Student ('Sara');

console.log(juan);
console.log(sara);

juan.introduce();

let studentArray = [Sara, Juan];

for let (i = 0; i < studentArray.length; i++){
  studentArray[i].introduce();
  // add all stores together
}









Remember to do this 
WHY?
3 steps for creating webpage:
1. Create element(Most important one)
2. give content: Other elements
3. append it to the DOM (add it to the page)

2. li.textcontent = 'test'

~10:20~

always make sure you get a proof of life. console.log

let oneStudent = {
    name: 'Steve',
    codeClass: 201,
    onLine: true,
}
console.log(oneStudent);

How do we make sure we don't have to keep writing this block over and over for different names?

Constructor functions
Object constructors

function Student() {
  this.codeClass = 201;
  this.onLine = true;
}

    create INSTANCES of student
let juan = new Student();
let sara = new Student();

console.log(juan)
console.log(sara)

function Student(name) {
  this.name = name;
  this.codeClass = 201;
  this.onLine = true;
}

function Student(name) {
  this.studentName = name;
  this.codeClass = 201;
  this.onLine = true;
}

name needs to be the same. studentName can be whatever we want it to be.



prototype
sara.haircolor = 'brown';
console.log(sara);
console.log(juan);

sara will be the only one with brown hair here.

~11:28~

Declare a constructor function
function Kitten (name, likes, src, alt) {
    this.name = name;
    this.about = about;
}
they always have uppercase letters to start

render makes the content show to the page.
Render?

