##  Responsive Web Design and Regular Expressions:


## What is grid:
A grid is an intersecting set of horizontal and vertical lines – one set defining columns, and the other, rows. Elements can be placed onto the grid, within these column and row lines. CSS grid layout has the following features:

- **Fixed and flexible track sizes**
You can create a grid with fixed track sizes – using pixels for example. This sets the grid to the specified pixel which fits to the layout you desire. You can also create a grid using flexible sizes with percentages or with the new fr unit designed for this purpose.

-  **Item placement**
You can place items into a precise location on the grid using line numbers, names or by targeting an area of the grid. Grid also contains an algorithm to control the placement of items not given an explicit position on the grid.

-  **Creation of additional tracks to hold content**
You can define an explicit grid with grid layout. The Grid Layout specification is flexible enough to add additional rows and columns when needed. Features such as adding “as many columns that will fit into a container” are included.

-  **Alignment control:**
Grid contains alignment features so we can control how the items align once placed into a grid area, and how the entire grid is aligned. 

-  **Control of overlapping content:**
More than one item can be placed into a grid cell or area and, they can partially overlap each other. This layering may then be controlled with the z-index property.

## Grid Layout:
 CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows.

## The Grid container: 
We create a grid container by declaring ``display: grid`` or ```display: inline-grid``` on an element. As soon as we do this, all direct children of that element become grid items.

## Grid Tracks
We define rows and columns on our grid with the ``grid-template-columns `` and ``grid-template-rows`` properties.

### The fr Unit
Tracks can be defined using any length unit. Grid also introduces an additional length unit to help us create flexible grid tracks.

## Grid cells:
A grid cell is the smallest unit on a grid. Conceptually it is like a table cell. 

## Grid areas
Items can span one or more cells both by row or by column, and this creates a grid area. Grid areas must be rectangular – it isn’t possible to create an L-shaped area.
## Gutters
Gutters or alleys between grid cells can be created using the ``column-gap`` and ``row-gap`` properties, or the shorthand ``gap``