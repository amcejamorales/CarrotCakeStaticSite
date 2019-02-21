# Styling and Formatting an Image

Besides padding and margins, another very useful aspect of CSS is that it allows you to reposition elements on the page. This allows you to take HTML which mostly stacks elements vertically and provide a very dynamic user experience.

Let's start by repositioning the image on your page. Move your image to the beginning of your first paragraph. In other words, nest the image element within the first p element before any of the text like so:
```
<p>
  <img src="..." />
  Lorem ipsum...
</p>
```

When you refresh the page what do you notice? You'll most likely see that the image appears before the text, but the first line of the text is in the same line as the image. This is because images are _inline_ elements, which basically means they don't insert a new line on the page. Elements can be either _inline_ (don't insert new lines), _block_ (do insert new lines), or *inline_block* (don't insert new lines but exhibit some block element behaviors). Knowing about these different types of elements and how to modify their `display` style is very important. For now, it's enough to understand why the image is on the same line as the text.

Where I actually want the image to show up is on the top right corner of the chunk of text. To achieve this I can apply the following style to my `img` element:
```
img {
  float: right;
}
```
The image should now appear right of the text and the text should wrap around it, i.e., it is literally "floating" to the right, or hugging the right edge of its parent element which is a `p` in this case. If the image is not small enough to see the effect of the text wrap around, I suggest using CSS to adjust the height or width properties of the image. (You could also directly indicate the height or width in the img HTML element).

This is all the formatting we'll cover regarding images. Try the following challenges before you move on.

> Challenge: Round the corners of the image.

> Challenge: Add some spacing between the edges of the image and the text around it. What should you use to do this? Padding or margin? 

[Previous: Formatting the Spacing Between Elements](css_format_spacing.md)

[Next: Putting it all Together](outro.md)
