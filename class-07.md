# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 201

# Read: 07 - HTML Tables; JS Constructor Functions

## [Domain Modeling Article](https://github.com/codefellows/domain_modeling#domain-modeling)

**_Domain Modeling_** is when you make a concept model in code for a specific problem. 
* **Object Oriented Model**- an entity that stores data in properties and encapsulates behaviors in methods

## [HTML & CSS]

### Chapter 6: Tables (p. 126-145)
**_Tables_** are a way to display information in a grid format. They allow for easy identification and reading of complex data.
**_Table cells_** are the individual blocks in a table. 

#### Basics
``` javaScript
<table>
  <tr>
    <td>15</td>
    <td>15</td>
    <td>30</td>
  </tr>
  <tr>
    <td>45</td>
    <td>60</td>
    <td>45</td>
  </tr>
  <tr>
    <td>60</td>
    <td>90</td>
    <td>90</td>
  </tr>
</table>
```

The **_table_** element is used to create the table. You then to proceed to write out inforation on the table row by row.
Each row begins with the **_tr_** tag, this stands for table row.
The **_td_** tag is used to create a **_table data_** element. This is each individual cell of the table.

#### Extra
``` javaScript
<table>
  <tr>
    <th></th>
    <th colspan="2"> Extended column</th>
  </tr>
  <tr>
    <td>45</td>
    <td>60</td>
    <td rowspan="2">45</td>
  </tr>
  <tr>
    <td>60</td>
    <td>90</td>
  </tr>
</table>
```
- **_Table Headings_** are contained within the **_<th>_** element tags and are used for table headings. Don't forget tho include an empty _th_ tag for spacing purposes.
- **_Spanning Columns_** are used to create a table heading or table data element that spans more than one column cell.
- **_Spanning Rows_** work similar to sanninng columns but extend the cell vertically

#### Long Tables

- **_thead_** - This should contain the table headings.
- **_tbody_** - This is where the body of the table should be placed.
- **_tfoot_** - This is where the table footer goes.

## [JavaScript & JQuery]

### Chapter 3: Functions, Methods, and Objects (p. 106-144 ONLY)

