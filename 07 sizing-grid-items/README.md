# Sizing grid items

Intead of relying on content size, or giving items a fixed width or height, you can use spanning to tell items to span a specific number of columns or rows.

Use `grid-column` or `grid-row` and tell it how many columns or rows to span.

If you tell an item to span more columns or rows than are currently available, it will automatically force the grid to become larger to provide the necessary implicit columns or rows.

```css
.item9 {
  background: #f4f4f4;
  grid-column: span 10;
  grid-row: span 2;
}
```

![Screenshot of sizing grid items example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550697706/Screenshot_2019-02-20_Sizing_Grid_items_1_nzomnl.png)
