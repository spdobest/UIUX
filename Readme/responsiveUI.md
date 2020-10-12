# RESPONSIVE UI DESIGN USING CSS
- Responsive web design makes your web page look good on all devices.
- Responsive web design uses only HTML and CSS.
- Responsive web design is not a program or a JavaScript.
- Web pages can be viewed using many different devices: desktops, tablets, and phones. Your web page should look good, and be easy to use, regardless of the device.
- Web pages should not leave out information to fit smaller devices, but rather adapt its content to fit any device:

## Viewport
- The viewport is the user's visible area of a web page.
- The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.
## Setting The Viewport
- HTML5 introduced a method to let web designers take control over the viewport, through the <meta> tag.
- You should include the following <meta> viewport element in all your web pages:
- ```<meta name="viewport" content="width=device-width, initial-scale=1.0">```
- The ```width=device-width``` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
- The ```initial-scale=1.0``` part sets the initial zoom level when the page is first loaded by the browser.
- **Ensure an accessible viewport**
- In addition to setting an initial-scale, you can also set the following attributes on the viewport:
- **minimum-scale**
- **maximum-scale**
- **user-scalable**

## Responsive Web Design - Grid-View
- **What is a Grid-View?**
- Many web pages are based on a grid-view, which means that the page is divided into columns:
- Using a grid-view is very helpful when designing web pages. It makes it easier to place elements on the page.
- A responsive grid-view often has 12 columns, and has a total width of 100%, and will shrink and expand as you resize the browser window.
- **Building a Responsive Grid-View**
- First ensure that all HTML elements have the box-sizing property set to border-box. This makes sure that the padding and border are included in the total width and height of the elements.
- Add the following code in your CSS:
```
  * {
    box-sizing: border-box;
  }
```
```
.menu {
  width: 25%;
  float: left;
}
.main {
  width: 75%;
  float: left;
}
```
- 