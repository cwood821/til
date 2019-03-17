# Use `font-display: swap;` to render text in fallback font until @font-face font loads

When using the [@font-face](https://css-tricks.com/snippets/css/using-font-face/) in CSS, set the `font-display` property to `swap`. This will render text in the next available fallback font until the custom font has loaded. 

Here's a tweaked snippet from [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-display):
```css
@font-face {
  font-family: ExampleFont;
  src: url(/path/to/fonts/examplefont.woff) format('woff'),
       url(/path/to/fonts/examplefont.eot) format('eot');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}
```

This would then apply to this snippet:
```
p {
  font-family: "ExampleFont", "Helvetica", "Arial", sans-serif;
}
```

Learned from this [CSS Tricks article](https://css-tricks.com/font-display-masses/).
