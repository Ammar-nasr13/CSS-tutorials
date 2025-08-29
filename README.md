## what is CSS ? 
- Used to design Html and Xml elements .
- CSS stands for Cascading Style Sheet .

  | Cascading | Style | Sheet   |
  |:--------:|:-----:|:-----------:|
  | It means that if we have more than one property applied to the element, the choice is left to the browser.   | Formats applied to CSS files  | Css Files    |

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
**Simple Selector**
- Name Tag => Example : h1{}
- (*)  => select all .. of html.
- Comma => select all element with same properties.
- id => give element id property and identifiers then call this elements by #
- class => give element class property and idntifiers then call this elements by .

**Notes** ➡️ *identifiers*

- start with letter only. ( a to z )
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
