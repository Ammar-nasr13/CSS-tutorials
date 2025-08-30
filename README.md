## what is CSS ? 
- Used to design Html and Xml elements .
- CSS stands for Cascading Style Sheet .

  | `Cascading` | `Style` | `Sheet`  |
  |:--------:|:-----:|:-----------:|
  | `It means that if we have more than one property applied to the element, the choice is left to the browser.`   | `Formats applied to CSS files`  | `Css Files`    |

 ➡️ **The browser chooses which property to apply to the element based on:**
 - **Source code** => mean use ( **inline style** - **internal style** - **external style**)
 - **Specficity** => Each element has a priority order.
 - **Order** => mean Arranging elements on a web page
 ---  
## what are version of CSS ?

- **CSS1** ➡️ The formats have been separated from the html file and placed in a separate file.
- **CSS2** ➡️ Many features have been added such as lines, shadows, etc.
- **CSS3** ➡️ Many features have been added such as responsive design using media query and printing .


---
## what are benefits of CSS ?
- Time Saving
- Easy to Modify
- Fast Loading
- W3C Standared
- Customize Printing
- Responsine Design
---
## what are Styles of CSS ?
- inline style
- internal style
- external style
- **Notes** ➡️ inline styles is the stronger style.

  ---
  
## what are comments in CSS ?
   ➡️ *used to explain certian code or leave notes*.
  - single line comment => //
  - multi line comment => /* */

    ---

## what are rules of write CSS code ?
 
   - **selector**  => ways to select element of HTML .
   - **{}**  => block of CSS code
   - **property : value ;**
 
- **Notes ➡️  property : value ; called declration**




     ```css
    selector {

    property : value ;

    }


     ---
## what are selector of CSS ?

- **Simple Selector**
- **Combinator Selector**
- **Pseudo Class Selector**
- **Pseudo Elemnts Selector**
- **Atrributs Selector**

----
1- **Simple Selector**
- Name Tag => Example : h1{}
- (*)  => select all .. of html.
- Comma => select all element with same properties.
- id => give element id property and identifiers then call this elements by #
- class => give element class property and idntifiers then call this elements by .

**Notes** ➡️ *identifiers*

- start with letter only. ( a to z - A to Z)
- don't start with number or symbols. ( 1,2,3 .... , @ ,# , _ ....)
- don't start with underscore.
- styles => case type => kabab case

**Case types**

- String (lower case) = word word 
Example : prodect id
- String (upper case) = WORD WORD
 ➡️ Example : PRODECT ID

- Pascal Case = WordWord
 ➡️ Example : ProdectId

- Camel Case = WordWORD
➡️ Example : prodectId

- Kabab Case (lower case) = word-word
➡️ Example : prodect-id

- Kabab Case (Upper case) = WORD-WORD
➡️ Example : PRODECT-ID

- Snake Case (lower case) = word_word
➡️ Example : prodect_id

- Snake Case (Upper case) = word_word
➡️ Example : PRODECT_ID

**Diffrence between Class - Id**

- you can give class and id property many identifiers and shouid put space between them and call class by any identifiers.
- you can give many elements same identifiers in class property.
- you can't give many elements same identifiers in Id property. so any element shouid have unique id.


2- **Combinator Selector**

- descendant selector = space  ➡️ select all children. 
- child selector (>)  ➡️ select direct children.
- adjacent sibling selector (+)  ➡️ select direct sibling (brother)
- general sibling selector (~)   ➡️ select all sebling (brother)


3- **Pseudo Class Selector** <br>

  - ➡️ It means adding formats to the element in a specific state and this state is set using pseudo class.
  - these class talk about => ( link - list - inputs - some class about general elements )

    
 | Pseudo-class          | Description                                                                 | Example                             |
|-----------------------|-----------------------------------------------------------------------------|-------------------------------------|
| `:link`               | Unvisited links                                                            | `a:link { color: blue; }`           |
| `:visited`            | Visited links                                                              | `a:visited { color: purple; }`      |
| `:hover`              | When the user hovers over an element                                        | `button:hover { color: red; }`      |
| `:active`             | Active element (e.g., while clicking)                                      | `a:active { color: green; }`        |
| `:focus`              | Element in focus                                                           | `input:focus { border: 2px solid; }`|
| `:first-child`        | First child of its parent                                                  | `p:first-child { color: red; }`     |
| `:last-child`         | Last child of its parent                                                   | `p:last-child { color: blue; }`     |
| `:nth-child(n)`       | Nth child of its parent                                                    | `li:nth-child(2)`                   |
| `:nth-last-child(n)`  | Nth child counting from the end                                            | `li:nth-last-child(1)`              |
| `:only-child`         | Element that is the only child                                             | `p:only-child { color: red; }`      |
| `:first-of-type`      | First element of its type                                                  | `p:first-of-type { color: red; }`   |
| `:last-of-type`       | Last element of its type                                                   | `p:last-of-type { color: red; }`    |
| `:nth-of-type(n)`     | Nth element of its type                                                    | `p:nth-of-type(2)`                  |
| `:nth-last-of-type(n)`| Nth element of its type counting from the end                              | `p:nth-last-of-type(1)`             |
| `:only-of-type`       | Element that is the only one of its type                                   | `p:only-of-type { color: red; }`    |
| `:empty`              | Elements with no children                                                  | `div:empty { display: none; }`      |
| `:not(selector)`      | Elements not matching selector                                             | `p:not(.intro)`                     |
| `:checked`            | Checked inputs (checkbox/radio)                                            | `input:checked`                     |
| `:disabled`           | Disabled form elements                                                     | `input:disabled`                    |
| `:enabled`            | Enabled form elements                                                      | `input:enabled`                     |
| `:required`           | Inputs with `required`                                                     | `input:required`                    |
| `:optional`           | Inputs without `required`                                                  | `input:optional`                    |
| `:valid`              | Form elements with valid value                                             | `input:valid`                       |
| `:invalid`            | Form elements with invalid value                                           | `input:invalid`                     |
| `:in-range`           | Inputs within a specified range                                            | `input:in-range`                    |
| `:out-of-range`       | Inputs outside a specified range                                           | `input:out-of-range`                |
| `:read-only`          | Elements with `readonly`                                                   | `input:read-only`                   |
| `:read-write`         | Editable elements                                                          | `input:read-write`                  |
| `:target`             | Element targeted by a URL fragment (`#id`)                                 | `#section:target`                   |
| `:root`               | Root element (`html`)                                                      | `:root { --main: red; }`            |
| `:lang(lang)`         | Elements with specific language                                            | `p:lang(en)`                        |
| `:scope`              | Reference point element in query selector                                  | `:scope > p`                        |
| `:is()`               | Matches any selector in a list                                             | `p:is(.intro, .main)`               |
| `:where()`            | Same as `:is()` but zero specificity                                       | `p:where(.intro, .main)`            |
| `:has()`              | Matches elements that contain selector inside                             | `div:has(p)`                        |
| `:any-link`           | Matches both `:link` and `:visited`                                       | `a:any-link`                        |
| `:autofill`           | Inputs that are autofilled by the browser                                 | `input:autofill`                    |
| `:placeholder-shown`  | Inputs showing placeholder text                                            | `input:placeholder-shown`           |
| `:fullscreen`         | Element currently displayed fullscreen                                     | `video:fullscreen`                  |



4- **Pseudo Elemnts Selector**

| Pseudo-element   | Description                                               | Example                             |
|------------------|-----------------------------------------------------------|-------------------------------------|
| `::before`       | Inserts generated content before an element’s content     | `p::before { content: "Note: "; }`  |
| `::after`        | Inserts generated content after an element’s content      | `p::after { content: " ✔"; }`       |
| `::first-line`   | Styles the first line of a block                          | `p::first-line { color: blue; }`    |
| `::first-letter` | Styles the first letter of a block                        | `p::first-letter { font-size: 2em; }` |
| `::selection`    | Styles the part of an element selected by the user        | `p::selection { background: yellow; }` |
| `::placeholder`  | Styles placeholder text of an input                       | `input::placeholder { color: gray; }` |
| `::marker`       | Styles the marker (bullet/number) of list items           | `li::marker { color: red; }`        |
| `::file-selector-button` | Styles the file upload button in input type="file"| `input::file-selector-button { color: green; }` |
| `::cue`          | Styles WebVTT captions/subtitles in media elements        | `video::cue { color: white; }`      |
| `::backdrop`     | Styles the backdrop of fullscreen or modal elements       | `dialog::backdrop { background: rgba(0,0,0,0.5); }` |
| `::part(name)`   | Styles a part of a shadow DOM component                   | `my-element::part(header)`          |
| `::slotted()`    | Styles slotted elements in shadow DOM                     | `slot::slotted(span)`               |


5- **Atrributs Selector**


| Selector            | Description                                                                 | Example                               |
|---------------------|-----------------------------------------------------------------------------|---------------------------------------|
| `[attr]`                | Selects elements with the given attribute                                   | `input[required] { border: red; }`    |
| `[attr="value"]`        | Selects elements with the attribute exactly equal to "value"                | `a[target="_blank"]`                  |
| `[attr~="value"]`       | Selects elements where the attribute value contains the word "value"        | `[title~="flower"]`                   |
|  [attr|="value"]          | Selects elements where the attribute value is exactly "value" OR starts with "value-" | `[lang|="en"]`            |
| `[attr^="value"]`            | Selects elements where the attribute value **starts with** "value"          | `a[href^="https"]`                    |
| `[attr$="value"]`           | Selects elements where the attribute value **ends with** "value"            | `a[href$=".pdf"]`                     |
| `[attr*="value"]`           | Selects elements where the attribute value **contains** "value"             | `a[href*="google"]`                   |
| `[attr operator value i]`   | Case-insensitive attribute selector (add `i` at the end)               | `a[href$=".PDF" i]`                   |
| `[attr operator value s]`   | Case-sensitive attribute selector (add `s` at the end, default in some cases) | `[type="Text" s]`              |


----

## important keyword (global keyword)

- ➡️ important keyword is keyword use to value of all elements in css .
  
- initial => this value return element to intial value => بترجع الخاصية للقيمة الافتراضية اللي مطورين اللغة وضعوها  .
- inherit => this value inherit element value from parent.
- unset => inhert - initial =>  If the property is inherited, it works as an inheritance property, and if the property is not inherited, it works as a initial        property.
- revert => this value return element to intial value.=> اللي المتصفح عاطيها للخاصية
-  **Notes** ➡️ all this value can used in property all to implement this property all properties of element.


## what are inheritance in CSS ?

- Mean children inhert parent some properties such as fontsize - fontweitgh - fontfimaly - width - color - .....
- Elements which inside another elements call childern.


## what are box model ?
- any element exist in page have box model.
- box model are (content - padding - margin - border - outline)

➡️ **padding**

- used to padding which sperated between content - border.
- padding-left
- padding-top
- padding-right
- padding-bottom
- shorthand property => padding => accept 4 value .( padding-left - padding-top - padding-right - padding-bottom )<br><br>
 ➡️*Notes*
- padding-block-start => used to padding vertically ( y ) => top
- padding-block-end =>  used to padding vertically ( y ) => bottom
- shorthand property => padding-block => accept 2 value .
- padding-inline-start => used to padding horizontally (x ) => left
- padding-inline-end =>  used to padding horizontally ( x ) => right
- shorthand property => padding-inline => accept 2 value .<br><br>
 ➡️*Notes* <br>
 - **what differance between padding , padding-block , padding-inline**.
 - When using padding-block or padding-inline, this makes it flexible because it changes when you change the direction of the page writing, unlike padding, which requires manual adjustment.

➡️ **border**

- used to sperated between padding -margin.
- border-style => ( solid - dotted - groove - double )
- border-width => units
- border-color => color
- shorthand property => border => accept 3 value. work in 4 direction
- if you used border in specific direction use ↩️<br>

*left*

- border-left-style
- border-left-width
- border-left-color
- shorthand property => border-left => accept 3 value. <br>

*top*

- border-top-style
- border-top-width
- border-top-color
- shorthand property => border-top => accept 3 value. <br>

*right*

- border-right-style
- border-right-width
- border-right-color
- shorthand property => border-right => accept 3 value. <br>

*bottom*

- border-bottom-style
- border-bottom-width
- border-bottom-color
- shorthand property => border-bottom => accept 3 value. <br>


*border-raduis*

- Used to control the 4 corners.
- border-raduis-top-left
- border-raduis-top-right
- border-raduis-bottom-right
- border-raduis-bottom-left
- shorthand property => border-raduis <br>

*border-image*

- border-image-source=> url(path of image);
- border-image-width => width of image in border
- border-image-slice => It is used to cut the image from 4 directions. accept 4 value.
- border-image-outset => Used to move the image out of the element. accept units.
- border-image-repeat => Specifies how to duplicate or extend the side portions of the image. accept this value => ( stretch - repeat - round - space)
- shorthand property => border-image=> accept 5 value => ( source - width - slice - outset - repeat )
  
  
➡️**margin**

- used to margin which sperated between element - another element.
- margin-left
- margin-top
- margin-right
- margin-bottom
- shorthand property => margin => accept 4 value .( margin-left - margin-top - margin-right - margin-bottom )<br><br>
 ➡️*Notes* <br>
- margin-block-start => used to margin vertically ( y ) => top
- margin-block-end =>  used to margin vertically ( y ) => bottom
- shorthand property => margin-block => accept 2 value .
- margin-inline-start => used to margin horizontally (x ) => left
- margin-inline-end =>  used to margin horizontally ( x ) => right
- shorthand property => margin-inline => accept 2 value . <br>

➡️*Notes* <br>

- concept => margin collapse => mean if you give element margin-bottom = 50 and you give another element margin-top = 30 => total margin between them = 50 .
- if you want to put element in the middel on the page you can use => margin = auto;
- margin accept negative value.

➡️ **outline**

- work in only 4 direction.
- ouline-style
- outline-width
- outline-color
- shorthand property => outline => accept 3 value.
- outline-offset => Used to create spacing between the outline and the element itself.

## block - inline - inlineblock - ( width - height - function - margin )

 ➡️ **block**  <br>

*width*

- Default width => 100% parent.
- width => respect => you can give block element width => px - %  <br>

*height*

- Default height => fit content
- height => respect => you can give block element height => px - %
- **Note** => if you give block element height with % you have problem. to solve this problem you must be give parent element height.<br>

*new line*

- block elements respect new line.<br>


*margin*

- block elements respect margin from all direction.<br>


➡️ **inline**  <br>

*width*

- Default width => fit content.
- width => don't respect => you can't give inline element width  <br>

*height*

- Default height => fit content
- height => don't respect => you can't give inline element height.
<br>

*new line*

- inline elements don't respect new line.<br>


*margin*

- inline elements respect margin  only from left and right direction.<br>


➡️ **inline-block**  <br>

*width*

- Default width => fit content.
- width => respect => you can give inline-block element width  <br>

*height*

- Default height => fit content
- height =>  respect => you can give inline-block element height.
<br>

*new line*

- inline-block elements respect new line.<br>


*margin*

- inline-block elements respect margin from all direction.<br>

➡️ **Notes**  <br>

*width*

- min-width property => Specifies the minimum width that can be reached. max-width => open
- max-width property => Specifies the maximum width that can be reached. min-width => open
- There are a set of values ​​that are used  with the width. ( min-content - max-contenet - fit-content )

<br>

*height*

- min-height property => Specifies the minimum height that can be reached. max-height => open
- max-height property => Specifies the maximum height that can be reached. min-height => open

**Function**

- calc() => هي تقبل قيمتين ويتم عمل عليهم عمليات حسابية لاخذ القيمة المناسبة
- min()  => هل تقبل قيمتين ويتم اخذ القيمة الاصغر المناسبة للشاشة
- max() => هي تقبل قيمتين ويتم اخذ القيمة الاكبر المناسبة للشاشة
- clamp() => هي تقبل ثلاثه قيم القيمة الاولي هي تحدد الحد الادني والقيمة الثانية هي تحدد القيمة المفضلة والقيمة الثالثة هي تحدد الحد الاقصي

**Units**

- Units divided into ( absolute units - relative units )  <br>

*absolute units*

- there are many absolute units but important absolute units is px.  <br>



*relative units*

- They are units that are calculated relative to the parent.  <br>


*Especially font size*

- rem => Its value is calculated relative to root element.
- em - % => Its value is calculated relative to parent. <br>

*Especially width - height*

- 1vm = 1% form width screen  => Its value is calculated relative to the screen.
- 1vh = 1% form height screen  => Its value is calculated relative to the screen.
- fr	A fractional unit. 1fr equals 1 part of the available space.


## Color in CSS.

- color property used to text. <br>

*value of color*

- color Name => 140 color name.
- A hexadecimal color is specified with: #RGB or #RRGGBB. => 0-9 or A-Z.
- RGB(R , G , B) => 0 - 255
- RGBA(R - G - B - alpha) => alpha => هي تعني الشفافية وقيمتها تتراوح من صفر الي واحد وكلما اقتربنا للصفر كلما كان العنصر اكثر شفافية
- hsl(hue, saturation, lightness)
- Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.
- Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color.
- Lightness is also a percentage. 0% is black, 50% is neither light or dark, 100% is white
- hsla(hue, saturation, lightness, alpha)

➡️ **color keyword**

- transparent, currentcolor, and inherit keywords.
- The transparent keyword is used to make a color transparent. This is often used to make a transparent background color for an element.
- The currentcolor keyword is like a variable that holds the current value of the color property of an element.
- The inherit keyword specifies that a property should inherit its value from its parent element.


➡️ **opacty**

- The opacity property specifies the opacity/transparency of an element.
- The opacity property can take a value from 0.0 - 1.0↩️
- 0.0 - The element will be completely transparent.
- 0.5 - The element will be 50% transparent.
- 1.0 - Default. The element will be fully opaque.


## background - gradients in CSS.

**background**

- backgroun-color => color value - color keyword
- backgroun-image => url(path)
- backgroun-repeat => default value is repeat  => repeat-x => repeat Horizontally  => repeat-y => repeat Vertically  (no-repeat)
- backgroun-position => left top - left center - left bottom - top - center center - center bottom - right top - right center - right bottom.
- background-size => The CSS background-size property allows you to specify the size of background images. <br>

*Values*

- defualt value => auto => هي تعني اظهار الصورة كما هي في الحقيقة
- width - height => Example : background-size : 100px 200px;
- cover => بتحاول انها تكون داخل العنصر باكمله فتقوم باعادة ضبط طولها وعرضها لكي يتناسب مع العنصر ولا تحافظ علي الابعاد الاساسية لها وهي الطول والعرض لان الهدف منها تغطية العنصر بالكامل  
- contain => بتحاول انها تكون داخل العنصر باكمله فتقوم باعادة ضبط طولها وعرضها لكي يتناسب مع العنصر وتحافظ علي الابعاد الاساسية لها وهي الطول والعرض واذا لم يغطي العنصر باكلمه فانها تترك فراغ حولها


- background-attatchment => scroll هي تستخدم للتحكم في صورة خلفية العنصر اثناء عمل المستخدم
- default value => scroll => في حالة كان التمرير داخل العنصر نفسه فان الصورة تظل ثابته وفي حالة تمرير الصفحة نفسها فان الصورة تتحرك مع العنصر
-  fixed => في حالة كان التمرير داخل العنصر نفسه فان الصورة تظل ثابته وفي حالة تمرير الصفحة نفسها فان الصورة تظل ايضا ثابتة مع العنصر
-  local => في حالة كان التمرير داخل العنصر نفسه فان الصورة تتحرك  وفي حالة تمرير الصفحة نفسها فان الصورة تتحرك مع العنصر
- background-origin => The CSS background-origin property specifies where the background image is positioned.
- default value => padding-box => تعني ان الصورة سوف تبدا من عند الهوامش الداخلية
- border-box => وهي تعني ان الصورة سوف تبدامن عند الحدود
- content-box => تعني ان الصورة سوف تبدا من عند الحافة الخارجية لمحتوي العنصر
- background-clip => The CSS background-clip property specifies the painting area of the background. هي تحدد اين سوف تنتهي او تقص صورة او لون خلفية العنصر
- default value => padding-box => تعني ان الصورة سوف تنتهي  عند الهوامش الداخلية
- content-box => تعني ان الصورة سوف تنتهي  عند الحافة الخارجية لمحتوي العنصر
- content-box => تعني ان الصورة سوف تنتهي من عند الحافة الخارجية لمحتوي العنصر
