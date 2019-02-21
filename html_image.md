# Adding an Image

Image elements are rare in that they are both self closing – they don't need closing tags – _and_ also require an attribute.
The syntax for an image element is this:
```
<img src="image_address" />
```
The forward slash before the closing caret, `/>`, indicates that this is a self-closing element. The `src` attribute is very similar to the `href` attribute of an anchor tag. Its value is the url address of the image you'd like to add to your page. For example, if I wanted to add an image of a carrot cake, I'd write:
```
<img src="https://minimalistbaker.com/wp-content/uploads/2017/06/THE-BEST-Vegan-Gluten-Free-Carrot-Cake-1-Bowl-rich-moist-with-5-FROSTING-options-vegan-glutenfree-carrotcake-cake-recipe-minimalistbaker-4.jpg" width="300px" alt="Carrot Cake on a Platter"/>
```
You should see the following:

<img src="https://minimalistbaker.com/wp-content/uploads/2017/06/THE-BEST-Vegan-Gluten-Free-Carrot-Cake-1-Bowl-rich-moist-with-5-FROSTING-options-vegan-glutenfree-carrotcake-cake-recipe-minimalistbaker-4.jpg" width="300px" alt="Carrot Cake on a Platter"/>

You will have noticed two additional attributes on this image element besides the necessary `src` attribute: `width` and `alt`.

The width attribute does just what you'd think – it resizes the image to the desired width (in pixels). It is typically best to include only width or height as attempting to set the size of both may distort the image if the width-to-height ratio is changed. It's also best not to make the image larger than its original size as this will likely lead to pixelation. NOTE: You can also resize an image using CSS.

The alt attribute is text _about_ the image that's useful to include for screen readers so anyone with a visual impairment can still know what image you included on your page. It's also helpful in case the image fails to load so anyone reading your page can know what kind of image they were supposed to see in place of the alt text.

Add this or any other image to your web page.

[Previous: Adding a Link](html_link.md)

[Next: Adding Lists](html_lists.md)
