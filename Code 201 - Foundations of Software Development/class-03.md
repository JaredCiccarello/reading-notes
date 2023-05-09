
If there are no questions provided, summarize and explain this topic via an analogy from your previous work or home experience.
If you utilize any content directly from the reading sources, be sure to identify what you are quoting, and cite the source.

This topic matters because it gives us insight to how and why lists are made as well as the different functions that lists can provide. When creating a web page we often need lists to help us keep things organized, make them easier to read, help users find information faster, and even help users understand the purpose of our webpage. 

## <span style="color:orange"> < ol > Ordered list elements </span>

` Reversed `

    This Boolean attribute specifies that the list's items are in reverse order. Items will be numbered from high to low.

`Start`

    An integer to start counting from for the list items. Always an Arabic numeral (1, 2, 3, etc.), even when the numbering type is letters or Roman numerals. For example, to start numbering elements from the letter "d" or the Roman numeral "iv," use start="4".

` type `

    Sets the numbering type:

* a for lowercase letters
* A for uppercase letters
* i for lowercase Roman numerals
* I for uppercase Roman numerals
* 1 for numbers (default)

<ol>
  <li>first item</li>
  <li>
    second item
    <!-- closing </li> tag is not here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
  </li>
  <!-- Here's the closing </li> tag -->
  <li>third item</li>
</ol>

## <span style="color:orange">< ul > Unordered list elements </span>

    The <ul> HTML element represents an unordered list of items, typically rendered as a bulleted list.

<ul>
    <li>Milk</li>
    <li>Cheese
        <ul>
            <li>Blue cheese</li>
            <li>Feta</li>
        </ul>
    </li>
</ul>

` Compact `
    
    This Boolean attribute hints that the list should be rendered in a compact style. The interpretation of this attribute depends on the user agent, and it doesn't work in all browsers.

Warning: Do not use this attribute, as it has been deprecated: use CSS instead. To give a similar effect as the compact attribute, the CSS property line-height can be used with a value of 80%.

` type ` 

    This attribute sets the bullet style for the list. The values defined under HTML3.2 and the transitional version of HTML 4.0/4.01 are:
<ul>
    <li>circle</li> 
    <li>disc</li> 
     <li>square</li> 
</ul>

<ul>
  <li>first item</li>
  <li>
    second item
    <!-- Look, the closing </li> tag is not placed here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
    <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>

<br></br>

When should you use an unordered list in your HTML document?

    A: Display a list that does not need a specific order.

How do you change the bullet style of unordered list items?
    
    A: use list-style-type property

When should you use an ordered list vs an unorder list in your HTML document?
    
    A: When you need a list to go in a specific order.

Describe two ways you can change the numbers on list items provided by an ordered list? (Try this one again)
   
    A: Type and start. Type sets the numbers for upper and lowercase as well as roman numerals. Start allows us to start from a number and work down or up such as in the example start=4

<br> </br>
___
---
---
---
___
___
<br></br> 

## <span style="color:orange">The Box Model </span>

Everything in CSS has a box around it, and understanding these boxes is key to being able to create more complex layouts with CSS, or to align items with other items.

` Block and inline boxes `

    Boxes have an inner display type and an outer display type.

    In general, you can set various values for the display type using the display property, which can have various values.

` Outer display type `

    If a box has an outer display type of block, then:

The box will break onto a new line.
The width and height properties are respected.
Padding, margin and border will cause other elements to be pushed away from the box.
If width is not specified, the box will extend in the inline direction to fill the space available in its container. In most cases, the box will become as wide as its container, filling up 100% of the space available.

<br></br>
<br></br>
<br></br>

    Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
A: 

    List and describe the four parts of an HTML elements box as referred to by the box model.
A: Content, Padding, Border, and Margin. The area

## <span style="color:orange"> Arrays </span> 

    What data types can you store inside of an Array?
A: strings, numbers, objects, and even other arrays.

    Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
A: Yes, people array is a valid array.

    List five shorthand operators for assignment in javascript and describe what they do.
A:  x = f() is assigning,

    Read the code below and evaluate the last expression and explain what the result would be and why.
A:

    Describe a real world example of when a conditional statement should be used in a JavaScript program.
A:

    Give an example of when a Loop is useful in JavaScript.
A:
