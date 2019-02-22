# Placing Grid Items

`grid-column` is shorthand for `grid-column-start` and `grid-column-end`

So `grid-column: span 2` is the same as `grid-column-start: span 2` and `grid-column-end: auto`.

You can use `grid-column-start` and `grid-column-end` to tell items to start and end at a particular grid track.

So setting an item to `grid-column-start: 2` and `grid-column-end: 5` will cause it to span from track 2 to track 5.

The shorthand for this would be `grid-column: 2 / 5;`.

You can mix and match this with `span` to tell an item to start or end at a particular track and span a particular number of tracks.

For example, `grid-column: 1 / span 5;` will cause the item to start at track 1 and span 5 tracks.

If you don't know how many tracks your grid will have, use -1 to place an item at the last track.

`grid-column: 1 / -1` will span the entire width of the grid.

`grid-row` does the same thing for rows.

One gotcha is that -1 will only go to the end of the explicit grid. For example, `grid-row: 1 / -1` won't work if you haven't explicitly defined any rows.

```css
.cool {
  background: greenyellow;
  grid-column: span 2;
  grid-row: 1 / -1;
}
```

![Screenshot of placing grid items example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550698665/Screenshot_2019-02-20_Placing_Grid_items_wi6loz.png)
