# CSS Tutorial
- It stands for Cascading Style Sheet
- It is used to style the HTML page
- Before CSS, style is added to all the html page and it become very huge and also difficult to maintain.
  
## What can you do with CSS
- easily apply same style rules on multiple elements.
- control the presentation of multiple pages of a website with a single style sheet.
- present the same page differently on different devices.
- style dynamic states of elements such as hover, focus, etc. that isn't possible otherwise.
- change the position of an element on a web page without changing the markup.
- alter the display of existing HTML elements.
- transform elements like scale, rotate, skew, etc. in 2D or 3D space.
- create animations and transitions effects without using any JavaScript.
- create print friendly version of your web pages.
  
## Advantages of Using CSS
- CSS Save Lots of Time
- Easy Maintenance
- Pages Load Faster
- Superior Styles to HTML
- Multiple Device Compatibility

## How to include CSS in html page
- There are 3 ways to do this
1. Inline styles — Using the style attribute in the HTML start tag  
2. Embedded styles — Using the <style> element in the head section of a document  
3. External style sheets — Using the <link> element, pointing to an external CSS file  
  
## Inline Styles
```
    <h1 style="color:red; font-size:30px;">This is a heading</h1>
    <p style="color:green; font-size:22px;">This is a paragraph.</p>
    <div style="color:blue; font-size:14px;">This is some text content.</div>
```
## Embedded styles
```
    <html lang="en">
    <head>
        <title>My HTML Document</title>
        <style>
            body { background-color: YellowGreen; }
            p { color: #fff; }
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph of text.</p>
    </body>
    </html>
```
## External style sheets
- Create another style.css file and include in the html page like this
- Include the style.css file inside head tag
- In below Example style.css is the file where all styles declared
- ```
  <head>
      <title>My HTML Document</title>
      <link rel="stylesheet" href="css/style.css">
  </head>
```
## How to import external Style sheet
- ```
    <style>
    @import url("css/style.css");
    p {
        color: blue;
        font-size: 16px;
    }
  </style>
  
  @import url("css/layout.css");
  @import url("css/color.css");
  body {
    color: blue;
    font-size: 14px;
  }
```

