# Class 3

## HTML

### Ordered and Unordered lists

Ordered lists are represented by <ol>
<ol type="i"> this will use Roman Numerals in the list
<ol start="4"> this will start at 4, then move on to 5,6,7,etc...

Unordered Lists are represented by <ul> and can nested in Ordered lists

## CSS

In CSS we broadly have two types of boxes — block boxes and inline boxes. The type refers to how the box behaves in terms of page flow and in relation to other boxes on the page. Boxes have an inner display type and an outer display type.

If a box has an outer display type of block, then:
The box will break onto a new line.
The width and height properties are respected.
Padding, margin and border will cause other elements to be pushed away from the box.
The box will extend in the inline direction to fill the space available in its container. In most cases, the box will become as wide as its container, filling up 100% of the space available.

If a box has an outer display type of inline, then:
The box will not break onto a new line.
The width and height properties will not apply.
Vertical padding, margins, and borders will apply but will not cause other inline boxes to move away from the box.
Horizontal padding, margins, and borders will apply and will cause other inline boxes to move away from the box.

Parts of the box include:
Content box: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
Padding box: The padding sits around the content as white space; size it using padding and related properties.
Border box: The border box wraps the content and any padding; size it using border and related properties.
Margin box: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.