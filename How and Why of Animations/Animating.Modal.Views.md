# Animating Modal Views

> **_Modal views are for important messages, and for which you have very good reasons to block the user interface._**
>
> **_Adding some animation will bring them to life_**

## TL;DR

- Use modal views sparingly
- Adding `scale` to the `animation` gives a nice `"drop on"` effect
- Get rid of the `modal` view `quickly` when the user dismisses it
- _Bring the modal view onto the screen a little more slowly so that it doesn't surprise the user_

- The modal overlay should be aligned to the `viewport`, so set its `position` to `fixed`:

```css
.modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;

  pointer-events: none;
  opacity: 0;

  will-change: transform, opacity;
}
```

- It has an initial opacity of `0`, so it's hidden from view

  - It also needs `pointer-events` set to `none` so that `clicks and touches pass through` - It animates its `opacity` and `transform`, they are marked as changing with `will-change`

- When the view is visible, it needs to accept interactions and have an `opacity` of `1`:

```css
.modal.visible {
  pointer-events: auto;
  opacity: 1;
}
```

- Now whenever the modal view is required, you can use JavaScript to toggle the `"visible"` class:

```js
modal.classList.add("visible");
```

- At this point, the modal view appears without any animation, so you can now add that in;

```css
.modal {
  transform: scale(1.15);

  transition: transform 0.1s cubic-bezier(0.465, 0.183, 0.153, 0.946), opacity
      0.1s cubic-bezier(0.465, 0.183, 0.153, 0.946);
}
```

- Adding `scale` to the `transform` makes the view appear to drop onto the screen slightly
- The default `transition` applies to both `transform` and `opacity` properties with a `custom curve` and a duration of `0.1` seconds
  - The duration is pretty short, ideal for when the user dismisses the view
  - But too aggressive for when the modal view appears. let's fix this

```css
.modal.visible {
  transform: scale(1);
  transition: transform 0.3s cubic-bezier(0.465, 0.183, 0.153, 0.946), opacity
      0.3s cubic-bezier(0.465, 0.183, 0.153, 0.946);
}
```

- Now the modal view takes `0.3` seconds to come onto the screen
