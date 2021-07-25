display: grid
    makes an element into a grid container
    e.g <body>
grid-template-columns
    defines the number of columns in a grid container and their widths
    takes in a list of track sizes
    e.g body {
        grid-template-columns: 15em auto 15em;
    }
grid-column-start
    defines the grid line a grid item should start at
grid-column-end
    defines the grid line a grid item should end at
    e.g grid-column-start: 1;
    grid-column-end: 4;

grid-template-rows
    defines the number of rows in a grid container and their heights
min-content
    defines a track size which is large enough to hold its content but no larger

#1 Define grid
    Reference designs or sketch
    Choose grid container
    Define grid columns, rows
#2 Position items
    Items will go in next available cell
    ...unless you define special rules.

Grid Track Sizes
    Static values
        ems, rems, pixels, ch, pt, pc...
    Percentage
        relative to the size of the grid
    auto
        let the browser decide
    fr
        fractional unit: divide up the remaining space
    min-content
        make track as small as possible to fit its content
    max-content
        makes track as large as necessary to contain its content
    minmax(min size, max size)
        function to specify minimum and maximum values for a track
    fit-content
        fit track size to the content, but don't go above specified value


Grid shorthands
    repeat
        function to repeat a pattern of track sizes multiple times
    grid-template
        property to consolidate grid-template-rows and grid-template-columns
    grid
        property to consolidate grid-template-rows and grid-template-columns and some additional things    

    Your objective as a developer is not to write the least possible code but to write code that gets the job done.

Grid Flow
    grid-auto-flow
        whether the grid fills rows or columns first while assigning grid items. Default: row

Implicit Grid
    the columns and rows CSS Grid creates itself to accomodate your grid items
    grid-auto-rows
        the size of any implicintly-created rows. default: auto
    grid-auto-columns
        the size of any implicintly-created columns
    auto-flow *grid
        a keyword added to the grid shorthand property which determines the axis new tracks are added implicitly, and their size
    
Explicit Grid
    columns and rows that you define yourself

Grid gaps
    grid-column-gap
        the gap between each column in your grid
    grid-row-gap
        the gap between each row in your grid
    grid-gap
        property to define grid-row-gap and grid-column-gap at once
12-column grid system
    12-column/start/12-column.html


All CSS Grid Properties
Property	Description
column-gap	Specifies the gap between the columns
gap	A shorthand property for the row-gap and the column-gap properties
grid	A shorthand property for the grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and the grid-auto-flow properties
grid-area	Either specifies a name for the grid item, or this property is a shorthand property for the grid-row-start, grid-column-start, grid-row-end, and grid-column-end properties
grid-auto-columns	Specifies a default column size
grid-auto-flow	Specifies how auto-placed items are inserted in the grid
grid-auto-rows	Specifies a default row size
grid-column	A shorthand property for the grid-column-start and the grid-column-end properties
grid-column-end	Specifies where to end the grid item
grid-column-gap	Specifies the size of the gap between columns
grid-column-start	Specifies where to start the grid item
grid-gap	A shorthand property for the grid-row-gap and grid-column-gap properties
grid-row	A shorthand property for the grid-row-start and the grid-row-end properties
grid-row-end	Specifies where to end the grid item
grid-row-gap	Specifies the size of the gap between rows
grid-row-start	Specifies where to start the grid item
grid-template	A shorthand property for the grid-template-rows, grid-template-columns and grid-areas properties
grid-template-areas	Specifies how to display columns and rows, using named grid items
grid-template-columns	Specifies the size of the columns, and how many columns in a grid layout
grid-template-rows	Specifies the size of the rows in a grid layout
row-gap	Specifies the gap between the grid rows
