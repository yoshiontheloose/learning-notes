# Domain Modeling
Article [https://github.com/codefellows/domain_modeling#domain-modeling]

**Domain Modeling** - Creating a conceptual model in code for a specific problem

**Object oriented model** - entity that stores data in properties and summarizes behaviors in methods

Use constructor function to derfine the same properties between many objects.
Constructor function is defined with a _function expression_


_Duckett HTML book_
# Chapter 6: Tables (p126-142)

## Basic Table Structure  
`<table>` - element to create table  
`<tr>` - element to start a row  
`<td>` - Table Data. Element to represent each cell.  
`<th>` - Table Heading.

- used for a row or column
- Browsers usually disply in bold and middle of cell
- **Scope** attribute is used to indicate if heading is a row or column.  EX:
  * Column: `<th scope="col"></th>`
  * Rows: `<th scope="row"></th>`

Empty cells still need a `<td>` or `<th>` element.  

## Spanning

- used on `<th>` or `<td>` elements.
- Cells that are used for spanning are not included in the code
- number in the quotes is quantity of cells taken

Colspan attribute - widens the cell to have a larger column across the table.
- `<td colspan="3">data</td>`

Rowspan attribute - lengthens the cell to have a larger row down the table.
- `<td rowspan="3">data</td>`

## Long Tables

`<thead>` - headings of the table live here

`<tbody>` - body of the table lives here  

`<tfoot>`  - footer of the table lives here

There are header and footer elements for taller tables so the browswer can keep them visible while scrolling

Old code ways on (p137-8)

---
_Duckett JS Book_
# Chapter 3: Functions, Methods, and Objects (p106-144)

