# Adding Lists

To complete the content on our page we're going to add two different kinds of lists, ordered lists and unordered lists.

Underneath all of the paragraphs in your `index.html` file add two sub-headings for Ingredients and Instructions:
```
<h2>Ingredients</h2>

<h2>Instructions</h2>
```

Both ingredients and instructions seem to be good candidates for lists, but semantically they should have different functions. We'll use an `unordered list` for ingredients since the order in which you get the ingredients doesn't matter, and we'll use an `ordered list` for instructions since the order in which you perform the steps is very important.

## Unordered List

We will use two tags for the unordered list: the `unordered list` or `ul` tag, and the `list item` or `li` tag. As the names imply, the `ul` tag indicates what kind of list we're making and therefore applies to the entire list, whereas the `li` tag just indicates a single item on the list. Therefore it makes sense that `li` elements be nested within a `ul` element. The syntax is as follows:
```
<ul>
  <li>First Item</li>
  <li>Second Item</li>
  <li>Third Item</li>
</ul>
```
In practice, your list will look like this:
- First Item
- Second Item
- Third Item

The `li` elements indicate that their content represent a single item on the list and should therefore be on their own line. The `ul` element indicates that this list is unordered and therefore the list items should have bullet points.

Go ahead and add some ingredients under your ingredients sub-heading. Try:
- eggs
- milk
- flour
- baking powder
- baking soda
- brown sugar
- butter
- salt
- shredded carrots
- chopped canned pineapple
- cinnamon
- cream cheese for frosting
- granulated sugar for frosting

> Challenge: Try looking up how to put an ordered list in a webpage before moving on to the next section.

## Ordered List
The only real difference between an unordered list and an ordered list is that the latter uses an `ol` tag. See:
```
<ol>
  <li>First Item</li>
  <li>Second Item</li>
  <li>Third Item</li>
</ol>
```

This would give you a list that looks like:
1. First Item
1. Second Item
1. Third Item

Go ahead and add some steps under your instructions sub-heading. (Please note that these are made up steps. Please do not attempt to follow them). Try:
1. turn on the oven
1. sift flour
1. add baking powder, baking soda, brown sugar, cinnamon, and salt to flour
1. add melted butter, eggs, and milk to flour mixture
1. mix in carrots and pineapple
1. grease a pan and pour the mixture
1. bake mixture in oven until it is ready
1. mix cream cheese and sugar to make cream cheese frosting
1. allow baked cake to cool
1. cover cake in frosting


You've gotten to the end of the HTML section. Next up we'll add some CSS to our page.

[Previous: Adding an Image](html_image.md)

[Next: Changing the Font](css_font.md)
