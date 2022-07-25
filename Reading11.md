# Class 11

## Video and Audio Content
src
In the same way as for the <img> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.

controls
Users must be able to control video and audio playback (it's especially critical for people who have epilepsy.) You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.

The paragraph inside the <video> tags
This is called fallback content — this will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

width and height
You can control the video size either with these attributes or with CSS. In both cases, videos maintain their native width-height ratio — known as the aspect ratio. If the aspect ratio is not maintained by the sizes you set, the video will grow to fill the space horizontally, and the unfilled space will just be given a solid background color by default.

autoplay
Makes the audio or video start playing right away, while the rest of the page is loading. You are advised not to use autoplaying video (or audio) on your sites, because users can find it really annoying.

loop
Makes the video (or audio) start playing again whenever it finishes. This can also be annoying, so only use if really necessary.

muted
Causes the media to play with the sound turned off by default.

poster
The URL of an image which will be displayed before the video is played. It is intended to be used for a splash screen or advertising screen.

preload
Used for buffering large files; it can take one of three values:

"none" does not buffer the file
"auto" buffers the media file
"metadata" buffers only the metadata for the file

## Grids

grid – generates a block-level grid
inline-grid – generates an inline-level grid
<line> – can be a number to refer to a numbered grid line, or a name to refer to a named grid line
span <number> – the item will span across the provided number of grid tracks
span <name> – the item will span across until it hits the next line with the provided name
auto – indicates auto-placement, an automatic span, or a default span of one

grid-column-start
grid-column-end
grid-row-start
grid-row-end
Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.

grid-column
grid-row
Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end, respectively.



## Responsive Images

srcset defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma. For each one, we write:

An image filename (elva-fairy-480w.jpg)
A space
The image's intrinsic width in pixels (480w) — note that this uses the w unit, not px as you might expect. An image's intrinsic size is its real size, which can be found by inspecting the image file on your computer (for example, on a Mac you can select the image in Finder and press Cmd + I to bring up the info screen).
sizes defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true — these are the hints we talked about earlier. In this case, before each comma we write:

A media condition ((max-width:600px)) — you'll learn more about these in the CSS topic, but for now let's just say that a media condition describes a possible state that the screen can be in. In this case, we are saying "when the viewport width is 600 pixels or less".
A space
The width of the slot the image will fill when the media condition is true (480px)
