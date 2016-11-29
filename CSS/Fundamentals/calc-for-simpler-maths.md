# `calc()` for simpler maths
author: nene

levels:

  - basic

  - medium

type: normal

category: how to

tags:

  - layout

links:

  - >-
    [css-tricks.com](https://css-tricks.com/a-couple-of-use-cases-for-calc/){website}

---
## Content

For styling a 7-column grid you may use something like : 
```
.column-1-7 {
   width: 14.2857%;
}
.column-2-7 {
   width: 28.5714%;
}
.column-3-7 {
   width: 42.8571%;
}
```

Use the calc() function instead to make the maths behind the layout easier to understand :
```
.column-1-7 {
   width: calc(100% / 7);
}
.column-2-7 {
   width: calc(100% / 7 * 2);
}
.column-3-7 {
   width: calc(100% / 7 * 3);
}
```

You can also mix units!
```
.mixing {
   width: calc(50% + 30px);
}

```

---
## Revision

What value for *w_dimension* and *h_dimension* respectively does the following CSS code generate using the *calc()* function? ???
```css
.generate {
   w_dimension: calc(30% - 21px);
   h_dimension: calc(100% / 3 * 4);
}
```
*