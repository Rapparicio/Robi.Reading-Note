# Key Question- What is JavaScript?

[Intro JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

JavaScript is a cross-platform, object-oriented scripting language used to make
webpages interactive (e.g., having complex animations, clickable buttons, popup menus, etc.).
There are also more advanced server side versions of JavaScript such as Node.js, which allow 
you to add more functionality to a website than downloading files (such as realtime collaboration
between multiple computers). Inside a host environment (for example, a web browser), 
JavaScript can be connected to the objects of its environment to provide programmatic control over them.

JavaScript contains a standard library of objects, such as Array, Date, and Math, and a 
core set of language elements such as operators, control structures, and statements. 
Core JavaScript can be extended for a variety of purposes by supplementing it with additional objects; for example:
  - Client-side JavaScript extends the core language by supplying objects to control a browser and its Document Object Model (DOM).
For example, client-side extensions allow an application to place elements on an HTML form and respond to user events 
such as mouse clicks, form input, and page navigation.
  -	Server-side JavaScript extends the core language by supplying objects relevant to running JavaScript on a server.
For example, server-side extensions allow an application to communicate with a database, provide continuity of information
from one invocation to another of the application, or perform file manipulations on a server.

This means that in the browser, JavaScript can change the way the webpage (DOM) looks. 
And, likewise, Node.js JavaScript on the server can respond to custom requests from code written in the browser.

## JavaScript and Java

JavaScript and Java are similar in some ways but fundamentally different in some others. 
The JavaScript language resembles Java but does not have Java's static typing and strong type checking. 
JavaScript follows most Java expression syntax, naming conventions and basic control-flow constructs 
which was the reason why it was renamed from LiveScript to JavaScript.

  - In contrast to Java's compile-time system of classes built by declarations, JavaScript supports a 
runtime system based on a small number of data types representing numeric, Boolean, and string values.
JavaScript has a prototype-based object model instead of the more common class-based object model.
The prototype-based model provides dynamic inheritance; that is, what is inherited can vary for individual objects.
JavaScript also supports functions without any special declarative requirements. Functions can be properties of objects,
executing as loosely typed methods. 

  - JavaScript is a very free-form language compared to Java. You do not have to  declare all variables clases and methods. You do not have to be concerned with. whether methods are public, private, or protected, and you do not have to implement interfaces. Variables, 
parameters, and function return types are not explicitly typed.

  - Java is a class-based programming language designed for fast execution and type safety. Type safety means, for instance, that you can't cast a Java integer into an object reference or access private memory by corrupting Java bytecodes. Java's class-based model means that programs consist exclusively of classes and their methods. Java's class inheritance and strong typing generally require tightly coupled object hierarchies. These requirements make Java programming more complex than JavaScript programming.

- In contrast, JavaScript descends in spirit from a line of smaller, dynamically typed languages such as HyperTalk and dBASE. These scripting languages offer programming tools to a much wider audience because of their easier syntax, specialized built-in functionality, and minimal requirements for object creation.

- Getting started with JavaScript is easy: all you need is a modern Web browser. This guide includes some JavaScript features which are only currently available in the latest versions of Firefox, so using the most recent version of Firefox is recommended.
The Web Console tool built into Firefox is useful for experimenting with JavaScript; you can use it into two modes: single-line input mode, and multi-line input mode.

## Input Output in plan JavaScript

In the first article we saw how to change the DOM to display something, and then we saw how to handle user events. This time we are going to see how to get input from the user and combine that with the other two, to create a simple page that can great you.
examples/js/pure_js_greating.html
1.	<html>
2.	<head>
3.	  <title>Hello World</title>
4.	</head>
5.	<body>
6.	 
7.	First name: <input id="first_name">
8.	Last name: <input id="last_name">
9.	<button id="say">Say hi!</button>
10.	 
11.	<hr>
12.	<div id="result"></div>
13.	 
14.	<script>
15.	function say_hi() {
16.	    var fname = document.getElementById('first_name').value;
17.	    var lname = document.getElementById('last_name').value;
18.	 
19.	    var html = 'Hello <b>' + fname + '</b> ' + lname;
20.	 
21.	    document.getElementById('result').innerHTML = html;
22.	}
23.	 
24.	document.getElementById('say').addEventListener('click', say_hi);
25.	</script>
26.	 
27.	</body>
28.	</html>
29.	 

 
In the JavaScript code we have a function called say_hi. It used the getElementById we have already seen to locate the DOM element representing the input element with the id first_name. The object returned has a method value that will return the text the user has typed in that field.
We use this technique to retrieve the content of both input fields and assign their content to two variables: fname and lname.
Then, using these variable we create an HTML snippet and assign it to a new variable called html.
Then we set the innerHTML attribute as earlier to show the HTML we generated. The result might look like this:
 
Creating HTML is cumbersome
Even in such a simple HTML we wanted to create we had to use + several time and the code is quite unreadable. Imagine what would happen if we wanted to build a more complex application where we might want to build a list of items, or even a table. Building the HTML on the fly and the inserting in the DOM would be quite nasty.
In the back-end systems written in Perl, Python or Ruby, people have encountered the same problem and the solution was the creation of various templating engines. Basically a template would be an HTML snippet with some place holders and then a function call that gets the HTML snippet (the template) as a parameter, and gets several key-value pairs. The function then returns a new HTML snippet in which the place holders were replaced by the value of the appropriate key.
In a similar way, there are many templating system for JavaScript as well. We are going to look at HandlebarsJS, the JavaScript templating engine

Example
var pi = 3.14;
var person = "John Doe";
var answer = 'Yes I am!';

In the first article we saw how to change the DOM to display something, and then we saw how to handle user events. This time we are going to see how to get input from the user and combine that with the other two, to create a simple page that can great you.
examples/js/pure_js_greating.html
1.	<html>
2.	<head>
3.	  <title>Hello World</title>
4.	</head>
5.	<body>
6.	 
7.	First name: <input id="first_name">
8.	Last name: <input id="last_name">
9.	<button id="say">Say hi!</button>
10.	 
11.	<hr>
12.	<div id="result"></div>
13.	 
14.	<script>
15.	function say_hi() {
16.	    var fname = document.getElementById('first_name').value;
17.	    var lname = document.getElementById('last_name').value;
18.	 
19.	    var html = 'Hello <b>' + fname + '</b> ' + lname;
20.	 
21.	    document.getElementById('result').innerHTML = html;
22.	}
23.	 
24.	document.getElementById('say').addEventListener('click', say_hi);
25.	</script>
26.	 
27.	</body>
28.	</html>
29.	 

 
In the JavaScript code we have a function called say_hi. 
It used the getElementById we have already seen to locate the DOM element representing the input element with the id first_name. 
The object returned has a method value that will return the text the user has typed in that field.
We use this technique to retrieve the content of both input fields and assign their content to two variables: fname and lname.
Then, using these variable we create an HTML snippet and assign it to a new variable called html.
Then we set the innerHTML attribute as earlier to show the HTML we generated. The result might look like this:
 
Creating HTML is cumbersome

Even in such a simple HTML we wanted to create we had to use + several time and the code is quite unreadable. Imagine what would happen if we wanted to build a more complex application where we might want to build a list of items, or even a table. Building the HTML on the fly and the inserting in the DOM would be quite nasty.

In the back-end systems written in Perl, Python or Ruby, people have encountered the same problem and the solution was the creation of various templating engines. Basically a template would be an HTML snippet with some place holders and then a function call that gets the HTML snippet (the template) as a parameter, and gets several key-value pairs. The function then returns a new HTML snippet in which the place holders were replaced by the value of the appropriate key.
In a similar way, there are many templating system for JavaScript as well. We are going to look at HandlebarsJS, the JavaScript templating engine.

### [Variables](https://www.w3schools.com/js/js_variables.asp)

Variables are containers for storing data (values).
In this example, x, y, and z, are variables, declared with the var keyword:

Example
var x = 5;
var y = 6;
var z = x + y;


In programming, just like in algebra, we use variables (like price1) to hold values.

In programming, just like in algebra, we use variables in expressions (total = price1 + price2).

From the example above, you can calculate the total to be 11.

JavaScript variables are containers for storing data values.

### JavaScript Identifiers

All JavaScript variables must be identified with unique names.
These unique names are called identifiers.
Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:
•	Names can contain letters, digits, underscores, and dollar signs.
•	Names must begin with a letter
•	Names can also begin with $ and _ (but we will not use it in this tutorial)
•	Names are case sensitive (y and Y are different variables)
•	Reserved words (like JavaScript keywords) cannot be used as names

### JavaScript identifiers are case-sensitive.

The Assignment Operator
In JavaScript, the equal sign (=) is an "assignment" operator, not an "equal to" operator.
This is different from algebra. The following does not make sense in algebra:
x = x + 5

In JavaScript, however, it makes perfect sense: it assigns the value of x + 5 to x.
(It calculates the value of x + 5 and puts the result into x. The value of x is incremented by 5.)
The "equal to" operator is written like == in JavaScript.

### JavaScript Data Types

JavaScript variables can hold numbers like 100 and text values like "John Doe".
In programming, text values are called text strings.
JavaScript can handle many types of data, but for now, just think of numbers and strings.
Strings are written inside double or single quotes. Numbers are written without quotes.
If you put a number in quotes, it will be treated as a text string.

Example
var pi = 3.14;
var person = "John Doe";
var answer = 'Yes I am!';


All computer –Input, Store, Process, Output








