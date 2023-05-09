Class 04 reading 

## Creating hyperlinks
Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address.

A basic link is created by wrapping the text or other content inside an <a> element and using the href attribute, also known as a Hypertext Reference, or target that contains the web address.

` Block level links `

If you want to make a heading element a link then wrap it in an anchor (<a>)

` Image links `

If you have an image you want to make into a link, use the <a> element to wrap the image file referenced with the <img> element

` Adding supporting information with the title attribute `

Another attribute you may want to add to your links is title.

To fully understand link targets, you need to understand URLs and file paths.

A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web.
URLs use paths to find files. Paths specify where the file you're interested in is located in the filesystem.

Moving down into subdirectories: If you wanted to include a hyperlink inside index.html (the top level index.html) pointing to projects/index.html, you would need to go down into the projects directory before indicating the file you want to link to. This is done by specifying the directory's name, then a forward slash, then the name of the file.
<p>Visit my <a href="projects/index.html">project homepage</a>.</p>

`Document fragments `
It's possible to link to a specific part of an HTML document, known as a document fragment, rather than just to the top of the document.
To do this you first have to assign an id attribute to the element you want to link to. It normally makes sense to link to a specific heading, so this would look something like the following:

<h2 id="Mailing_address">Mailing address</h2>

` Absolute versus relative URLS `

Two terms you'll come across on the Web are absolute URL and relative URL:

    absolute URL: Points to a location defined by its absolute location on the web, including protocol and domain name.
    An absolute URL will always point to the same location, no matter where it's used.

    relative URL: Points to a location that is relative to the file you are linking from, more like what we looked at in the previous section. 
    A relative URL will point to different places depending on the actual location of the file you refer from — for example if we moved our index.html file out of the projects directory and into the root of the website (the top level, not in any directories), the pdfs/project-brief.pdf relative URL link inside it would now point to a file located at https://www.example.com/pdfs/project-brief.pdf, not a file located at https://www.example.com/projects/pdfs/project-brief.pdf.

` Link best practices `

 We need to make our links accessible to all readers, regardless of their current context and which tools they prefer. For example:

Screen reader users like jumping around from link to link on the page, and reading links out of context.

Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to.

Visual readers skim over the page rather than reading every word, and their eyes will be drawn to page features that stand out, like links. They will find descriptive link text useful.

Example:
Good link text: Download Firefox
<p><a href="https://www.mozilla.org/firefox/">
  Download Firefox
</a></p>

Bad link text: Click here to download Firefox
<p><a href="https://www.mozilla.org/firefox/">
  Click here
</a>
to download Firefox</p>

    To create a basic link, we wrap text or other content inside what element?
A: <a> anchor tag

    The href attribute contains what information?\
A: The web address.

    What are some ways we can ensure links on our pages are accessible to all readers?
A: Screen readers, search engines, and visual readers.


## CSS Layout: Normal Flow
`Normal Flow`

This article explains normal flow, or the way that webpage elements lay themselves out if you haven't changed their layout.

`How are elements laid out by default?`
The process begins as the boxes of individual elements are laid out in such a way that any padding, border, or margin they happen to have is added to their content. This is what we call the box model.

By default, a block level element's content fills the available inline space of the parent element containing it and the element grows along the block dimension to accommodate its content. The size of inline elements is just the size of their content. You can't set width or height on inline elements — they just sit inside the content of block level elements — except for images. Unlike other inline elements, images can be resized without changing their display property. If you want to control the size of an inline element in this manner, you need to set it to behave like a block level element (e.g., with display: block; or display: inline-block;, which mixes characteristics from both).

The normal layout flow (mentioned in the layout introduction article) is the system by which elements are placed inside the browser's viewport. By default, block-level elements are laid out in the block flow direction, which is based on the parent's writing mode (initial: horizontal-tb). Each element will appear on a new line below the last one, with each one separated by whatever margin that's been specified. In English, for example, (or any other horizontal, top to bottom writing mode) block-level elements are laid out vertically.

Inline elements behave differently. They don't appear on new lines; instead, they all sit on the same line along with any adjacent (or wrapped) text content as long as there is space for them to do so inside the width of the parent block level element. If there isn't space, then the overflowing content will move down to a new line.

If two vertically adjacent elements both have a margin set on them and their margins touch, the larger of the two margins remains and the smaller one disappears. This is known as margin collapsing. Collapsing margins is only relevant in the vertical direction.

Let's look at a simple example that explains all of this:

<h1>Basic document flow</h1>
<p>
  I am a basic block level element. My adjacent block level elements sit on new
  lines below me.
</p>
<p>
  By default we span 100% of the width of our parent element, and we are as tall
  as our child content. Our total width and height is our content + padding +
  border width/height.
</p>
<p>
  We are separated by our margins. Because of margin collapsing, we are
  separated by the width of one of our margins, not both.
</p>
<p>
  Inline elements <span>like this one</span> and <span>this one</span> sit on
  the same line along with adjacent text nodes, if there is space on the same
  line. Overflowing inline elements will
  <span>wrap onto a new line if possible (like this one containing text)</span>,
  or just go on to a new line if not, much like this image will do:
  <img src="long.jpg" alt="snippet of cloth" />
</p>

What is meant by “normal flow”?
What are a few differences between block-level and inline elements?
___ positioning is the default for every html element.
Name a few advantages to using absolute positioning on an element.
What is a key difference between fixed positioning and absolute positioning?



## CSS Layout: Positioning
Positioning allows you to take elements out of normal document flow and make them behave differently, for example, by sitting on top of one another or by always remaining in the same place inside the browser viewport.

`Introduce Positioning`
Positioning allows us to produce interesting results by overriding normal document flow. What if you want to slightly alter the position of some boxes from their default flow position to give a slightly quirky, distressed feel? Positioning is your tool. Or what if you want to create a UI element that floats over the top of other parts of the page and/or always sits in the same place inside the browser window no matter how much the page is scrolled? Positioning makes such layout work possible.










What is meant by “normal flow”?
What are a few differences between block-level and inline elements?
___ positioning is the default for every html element.
Name a few advantages to using absolute positioning on an element.
What is a key difference between fixed positioning and absolute positioning?

## Functions – Reusable Blocks of Code
Describe the difference between a function declaration and a function invocation.
What is the difference between a parameter and an argument?

## 6 Reasons for Pair Programming
Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.