# grid-auto-flow dense

If there are not enough free columns available to place a grid item, the item will simply shift onto the next row. This can leave empty spaces.

`grid-auto-flow: dense` will layout the items that need to go in a specific spot first and then will attempt to fit subsequent grid items into any empty spaces even if that leaves grid items out of order.

This is useful for masonary-style layouts if you don't care about the order of the grid items.

![Screenshot of grid-auto-flow dense example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1549196212/Screenshot_2019-02-03_grid-auto-flow_dense_Block_Fitting_zwzqkm.png)
