- [Overview](#overview)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

### Screenshot

![](./screenshot.jpg)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- SASS
- float
- Mobile-first workflow

### What I learned

```html
<h1>Some HTML code I'm proud of</h1>
```

```css
.shoe-red {
  --clr-inner: #faa700;
  --clr-outer: #e48d00;
  --clr-accent: #a1173c;
}

.shoe-white {
  --clr-inner: #fce4b3;
  --clr-outer: #eac886;
  --clr-accent: #2f4858;
}

.shoe-blue {
  --clr-inner: #6dd5ed;
  --clr-outer: #2193b0;
  --clr-accent: #008591;
}

.product {
  background: radial-gradient(
    var(--clr-inner, limegreen),
    var(--clr-outer, purple)
  );
  padding: 3rem;
  border-radius: 3em;
  margin-bottom: 5rem;
  text-align: center;

  &__title {
    font-size: clamp(3rem, calc(5vw + 1rem), 5.5rem);
    line-height: 1;
    text-transform: uppercase;
    color: #fff;
    text-shadow: 0 0 0.2em rgba(#000, 0.2);
  }

  &__image {
    margin: -5rem 0 0 0;
  }

  @media (min-width: 45em) {
    text-align: left;
    &__title {
      margin: 0;
    }

    &__image {
      float: right;
      width: 65%;
      shape-outside: url(./img/shoe-1.png);
      shape-margin: 1em;
      margin: 0 -5rem 0 0;
    }
  }

  &.shoe-left {
    text-align: right;
    .product__image {
      float: left;
      shape-outside: url(./img/shoe-2.png);
      shape-margin: 1em;
      margin: 0 0 0 -5rem;
    }
  }
}
```

### Useful resources

- [shape-outside](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-outside)
- [shape-margin](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-margin)

## Author

- Website - [Leo Ma](https://frosty-swartz-dafd0f.netlify.app/)
