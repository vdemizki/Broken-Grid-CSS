## Welcome to Broken-Grid-CSS

#### Development of a CSS framework based on CSS Grid Layout for the implementation of the Broken-Grid approach. Broken-Grid CSS follows the Atomic CSS principle to make the development of a website faster and more comfortable. Due to the special feature of Atomic CSS, it is no longer necessary for the user to pay attention to the CSS, but can design the website in HTML.

### What is Broken-Grid? 
Broken-Grid is a design method to make a website unusual and individual. The positioning of the elements respectively the overlapping of the elements is the main feature of Broken Grid. Broken Grid is ideal for presenting something like products, activities or people who want to stand out from the crowd. The following illustration shows how a website could look like using this method. 

<img src="https://github.com/vdemizki/broken-grid-design-with-CSS-grid/blob/master/images/broken-grid-example/finished-website-example.png" alt="My Webdesign">


### Getting started

#### Use locally
Just download the repository and copy the stylesheet <link> into your HTML document <head> and you can use it.
 
```
<link rel="stylesheet" href="../code/css/broken-grid.css">
```

### Layout - Grid
This framework concentrates solely on the layout and offers many functions for the individual design of a grid and the placement of elements (grid items). Broken-Grid CSS can define a grid with a maximum of 24 columns and rows, which guarantees a larger design possibility. In addition, columns and rows sizes can be mixed with each other, so for example a grid can consist of five columns and 14 rows.

#### Container
With the class `grid-container` you define a grid-container. This contains all other elements that use this grid. 

```
    <div class="grid-container"></div>
```

#### Columns & Rows
With the class `columns` and `rows` you define the columns and rows of the grid-container. Below is an example of how to define six columns and six rows.

```
    <div class="grid-container columns-6 rows-6"></div>
```
Placing elements (grid items) on the grid is something special with CSS Grid Layout. In the following figure the example grid with six columns and six rows is shown visually. 

<img src="https://github.com/vdemizki/Broken-Grid-CSS/blob/master/code/images/6x6.png" alt="6x6 Grid" width="600">

The placement of the elements (grid items) is determined by the numbers after the prefix `row-` or `column-`. For example, "column-1to2" places the element between the first and second column lines. The numbers can have any value from one to 25 inclusive. Any possible combination of numbers can be used. In order to avoid mistakes, the limitation of the grid, which was defined before, should be observed. This means a grid that has six columns cannot have 12 lines that you want to access.

| Effected                  | Classname      | 
| :------------------------ |:--------------:|
| From column line 1 to  2  | `column-1to2`  | 
| From column line 24 to 25 | `column-24to25`|
|                           |                |
| From row line 1 to  2     | `row-1to2`     | 
| From row line 24 to 25    | `row-24to25`   |

With the classes `colum-span-` or `row-span-` you can place elements without paying attention to the column and row lines. For example, column-span-1 can be used to directly determine which element gets the first available column.The following figure shows the possibilities of placement with `colum-span-` and `row-span-`. 

<img src="https://github.com/vdemizki/Broken-Grid-CSS/blob/master/example-images/span-column.png" alt="column-span" width="700">
<img src="https://github.com/vdemizki/Broken-Grid-CSS/blob/master/example-images/span-row.png" alt="row-span">

#### Display
The `display` class is a help to see the corresponding grid.

```
    <div class="grid-container columns-3 rows-3 display-grid-6x6"></div>
```
| Effect            | Classname           |
| ----------------: |:--------------------| 
| display 6x6 grid  | `display-grid-6x6`  | 
| display 12x12 grid| `display-grid-12x12`| 
| display 24x24 grid| `display-grid-24x24`| 

#### Gap
The `gap` class is used to determine the distance between columns or rows. These gaps are available in several variants with different sizes.

| Effect        | Classname      | Alternative Classname  |
| ------------: |:---------------| :----------------------|
| 5 Pixel       | `gap-5px`      | `gap-small`            |
| 15 Pixel      | `gap-15px`     | `gap-middel`           |
| 50 Pixel      | `gap-50px`     | `gap-huge`             |
| 100 Pixel     | `gap-100px`    | *none*                 |
| 150 Pixel     | `gap-150px`    | *none*                 |
| 250 Pixel     | `gap-250px`    | *none*                 |

#### Padding
Class `padding` serves, as usual in CSS, the inner distance between container and items.

| Effect        | Classname      |
| ------------: |:---------------| 
| 5 Pixel       | `padding-5px`  | 
| 15 Pixel      | `padding-15px` | 
| 50 Pixel      | `padding-50px` | 
| 100 Pixel     | `padding-100px`| 
| 150 Pixel     | `padding-150px`| 
| 250 Pixel     | `padding-250px`|


#### z-index
The class `z-index` is used to determine how far an element moves into the background. This allows you to determine which element is in front if the elements overlap. The higher the number (1-10), the further forward the element is.


| Effect        | Classname      | 
| :-----------: |:--------------:|
| 1             | `z-index-1`    | 
| 2             | `z-index-2`    | 
| .             | .              | 
| .             | .              | 
| 8             | `z-index-8`    | 
| 9             | `z-index-9`    | 
| 10            | `z-index-10`   |


