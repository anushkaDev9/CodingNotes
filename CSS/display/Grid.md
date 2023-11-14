# Grid
CSS Grid Layout Module offers a grid-based layout system, with rows and columns
## Different Properties of Grid 
**1) grid-template-columns** -defines the number of columns in your grid layout, and it can define the width of each column.
<pre>
  grid-template-columns: auto auto auto auto; automatically sets the width
  -more than 4 items in a 4 columns grid, the grid will automatically add a new row to put the items in.
  grid-template-columns: 80px 200px auto 40px; 4 rows with preference width.
</pre>
**2) grid-template-rows**- property defines the height of each row.
<pre>
  reference- https://www.w3schools.com/css/css_grid_container.asp
</pre>
**3)justify-content Property** -used to align the whole grid inside the container
<pre>
  types
  space-evenly-give the columns equal amount of space between, and around them.
  space-around-will give the columns equal amount of space around them:
  space-between- will give the columns equal amount of space between them:
  center-will align the grid in the middle of the container.
  start-will align the grid at the beginning of the container.
  end-will align the grid at the end of the container
</pre>
**4)align-content**- used to vertically align the whole grid inside the container.
<pre>
  types same as above.
  reference- https://www.w3schools.com/css/css_grid_container.asp
</pre>
