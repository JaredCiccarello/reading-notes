Class 1 Reading

    Why this topic matters:
A: This topic matters because it explains in depth the relationship, ability, and format for those new to computers.

## How the web works
Clients and servers
Computers connected to the internet are called clients and servers.

Clients are the typical web user's internet-connected devices (for example, your computer connected to your Wi-Fi, or your phone connected to your mobile network) and web-accessing software available on those devices (usually a web browser like Firefox or Chrome).

Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's web browser.

Your internet connection: Allows you to send and receive data on the web.

TCP/IP: Transmission Control Protocol and Internet Protocol are communication protocols that define how data should travel across the internet. 

HTTP: Hypertext Transfer Protocol is an application protocol that defines a language for clients and servers to speak to each other. 

Component files: A website is made up of many different files.

Assets: This is a collective name for all the other stuff that makes up a website, such as images, music, video, Word documents, and PDFs.

So what happens, exactly?
When you type a web address into your browser (for our analogy that's like walking to the shop):

The browser goes to the DNS server, and finds the real address of the server that the website lives on (you find the address of the shop).
The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client (you go to the shop and order your goods). This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP.
If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is", and then starts sending the website's files to the browser as a series of small chunks called data packets (the shop gives you your goods, and you bring them back to your house).
The browser assembles the small chunks into a complete web page and displays it to you (the goods arrive at your door — new shiny stuff, awesome!).

DNS explained
Real web addresses aren't the nice, memorable strings you type into your address bar to find your favorite websites. They are special numbers that look like this: 63.245.215.20.

## Website Design and Process
To begin, you'll need to answer these questions:

What is your website about? Do you like dogs, New York, or Pac-Man?
What information are you presenting on the subject? Write a title and a few paragraphs and think of an image you'd like to show on your page.
What does your website look like, in simple high-level terms? What's the background color? What kind of font is appropriate: formal, cartoony, bold and loud, subtle?

Next, sketch out roughly how you want your site to look.

Next, choose a color, go to the Color Picker and find a color you like.

When you click on a color, you'll see a strange six-character code like #660066. That's called a hex code

Next, choose an image. Right click and cop the image web address.

Next, choose a font:

Go to Google Fonts and find one you like.
Copy the lines of code Google gives you into your text editor to save for later.

    Compose a short poem describing how HTTP sends data between computers.
A: A poem; Send your message quickly, your clients cannot wait, they require this matter carried swiftly, your server may already be late.

    Describe how HTML, CSS, and JS files are “parsed” in the browser.
A: When using a coding format, such as VS code, we utilize different languages. In order for each language to be distinguished between the other we format the languages by seperating them into HTML, CSS, and JS or "Hyper Text Markup Language" "Cascading Style Sheets" and "JavaScript".

    How can you find images to add to a Website?
A: Copy paste your image into your HTML using an <img> tag

    How do you create a String vs a Number in JavaScript?
A:  A string can be created using double/single quotes or backticks. While a number can be be written as is.

    What is a Variable and why are they important in JavaScript?
A: A name of a storage location. They are important because they hold data value, this value can be changed.


## Introduction to HTML
At its heart, HTML is a language made up of elements, which can be applied to pieces of text to give them different meaning in a document.

## Getting started with HTML
    (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit.
    If we wanted the text to stand by itself, we could specify that it is a paragraph by enclosing it in a paragraph (<p>) element: <p>My cat is very grumpy</p>
    The anatomy of our element is:

The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.

The content: This is the content of the element. In this example, it is the paragraph text.

The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

Using <em></em> should give the line italic text.

    **Nesting Elements** 
    Elements can be placed within other elements. This is called nesting.
<p>My cat is <strong>very</strong> grumpy.</p> RIGHT WAY
    For proper nesting, we should close the strong element first, before closing the p.
<p>My cat is <strong>very grumpy.</p></strong> WRONG WAY

A block-level element appears on a new line following the content that precedes it. 
For example, a block-level element might represent headings, paragraphs, lists, navigation menus, or footers.

Void elements
Some elements consist of a single tag, which is typically used to insert/embed something in the document.

Attributes
Elements can also have attributes.

An attribute should have:

A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
The attribute name, followed by an equal sign.
An attribute value, wrapped with opening and closing quote marks.

ref
This attribute's value specifies the web address for the link. For example: href="https://www.mozilla.org/".

title
The title attribute specifies extra information about the link, such as a description of the page that is being linked to. For example, title="The Mozilla homepage". This appears as a tooltip when a cursor hovers over the element.

target
The target attribute specifies the browsing context used to display the link. For example, target="_blank" will display the link in a new tab. If you want to display the linked content in the current tab, just omit this attribute.

Boolean attributes
Sometimes you will see attributes written without values. This is entirely acceptable.

Make sure you don't mix single quotes and double quotes. This example (below) shows a kind of mixing quotes that will go wrong:

<a href="https://www.example.com'>A link to my example.</a>

To use quote marks inside other quote marks of the same type (single quote or double quote), use HTML entities. For example, this will break:

<a href='https://www.example.com' title='Isn't this fun?'>A link to my example.</a>
Instead, you need to do this:

<a href='https://www.example.com' title='Isn&apos;t this fun?'>A link to my example.</a>

<!DOCTYPE html>: The doctype. When HTML was young (1991-1992), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML. Doctypes used to look something like this:
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
More recently, the doctype is a historical artifact that needs to be included for everything else to work right. <!DOCTYPE html> is the shortest string of characters that counts as a valid doctype. That is all you need to know!

    What is an HTML attribute?
A: A piece of markup language used to adjust the behavior or display of an HTML element

    Describe the Anatomy of an HTMl element.
A: Opening Tag, closing tag, content, and element.

    What is the Difference between <article> and <section> element tags?
A: Article tags wrap content on a page. Section tag simply defines a section within a document.

    What Elements does a “typical” website include?
A: Links. Paragraphs. Headings. Numbered and bulleted lists. Tables. Regions. Images.

    How does metadata influence Search Engine Optimization?
A: This helps search engines better understand the topic of your webpages and content.

    How is the <meta> HTML tag used when specifying metadata?
A: <meta> is usually placed in the <head> element and used to help specify types of metadata. It's purpose is to help create a search engine-friendly document.


## How to start to design a Website
there are a few questions you should answer before anything else:

What exactly do I want to accomplish?
How will a website help me reach my goals?
What needs to be done, and in what order, to reach my goals?

All of this is called project ideation and is a necessary first step to reach your goal.

What exactly do I want to accomplish?
This is the most important question to answer, since it drives everything else. Start creating a list.

How can a website help me reach my goals? By answering that, you'll find the best way to reach your goals and save yourself from wasted effort.

What needs to be done, and in what order, to reach my goals?
Now that you know what you want to accomplish, it's time to turn those goals into actionable steps. As a side note, your goals are not necessarily set in stone. They evolve over time even in the course of the project, especially if you run across unexpected obstacles or just change your mind.

    What is the first step to designing a Website?
A: Determine your site's objective.

    What is the most important question to answer when designing a Website?
A: What do I want to accomplish?

## Semantics
In programming, Semantics refers to the meaning of a piece of code.
Semantics in JavaScript
In JavaScript, consider a function that takes a string parameter, and returns an <li> element with that string as its textContent. Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?

Semantics in CSS
In CSS, consider styling a list with li elements representing different types of fruits. Would you know what part of the DOM is being selected with div > ul > li, or .fruits__item?

Semantics in HTML
In HTML, for example, the h1 element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

Some of the benefits from writing semantic markup are as follows:

Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
Screen readers can use it as a signpost to help visually impaired users navigate a page
Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
Suggests to the developer the type of data that will be populated
Semantic naming mirrors proper custom element/component naming.

Some examples of semantic tags are <Header> <footer> <main

    Why should you use an <h1> element over a <span> element to display a top level heading?
A: Span elements are typically used for small text, images, and other elements. An h1 tag is specifically for the web page title.

    What are the benefits of using semantic tags in our HTML?
A: Using semantic tags makes your webpage more adaptable, helping browsers to interpret your webpage content.

## What is JavaScript?
JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, and even animate images.
The core client-side JavaScript language consists of some common programming features that allow you to do things like:

Store useful values inside variables. In the above example for instance, we ask for a new name to be entered then store that name in a variable called name.
Operations on pieces of text (known as "strings" in programming). In the above example we take the string "Player 1: " and join it to the name variable to create the complete text label, e.g. "Player 1: Chris".
Running code in response to certain events occurring on a web page. We used a click event in our example above to detect when the label is clicked and then run the code that updates the text label.

Browser APIs are built into your web browser, and are able to expose data from the surrounding computer environment, or do useful complex things. For example:

The DOM (Document Object Model) API allows you to manipulate HTML and CSS, creating, removing and changing HTML, dynamically applying new styles to your page, etc. Every time you see a popup window appear on a page, or some new content displayed (as we saw above in our simple demo) for example, that's the DOM in action.
The Geolocation API retrieves geographical information. This is how Google Maps is able to find your location and plot it on a map.
The Canvas and WebGL APIs allow you to create animated 2D and 3D graphics. People are doing some amazing things using these web technologies — see Chrome Experiments and webglsamples.
Audio and Video APIs like HTMLMediaElement and WebRTC allow you to do really interesting things with multimedia, such as play audio and video right in a web page, or grab video from your web camera and display it on someone else's computer (try our simple Snapshot demo to get the idea).
A very common use of JavaScript is to dynamically modify HTML and CSS to update a user interface.

    Describe 2 things that require JavaScript in the Browser?
A: Dynamic content and form validation.

    How can you add JavaScript to an HTML document?
A: Using the <script> tag with the attribute src.
    <script src="js/script.js"></script>