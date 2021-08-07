# CSS Setting height and width for images :

The height and width properties are used to set the height and width of an element.

The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.

`img {
  height: 200px;
  width: 50%;
}`

## How TO - Align Images Side By Side :

`.column {
  float: left;
  width: 33.33%;
  padding: 5px;
}`

`.row::after {
  content: "";
  clear: both;
  display: table;
}`


## Add Responsiveness :
Optionally, you could add media queries to make the images stack on top of each other instead of floating next to each other, on a specific screen width.

## CSS background-image :

The `background-image` property specifies an image to use as the background of an element.

By default, the image is repeated so it covers the entire element.

Example:

The background image for a page can be set like this:

`body {
  background-image: url("paper.gif");
}`

## CSS background-repeat Property :
To create a linear gradient you must define at least two color stops. Color stops are the colors you want to render smooth transitions among. You can also set a starting point and a direction (or an angle) along with the gradient effect.

Example
`#grad {
  background-image: linear-gradient(red, yellow);
}`

## What Is SEO?
SEO stands for “search engine optimization.” It is the process of getting traffic from the “free,” “organic,” “editorial” or “natural” search results on search engines.

## On-page SEO :

On-page SEO is the practice of optimizing individual web pages in order to rank higher and earn more relevant traffic in search engines. On-page refers to both the content and HTML source code of a page that can be optimized, as opposed to off-page SEO which refers to links and other external signals.

## HTML Audio and Video DOM Reference :

The HTML5 DOM has methods, properties, and events for the `<audio>` and `<video>` elements.


## The HTMLMediaElement API :

Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play(), HTMLMediaElement.pause(), etc. This interface is available to both <audio> and <video> elements, as the features you’ll want to implement are nearly identical. Let’s go through an example, adding features as we go.

## Getting started :

To get started with this example, download our media-player-start.zip and unzip it into a new directory on your hard drive. If you downloaded our examples repo, you’ll find it in javascript/apis/video-audio/start/

At this point, if you load the HTML you should see a perfectly normal HTML5 video player, with the native controls rendered.

## Exploring the HTML :

The whole player is wrapped in a <div> element, so it can all be styled as one unit if needed. The <video> element contains two <source> elements so that different formats can be loaded depending on the browser viewing the site. The controls HTML is probably the most interesting: We have four <button>s — play/pause, stop, rewind, and fast forward. Each <button> has a class name, a data-icon attribute for defining what icon should be shown on each button (we’ll show how this works in the below section), and an aria-label attribute to provide an understandable description of each button, since we’re not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them. There is also a timer <div>, which will report the elapsed time when the video is playing. Just for fun, we are providing two reporting mechanisms — a <span> containing the elapsed time in minutes and seconds, and an extra <div> that we will use to create a horizontal indicator bar that gets longer as the time elapses. To get an idea of what the finished product will look like, check out our finished version. Exploring the CSS Now open the CSS file and have a look inside. The CSS for the example is not too complicated, but we’ll highlight the most interesting bits here. First of all, notice the .controls styling:










