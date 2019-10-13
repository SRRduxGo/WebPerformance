# Custom Easing

> Sometimes you won't want to use the easing keywords that are included with CSS, or you will be using Web Animations or a JavaScript framework. In these cases, you can typically define your own curves (or equations), and this provides a lot of control over the feel of your project's animations.

## TL;DR

- Custom easing allows you to give more personality to your projects
- You can create `cubic Bézier curves` that resemble the default animation curves (`ease-out`, `ease-in`, etc.), but **with emphasis in different places**
- Use JavaScript when you need more control over the animation timing and behavior, for example, `elastic` or `bounce` animations.
- If you're `animating` with `CSS`, you'll find that you can define `cubic Bézier curves` to define the timing

  - the keywords `ease`, `ease-in`, `ease-out`, and `linear` map to `predefined Bézier curves`
    - detailed in the CSS transitions specification and the Web Animations specification

- These `Bézier curves` take `four values`, or `two pairs of numbers`

  - Each pair describes the `X` and `Y` coordinates of a `cubic Bézier curve’s` control points
  - The `starting point` of the `Bézier curve` has `coordinates` `(0, 0)` and the `ending point` has `coordinates` `(1, 1)`

    - you get to set the `X` and `Y` values of the `two control points`
    - The `X` values for the `two control points` must be **`between 0 and 1`**
    - Each control point’s `Y` value can exceed the `[0, 1]` `limit`
      - The spec isn’t clear by how much.

  - Changing the `X` and `Y` value of each `control point` gives you a _vastly different curve_

  > For example, if the first control point is in the lower right area, the animation will be slow to start. If it’s in the top left area, it’s going to be fast to start. Conversely, if the second control point is in the bottom right area of the grid, it’s going to be fast at the end; if it’s in the top left, it will be slow to end.

### For comparison, here are two curves: a typical _ease-in-out_ curve and a _custom_ curve

#### Ease-in-out animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/ease-in-out-markers.png"/>

#### Custom animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/custom.png"/>

- The CSS for the custom curve is

```css
.customAnimate {
  transition: transform 500ms cubic-bezier(0.465, 0.183, 0.153, 0.946);
}
```

- The first two numbers are the `X` and `Y` `coordinates` of the `first` `control point`
- The second two numbers are the `X` and `Y` `coordinates` of the `second` `control point`
- Making a custom curve gives you significant control over the feel of the animation.

> For example, given the above curve, you can see that the curve resembles a classic ease-in-out curve, but with a shortened ease-in, or "getting started," portion, and an elongated slowdown at the end.

[Good tool to test values](https://googlesamples.github.io/web-fundamentals/fundamentals/design-and-ux/animations/curve-playground.html)
