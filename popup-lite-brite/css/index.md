---
layout: lesson
---

# Modifying the Lite-Brite CSS

CSS allows us to "dress up" the content on our page.

## Tour the Existing Code

- CSS allows us to target types of elements (ex: `section`, `div`) and specific elements based on class name (ex: `dot-container`).
- Once we've targeted an element, we can write rules for that element to follow. Rules can be things like _"the text of this element should be red"_ or, _"the background color should be grey"_.

### Explore to Learn:

After you complete each task that follows, observe the changes in the browser!
- On line 9 of the CSS file, change `black` to `magenta`
- On line 10, change `lightgrey` to `orange`
- On line 11, change `10px` to `50px`
- On line 12, change `5px` to `30px`, then `0px`

You may be wondering, "how does one know all these special keywords and commands to create these rules?". Great question! With time and practice, and the use of documentation like [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS) and [CSS Tricks](https://css-tricks.com/almanac/), developers slowly build their toolkit. Even the most experienced developers need to continually research and google to find the tool they need.
<br>
<br>

<div class="try-it-new">
  <h2>Modify the Existing Code</h2>
  <p>Now that we can see how some of the pieces come together with CSS, let's continue in this process of "making it our own".</p>
  <ul>
  <li><strong>Change the size of the dots on your Lite-Brite board.</strong></li>
  <li><strong>Change the amount of space around/between the dots on your Lite-Brite
  board.</strong></li>
  <li>Optional: Tinker with the colors used throughout your app!</li>
  </ul>
  <p>Play around with these sizes until you are satisfied with your board. <em>This may be the time where you also decide to go back to the HTML file and add more dots!</em></p>
  <p>You may notice that the layout of the dots in your dot container is responsive to the size of the window. This is because the dot container takes up as much space as it can horizontally, unless we tell it to do something different. If you want your dots to be in a fixed location, without considering the size of the window, set the width property on your `dot-container` to be a fixed pixel value, like 500px. <strong>You may have to play around with the right number of dots, size of the dots, space around the dots, and width until you get it lined up perfectly.</strong></p>
</div>

## CSS Summary

- CSS allows us to target an element and write specific rules for it to follow.
- Based on the type of rule, CSS will expect different values (ex: `magenta` for a color and `10px` for a measurement).
- There are many types of rules we can write; with practice, we become familiar with more but don't need to memorize them all.

### Up Next

- [What is Front End and Back End Engineering?](../what-is-fe-be)
- [Project Setup](../litebrite)
- [HTML - Content](../html)
- <strong>[CSS - Styles](../css)</strong>
- [JavaScript- Explore](../js-1)
- [JavaScript - Create](../js-2)
- [Extensions](../extensions)
- [Wrap-Up](../wrap-up)
