# Formatting the Spacing Between Elements

You may have noticed that your HTML elements look a bit crowded in your browser. There's a way to put some space between elements that leverages something known as the "CSS Box Model". A quick search on the CSS Box Model will go more in depth into how it works. For our purposes, just know that there's space _within_ an HTML element that's known as `padding` and there's also space _outside_ the element that's known as `margin`. The padding begins where the content of the element ends and it ends at the border of the element. The margin begins at the border of the element and ends where it comes in contact with the margins of other elements.

Since we already have two elements on our page with borders, let's go ahead and modify their padding and margin.

First, add the following style to your section style block:
```
padding: 10px 10px 10px 20px;
```

Refresh your page to see what's changed. You should have seen some spacing appear between the border of the sections and the content (i.e., the headings and lists).
In the style above, the property is `padding` and the value is actually four values: the `top padding`, `right padding`, `bottom padding`, and `left padding`. It's useful to remember this order as going clockwise from the top. For our particular style, this means that there will be 10px of empty space between the border and the top, right, and bottom of the content (the heading and list combos), and there will be 20px of empty space between the border and the left side of the content.

Let's now adjust the margin and see how it's different from the padding. Add the following style to your section style block:
```
margin: 20px 10px 20px 10px;
```

If you refresh your page you'll notice that now we have extra space _between_ the section elements and other elements on the page. In other words, there is more space _around_ the borders of the two sections. In the style above we put an extra 20 px of space between the top and bottom of the borders and other elements and an extra 10 px of space between the left and right sides of the borders and other elements.

Your section style block may now look something like this:
```
section {
  border: solid 3px #ffffff;
  margin: 20px 10px 20px 10px;
  padding: 10px 10px 10px 20px;
}
```

Let's add one last margin style to our page and in particular to our body element. You may have noticed that all the content tends to stick to the top and left sides of the page. Let's add a margin of 30 px to all sides of the body:
```
margin: 30px;
```

There's only one value here because all of the sides are going to get the same margin. You may be satisfied with this or you may want to add some more spacing at the top. Rather than doing the following:
```
margin: 50px 30px 30px 30px;
```
You could do this:
```
body {
  background-color: rgba(64,224,208, 0.3);
  margin: 30px;
  margin-top: 50px;
}
```

_This_ is the reason CSS is called _Cascading_ style sheets. What's going on here is that all sides of the body get the same margin value, 30px. However, _after_ this style is applied, the `margin-top` property gets overridden with a new value. The last value to get assigned is the one that is applied to the property.

[Previous: Adding a Border to Sections](css_section_borders.md)

[Next: Styling and Formatting an Image](css_format_image.md)
