# [Animations](https://developers.google.com/web/fundamentals/design-and-ux/animations)

## Avoid animating expensive properties

- Worst Animations - that cause the page to stutter.

  - This type of animation leaves users feeling frustrated and unhappy

- Some properties are more expensive to change
  - More likely to make things stutter
  - Example, changing the `box-shadow` of an element
    - Requires **`expensive paint operation`** than changing, say, its `text color`
  - Example, changing the `width` of an element is **`more expensive`** than changing its `transform`

## CSS Vs Javascript Animation

> What kind of Animation to choose depends on the other dependencies of your project, and what kinds of effects you're trying to achieve.

### TL;DR

- CSS animations - for simpler "one-shot" transitions, like toggling UI element states

- JavaScript animations - when you want to have advanced effects like bouncing, stop, pause, rewind, or slow down.

  - Use the Web Animations API or a JS modern framework

- For Most basic animations USE either CSS or JavaScript

  - The amount of effort and time differs Each has its pros and cons

#### Some guidelines

- Use CSS when you have smaller, self-contained states for UI elements

  - CSS transitions and animations - Use for bringing a navigation menu in from the side, or showing a tooltip
  - May end up using JavaScript to control the states
  - Animations themselves will be in your CSS

- Use JavaScript when you need significant control

  - The Web Animations API is the standards-based approach, available today in most modern browsers (experimental)
  - JavaScript is also useful when you need to stop, pause, slow down, or reverse your animations
  - Use `requestAnimationFrame` directly when you want to orchestrate an entire scene by hand
    - Useful if you're building a game or drawing to an HTML canvas

## Animate with CSS

- Animating with CSS is declarative, because you specify what you'd like to happen

- Example Below is some CSS that moves an element `100px` in both the `X` and `Y` axes
  - Used a CSS transition that's set to take `500ms`
  - When the `move` class is added, the `transform` value is changed and the transition begins

```css
.box {
  transform: translate(0, 0);
  transition: transform 500ms;
}

.box.move {
  transform: translate(100px, 100px);
}
```

- Besides the `transition's duration`, There are options for _`the easing`_, which is essentially how the animation feels.

  - [see The Basics of Easing guide](https://developers.google.com/web/fundamentals/design-and-ux/animations/the-basics-of-easing)

- use JavaScript to toggle each animation on and off:

```js
box.classList.add("move");
```

- You can focus on managing state with JavaScript, and simply set the appropriate classes on the target elements
- Leaving the browser to handle the animations
- you can listen to `transitionend` events on the element

```js
var box = document.querySelector(".box");
box.addEventListener("transitionend", onTransitionEnd, false);

function onTransitionEnd() {
  // Handle the transition finishing.
}
```

- you can also use CSS animations
  - Allows much more control over individual animation `keyframes`, `durations`, and `iterations`

> Note: If you’re new to animations, `keyframes` are an old term from hand-drawn animations
>
> Animators would create `specific frames for a piece of action`, called `key frames`, which would capture things like the most extreme part of some motion, and then they would set about `drawing all the individual frames in between the keyframes`
>
> We have a similar process today with CSS animations, where we instruct the browser what values CSS properties need to have at given points, and it fills in the gaps

### Example

```css
.box {
  /*Choose the animation*/
  animation-name: movingBox;

  /*The animation’s duration*/
  animation-duration: 1300ms;

  /*The number of times we want
the animation to run */
  animation-iteration-count: infinite;

  /*causesthe animation to reverse
 on every odd iteration */
  animation-direction: alternate;
}

@keyframes movingBox {
  0% {
    transform: translate(0, 0);
    opacity: 0.3;
  }

  25% {
    opacity: 0.9;
  }

  50% {
    transform: translate(100px, 100px);
    opacity: 0.2;
  }

  100% {
    transform: translate(30px, 30px);
    opacity: 0.8;
  }
}
```

- With CSS animations you define the animation itself independently of the `target` element
- Use the `animation-name` property to choose the required animation
- If you want your CSS animations to work on older browsers, you will need to add vendor prefixes

## Animate with JavaScript and the Web Animations API

- JavaScript animations are imperative, as you write them inline as part of your code
- You can also encapsulate them inside other objects

```js
var target = document.querySelector(".box");
var player = target.animate(
  [{ transform: "translate(0)" }, { transform: "translate(100px, 100px)" }],
  500
);
player.addEventListener("finish", function() {
  target.style.transform = "translate(100px, 100px)";
});
```

- By default, `Web Animations` **only modify** the `presentation` of an element
  - If you'd like to have your object remain at the location it has moved to, then you should modify its underlying styles when the animation has finished, as per the snippet above

### With JavaScript animations

- you can slow down animations
- pause them
- stop them
- reverse them
- manipulate elements
