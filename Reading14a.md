# Class 14

## CSS Transforms

Transform Syntax:
transform
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);

2D Transforms:
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees.

HTML

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

CSS

.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}


Combining Transforms:
It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

## CSS Transitions

Transitions: 
As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}

Transitional Property: 
The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  .box:hover {
    background: #ff7b29;
    border-radius: 50%;
  }

  background-color
  background-position
  border-color
  border-width
  border-spacing
  bottom
  clip
  color
  crop
  font-size
  font-weight
  height
  left
  letter-spacing
  line-height
  margin
  max-height
  max-width
  min-heigh
  min-width
  opacityoutline-color
  outline-offset
  outline-width
  padding
  right
  text-indent
  text-shadow
  top
  vertical-align
  visibility
  width
  word-spacing
  z-index