
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



the list
order list (Links to an external site.)
<ol> The ordered list is created with the <ol>element. <li> Each item in the list is placed between an opening <li> tag and a closing </li> tag. (The li stands for list item.)

unorder list (Links to an external site.)
<ul> The unordered list is created with the <ul> element. <li> Each item in the list is placed between an opening <li> tag and a closing </li> tag. (The li stands for list item.) Browsers indent lists by default.

defition list (Links to an external site.)
<dl> The definition list is created with the <dl> element and usually consists of a series of terms and their definitions. Inside the <dl> element you will usually see pairs of <dt>`and <dd>elements. <dt> This is used to contain the term being defined (the definition term). <dd>`` This is used to contain the definition. Sometimes you might see a list where there are two terms used for the same definition or two different definitions for the same

Nested Lists (Links to an external site.)
You can put a second list inside an <li> element to create a sublist or nested list. <ul> <li>Mousses</li> <li>Pastries <ul> <li>Croissant</li> <li>Mille-feuille</li> <li>Palmier</li> <li>Profiterole</li> </ul> </li> <li>Tarts</li> </ul>

The CSS Box Model
All HTML elements can be considered as boxes. In CSS, the term “box model” is used when talking about design and layout.

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:



Content - The content of the box, where text and images appear Padding - Clears an area around the content. The padding is transparent Margin - Clears an area outside the border. The margin is transparent

boxes height and width (Links to an external site.)
The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size. p { height: 75%; width: 75%; background-color: #0088dd;}

Limiting Widt hmin-width, max-width the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide. td.description { min-width: 450px; max-width: 650px; text-align: left; padding: 5px; margin: 0px;}

overflow (Links to an external site.)
hidden This property simply hides any extra content that does not fit in the box. scroll This property adds a scrollbar to the box so that users can scroll to see the missing content. p.one { overflow: hidden} p.two { overflow: scroll;}

the border The CSS border properties allow you to specify the style, width, and color of an element’s border. The border-style property specifies what kind of border to display.

The following values are allowed:

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
The border-style property can have from one to four values (for the top border, right border, bottom border, and the left border). -p.dotted {border-style: dotted;} p.dashed {border-style: dashed;} p.solid {border-style: solid;} p.double {border-style: double;} p.groove {border-style: groove;} p.ridge {border-style: ridge;} p.inset {border-style: inset;} p.outset {border-style: outset;} p.none {border-style: none;} p.hidden {border-style: hidden;} p.mix {border-style: dotted dashed solid double;}
border color (Links to an external site.)
You can specify the color of a border using either RGB values, hex codes or CSS color names border-top-color border-bottom-color border-left-color 

Shorthand Property (Links to an external site.)
to shorten the code, it is also possible to specify all the individual border properties in one property.

The border property is a shorthand property : p { width: 250px; border: 3px dotted #0088dd;} 

padding (Links to an external site.)
The padding property allows you to specify how much space should appear between the content of an element and its border. padding: 50px;

margin (Links to an external site.)
The margin property controls the gap between boxes. Its value is commonly given in pixels, although you may also use percentages or ems. margin: 20px;

Change Inline/Block (Links to an external site.)
The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can take are: inline This causes a block-level element to act like an inline element. block This causes an inline element to act like a block-level element. inline-block This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

hiddin box (Links to an external site.)
The visibility property allows you to hide boxes from users but It leaves a space where the element would have been. This property can take two values: hidden This hides the element. visible This shows the element. If the visibility of an element is set to hidden, a blank space will appear in its place. li { display: inline; margin-right: 10px;} li.coming-soon { visibility: hidden;}

border-image (Links to an external site.)
This property requires three pieces of information: 1: The URL of the image 2: Where to slice the image 3: What to do with the straight edges; the possible values are: stretch stretches the image repeat repeats the image round like repeat. 

## box shadow The box-shadow property allows you to add a drop shadow around a box. It works just like the text-shadow property that you met on page 288. It must use at least the first of these two values as well as a color: Horizontal offset Negative values position the shadow to the left of the box. Vertical offset Negative values position the shadow to the top of the box. Blur distance If omitted, the shadow is a solid line like a border. Sp read of shad ow If used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract. 

## border-radius CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels. border-radius: 10px; -moz-border-radius: 10px; -webkit-border-radius: 10px;} 


