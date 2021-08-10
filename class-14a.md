# Transforms 

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.
 
`   div {
  -webkit-transform: scale(1.5);
  
     -moz-transform: scale(1.5);
     
       -o-transform: scale(1.5);
       
          transform: scale(1.5);
}`


## 2D Transforms

Two-dimensional transforms work on the x and y axes.

### 2D Rotate
The rotate value provides the ability to rotate an element from 0 to 360 degrees.

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

### 2D Scale
Allows you to change the appeared size of an element.

## 2D Translate
The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow.

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

## 2D Skew
skew, is used to distort elements on the horizontal axis, vertical axis, or both.

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

## Combining Transforms

It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time.

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

## Transform Origin 

As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

`<figure class="box-4">Box 3</figure>`

## Perspective

In order for three-dimensional transforms to work the elements need a perspective from which to transform.
`<figure class="box">Box 1</figure>`

`<figure class="box">Box 2</figure>`

`<figure class="box">Box 3</figure>`

## Transitions & Animations

## Transitions
CSS transitions allows you to change property values smoothly, over a given duration.

There are two properties that are required in order for the transition to take effect:

1- transition-property
2- transition-duration

## transition-property
The transition-property specifies the CSS property where the transition will be applied. You may apply a transition to an individual property (e.g., background-color or tranform) or to all properties in the rule-set (i.e., all).

CSS syntax examples for transition-property


