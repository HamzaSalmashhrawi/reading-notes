# Javascripts 
## Object Literals
#### WHAT IS AN OBJECT?
##### Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,variables and functions take on new names. 
##### 1. Variables: IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES, If a variable is part of an object, it is called a property. Properties tell us about the object, such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.
##### 2. Functions: IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS, If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms.

### CREATING· OBJECTS USING LITERAL NOTATION

##### This example starts by creating an object using literal notation.
##### This object is called hotel which represents a hotel called Quay with 40 rooms (25 of which have been booked).
##### Next, the content of the page is updated with data from this object. It shows the name of the hotel by accessing the object's name property and the number of vacant rooms using the checkAvail ability() method.

##### To access a property of this object, the object name is followed by a dot (the period symbol) and the name of the property that you want.

##### Similarly, to use the method, you can use the object name followed by the method name. hotel . checkAvailability()

##### If the method needs parameters, you can supply them in the parentheses (just like you can pass arguments to a function). 

```
Javascript

var hotel = {
name: 'Quay',
rooms: 40,
booked : 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var el Name = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms.textContent = hotel .checkAvailability();
```

### CREATING MORE OBJECT LITERALS

##### Here you can see another object. Again it is called hote 1, but this time the model represents a different hotel. For a moment, imagine that this is a different page of the same travel website.

##### The Park hotel is larger. It has 120 rooms and 77 of them are booked.

```
Javascript

var hotel = {
name: 'Park',
rooms: 120,
booked : 77,
checkAvailabi lity: function() {
return this.rooms - this.booked;
}
} ;
var elName = document .getElementByid('hotelName') ;
elName .textContent =hotel .name ;
var el Rooms = document .getElementByid( 'rooms') ;
e 1 Rooms . text Content = hote 1 . checkAvai l abi lity(); 
```

##### The only things changing in the code are the values of the hot e 1 object's properties:
* The name of the hotel
* How many rooms it has
* How many rooms are booked

##### The rest of the page works in exactly the same way. The name is shown using the same code. The checkAvai 1 abi l ity() method has not changed and is called in the same way.

##### If this site had 1,000 hotels, the only thing that would need to change would be the three properties of this object. Because we created a model for the hotel using data, the same code can access and display the details for any hotel that follows the same data model. 

_________________________________________________________________________________________________________________________________________

------------------------------------------------------------------------


## Document object model 

##### Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

#### The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas: 
##### MAKING A MODEL OF THE HTML PAGE When the browser loads a web page, it creates a model of the page in memory.
##### The DOM specifies the way in which the browser should structure this model using a DOM tree.
##### The DOM is called an object model because the model (the DOM tree) is made of objects.
##### Each object represents a different part of the page loaded in the browser window

### ACCESSING AND CHANGING THE HTML PAGE
##### The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.
##### You will hear people call the DOM an Application Programming Interface (API). User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other. The DOM states what your script can "ask the browser about the current page, and how to tell the browser to update what is being shown to the user.

#### THE DOCUMENT NODE
##### Above, you can see the HTML code for a shopping list, and on the right hand page is its DOM tree. Every element, attribute, and piece of text in the HTML is represented by its own DOM node. At the top of the tree a document node is added; it represents the entire page (and also corresponds to the document object, which you first met on p36). When you access any element, attribute, or text node, you navigate to it via the document node. It is the starting point for all visits to the DOM tree. 

ELEMENT NODES
HTML elements describe the structure of an HTML
page. (The <h l > - <h6> elements describe what
parts are headings; the <p> tags indicate where
paragraphs of text start and finish; and so on.)
To access the DOM tree, you start by looking for
elements. Once you find the element you want, then
you can access its text and attribute nodes if you
want to. This is why you start by learning methods
that allow you to access element nodes, before
learning to access and alter text or attributes.