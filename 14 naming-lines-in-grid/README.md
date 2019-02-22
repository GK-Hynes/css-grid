# Naming Lines in Grid

When defining rows and columns, you can give them arbitrary names of your choosing to help keep things clear when placing grid items.

These names are written inside square brackets.

The same location can be given multiple names if it has multiple functions (for example, the end of the sidebar is also the start of the main content).

```css
.container {
  display: grid;
  grid-gap: 20px;
  grid-template-columns: [sidebar-start site-left] 1fr [sidebar-end content-start] 500px [content-end] 1fr [site-right];
  grid-template-rows: [content-top] repeat(10, auto) [content-bottom];
}
```

You can then use these names instead of track numbers when placing grid items.

```css
.item3 {
  grid-column: content-start;
  grid-row: content-top / content-bottom;
}
```

![Screenshot of naming lines in grid example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550431245/Screenshot_2019-02-17_Naming_Lines_in_CSS_Grid_ehl6qj.png)
