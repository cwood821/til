# Load animations based on user preference

For accessibility in CSS, we can choose to animate elements or not by checking the `prefers-reduced-motion` media query value.

A handy suggestion for some contexts, apply this at the file level and do not load the animation css when not needed: 

```html
<link rel="stylesheet" href="animations.css"
      media="(prefers-reduced-motion: no-preference)">
```

Code from [this Google post](https://web.dev/prefers-reduced-motion/)

See [this article](https://css-tricks.com/revisiting-prefers-reduced-motion-the-reduced-motion-media-query/) on CSS Tricks for further discussion.