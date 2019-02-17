# Area Line Names

You can create a grid without defining columns and rows by simply using area names (these can even be emoji for fun).

```css
.container {
  display: grid;
  grid-gap: 20px;
  grid-template-areas:
    "🍕 🍕 🍕 🍕 🍺 🍺 🍺 🍺"
    "🍕 🍕 🍕 🍕 🍺 🍺 🍺 🍺"
    "🍕 🍕 🍕 🍕 🍺 🍺 🍺 🍺"
    "🍕 🍕 🍕 🍕 🍺 🍺 🍺 🍺";
}
```

You can also use line names in place of track numbers to place grid items. Adding `-start` or `-end` to the area name lets you position items in relation to the start and end of a named grid area.

```css
.item3 {
  grid-column: 🍕-start / 🍺-end;
  grid-row-end: 🍕-end;
}
```

![Screenshot of area line names example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550429555/Screenshot_2019-02-17_Grid_Template_Areas_Line_Names_from_Grid_Areas_zirbl7.png)
