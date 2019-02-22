# repeat()

Instead of typing somthing like `grid-template-columns: 1fr 1fr 1fr 1fr;`, you can use the repeat function.

`repeat()` takes two parameters, how many times to repeat, and what unit you want to repeat.

So `grid-template-columns: repeat(4, 1fr);` gives you four columns, each `1fr` wide.

If you use `grid-template-columns: repeat(4, 1fr 2fr);` you will get eight columns alternating in width between `1fr` and `2fr`.

You can also mix and match `repeat()` with fixed values:

```css
grid-template-columns: 100px repeat(2, 1fr auto) 200px;
```

![Screenshot of repeat function example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550696264/Screenshot_2019-02-20_Repeat_function_whxaxs.png)
