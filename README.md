## Welcome to Broken-Grid-CSS

#### Development of a CSS framework based on CSS Grid Layout for the implementation of the Broken-Grid approach. Broken-Grid CSS follows the Atomic CSS principle to make the development of a website faster and more comfortable. Due to the special feature of Atomic CSS, it is no longer necessary for the user to pay attention to the CSS, but can design the website in HTML.

### What is Broken-Grid? 
Broken-Grid is a design method to make a website unusual and individual. The positioning of the elements respectively the overlapping of the elements is the main feature of Broken Grid. Broken Grid is ideal for presenting something like products, activities or people who want to stand out from the crowd. The following illustration shows how a website could look like using this method. 

[Abbildung]

### Getting started

#### Use locally
Just download the repository and copy the stylesheet <link> into your HTML document <head> and you can use it.
 
```
<link rel="stylesheet" href="../code/css/broken-grid.css">
```

### Layout - Grid
This framework concentrates solely on the layout and offers many functions for the individual design of a grid and the placement of elements (grid items). Broken-Grid CSS can define a grid with a maximum of 24 columns and rows, which guarantees a larger design possibility. In addition, columns and rows sizes can be mixed with each other, so for example a grid can consist of five columns and 14 rows.

#### Container
With the class `container` you define a grid-container. This contains all other elements that use this grid. 

```
    <div class="container"></div>
```

#### Columns & Rows
With the class `columns` and `rows` you define the columns and rows of the grid-container. Below is an example of how to define three columns and three rows.

```
    <div class="container columns-3 rows-3"></div>
```
#### Display
The `display` class is a help to see the corresponding grid.

```
    <div class="container columns-3 rows-3 display-grid-3x3"></div>
```

#### Gap
The `gap` class is used to determine the distance between columns or rows. These gaps are available in several variants with different sizes.

| Effected      | Classname      | Alternative Classname  |
| ------------: |:---------------| :----------------------|
| 5 Pixel       | `gap-5px`      | `gap-small`            |
| 15 Pixel      | `gap-15px`     | `gap-middel`           |
| 50 Pixel      | `gap-50px`     | `gap-huge`             |
| 100 Pixel     | `gap-100px`    | *none*                 |
| 150 Pixel     | `gap-150px`    | *none*                 |
| 250 Pixel     | `gap-250px`    | *none*                 |

#### Padding
Class `padding` serves, as usual in CSS, the inner distance between container and items.

| Effected      | Classname      | Alternative Classname  |
| ------------: |:---------------| :----------------------|
| 5 Pixel       | `padding-5px`  | *none*                 |
| 15 Pixel      | `padding-15px` | *none*                 |
| 50 Pixel      | `padding-50px` | *none*                 |
| 100 Pixel     | `padding-100px`| *none*                 |
| 150 Pixel     | `padding-150px`| *none*                 |
| 250 Pixel     | `padding-250px`| *none*                 |


#### z-index
The class `z-index` is used to determine how far an element moves into the background. This allows you to determine which element is in front if the elements overlap. The higher the number (1-10), the further forward the element is.


| Effected      | Classname      | 
| :-----------: |:--------------:|
| 1             | `z-index-1`    | 
| 2             | `z-index-2`    | 
| .             | .              | 
| .             | .              | 
| 8             | `z-index-8`    | 
| 9             | `z-index-9`    | 
| 10            | `z-index-10`   |


