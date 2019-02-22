# CSS Grid Fundamentals

CSS Grid allows you to take an element and divide it into columns and rows ("tracks") before laying out the items inside that element along those tracks.

Grid is all about the relationship between the grid container and the grid items.

First, set the container element to `display: grid`. The makes all the direct children of the container into grid items.

To create columns and rows use `grid-template-columns` and `grid-template-rows` and give them a list of values. For example, to create three columns, each 100px wide, use:

```css
grid-template-columns: 100px 100px 100px;
```

When you define columns, rows are automatically created.

You can set a space between columns and rows using `grid-gap`, for example:

```css
grid-gap: 20px;
```

You can also set the width or height of a grid item using the `auto` keyword and it will automatically take up whatever space is left over after the widths and heights of the explicitly sized items are taken into account.

For example, you might want a fixed sidebar of 300px and your main content to take up whatever space is left. You would set the column width for the main content to `auto`.

![Screenshot of CSS Grid Fundamentals](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549112476/Screenshot_2019-02-02_CSS_Grid_Fundamentals_wt9kl7.png)
