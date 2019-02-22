# minmax()

Instead of setting a fixed width or height on grid tracks, it's more flexible to have them just be as wide or high as they need to be.

The `minmax()` function lets you specify the minimum and maximum widths or heights for grid tracks.

```css
.container {
  display: grid;
  grid-gap: 20px;
  border: 10px solid var(--yellow);
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
}
```

`minmax()`, comnied with `auto-fit`, can replace a lot of media queries by being inherently flexible.

![Screenshot of minmax() example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550010338/Screenshot_2019-02-12_minmax_cauoms.png)

## fit-content

On a related note, the `fit-content()` function lets you clamp a maximum size on a grid track.

```css
grid-template-columns: fit-content(100px) 150px 150px 150px;
```
