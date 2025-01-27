---
layout: lesson
---

# Lite-Brite Extensions

If the class has extra time, or individuals want to continue building on their Lite-Brite after the workshop, here are some areas to explore!

## Let Your User Choose ANY Color!

Physical Lite-Brites are limited to the colors of the little pegs that are provided in the kit. However, building a virtual Lite-Brite really opens up the possibilities!

We can provide a "color picker" input to the user so that they can choose from, literally, any color available on a screen with something like this: <input class="color-picker" type="color" />

### Step 1

In your Lite-Brite codepen, add this code to the HTML file, inside of the `controls` section:

```html
<input type="color" class="color-option color-picker"/>
```

<br>

Let's break down this newly added line of code:
- `<input />` - the input tag is used to create controls such as text fields, checkboxes, date/time pickers, passwords, and more!
- `type="color"`- specifies what type of input we'd like the browser to show the user. The type `color` presents a small box that when clicked, provides several ways for a user to select a very specific color. _If you want to explore other types of inputs, change out `color` for `password`, `range` and/or `date`! You can read all about the [input types available on MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)_.
- `class="color-option color-picker"` - these classes were applied so we can use CSS styles and, later, access this element in JavaScript.

## Update the Active Color

As of now, your user should be able to select a new color from the picker. However, the color doesn't go anywhere. We have to use JavaScript to make this happen!

### Step 2

Our JavaScript file needs to know about the color picker input in order to keep track of which color was selected. Let's create a variable that stores the HTML element:

```js
var colorPicker = $('.color-picker');
```

Now, we need to instruct our program to listen for the user's input:

```js
colorPicker.on("input", changeActiveColor);

function changeActiveColor() {
  //code will go here later
}
```

### Step 3

The final step is to take the value from the color picker input, and update the `active` variable (declared on line 1) to hold that new value. Write a `changeActiveColor` function to include this:


```js
function changeActiveColor() {
  active = colorPicker.val();
}
```

The `.val()` method used in the previous snippet takes the value from an input. Whatever is in the input at the time will be stored in the `active` variable.

Run the program, and try this functionality out!

### Up Next

- [What is Front End and Back End Engineering?](../what-is-fe-be)
- [Project Setup](../litebrite)
- [HTML - Content](../html)
- [CSS - Styles](../css)
- [JavaScript- Explore](../js-1)
- [JavaScript - Create](../js-2)
- <strong>[Extensions](../extensions)</strong>
- [Wrap-Up](../wrap-up)
