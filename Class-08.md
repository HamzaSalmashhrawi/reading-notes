
# Layout 
### Key Concepts in Positioning Elements

### building Blocks 
##### CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

### Containing Elements
#### If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
#### Controlling the Position of Elements
##### CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.
#### Normal flow 
##### Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else)

###  Relative Positioning
#### This moves an element from the position it would be in normal flow, shifting it to the top, right bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.
#### Absolute positioning
##### This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

#### this picture bellow present the postioning
![flow](img/sc14.png)

_______________________________________________________________________ 

## Normal flow 
#### In normal flow, each block-level element sits on top of the nextone. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be:

`position: static;`

#### I haven't specified a width property for the heading element, so you can see how it stretches the width of the entire browser window by default.

#### The paragraphs are restricted to 450 pixels wide. This shows how the elements in normal flow start on a new line even if they do not take up the full width of the browser window

```
HTML 

<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking
 machine that would help him get around the
 royal gardens faster...</p>
</body>
```

```
CSS

body {
width: 750px;
font-family: Arial, Verdana, sans-serif;
color: #665544;}
h1 {
background-color: #efefef;
padding: 10px;}
p {
width: 450px;}
```