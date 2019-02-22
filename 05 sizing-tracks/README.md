# Sizing Grid Tracks

It's not advisable to use percentages to try to make grid tracks add up to 100% since the grid gap will be included and they will add up to over 100% of the width or height.

You can of course use percentages to make a grid track 80% or 50% of the total container.

The new fractional unit (`fr`) comes in very useful here.

The `fr` unit allows you to set the size of tracks as a fraction of the free space available in the grid container. Think `fr` = **fr**ee space.

For example, `grid-template-columns: 200px 1fr 1fr` will create three columns and the second and third will evenly split the free space.

With `grid-template-columns: 2fr 1fr` the first column will take up twice as much space as the second.

You can also use `auto` to make a track equal to the size of its largest item.

In the screenshot below, the third column is set to `auto` and so it is as wide as the text in the third grid item.

![Screenshot of sizing grdi tracks example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550610341/Screenshot_2019-02-19_Sizing_tracks_itgx1y.png)
