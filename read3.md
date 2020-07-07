  tag                         |     dissction 
 -------------------          |      --------------------
 '<li>'                       |    ' there is 2 type of list <ul><ol>Each item in the list is placed between an'
                              |     'opening <li> tag and a closing </li> tag. (The li stands for list item.)'
 '<text>'                     |     
                              |
 '<dl>'                       |   'The definition list is created with the <dl> element and usually consists of'
                              |   ' series of terms and their defintion '                         




> 
 # boxes 
 
 * By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can
    use the height and width properties.1
 
 * The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.2
 
 * When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box.3

 * When you use ems, the size of the box is based on the size of text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible across devices which have different-sized screens 4

 ### ex :

   <div>
      <p>The Moog company pioneered the commercial   manufacture of modular voltage-controlled    analog synthesizer systems in the early 1950s.</p> 
      
     </div> 

 # brder width and hight "boxes"
 > 
 p.one { border-width: 2px;} p.two { border-width: thick;} p.three { border-width: 1px 4px 12px 4px;}
 <p class="one">Hohner's "Clavinet" is essentially an   electric clavichord.</p> <p class="two">Hohner's "Clavinet" is essentially an   electric clavichord.</p> <p class="three">Hohner's "Clavinet" is essentially   an electric clavichord.</p> chapter-13/border-width.html HtMl
 The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:
  thin medium thick

 You can control the individual size of borders using four separate properties:
 border-top-width border-right-width border-bottom-width border-left-width
 You can also specify different widths for the four border values in one property, like so:
 border-width: 2px 1px 1px 2px;
 The values here appear in clockwise order: top, right, bottom, left.
  BorDer WiDth 





follow up
types of lists
list type	tags
ordered	<ol> <li>item</li> </ol>
unordered	<ul> <li>item</li> </ul>
definition	<dl> <dt>term</dt> <dd>definition</dd> </dl>
Lists can be nested inside one another.

boxes
There are many properties for boxes that we can tweak to achieve the desired look for the elements on the page.

width and height you can control them by setting the desired value and choosing the suitable unit(px, in, pt and so on).
You can set limits to how wide or narrow you want the box to be using max-width and min-width
if the content is too large for the box you can set the overflow value to either hidden or scroll.
padding is the space between the content and the border.
border thickness can be changed to user liking. margin: top right bottom left; or margin :horizantal vertical;
margin is the space between the borders of two elements
margin

display property can be used to hide or show boxes, also change the boxes to inline or block or inline-block.
visibility property can also hide or show the boxes.
Switch statement
switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).

    switch(condition){
        case val1:
            //do something;
            break;
        case val2:
            //do something else;
            break;
        .
        .
        .
        default:
            //do something;
    }
It is important when writing a condition to keep on mind Truthy and Faulty expressions (expressions that may not appear to be true or false directly). ex: NaN (not a number), null, 0 and undefined are considered false

for loops
For uses a counter as a condition to run code a number of times until the condition is false.

for (initialize, condition, update){}
while loop
while (condition){}
while runs the code block until the condition is false. It does not initialize or update the loop counter (unless you write the initialization and update by yourself in the code block).

Do while
Do while loop will go through the loop once before checking the condition then continue as while loop does.


