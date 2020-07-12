# Domain Modeling:
Domain Modeling
Domain modeling: is the process of creating a conceptual model in code for a specific problem. A model: describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity: stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

Tips:

When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
Model its attributes with a constructor function that defines and initializes properties.
Model its behaviors with small methods that focus on doing one job well.
Create instances using the new keyword followed by a call to a constructor function.
Store the newly created object in a variable so you can access its properties and methods from outside.
Use the this variable within methods so you can access the object's properties and methods from inside.


# Chapter 6: “Tables” (pp.126-145):
Table : represnts information in a grid format. Examples of tables include financial reports , TV schedules, and sports results.

Basic table structure: <table>, <tr>, <td>, <th>
Long tables: <thead>, <tbody>, <tfoot>.
JS Book:
# Chapter 3: “Functions, Methods, and Objects” (pp.106-144):
Built in objects: Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

The first thing you need to do is get to know what tools are available. You can imagine that your new toolkit has three compartments:

BROWSER OBJECT MODEL.
DOCUMENT OBJECT MODEL.
GLOBAL JAVASCRIPT OBJECTS.
The window object: The window object represents the current browser window or tab. It is the topmost object in the Browser Object Model, and it contains other objects that tell you about the browser.

THE DOCUMENT OBJECT: The topmost object in the Document Object Model (or DOM) is the document object. It represents the web page loaded into the current browser window or tab. You meet its child objects in Chapter 5.

In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).