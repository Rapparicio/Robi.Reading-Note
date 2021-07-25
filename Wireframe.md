# Important things to know about Wireframe and Semantics

[Article with 6 steps](https://user-images.githubusercontent.com/73135321/126911296-c0fc5ab6-d7d3-4a09-99be-2abda8a9f126.png)

### Here are a number of ways different designers can structure the process from design to implementation:

- Wireframe > Interactive Prototype > Visual > Design
- Sketch > Code
- Sketch > Wireframe > Hi-Def Wireframe > Visual > Code
- Sketch > Wireframe > Visual > Code

### Anatomy of an HTML element

Let's explore this paragraph element a bit further.
 ![image](https://user-images.githubusercontent.com/73135321/126911415-b55d3da2-462f-43a2-a509-e42926f81f0f.png)

### The main parts of our element are as follows:
  1. The opening tag: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
  1. The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
  1. The content: This is the content of the element, which in this case, is just text.
  1. The element: The opening tag, the closing tag, and the content together comprise the element.

Elements can also have attributes that look like the following:

 ![image](https://user-images.githubusercontent.com/73135321/126911468-46a4c681-15a0-431c-aa9d-5b9deb783149.png)
 
### An attribute should always have the following:
  1. A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
  1. The attribute name followed by an equal sign.
  1. The attribute value wrapped by opening and closing quotation marks.

### Important terms

- Nesting Elements
- Copy to Clipboard
- Empty Elements
- Anatomy of an HTML document

### Semantics

In programming, Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", 
or "what purpose or role does that HTML element have" (rather than "what does it look like?".)

- Semantics in JavaScript

In JavaScript, consider a function that takes a string parameter, and returns an <li> element with that string as its textContent.
Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?

- Semantics in CSS
 
In CSS, consider styling a list with li elements representing different types of fruits.
Would you know what part of the DOM is being selected with div > ul > li, or .fruits__item?

- Semantics in HTML
In HTML, for example, the h1 element is a semantic element, which gives the text it wraps around the role (or meaning) of -a top level heading on your page.

- Copy to Clipboard
 
By default, most browser's user agent stylesheet will style an h1 with a large font size to make it look like a heading (although you could style it to look like anything you wanted).

- On the other hand, you could make any element look like a top level heading. Consider the following:

span style="font-size: 32px; margin: 21px 0;">Is this a top level heading?</span 

Copy to Clipboard
 
This will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits as described above. It is therefore a good idea to use the right HTML element for the right job.

HTML should be coded to represent the data that will be populated and not based on its default presentation styling. Presentation (how it should look), is the sole responsibility of CSS.

Some of the benefits from writing semantic markup are as follows:

- Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
- Screen readers can use it as a signpost to help visually impaired users navigate a page
- Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
- Suggests to the developer the type of data that will be populated
- Semantic naming mirrors proper custom element/component naming
- When approaching which markup to use, ask yourself, "What element(s) best describe/represent the data that I'm going to populate?" For example, is it a list of data?; ordered, unordered?; is it an article with sections and an aside of related information?; does it list out definitions?; is it a figure or image that needs a caption?; should it have a header and a footer in addition to the global site-wide header and footer?; etc.

Semantic elements
These are some of the roughly 100 semantic elements available:

< article >
< aside >
< details >
< figcaption >
< figure >
< footer >
< header >
< main >
< mark >
< nav >
< section >
< summary >
< time >
 
