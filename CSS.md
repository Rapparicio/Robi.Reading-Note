<h1>What is CSS for?</h1>

As we have mentioned before, CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

CSS can be used for very basic document text styling 

  - For example changing the color and size of headings and links. 
  - It can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information.
  - It can even be used for effects such as animation. Have a look at the links in this paragraph for specific examples.


[CSS Colors](https://www.w3schools.com/css/css_colors.asp)

[CSS Structure](https://www.w3schools.com/cssref/pr_text_color.asp)

<h2>CSS Syntax</h2>

CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

For example "I want the main heading on my page to be shown as large red text."

The following code shows a very simple CSS rule that would achieve the styling described above:
h1 {
    color: red;
    font-size: 5em;
}

The rule opens with a selector. This selects the HTML element that we are going to style. In this case we are styling level one headings (< h1 >).
We then have a set of curly braces { }. Inside those will be one or more declarations, which take the form of property and value pairs. 
Each pair specifies a property of the element(s) we are selecting, then a value that we'd like to give the property.
Before the colon, we have the property, and after the colon, the value. CSS properties have different allowable values, depending on which property is being specified. 
In our example, we have the color property, which can take various color values. We also have the font-size property. This property can take various size units as a value.

<h2>External CSS</h2>

With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

<h2>Internal CSS</h2>
An internal style sheet may be used if one single HTML page has a unique style.
The internal style is defined inside the <style> element, inside the head section.
Example
Internal styles are defined within the <style> element, inside the <head> section of an HTML page:
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

  <h2>Inline CSS</h2>
An inline style may be used to apply a unique style for a single element.
  
To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
  
Example
Inline styles are defined within the "style" attribute of the relevant element:
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>

Tip: An inline style loses many of the advantages of a style sheet (by mixing content with presentation). Use this method sparingly.
  
  <h2>Multiple Style Sheets</h2>
  
If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used. 
Assume that an external style sheet has the following style for the <h1> element:
h1 {
  color: navy;
}
Then, assume that an internal style sheet also has the following style for the <h1> element:
h1 {
  color: orange;   



  
  
  
  
