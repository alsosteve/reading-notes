# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 201

# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions

## HTML & CSS

### Chapter 2: Text (p. 40-61)

When you make a web page, use mark-up tags to emphasize sertaint content within the text. **_Structural Markup_** is used to describe headings and pharagraphs. **_Semantic Markuo_** is used to provide extra emphasisin a sentance.

#### Headings 
HTML has 6 levels of headings. The **<h1>** tag is ised for main headings. **<h2>** is used for subheadings. The rest are used to further divide sections of your web page as you see fit.

#### Paragraphs
Pharagraphs are identified with the **<p>** tag. New paragraphs automatically start on a new line with some spacing inbetween it and the last paragraph.

#### Emphasis
**_Bold_** elements are found in the **<b>** tag.
**_Italics_** are inserted with the **<i>** tag.
The **_Strong_** element tag is **<stronh>** it indicates a strong importance in text.
the **<em>** tag creates **_emphasis_** in a sentance that subtly changes its meaning.

#### Superscript & Subscript
The **<sup>** element creates superscript.
The **<sub>** element creates a subscript.

#### White Space
Programmers use extra spaces and page breaks to make the code easy to read. HTML ignores the extra spaces and counts them as one space, also known as **White Space Collapsing**.

#### Line Breaks & Horizontal Rules
Use the **<br />** tag to add a line break in the middle of a paragraph.
the **<hr />** tag inserts a horizontal rule in the page.

#### Quotes & References
**_Blockquotes_**- the **<blockquote>** tag is used to highlight quotes longer than a pharagraph. They are also usually indented.
**_Quotes_**- the **<q>** tag is used for smaller quotes that sit within a pharagraph.
**_Citations_**- use **<cite>** tag to indicate where a citation is from.

### Chapter 10: Ch.10 Introducing CSS (p. 226-245)


CSS works by changing the way elements within certaint tags look in HTML.
For more information on designing with CSS see previous notes: [Reading-Notes-102: Design web pages with CSS](https://alsosteve.github.io/reading-notes/designwithcss)

## JavaScript & JQuery

### Chapter 2: Basic JavaScript Instructions (p. 53-84)

A **_Script_** is a set of instructions that the programm follows to complete a task. Each individual action or step is know as a **_statement_**. 

#### Comments
Comments in code are writen by developers to explain what the code does. You can add a comment by using the "//" in the beginning of a line before you start typing. Multyple line comments are contained within: */ Comments go here /*

#### Variables
A **_variable_** is where information in code is stored. Variables have 6 rules for naming them:
1. The name needs to start with a letter, dollar sign, or underscore. No numbers!
2. The rest can contain the characters allowed in the first rule in any order, but can include numbers now. No dashes or periods.
3. No keyword or reserved words
4. Variables are case sensitive
5. Use a name that describes the information
6. For multi word variables: no spaces, first word lowercase, second word uppercase

#### Data Types
There are 3 data types:
1. Numeric Data - numbers
2. String Data  - text
3. Boolean Data - true or false

#### Array
An **_Array_** stores a list of variables. Items listed within an array start with the number 0, not 1.

### Chapter 4: Decisions and Loops (p. 145-162)


#### Comparison operators
a == b 'loose equality' 10 == '10' Value must be the same but type can be different 

a === b 'strict eqaulity' both the type and the value have to be the same 10 === 10

a != b 'inequality' 10 != '10' (this is false)

a !== b 'strict inquality' 10 !== '10' (this is true)

a > b 'greater than' 

a < b 'less than'

a >= b 'greater than or equal to'

a <= b 'less than or equal to'


#### logical operators
a && b "and"

a || b "or"

!a "not a" - bang/ opposite day


See previous notes about this topic here: [Reading-Notes-102: Operators and Loops](https://alsosteve.github.io/reading-notes/opsandloops)