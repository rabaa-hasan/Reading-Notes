# Object-Oriented Programming, HTML Tables
## Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## Define a constructor and initialize properties
 Implementation of the EpicFailVideo constructor function:
```
var EpicFailVideo = function(epicRating, hasAnimals) {
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

The two newly created objects are logged to the console.

![dom](https://camo.githubusercontent.com/55928963ae0dc919186799ab35c1cd669724ddbeb0658d0ca4b9e79b38e1804e/68747470733a2f2f692e696d6775722e636f6d2f47326250456c462e706e67)

This is object-oriented programming in JavaScript at its most fundamental level:

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.

## Generate random numbers
To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a __Math.random()__ function for just this sort of occasion.

```
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));
```

## Tips for building your own domain models
1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.

# Tabels in HTML
What's a Table?

A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

Each block in the grid is referred to as a table __cell__. In HTML a table is written out row by row.

### Basic Table Structure
#### `<table>`
The `<table>` element is used to create a table.
#### `<tr>`
The tr stands for table row.
#### `<td>`
Each cell of a table is represented using a `<td> `element. (The td stands for table data.)

```
<table>
<tr>
<td>15</td>
<td>15</td>
</tr>
<tr>
<td>15</td>
<td>15</td>
</tr>
</table>
```

### Table Headings  `<th>`
The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)
### Spanning ColumnS,Spanning Rows
Sometimes you may need the entries in a table to stretch across more than one column. The colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across.

```
<tr>
<th>Tuesday</th>
<td colspan="3">Gym</td>
<td>Home Ec</td>
</tr>
```

You may also need entries in a table to stretch down across more than one row. The rowspan attribute can be used on a `<th>` or `<td> `element to indicate how many rows a cell should span down the table.
```
<tr>
<th>6pm - 7pm</th>
<td rowspan="2">Movie</td>
<td>Comedy</td>
<td>News</td>
</tr>
```

![span](https://flylib.com/books/2/631/1/html/2/images/08fig19.jpg)

### Long Tables
There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content). These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table.
```
<thead>
<tbody>
<tfoot>
```

## creating objects in javascript
![object](https://skryvets.com/blog/2018/08/01/6-ways-to-create-a-javascript-object/6-ways-to-create-a-javascript-object.png)

## updating objects in javascript
![update](https://www.codegrepper.com/codeimages/change-value-of-key-in-object-javascript.png)

## CREATING MANY OBJECTS: CONSTRUCTOR NOTATION
Sometimes you will want several objects to represent similar things.

Object constructors can use a function as a template for creating objects.

First, create the template with the object's properties and methods.

![construct](https://miro.medium.com/max/3916/1*2s2U-uXrRGFrkqYaFhBBUA.png)

## Arrays are objects javascript
![array](https://miro.medium.com/max/470/1*oNiNLXLML6i0kknHkOGArQ.png)

 The built-in objects are __Date, Math, String, Array, and Object__.


An object is a series of variables and functions thatrepresent something from the world around you.

In an object, __variables__ are known as __properties__ of the object; __functions__ are known as __methods__ of the object.




