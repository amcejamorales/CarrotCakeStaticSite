# Adding a Border to Sections

Before we add a border to a section, we need to know what a section even is.

A section is another HTML element that groups related content (recall the earlier section on nesting related elements together). This provides an easy way to apply styles to related content easily, but it also lets you style _different_ sections that are similar in nature but have different content.

A good example of this in our carrot cake page is the ingredients and instructions lists. They both have similar structure (a heading and a list) and have a similar nature (to list items).

Let's go ahead and put these elements into their own sections. Back in your `index.html` file, go ahead and nest the Ingredients heading and the unordered list within a `section` element. Next, do the same to the Instructions heading and the ordered list with a second `section` element. (Hint: section elements require both opening and closing tags and may have, but do not require any attributes).
This section of your HTML file should look something like this:
```
<section>
  <h2>Ingredients</h2>
  <ul>
    <li>...</li>
    <li>...</li>
    ...
  </ul>
</section>

<section>
  <h2>Instructions</h2>
  <ol>
    <li>...</li>
    <li>...</li>
    ...
  </ol>
</section>
```

You can now return to the CSS file to style your newly created sections. (Remember to save the change you just made on your HTML file).

In your CSS file, select the section element and give it a border. You could follow this example:
```
section {
  border: solid 3px #ffffff;
}
```

In the example above, the selector is _section_, the property is _border_, and interestingly enough the value is actually three values: the _style_ of the border (it could be solid, dotted, dashed, etc.), the _thickness_ of the border (here indicated in pixels), and the _color_ of the border.

Go ahead and add a custom border to your sections and play around with the different styles. Once you refresh the page you should see the border applied to both your ingredients and instructions sections. That's the utility of using sections to apply styles to more than one chunk of elements.

> Challenge: Figure out how to round out the corners on the borders in your sections using CSS.

[Previous: Changing the Background Color](css_background_color.md)

[Next: Formatting the Spacing Between Elements](css_format_spacing.md)
