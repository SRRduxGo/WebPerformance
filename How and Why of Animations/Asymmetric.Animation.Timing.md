# [Asymmetric animation timing](https://developers.google.com/web/fundamentals/design-and-ux/animations/asymmetric-animation-timing)

> Asymmetric animation timing improves the user experience by allowing you to express personality while at the same time respond quickly to user interactions. It also provides contrast to the feel, which makes the interface more visually appealing.

## TL;DR

- Use asymmetric animation timing to add personality and contrast to your work.
- Always favor the user's interaction; use shorter durations when responding to taps or clicks, and reserve longer durations for times when you aren't.

> The rule of thumb is to always respond to a user interaction quickly. That said, most of the time the user's action is asymmetric, and therefore the animation can be, too.

## The general rule of thumb, then, is the following

- **_For UI animations `triggered by a user’s interaction`, such as view transitions or showing an element, have a `fast intro (short duration)`, but a `slow outro (longer duration)`_**
- **_For UI animations triggered by your code, such as errors or modal views, have a `slower intro (longer duration)`, but a `fast outro (short duration)`_**
