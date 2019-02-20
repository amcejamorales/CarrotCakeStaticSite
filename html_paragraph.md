# Adding Text to a Page

Before you can code your webpage you should create a folder in your computer where you'll put your HTML and CSS files. I recommend creating a folder in your Desktop (you can call it anything, e.g., "recipe").

Then open your code editor, e.g., Atom, and navigate to where the folder is located. Inside Atom go to `File > Open`. In the Window select Desktop, then recipe. This should open Atom to the empty folder you just created. You're now ready to make your HTML file. Inside Atom go to `File > New File`. This will open up a new file called "untitled" in Atom. Inside this file go to `File > Save As`, give your file the name `index.html` and click `Save`. You can now start coding HTML!

---

## Adding Text

The most common element you're likely to see on a page is text. You could actually add simple text to your page without any HTML syntax and see it appear on your browser (this may depend on the browser you use). Go ahead and try it. Add the following text to your `index.html` file:
```
Hello World
```
Save your changes. On your computer navigate to your recipe folder and right-click on your `index.html` file, you should have the option to choose an application to open your file, e.g., `Open With > Google Chrome`. This will open your HTML file on your browser. Now you can see what your file would actually look like on the web.
Keep your file open in your browser as you code and each time you make a change save your file and refresh the page on your browser to see the change reflected.

At this point you should see `Hello World` in your page on the browser. You can keep adding text, save your changes, and refresh your browser to see the text you added.

This, however, is not HTML. To turn this piece of text into an HTML paragraph, you need to put the text inside an paragraph tag.

## Turning Your Text into a Paragraph

An HTML _element_ is the most basic unit of HTML you can write. It's made up of a _tag_, _attributes_ (these are optional and depend on the tag), and _content_. We'll cover attributes later. For now, the format of an element is as follows:
```
<tagName>Content</tagName>
```
For example, to turn the text above into a paragraph element, I'd write:
```
<p>Hello World</p>
```
Here, we're using the _p tag_, which will give us a paragraph. Go ahead and replace the text in your index.html file with the paragraph element above. If you refresh your page you won't see any changes yet.

### A Note on Opening and Closing Tags
You'll notice the content in our paragraph element is _wrapped_ in two p tags. The content is preceded by an _opening p tag_ and followed by a _closing p tag_. The only difference between the two is that the closing p tag starts with a forward slash. Besides this they should be exactly the same. This is the format you'll use for most HTML elements. There are some elements that are self-closing so you won't need a closing tag. We'll take a look at an example of this later.

> Challenge: Modify your HTML so that `Hello` appears on one line and `World` appears on the line beneath it.

## Adding a Second Paragraph

It's possible you hit enter after `Hello` in your `index.html` file to put `World` on its own line:
```
<p>Hello
World</p>
```
If you did this you shouldn't have seen a change in your browser. That's because although this is intuitive, HTML still sees the text between the p tags as belonging to a single paragraph. It'll ignore any whitespace within the content.

Therefore if you wanted to add two paragraphs to your page, you'd need two paragraph elements. Recall, HTML cares about _semantic labeling_, therefore, any text that you want to appear as two distinct paragraphs should be labeled as such. Change your file thus:
```
<p>Hello</p>
<p>World</p>
```
`Hello` and `World` should now appear on their own lines.

Go ahead now and replace these elements with several paragraphs of real content.

[Previous: About HTML, CSS, and JS](about_html_css_js.md)

[Next: Adding A Heading](html_heading.md)
