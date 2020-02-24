# CSS3
  
## What is CSS?  
CSS stands for Cascading Style Sheets  
CSS describes how HTML elements are to be displayed on screen, paper, or in other media  
CSS saves a lot of work. It can control the layout of multiple web pages all at once  
External stylesheets are stored in CSS files   
  
## What CSS do ?  
HTML is only intend to show the content in the web page. HTML should not hold any design login and design parameters in the HTML code. Otherwise it will be very difficult to manage the HTML code.  
    
To solve the above problem we define all the styles in the .css file and add the style to the HTML page which helps to reuse the styles and also  easy to maintain the HTML code.  
  
## How can we define the styles in HTML ?  
There are different ways to define styles in HTML.  
1. **Internal CSS** We can define styles inside the HTML file   
2. **External CSS** we can define styles in another .css file and include that .css file in the HTML file where we want to apply the list of styles defined in that HTML file.  
3. **Inline CSS**  
  
**Here is the example of above two methods**  
```  
<!DOCTYPE html>
<html>
<head>

<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>

</head>
<body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```   
**Another way to define styles inside separate .css file. Like below.**  
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
  
**Remove the style block from the HTML file.  
In the HTML file, add a link tag after the closing title tag that points to StyleSheet.css.**   
```  
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
``` 
**EXAMPLE OF INLINE CSS**  
```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```
  
## CSS Selectors  
CSS selectors are used to "find" (or select) the HTML elements you want to style.  
  
We can divide CSS selectors into five categories:  

**Simple selectors (select elements based on name, id, class)  
Combinator selectors (select elements based on a specific relationship between them)  
Pseudo-class selectors (select elements based on a certain state)  
Pseudo-elements selectors (select and style a part of an element)  
Attribute selectors (select elements based on an attribute or attribute value)**  
    
## ELEMENT SELECTOR ( Without using any prefix like below )  
```
p {
  text-align: center;
  color: red;
}   
```  
## ID SELECTOR ( Using # front of the id name )  
The CSS rule below will be applied to the HTML element with id="para1":   
```   
#para1 {
  text-align: center;
  color: red;
}
```  
## CLASS SELECTOR ( by using . before the class name )   
In this example all HTML elements with class="center" will be red and center-aligned:   
  
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

**OTHER EXAMPLEs**   
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
  
  
     
     
