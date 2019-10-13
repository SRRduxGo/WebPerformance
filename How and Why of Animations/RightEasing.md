# [Choosing the Right Easing](https://developers.google.com/web/fundamentals/design-and-ux/animations/choosing-the-right-easing)

## TL;DR

- Use ease-out animations for UI elements
  - A [`Quintic`](http://easings.net/#easeOutQuint) ease-out
- Animation duration
  - `ease-outs` and `ease-ins` should be `200ms-500ms`
  - `bounces` and `elastic` `eases` should be of longer duration of `800ms-1200ms`

### A Quintic ease-out animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/quintic-ease-out-markers.png"/>

> An `ease-out` is a good default but with a nice slowdown at the end
>
> There is a group of well-known ease-out equations beyond the one specified with the `ease-out` keyword in CSS
>
> Other easing equations, particularly bounces or elastic eases, should be used sparingly, and only when it’s appropriate to your project

## Pick the right animation duration

- Too short and the animation will feel aggressive and sharp
- Too long and it will be obstructive and annoying.

- **_Ease-outs: around `200ms-500ms`_** - This gives the eye a chance to see the animation, but it doesn’t feel obstructive.
- **_Ease-ins: around `200ms-500ms`_** - Bear in mind that it will jolt at the end, and no amount of timing changes will soften that impact
- **_Bounce or elastic effects: around `800ms-1200ms`_** - You need to allow time for the elastic or bounce effect to "settle."
