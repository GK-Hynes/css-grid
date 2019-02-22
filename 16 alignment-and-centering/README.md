# Alignment and Centering

Besides its usefulness for making grids, CSS Grid is very useful for aligning and centering items.

There are six properties:

## justify-items and align-items

`justify-items` lays out grid items along the row axis

`align-items` lays out grid items along the column axis

These properties can take the values: `start`, `end`, `center`, `stretch` (the default).

## justify-content and align-content

If the grid is not as big as the grid container:

`justify-content` lays out the grid along the row axis

`align-content` lays out the grid along the column axis

These properties can take the values:

`start`, `end`, `center`, `stretch`, `space-around`, `space-between`, and `space-evenly`.

## justify-self and align-self

`justify-self` lays out a grid item inside a cell along the row axis

`align-self` lays out a grid item inside a cell along the column axis

These properties can take the values: `start`, `end`, `center`, `stretch` (the default).

Remember, `justify-` is on the row axis while `align-` is on the column axis

Unlike with Flexbox, the axes don't switch.

![Screenshot of alignment and centering example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549230248/Screenshot_2019-02-03_CSS_Grid_Alignment_and_Centering_rsnwyx.png)
