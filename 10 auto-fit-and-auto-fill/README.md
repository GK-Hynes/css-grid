# auto-fit and auto-fill

## auto-fill

`auto-fill` is a keyword you can pass to the `repeat()` function. It will work out the largest number of columns that will fit in the current size of the grid.

It will do its best to **fill** the grid and will create implicit columns if there is space left over.

```css
grid-template-columns: repeat(auto-fill, 150px);
```

![Screenshot of auto-fill example](https://res.cloudinary.com/gerhynes/image/upload/v1549918956/Screenshot_2019-02-11_auto-fit_and_auto-fill_1_dvyqo7.png)

## auto-fit

`auto-fit` is also a keyword you can pass to `repeat()`. It creates the number of columns needed by the grid items and **fits** them into the available space.

Like with `auto-fill`, if there is extra space, `auto-fit` will also generate enough columns to fill the row, but `auto-fit` collapses any that aren't needed after all the grid items have been placed.

If the grid items are able to stretch (like they are set to `1fr`), `auto-fit` will expand them so that they take up all available space.

```css
grid-template-columns: repeat(auto-fit, 150px);
```

![Screenshot of auto-fit example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549919027/Screenshot_2019-02-11_auto-fit_and_auto-fill_2_kppirn.png)

If you want to lay out the grid items in even columns and then have one item off to the right, you can use `auto-fill` to create implicit columns and `grid-column-end: -1` to put the selected item in the final column.

```css
.container {
  display: grid;
  grid-gap: 20px;
  border: 10px solid var(--yellow);
  grid-template-columns: repeat(auto-fill, 150px);
}

.item4 {
  grid-column-end: -1;
}
```

![Screenshot of auto-fill and grid-column-end](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549918133/Screenshot_2019-02-11_auto-fit_and_auto-fill_prumjj.png)
