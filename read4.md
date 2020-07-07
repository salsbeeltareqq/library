# Chapter 4: Ch.4 “Links” (pp.74-93):

we use ```<a>``` to adda link
everything in between the brackets will be clickable as alink.

```<a href="https://www.whatever.com">this is a link</a>```
you can either make a link to an external website  or Linking to Other Pages
on the Same Site


thisis how to link to an email ond open the user's email program:
```<a href="mailto:jon@example.org">Email Jon</a>```

```<a href="http://www.imdb.com" target="_blank"> Internet Movie Database</a> ```(opens in new window)

```<a href="#top">``` links to a place in the same page , you must give the point (h1 for example) a unique  id attribute nd put it's same value in the href in the a tag.


```<a href="http:/www.htmlandcssbookcom/#bottom">``` this is how to link to a specific point in another page otr website


 If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.


# Chapter 15: “Layout” (pp.358-404):

When you move
any element from
normal flow, boxes
can overlap. The
z-index property
allows you to control
which box appears
on top.
When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page.

position:fixed:
It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.





z-index
When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.



Fixed Width Layouts
Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.


# Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY):


how to declare a function:
```function myFunction(p1, p2) {```
  ```return p1 * p2;   // The function returns the product of p1 and p2}```
calling a function:
```hello();```


**getting mutiple values form a function:**


```function getSize (width, height, depth) {```
```var area = width * height;```
```}```
```var volume = width * height * depth;```
```var sizes= [area , volume];```
```return sizes;```
```var areaOne = getSize (3, 2, 3)[0];```
```var volumeOne = getSize (3, 2, 3)[1];```

# Article: “6 Reasons for Pair Programming”:

**What is pair programming ?**
it is the practice of two developers sharing a single workstation to interactively tackle a coding task together.


 the Driver and the Navigator :
 the driver is who writes the code 
 the navigator: The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs


 Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves. 

**Benfits of Pair programming:**
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

