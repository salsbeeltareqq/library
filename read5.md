## Read: 05 - HTML Images; CSS Color & Text

### HTML Images:
 - this is the tag for adding images to pages:




 ```
 <img src="images/quokka.jpg" alt="A family of
 quokka" title="The quokka is an Australian
 marsupial that is similar in size to the
 domestic cat." />
 ```

- Figure and Figure Caption : use it to add photo and caption for it:
/



```
<figure>
<img src="images/otters.jpg" alt="Photograph of
 two sea otters floating in water">
<br />
 <figcaption>Sea otters hold hands when they
 sleep so they don't drift away from each
 other.</figcaption>
</figure>
```
- Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.


### Colors in CSS:

- **change color by name** ``` h1 {color: DarkCyan;}```
- **change hex by code** ```h2 {color: #ee3e80;}```
- **change rgb by value** ```p {color: rgb(100,100,90);}```


### Notes on Color in CSS:
1. Color not only brings your site to life, but also helps convey the mood and evokes reactions.
2. There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
3. Color pickers can help you find the color you want.
4. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
5. CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
6. CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


### Text in css:
- font-family
- font-size
- @font-face
- font-weight
- font-style
- text-transform
- text-decoration
- line-height
- letter-spacing, word-spacing 
- text-align
- vertical-align
- text-indent
- text-shadow
- :first-letter, :first-line
- :link, :visited
- Responding to Users :hover, :active, :focus

- 
- # Chapter 5: “Images” (pp.94-125):

A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.

A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.


image tag:
```<img src="images/quokka.jpg" alt="A family of```
```quokka" title="The quokka is an Australian```
```marsupial that is similar in size to the```
```domestic cat." />```


The text used in the alt attribute
is often referred to as alt text.
It should give an accurate
description of the image content
so it can be understood by
screen reader software (used by
people with visual impairments)
and search engines.


Images often come with
captions. HTML5 has introduced
a new ```<figure>``` element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the ```<figure>```
element as long as they all share
the same caption.




# Chapter 11: “Color” (pp.246-263):


you can specify colors in CSS !!



 You can specify any
color in CSS in one of three ways:


1. rgb values

These express colors in terms
of how much red, green and
blue are used to make it up. For
example: 
 rgb(100,100,90)


2. hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80


3. color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan


CSS 3: Opacity opacity, rgba


hsl, hsla : 
hue
This is expressed as an angle
(between 0 and 360 degrees).
saturation
This is expressed as a
percentage.
lightness
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.


# Chapter 12: “Text” (pp.264-299):

you can specify the **style** of the **text** (Normal , *Italic* or *Oblique* ).
or weight : light , medium , **bold** or **Black**
or strech :Condensed ,Regular or Extended.
or font-type : sans serif ...etc
and of course , font-size!

or
**uppercase**
This causes the text to appear
uppercase.
**lowercase**
this causes the text to appear
lowercase.
**capitalize**
This causes the first letter of
each word to appear capitalized.

The text-decoration property
allows you to specify the
following values:
**none**
This removes any decoration
already applied to the text.
**underline**
This adds a line underneath the
text.
**overline**
This adds a line over the top of
the text.
**line-through**
This adds a line through words.
**blink**
This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying).


**text-align**
 this allows you to align text to right ,left or center
 
 
 *justify*
This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.


**vertical-align**
baseline
sub
super
top
text-top
middle
bottom
text-bottom




**text-shadow:**
```text-shadow: 1px 1px 0px #000000;```


**styling links:**
When pseudo-classes are
used, they should appear in this
order: :link, :visited, :hover,
:focus, :active.



the end


