# Class 05

## HTML 

*alt:* Its value is supposed to be a textual description of the image, for use in situations where the image cannot be seen/displayed or takes a long time to render because of a slow internet connection. 
Decoration. You should use CSS background images for decorative images, but if you must use HTML, add a blank alt="". If the image isn't part of the content, a screen reader shouldn't waste time reading it.
Content. If your image provides significant information, provide the same information in a brief alt text – or even better, in the main text which everybody can see. Don't write redundant alt text. How annoying would it be for a sighted user if all paragraphs were written twice in the main content? If the image is described adequately by the main text body, you can just use alt="".
Link. If you put an image inside <a> tags, to turn an image into a link, you still must provide accessible link text. In such cases you may, either, write it inside the same <a> element, or inside the image's alt attribute – whichever works best in your case.
Text. You should not put your text into images. If your main heading needs a drop shadow, for example, use CSS for that rather than putting the text into an image. However, If you really can't avoid doing this, you should supply the text inside the alt attribute.


## CSS

Font styles: Properties that affect a text's font, e.g., which font gets applied, its size, and whether it's bold, italic, etc.
Text layout styles: Properties that affect the spacing and other layout features of the text, allowing manipulation of, for example, the space between lines and letters, and how the text is aligned within the content box.
px (pixels): The number of pixels high you want the text to be. This is an absolute unit — it results in the same final computed value for the font on the page in pretty much any situation.
ems: 1 em is equal to the font size set on the parent element of the current element we are styling (more specifically, the width of a capital letter M contained inside the parent element). This can become tricky to work out if you have a lot of nested elements with different font sizes set, but it is doable, as you'll see below. Why bother? It is quite natural once you get used to it, and you can use em to size everything, not just text. You can have an entire website sized using em, which makes maintenance easy.
rems: These work just like em, except that 1 rem is equal to the font size set on the root element of the document (i.e. <html>), not the parent element. This makes doing the maths to work out your font sizes much easier, although if you want to support really old browsers, you might struggle — rem is not supported in Internet Explorer 8 and below.
color
The color to use when drawing the text and any text decorations (such as the addition of under- or overlines, strike-through lines, and so forth.

### Things that can have color

background-color
The text's background color.

text-shadow
Configures a shadow effect to apply to text. Among the options for the shadow is the shadow's base color (which is then blurred and blended with the background based on the other parameters). See Text drop shadows in Fundamental text and font styling to learn more.

text-decoration-color
By default, text decorations (such as underlines, strikethroughs, etc) use the color property as their colors. However, you can override that behavior and use a different color for them with the text-decoration-color property.

text-emphasis-color
The color to use when drawing emphasis symbols adjacent to each character in the text. This is used primarily when drawing text for East Asian languages.

caret-color
The color to use when drawing the caret (sometimes referred to as the text input cursor) within the element. This is only useful in elements that are editable, such as <input> and <textarea> or elements whose HTML contenteditable attribute is set.

Borders
See the section Borders for a list of the CSS properties you can use to set the colors of a box's borders.

background-color
The background color to use in areas of the element that have no foreground content.

column-rule-color
The color to use when drawing the line separating columns of text.

outline-color
The color to use when drawing an outline around the outside of the element. This outline is different from the border in that it doesn't get space set aside for it in the document (so it may overlap other content). It's generally used as a focus indicator, to show which element will receive input events.

### Boxes

Borders
See the section Borders for a list of the CSS properties you can use to set the colors of a box's borders.

background-color
The background color to use in areas of the element that have no foreground content.

column-rule-color
The color to use when drawing the line separating columns of text.

outline-color
The color to use when drawing an outline around the outside of the element. This outline is different from the border in that it doesn't get space set aside for it in the document (so it may overlap other content). It's generally used as a focus indicator, to show which element will receive input events.

### Borders

border-color
Specifies a single color to use for every side of the element's border.

border-left-color, border-right-color, border-top-color, and border-bottom-color
Lets you set the color of the corresponding side of the element's border.

border-block-start-color and border-block-end-color
With these, you can set the color used to draw the borders which are closest to the start and end of the block the border surrounds. In a left-to-right writing mode (such as the way English is written), the block start border is the top edge and the block end is the bottom. This differs from the inline start and end, which are the left and right edges (corresponding to where each line of text in the box begins and ends).

border-inline-start-color and border-inline-end-color
These let you color the edges of the border closest to the beginning and the end of the start of lines of text within the box. Which side this is will vary depending on the writing-mode, direction, and text-orientation properties, which are typically (but not always) used to adjust text directionality based on the language being displayed. For example, if the box's text is being rendered right-to-left, then the border-inline-start-color is applied to the right side of the border.