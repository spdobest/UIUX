# Beginner CSS3
  
## What is CSS?  
CSS stands for Cascading Style Sheets  
CSS describes how HTML elements are to be displayed on screen, paper, or in other media  
CSS saves a lot of work. It can control the layout of multiple web pages all at once  
External stylesheets are stored in CSS files   
  
## What CSS do ?  
HTML is only intend to show the content in the web page. HTML should not hold any design login and design parameters in the HTML code. Otherwise it will be very difficult to manage the HTML code.  
    
To solve the above problem we define all the styles in the .css file and add the style to the HTML page which helps to reuse the styles and also  easy to maintain the HTML code.  
  
## Applying CSS to HTML page ?  
There are different ways to define styles in HTML.  
- 1. **Inline CSS**  
- 2. **Internal CSS** We can define styles inside the HTML file   
- 3. **External CSS** we can define styles in another .css file and include that .css file in the HTML file where we want to apply the list of styles defined in that HTML file.  

## 1. Inline css
- Inline styles are plonked straight into the HTML tags using the style attribute.
- They look something like this:
- for more details look at the example below
``` <p style="color: red">text</p> ``` 
## Embedded, or internal CSS
-  Embedded, or internal, styles are used for the whole page. Inside the head element, the style tags surround all of the styles for the page.
```  
<!DOCTYPE html>
<html>
<head>
<title>CSS Example</title>
<style>
    p {
        color: red;
    }
    a {
        color: blue;
    }
</style>
...
```   
- This will make all of the paragraphs in the page red and all of the links blue.
## External CSS
- In this weay define all the style inside another .css file and include the css file in the html file

```
h1 {
  text-align: center;
  font-size: 1em;
  color: #009;
  margin-bottom: .3em;
  text-decoration: underline;
}

table {
  margin: .3em;
  width: 290px;
}

th {
  padding: .2em;
}

td {
  padding-left: .5em;
  padding-right: .5em;
  border: 1px solid #900;
  background-color: #ffc;
}

#trHeader {
  text-decoration: underline;
  color: #900;
}

.centerCell {
  text-align: center;
}
```
- Remove the style block from the HTML file.  
- In the HTML file, add a link tag after the closing title tag that points to StyleSheet.css.**   
```  
<!DOCTYPE html>
<html>
<head>
    <title>CSS Example</title>
    <link rel="stylesheet" href="style.css">
...
``` 
## Selectors properties and values
- Whereas HTML has tags, CSS has selectors. Selectors are the names given to styles in internal and external style sheets. 
- In this CSS Beginner Tutorial we will be concentrating on HTML selectors, which are simply the names of HTML tags and are used to change the style of a specific type of element.
- For each selector there are “properties” inside curly brackets, which simply take the form of words such as color, font-weight or background-color.
- A value is given to the property following a colon (NOT an “equals” sign). Semi-colons are used to separate the properties.
```
body {
    font-size: 14px;
    color: navy;
}
```
- This will apply the given values to the font-size and color properties to the body selector.
## Lengths and Percentages
- There are many property-specific units for values used in CSS, but there are some general units that are used by a number of properties and it is worth familiarizing yourself with these before continuing.
- **px** (such as font-size: 12px) is the unit for pixels.
- **em** (such as font-size: 2em) is the unit for the calculated size of a font. So “2em”, for example, is two times the current font size.
- **pt** (such as font-size: 12pt) is the unit for points, for measurements typically in printed media.
% (such as width: 80%) is the unit for… wait for it… percentages.
## Colors
- CSS brings 16,777,216 colors to your disposal. They can take the form of a name, an RGB (red/green/blue) value or a hex code.
  - red
  - rgb(255,0,0)
  - rgb(100%,0%,0%)
  - #ff0000
  - #f00
## color and background-color
- Colors can be applied by using color and background-color (note that this must be the American English “color” and not “colour”).
```
h1 {
    color: yellow;
    background-color: blue;
}
```
## font-family
- This is the font itself, such as Times New Roman, Arial, or Verdana.
- Note: if the name of a font is more than one word, it should be put in quotation marks, such as font-family: "Times New Roman".
## font-size
## font-weight
- font-weight states whether the text is bold or not. Most commonly this is used as font-weight: bold or font-weight: normal but other values are bolder, lighter, 100, 200, 300, 400 (same as normal), 500, 600, 700 (same as bold), 800 or 900.
## font-style
- font-style states whether the text is italic or not. It can be font-style: italic or font-style: normal.
## text-decoration
- text-decoration states whether the text has got a line running under, over, or through it.
- **text-decoration:** underline, does what you would expect.
- **text-decoration:** overline places a line above the text.
- **text-decoration:** line-through puts a line through the text (“strike-through”).
## text-transform
- text-transform will change the case of the text.
- **text-transform:** capitalize turns the first letter of every word into uppercase.
- **text-transform:** uppercase turns everything into uppercase.
- **text-transform:** lowercase turns everything into lowercase.
- **text-transform:** none I’ll leave for you to work out.
## Spacing
- letter spacing
- word spacing
- line spacing
## Margins and Padding
- margin and padding are the two most commonly used properties for spacing-out elements. 
- A margin is the space outside something, whereas padding is the space inside something.
```
h2 {
    font-size: 1.5em;
    background-color: #ccc;
    margin: 20px;
    padding: 40px;
}

p {
    margin-top: 1px;
    margin-right: 5px;
    margin-bottom: 10px;
    margin-left: 20px;
}
```
## Styling Links with CSS
- A link has four different states — link, visited, active and hover. These four states of a link can be styled differently through using the following anchor pseudo-class selectors.
  - **a:link** — define styles for normal or unvisited links.
  - **a:visited** — define styles for links that the user has already visited.
  - **a:hover** — define styles for a link when the user place the mouse pointer over it.
  - **a:active**— define styles for links when they are being clicked.
```
a:link {    /* unvisited link */
    color: #ff0000;
    text-decoration: none;
    border-bottom: 1px solid;
}
a:visited {    /* visited link */
    color: #ff00ff;
}
a:hover {    /* mouse over link */
    color: #00ff00;
    border-bottom: none;
}
a:active {    /* active link */
    color: #00ffff;
}
```
- For more details visit **https://www.tutorialrepublic.com/css-tutorial/css-links.php**
- 
## CSS Lists 
- There are three different types of list in HTML:
- **Unordered lists** — A list of items, where every list items are marked with bullets.
- **Ordered lists** — A list of items, where each list items are marked with numbers.
- **Definition list** — A list of items, with a description of each item.  

## The Box Model
- Margins, padding and borders (see next page) are all part of what’s known as the Box Model. 
- The Box Model works like this: in the middle you have the content area (let’s say an image), surrounding that you have the padding, surrounding that you have the border and surrounding that you have the margin.
## Borders
- Borders can be applied to most HTML elements within the body.
- To make a border around an element, all you need is border-style. The values can be **solid, dotted, dashed, double, groove, ridge, inset and outset**.
```
h2 {
    border-style: dashed;
    border-width: 3px;
    border-left-width: 10px;
    border-right-width: 10px;
    border-color: red;
}
```
## CSS Selectors 
- **For More detsils follow https://www.tutorialrepublic.com/css-tutorial/css-selectors.php**
- CSS selectors are used to "find" (or select) the HTML elements you want to style.
- We can divide CSS selectors into five categories:  
- 1. **Simple selectors** (select elements based on name, id, class)  
- 2. **Combinator selectors** (select elements based on a specific relationship between them)  
- 3. **Pseudo-class selectors** (select elements based on a certain state)  
- 4. **Pseudo-elements selectors** (select and style a part of an element)  
- 5. **Attribute selectors** (select elements based on an attribute or attribute value)**  

## ELEMENT SELECTOR ( Without using any prefix like below )  
```
p {
  text-align: center;
  color: red;
}   
```  
## ID SELECTOR ( Using # front of the id name )  
- The CSS rule below will be applied to the HTML element with id="para1":   
```   
#para1 {
  text-align: center;
  color: red;
}
```  
## CLASS SELECTOR ( by using . before the class name )   
- In this example all HTML elements with class="center" will be red and center-aligned:   
  
```
.center {
  text-align: center;
  color: red;
}
```  
**You can define like below**  
In this example only <p> elements with class="center" will be center-aligned:  
  
```  
p.center {
  text-align: center;
  color: red;
}
```  
    
## Universal Selector  
The CSS rule below will affect every HTML element on the page:   
```
* {
  text-align: center;
  color: blue;
}  
```  

## OTHER EXAMPLES
```
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```  
You can convert the above style to below  
```
h1, h2, p {
  text-align: center;
  color: red;
}
```  
## List of basic properties used in CSS  
**1.Background**  
      a. background-color - specifies the background color of an element   
      b. background-image - specifies an image to use as the background of an element   
      c. background-repeat - property repeats an image both horizontally and vertically  
      d. background-attachment - property specifies whether the background image should scroll or be fixed  
      e. background-position - To shorten the code, it is also possible to specify all the background properties in one single          property  
      **Example**  
```
      background-color: lightblue;
      background-image: url("paper.gif");
      background-image: url("img_tree.png");
      background-repeat: no-repeat;
      background-position: right top;
      background-attachment: fixed;
```   
**2.Boarder Style**   
      border-width: 5px;
      border-color: red;
      Boarder slide  
      border-radius: 5px;  
```
      border-top-style: dotted;
      border-right-style: solid;
      border-bottom-style: dotted;
      border-left-style: solid;  
```
   dotted - Defines a dotted border  
   dashed - Defines a dashed border  
   solid - Defines a solid border  
   double - Defines a double border  
   groove - Defines a 3D grooved border. The effect depends on the border-color value  
   ridge - Defines a 3D ridged border. The effect depends on the border-color value  
   inset - Defines a 3D inset border. The effect depends on the border-color value  
   outset - Defines a 3D outset border. The effect depends on the border-color value  
   none - Defines no border  
   hidden - Defines a hidden border  
        
```
        p.dotted {border-style: dotted;}
        p.dashed {border-style: dashed;}
        p.solid {border-style: solid;}
        p.double {border-style: double;}
        p.groove {border-style: groove;}
        p.ridge {border-style: ridge;}
        p.inset {border-style: inset;}
        p.outset {border-style: outset;}
        p.none {border-style: none;}
        p.hidden {border-style: hidden;}
        p.mix {border-style: dotted dashed solid double;}
        in the above code, p is for <p class = "dotted"> <p>
```  
**3.Padding**  
```
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```  
  
```
p {
  margin: 25px 50px 75px 100px;
}
```  
  
***Note: we define padding same as marggin above***  
  
**4.Width/Height**  
a.  height     - Sets the height of an element  
b.  max-height -	Sets the maximum height of an element  
c.  max-width  - Sets the maximum width of an element  
d.  min-height - Sets the minimum height of an element  
e.  min-width  - Sets the minimum width of an element  
f.  width      - Sets the width of an element  
  
**5.font**  
```
p {
  font-family: "Times New Roman", Times, serif;
}
```  
  
**6. List Style**  
```
ul.a {
  list-style-type: circle;
}

ul.b {
  list-style-type: square;
}

ol.c {
  list-style-type: upper-roman;
}

ol.d {
  list-style-type: lower-alpha;
}
```  
  
  
     
     
