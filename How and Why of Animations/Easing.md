# [Easing](https://developers.google.com/web/fundamentals/design-and-ux/animations/the-basics-of-easing)

> **_Nothing in nature moves linearly from one point to another_**  
> _In reality, things tend to accelerate or decelerate as they move_  
> _Natural motion makes your users feel more comfortable with your apps, which in turn leads to a better overall experience_

## TL;DR

- Easing makes your animations feel more natural
- Choose `ease-out` animations for `UI elements`
- Avoid `ease-in` or `ease-in-out` animations unless you can keep them short
  - they tend to feel sluggish

> In classic animation, the term for motion that starts `slowly and accelerates` is `"slow in"` or `“ease in”`
> Motion that starts `quickly and decelerates` is `"slow out"` - `“ease out”`  
> Sometimes the two are combined, which is called `"ease in out"`  
> Easing, then, is really the process of making the animation `less severe or pronounced`

### Easing keywords

- CSS transitions and animations let you choose the `easing` you want
- Use `keywords` that affect the `easing` (or timing, as it's sometimes called)
- You can also go completely custom with your easing

  - Here are some of the keywords that you can use in CSS:
    - `linear`
    - `ease-in`
    - `ease-out`
    - `ease-in-out`

- `steps` keyword - Allows you to create transitions that have discrete steps
- keywords listed above are the most useful for creating animations that feel natural

## Linear animations

### Linear ease animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/linear.png"/>

- Animations `without` any kind of `easing` are referred to as `linear`
- As time moves along, the value increases in equal amounts
- With linear motion, things tend to feel robotic and unnatural
- To achieve the effect above with CSS, the code would look something like this:

```css
.linearAnimate {
  transition: transform 500ms linear;
}
```

## Ease-out animations

### Ease-out animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/ease-out.png"/>

- Animations start more quickly than linear ones
- It also has deceleration at the end
- `Easing out` best for user interface work

  - the fast start gives a feeling of responsiveness
  - while still allowing for a natural slowdown at the end

- the simplest is the `ease-out` keyword in CSS:

```css
.easeOutAnimate {
  transition: transform 500ms ease-out;
}
```

## Ease-in animations

### Ease-in animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/ease-in.png" />

- Ease-in animations start slowly and end fast
- From an interaction point of view ease-ins can feel a little unusual because of their abrupt
- Ease-ins effect of feeling sluggish when starting

  - negatively impacts the perception of responsiveness

- you can use its keyword:

```css
.easeInAnimate {
  transition: transform 500ms ease-in;
}
```

## Ease-in-out animations

### Ease-in-out animation curve

<img src="https://developers.google.com/web/fundamentals/design-and-ux/animations/images/ease-in-out.png" />

- Easing both in and out is akin to a car accelerating and decelerating
- Can provide a more dramatic effect than just easing out
- Do not use an overly long animation duration, because of the sluggishness of an ease-in start to the animation
  - Something in the range of 300-500ms is typically suitable
- Because of the slow start, fast middle, and slow end, there is increased contrast in the animation, which can be quite satisfying for users.
- To get an ease-in-out animation, you can use the ease-in-out CSS keyword:

```css
easeInOutAnimate {
  transition: transform 500ms ease-in-out;
}
```
