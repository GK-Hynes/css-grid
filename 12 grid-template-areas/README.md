# Grid Template Areas

Grid template areas allow you to both size and place grid items by giving names to specific areas on the grid.

It is very explicit, almost like ASCII art. You define the grid template areas between quotes (the dev tools will allow you to view the area names):

```css
.container {
  grid-template-areas:
    "sidebar-1 content sidebar-2"
    "sidebar-1 content sidebar-2"
    "footer footer footer";
}
```

And then assign items to those areas using `grid-area`.

```css
.item1 {
  grid-area: sidebar-1;
}
.item2 {
  grid-area: content;
}
```

If you want to leave an area empty, use `.`

You can then make the grid responsive by redefining the grid template areas inside a media query.

```css
@media (max-width: 700px) {
  .container {
    grid-template-areas:
      "content content content"
      "sidebar-1 sidebar-1 sidebar-2"
      "footer footer footer";
  }
}
```

![Screenshot of Grid Template Areas example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550429386/Screenshot_2019-02-17_Grid_Template_Areas_v4pdh5.png)
