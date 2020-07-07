  tag                         |     dissction 
 -------------------          |      --------------------
 <li>                         |     there is 2 type of list <ul><ol>Each item in the list is placed between an
                              |     opening <li> tag and a closing </li> tag. (The li stands for list item.)
 <text>                       |     
                              |
 <dl>                         |   The definition list is created with the <dl> element and usually consists of
                              |    series of terms and their defintion                       |     




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
  







