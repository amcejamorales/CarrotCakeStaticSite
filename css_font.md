# Changing the Font

Changing the font style on a webpage is one of the most common use cases for CSS. To create a CSS file add a new file in the same folder as your `index.html` and save it as `styles.css`.

Before modifying the font let's go over how CSS syntax works:
```
selector {
  property: value;
}
```

The `selector` is essentially the HTML target element that you want to apply a style to. It would be your `p` tag, `h1`, `h2`, `li`, etc.
The `property` is _what you want to change_ about your HTML element, and the `value` is _how you want to change it_. You can have more than one selector so that you can apply the same styles to multiple HTML elements. You can also have more than one _declaration_ in a style block. A declaration is a property-value pair that makes up one style. For example, you could change the font and color within the same style block.

Let's change the font of the text on the page so it looks a bit more modern. Following the convention above change the font of the heading to `Futura`. See this example:
```
h1 {
  font-family: Futura;
}
```

Refresh your page to see the change take effect.

Did anything change? It shouldn't have. This is because the HTML page doesn't know about the styles in `styles.css`. A single line addition in `index.html` will change that.

Go to your `index.html` file and anywhere in the `head` element, add the following line:
```
<link rel="stylesheet" type="text/css" href="styles.css">
```

The `head` element holds all the metadata about your webpage that isn't visible on the browser. It's importance here is that the head is where we link our HTML to our CSS. Your page may now look like this:

```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
    <link rel="stylesheet" type="text/css" href="styles.css">
  </head>
  <body>

  </body>
</html>
```

_Now_ if you refresh your page you'll see that your heading font changed. Now let's apply the same style to the paragraph elements:
```
h1, p {
  font-family: Futura;
}
```

The example above combines the `h1` and `p` selectors and applies the Futura font-family style to both of them. We could keep going like this and apply the style to the lists as well. There's another alternative, though. We can use the `*` selector. This selector applies to everything in your webpage so you don't have to keep listing everything you want to style if you're going to style everything on the page anyway.
```
* {
  font-family: Futura;
}
```

All the text on the page should now have the Futura font style.

[Previous: Adding Lists](html_lists.md)

[Next: Changing the Heading Position](css_heading_position.md)
