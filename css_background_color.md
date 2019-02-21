# Changing the Background Color

What do you target when you want to change the background color of the entire page? There's more than one way to go about this, but perhaps the simplest is to go for the entire `body` element. If we go with this option, our selector would then be `body`, our property would be `background-color`, and our value would be whatever we'd like.

## Working with colors in CSS
There are four ways you can add color to your page, whether it be for your background color, your font color, even gradients!

1. Use a common name

A quick search on CSS colors will give you a list of common colors that you could reference directly by name in your CSS. Examples are green, red, blue, yellow, orange, etc.
For example:
```
body {
  background-color: turquoise;
}
```

However, there are so many colors you could use that not all of them have names. So if you want a very specific color, you could do the following:

2. Use RGB or RGBA

RGB stands for red, green, and blue and it allows you to indicate the exact levels of red, green, and blue that you want to put into your custom color. The "A" in RGBA stands for "alpha" and lets you determine the opacity of the color you indicated with your rgb values. _All values_, red, green, blue, _and_ alpha range from 0 to 255.
Here's an example of a light blue color that uses RGBA:

```
body {
  background-color: rgba(64,224,208, 0.3);
}
```

3. Use Hexadecimal Values

A very common way to add color to your page is to use hexadecimal values. A hexadecimal is composed of a hash sign, `#` followed by six characters ranging from 0 to 9 and A through F. Yes, this base-16 system for counting uses both numbers and letters. There's no need to worry about what this means for now. The important point to note is that it's very much like RGB in that the values are arranged like this: #RRGGBB. The first two values indicate the level of red you want in your custom color, the middle two values indicate the level of green, and the last two values indicate the level of blue. It takes a little more effort to think of this in base-16, but just know that there are some common hexadecimal values you may encounter and which you'll come to recognize immediately in time. For example, black is #000000, meaning there is no red, green, or blue. This makes sense because there's simply no color at all. Conversely, white is #FFFFFF, because it dials up the red, green, and blue levels all the way up to the maximum value. Red is #FF0000, meaning it has the red levels all the way up and no green or blue.

> Challenge: Can you guess what the hexadecimal values for green and blue are?

Making your background red using hexadecimal values would look like this:

```
body {
  background-color: #FF0000;
}
```

4. Use HSL or HSLA

HSL stands for hue, saturation, and lightness. The "A" in HSLA also stands for alpha. I won't cover how HSL/A works here, but just know that it exists.

---

Choose one of the methods above for changing the background color of your webpage to the color of your choice! 

[Previous: Changing the Position of the Heading](css_heading_position.md)

[Next: Adding a Border to Sections](css_section_borders.md)
