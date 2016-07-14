# Exercise: Javascript Slider

The eternal *slider* - written by every developer at some point in their career, it's the backbone of crappy Wordpress sites everywhere.  In this exercise, your mission is to build one of these creatures.

## But maaaaaa why a slider?

Sliders can become very complex.  As requirements change, often developers will often just create new ones, breeding them like rabbits - we don't want this.

To prevent this complexity, it presents us the opportunity to employ design patterns and utilize performance optimizations.  The goal of this exercise isn't so much as to produce a slider but to *learn the lessons* in architecting one.

## Wats a slider?

A slider is made of 5 types of elements.

* Window: The parent that is responsible for defining the size of the slider.  Has fixed width/height.
* Container: Single element container for slides that is moves all of the slides.
* Slides: Elements that are/contain images or content.
* Controls: Previous and Next buttons are responsible for advancing/retreating the slides.
* Indicators: Visual indication of what slide you are on - often in the form of bubbles.  These can also be "controls" and jump slides.

## U want me to wat?

To normalize this exercise, HTML and CSS are provided in index.html.  Write a javascript slider module that performs like the one on the Society6.com homepage.  However, UNLIKE the Society6 slider, when the carousel reaches the end, it can reset to the beginning rather than append the first slide to the end.  It must be modular, easy to learn, and reusable across other sites.

You can use libraries like JQuery or Zepto or even pure Javascript if you want (take advantage of ECMAScript6).  You can add and modify the CSS in ```index.html``` but not the html structure.

### Requirements
* Auto calculate number of slides based on provided HTML and work from there.
* Generate clickable indicator bubble elements based on number of slides.
* Controls that provide previous/next functionality
* Indicators of which slide you are on and when clicked will jump to the slide
* Recycling - when reach the end, should start at the beginning

### Configurable Parameters
* delay (number): number of seconds before advancing
* cycle (bool): whether or not to auto advance to next slide
* easing (number): how smooth the transition is

### Selectors
* elWindow: CSS selector for window element
* elContainer: CSS selector for container element
* elControl: CSS selector for control elements
* any others you need or want to add

## Judging

Submissions will be evaluated based on the following criteria in no particular order -

* Perceived performance
* Modularity and Extensibility
* Code elegance
* Design pattern usage
* Calculated performance
* Bonus points awarded to mobile device considerations

## Structure

Write your code in ```js/slider.js``` which is already included in index.html.  If you are using a library you must add it to index.html yourself.

```
js/slider.js
index.html
```
