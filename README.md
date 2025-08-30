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

- Used to control the 4 cornersز
  
  
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
