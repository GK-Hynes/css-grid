# Implicit and Explicit Grid Tracks

Columns and rows are explictly defined using `grid-template-columns` and `grid-template-rows`.

If there are more grid items than there are explicit columns, the items will wrap onto a new row.

You haven't explicitly created these rows, so they are implicit rows.

The same occurs if you explicitly create rows but not columns.

Using the Firefox grid inspector dev tools, solid lines show the start and end of the explicit grid, dashed lines show explicit columns and rows, while dotted lines show implicit columns and rows.

Explicit columns and rows are sized using `rid-template-columns` and `grid-template-rows`.

`grid-auto-columns` and `grid-auto-rows` will define how big implicit columns and rows are when they are added.

By default, you define columns and any extra elements will be turned into rows. `grid-auto-flow` can however override this.

### Note

Currently (Feb 2019), in Firefox you can only pass one value to `grid-auto-rows` so

```css
grid-auto-rows: 100px 300px;
```

will create two 100px rows in Firefox while in Chrome it will create a 100px row and a 300px row.

![Screenshot of Implicit and Explicit Tracks](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549191707/Screenshot_2019-02-03_CSS_Grid_-_Implicit_and_Explicit_Tracks_prhzox.png)
