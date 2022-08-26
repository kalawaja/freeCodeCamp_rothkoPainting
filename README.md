
# Learn HTML Forms by Building a Registration Form, Completed

> - Every HTML element is its own box – with its own spacing and a border. This is called the Box Model.
> - In this course, you'll use CSS and the Box Model to create your own Rothko-style rectangular art pieces.
---

> **Step 1** <br>
By now, you should be familiar with the basic elements an HTML page should have.<br>
Set up your code with a `DOCTYPE` declaration, an `html` element with the language set to English, a `head` element, and a `body` element.

```html
#index.html
<!DOCTYPE html>
<html lang="en">
  <head></head>
  <body></body>
```
```html
#index.html
</html>
```
> **Step 2** <br>
Within the `head` element, add a `meta` tag which sets the `charset` to `UTF-8`, and a `title` element with the value `Rothko Painting`.<br>
Within the `body` element, add an `img` element with a `src` of `https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-1.png`.

```html
#index.html
  <head>
    <meta charset="UTF-8">
    <title>Rothko Painting</title>
  </head>
  <body>
    <img src="https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-1.png">
  </body>
```
> **Step 3** <br>
In the CSS box model, every HTML element is treated as a box with four areas.<br>
Imagine you receive a box from your favorite online retailer -- the content is the item in the box, or in our case, a header, paragraph, or image element.<br>
Change the `src` attribute in the `<img>` from <br> `https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-1.png` to <br> 
`https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-2.png`.

```html
#index.html
    <img src="https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-2.png">
```
> **Step 4** <br>
The content is surrounded by a space called padding, similar to how bubble wrap separates an item from the box around it.<br>
Think of the border like the cardboard box your item was shipped in.<br>
Change the `src` attribute to <br> 
`https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-3.png`

```html
#index.html
    <img src="https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-3.png">
```
> **Step 5** <br>
Margin is the area outside of the box, and can be used to control the space between other boxes or elements.<br>
Here the bottom element has a larger top margin, pushing it further down the page.<br>
Now that you understand the CSS box model, let's get started on the Rothko painting.<br>
Remove the `<img>` element.

```html
#index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Rothko Painting</title>
  </head>
  <body>
  </body>
</html>
```
> **Step 6** <br>
Add a `div` element in the `body`.<br>
Set the `class` attribute equal to `canvas`. <br> 
For example, `<div class="my-div">` <br>
This will act as the canvas for your painting.

```html
#index.html
  <body>
    <div class="canvas">
  </body>
```
> **Step 7** <br>
Before you can start styling the `div` you added, you need to link your CSS to your HTML.<br>
Add a `link` element to link your `styles.css` file. Set the `href` to `./styles.css`, and remember to set the `rel` attribute to `stylesheet`.

```html
#index.html
  <head>
    <meta charset="UTF-8">
    <title>Rothko Painting</title>
    <link href="./styles.css" rel="stylesheet">
  </head>
```
> **Step 8** <br>
Time for CSS.<br>
Even though your `<div>` has no text, it's still treated as a box with content. Write a CSS rule that uses the `.canvas` class selector and set its `width` to 500 pixels. Here's a CSS rule that sets the width of the class `card` to 300 pixels: <br>
> ```css
> #styles.css
> .card {
>   width: 300px;
> }
> ```
> <br>
<br>

```css
#styles.css
.canvas {
  width: 500px;
}
```
> **Step 9** <br>
Add the `height` property with the value `600px` to your `.canvas` rule.

```css
#styles.css
.canvas {
  width: 500px;
  height: 600px;
}
```
> **Step 10** <br>
Change the `background-color` of the canvas to `#4d0f00`.

```css
#styles.css
.canvas {
  width: 500px;
  height: 600px;
  background-color: #4d0f00;
}
```
> **Step 11** <br>
Every painting needs a frame.<br>
Wrap the `.canvas` element in another `div`. Give that `div` the `frame` class.

```html
#index.html
    <div class="frame">
      <div class="canvas">
      </div>
    </div>
```
> **Step 12** <br>
Write a new rule using the `.frame` class selector.<br>
Use the `border` shorthand declaration to give the `.frame` element a solid, black border with a width of `50px`.

```css
#styles.css
.frame {
  border: 50px solid black;
}
```
> **Step 13** <br>
The frame is much too wide.<br>
In `.frame`, set its `width` to 500 pixels.

```css
#styles.css
.frame {
  border: 50px solid black;
  width: 500px;
}
```
> **Step 14** <br>
Use padding to adjust the spacing within an element.<br>
In `.frame`, use the `padding` shorthand property to increase the space between the `.frame` and `.canvas` elements by `50px`. The shorthand will increase space in the top, bottom, left, and right of the element's border and canvas within.

```css
#styles.css
.frame {
  border: 50px solid black;
  width: 500px;
  padding: 50px;
}
```
> **Step 15** <br>
Use margins to adjust the spacing outside of an element.<br>
Using the `margin` property, give the `.frame` element vertical margin of `20px`, and horizontal margin of `auto`. This will move the frame down 20 pixels and horizontally center it on the page.

```css
#styles.css
.frame {
  border: 50px solid black;
  width: 500px;
  padding: 50px;
  margin: 20px auto;
}
```
> **Step 16** <br>
Add a new `div` element inside of your `.canvas` element.<br>
Give the new `div` the `class` attribute with a value of `one`. This will be your first rectangle.

```html
#index.html
  <body>
    <div class="frame">
      <div class="canvas">

        <div class="one">

        </div>

      </div>
    </div>
   </body>
```
> **Step 17** <br>
Write a new rule that targets `.one` and set its `width` to 425 pixels.

```css
#styles.css
.one {
  width: 425px;
}
```
> **Step 18** <br>
Now set the `height` for `.one` to 150 pixels.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
}
```
> **Step 19** <br>
Set the `background-color` of `.one` to `#efb762`.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
}
```
> **Step 20** <br>
Use margins to position the `.one` element on the canvas.<br>
Add the shorthand `margin` property with a vertical margin of `20px` and a horizontal margin of `auto`.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
}
```
> **Step 21** <br>
Now `.one` is centered horizontally, but its top margin is pushing past the canvas and onto the frame's border, shifting the entire canvas down 20 pixels.<br>
Add `padding` of `1px` to the `.canvas` element to give the `.one` element something solid to push off of.

```css
#styles.css
.canvas {
  width: 500px;
  height: 600px;
  background-color: #4d0f00;
  padding: 1px;
}
```
> **Step 22** <br>
Adding 1 pixel of padding to the top, bottom, left, and right of the canvas changed its dimensions to 502 pixels x 602 pixels.<br>
Replace the `padding` property with `overflow` set to `hidden` - changing the canvas back to its original dimensions.

```css
#styles.css
.canvas {
  width: 500px;
  height: 600px;
  background-color: #4d0f00;
  overflow: hidden;
}
```
> **Step 23** <br>
Add another `div` with a `class` value of `two` just below your `one` element. This will be your second rectangle.

```html
#index.html
  <body>
    <div class="frame">
      <div class="canvas">
        <div class="one">
        </div>

        <div class="two">
        </div>

      </div>
    </div>
   </body>
```
> **Step 24** <br>
Create a new CSS rule using the `.two` selector and set its `width` to 475 pixels.

```css
#styles.css
.two {
  width: 475px;
}
```
> **Step 25** <br>
Set the `height` of the `.two` element to 200 pixels.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
}
```
> **Step 26** <br>
Set the `background-color` of the `.two` element to `#8f0401`.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;
}
```
> **Step 27** <br>
Center the `.two` element by setting its `margin` to `auto`.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;
  margin: auto;
}
```
> **Step 28** <br>
Create a new `div` with a `class` value of `three` right under the `.two` element. This will be your third rectangle.

```html
#index.html
  <body>
    <div class="frame">
      <div class="canvas">
        <div class="one">
        </div>
        <div class="two">
        </div>

        <div class="three">
        </div>

      </div>
    </div>
   </body>
```
> **Step 29** <br>
You don't always have to use pixels when sizing an element.<br>
Create a new rule, `.three`, and set its `width` to 91%`.

```css
#styles.css
.three {
  width: 91%;
}
```
> **Step 30** <br>
Set the `height` of `.three` to `28%`.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
}
```
> **Step 31** <br>
Change the `background-color` of `.three` to `#b20403`.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
}
```
> **Step 32** <br>
Center the `.three` element on the canvas by setting its `margin` to `auto`.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
  margin: auto;
}
```
> **Step 33** <br>
It's helpful to have your margins push in one direction.<br>
In this case, the bottom margin of the `.one` element pushes `.two` down 20 pixels.<br>
In the `.two` selector, use `margin` shorthand property to set top margin to `0`, horizontal margin to `auto`, and bottom margin to `20px`. This will remove its top margin, horizontally center it, and set its bottom margin to 20 pixels.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;margin-top: 0;
  margin-bottom: 20px;
  margin-left: auto;
  margin-right: auto;
}
```
> **Step 34** <br>
The colors and shapes of your painting are too sharp to pass as a Rothko.<br>
Use the `filter` property to `blur` the painting by `2px` in the `.canvas` element.<br>
<br>
Here's an example of a rule that add a 3px `blur`:<br>
> <br>
> ```css
> #styles.css
> p {
>   filter: blur(3px);
> }
> ```
> <br>
<br>

```css
#styles.css
.canvas {
  width: 500px;
  height: 600px;
  background-color: #4d0f00;
  overflow: hidden;
  filter: blur(2px);
}
```
> **Step 35** <br>
Create a rule that targets both `.one` and `.two` and increase their `blur` effect by 1 pixel.

```css
#styles.css
.one, .two {
  filter: blur(1px);
}
```
> **Step 36** <br>
Increase the `blur` of `.three` by 2 pixels.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
  margin: auto;
  filter: blur(2px);
}
```
> **Step 37** <br>
The rectangles are too small and their edges don't have the soft quality of a painting.<br>
Increase the area and soften the edges of `.one` by setting its `box-shadow` to `0 0 3px 3px #efb762`.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762;
}
```
> **Step 38** <br>
Use the same `box-shadow` declaration for `.two`, but change the color from `#efb762` to `#8f0401`.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;margin-top: 0;
  margin-bottom: 20px;
  margin-left: auto;
  margin-right: auto;
  box-shadow: 0 0 3px 3px #8f0401;
}
```
> **Step 39** <br>
Add a `box-shadow` to `.three` with the values `0 0 5px 5px #b20403`.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
  margin: auto;
  filter: blur(2px);
  box-shadow: 0 0 5px 5px #b20403;
}
```
> **Step 40** <br>
The corners of each rectangle are still too sharp.<br>
Round each corner of the `.one` element by 9 pixels, using the `border-radius` property.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762;
  border-radius: 9px;
}
```
> **Step 41** <br>
Use the `border-radius` property on the `.two` selector, to set its top-left and bottom-right radii to `8px`, and top-right and bottom-left radii to `10px`.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;margin-top: 0;
  margin-bottom: 20px;
  margin-left: auto;
  margin-right: auto;
  box-shadow: 0 0 3px 3px #8f0401;border-radius: 8px 10px;
}
```
> **Step 42** <br>
The `border-radius` property accepts up to four values to round the top-left, top-right, bottom-right, and bottom-left corners.<br>
Round the top-left corner of `.three` by 30 pixels, the top-right by 25 pixels, the bottom-right by 60 pixels, and bottom-left by 12 pixels.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
  margin: auto;
  filter: blur(2px);
  box-shadow: 0 0 5px 5px #b20403;
  border-radius: 30px 25px 60px 12px;
}
```
> **Step 43** <br>
Rotate each rectangle to give them more of an imperfect, hand-painted look.<br>
Use the `transform` property on the `.one` selector to `rotate` it counter clockwise by 0.6 degrees.

```css
#styles.css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762;
  border-radius: 9px;
  transform: rotate(-0.6deg);
}
```
> **Step 44** <br>
Rotate the `.two` element clockwise by 0.4 degrees.

```css
#styles.css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;margin-top: 0;
  margin-bottom: 20px;
  margin-left: auto;
  margin-right: auto;
  box-shadow: 0 0 3px 3px #8f0401;border-radius: 8px 10px;
  transform: rotate(0.4deg);
}
```
> **Step 45** <br>
Rotate `.three` counter clockwise by 0.2 degrees.<br>
<br>
With this final step, your Rothko painting is now complete.

```css
#styles.css
.three {
  width: 91%;
  height: 28%;
  background-color: #b20403;
  margin: auto;
  filter: blur(2px);
  box-shadow: 0 0 5px 5px #b20403;
  border-radius: 30px 25px 60px 12px;
  transform: rotate(-0.2deg);
}
```