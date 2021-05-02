# HTML
## tables 
##### A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.
### Basic Table Structure

`<table>`
##### The `<table>` element is used to create a table. The contents of the table are written out row by row.
`<tr>`
##### You indicate the start of each row using the opening <tr> tag. (The tr stands for table row.) It is followed by one or more
`<td>` 
##### elements (one for each cell in that row). At the end of the row you use a closing `</tr>` tag. `<td>` Each cell of a table is represented using a `<td>` element. (The td stands for table data.)At the end of each cell you use a closing `</td>` tag.

```
<table>
 <tr>
 <td>15</td>
 <td>15</td>
 <td>30</td>
 </tr>
 <tr>
 <td>45</td>
 <td>60</td>
 <td>45</td>
 </tr>
 <tr>
 <td>60</td>
 <td>90</td>
 <td>90</td>
 </tr>
</table>
```

### Long Tables
##### There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).
##### These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table (as you will see when you learn about CSS).

#### `<thead>`
##### The headings of the table should sit inside the `<thead>` element.
#### `<tbody>`
##### The body should sit inside the `<tbody>` element.
#### `<tfoot>`
##### The footer belongs inside the `<tfoot>` element

```
<table>
 <thead>
 <tr>
 <th>Date</th>
 <th>Income</th>
 <th>Expenditure</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <th>1st January</th>
 <td>250</td>
 <td>36</td>
 </tr>
 <tr>
 <th>2nd January</th>
 <td>285</td>
 <td>48</td>
 </tr>
 <!-- additional rows as above -->
 <tr>
 <th>31st January</th>
 <td>129</td>
 <td>64</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td></td>
 <td>7824</td>
 <td>1241</td>
 </tr>
 </tfoot>
</table>
```

__________________________________________________________________
-------------------------------------------------------------------

# Javascript

### CREATING OBJECTS USING CONSTRUCTOR SYNTAX 

##### On the right, an empty object called hote 1 is created using the constructor function. Once it has been created, three properties and a method are then assigned to the object.

##### (If the object already had any of these properties, this would overwrite the values in those properties.)

##### To access a property of this object, you can use dot notation, just as you can with any object. For example, to get the hotel's name you could use: hotel .name

##### Similarly, to use the method, you can use the object name followed by the method name: hotel.checkAvailability() 

``` 
var hotel = new Object();
hotel.name= 'Park';
hotel.rooms = 120;
hotel .booked = 77;
hotel .checkAvailability = function()
return this.rooms - this.booked;
} ;
JAVASCRIPT
var elName = document.getElementByid('hotelName');
elName.textContent = hotel . name;
var elRooms = document .getElementByid('rooms');
elRooms.textContent = hotel .checkAvailability(}; 
```
### ADDING AND REMOVING PROPERTIES 
##### Once you have created an object (using literal or constructor notation), you can add new properties to it.
##### In this example, you can see that an instance of the hotel object is created using an object literal.

##### Immediately after this, the hotel object is given two extra properties that show the facilities (whether or not it has a gym and/or a pool). These properties are given values that are Booleans (true or false).

##### Having added these properties to the object, you can access them just like any of the objects other properties. Here, they update the value of the class attribute on their respective elements to show either a check mark or a cross mark.

##### To delete a property, you use the keyword delete, and then use dot notation to identify the property or method you want to remove from the object. In this case, the booked property is removed from the object. 

```
Javascript

var hotel = {
name : 'Park' ,
rooms : 120,
booked : 77.
} ;
hotel .gym = t rue;
hotel .pool = fal se;
delete hotel .booked;
var elName = document .getEl ementByld('hotelName ');
elName.textContent = hotel . name;
var el Pool = document .getElementByid ('pool ') ;
elPool.cl assName = ' Pool: ' + hotel. pool ;
var elGym = document .getEl ementByld('gym' };
elGym.className = 'Gym: ' + hotel .gym; 
```
#### References : this reading note info taken from javascript_and_jquery_interactive BOOK.