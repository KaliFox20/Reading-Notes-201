# Class 12

## JS Canvas

HTML5 features the <canvas> element that allows you to draw 2D graphics using JavaScript.

The <canvas> element requires at least two attributes: width and height that specify the size of the canvas

Unlike the <img> element, The <canvas> element requires the closing tag </canvas>. Any content between the opening and closing tags is fallback content that will display only if the browser doesn’t support the <canvas> element.

The <canvas> element features the getContext() method that returns a render context object.

The getContext() takes one argument which is the type of context. For example, you use the "2d" to get a 2D rendering context object, which is an instance of the CanvasRenderingContext2D interface.

The 2D rendering context allows you to draw shapes, text, images, and other objects.

The following example shows how to select the canvas element using the querySelector() method and access the drawing context by calling its getContext() method


