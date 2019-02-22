# Nesting Grids

You can nest one grid inside another by making a grid item into a grid container.

```css
.albums {
  display: grid;
  grid-gap: 20px;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.album {
  display: grid;
  grid-gap: 10px;
  grid-template-columns: 150px 1fr;
  align-items: center;
}
```

![Screenshot of nesting grid example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550870145/Screenshot_2019-02-22_Nesting_Grid_with_Album_Layouts_wb0ig7.png)
