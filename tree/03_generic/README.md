# Generic
For globals and wild cards.

## Boxes

### Box sizing

* [Understanding box-sizing](https://zellwk.com/blog/understanding-css-box-sizing/)

```css
html {
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}
```

## Typography

### Rythmic cohesion

* [Axiomatic CSS and lobotomized owls](https://alistapart.com/article/axiomatic-css-and-lobotomized-owls)

Implemention code from the article above :  

```css
* + * {
	margin-top: 1.5em;
}

.compact * + * {
	margin-top: 0.75em;
}

.margins-off > * {
	margin-top: 0;
}
```

### Scalable units
* [Comprehensive guide to REM and EM units](https://webdesign.tutsplus.com/tutorials/comprehensive-guide-when-to-use-em-vs-rem--cms-23984)

Implementation code from [Knacss](https://knacss.com) :

```css
html {
  /* set base font-size to equiv "10px", which is adapted to rem unit */
  font-size: 62.5%;
  /* IE9-IE11 math fixing. See http://bit.ly/1g4X0bX */
  /* thanks to @guardian, @victorbritopro and @eQRoeil */
  font-size: calc(1em * 0.625);
}

body {
  font-size: 1.4rem;
  line-height: 1.4;
}
```