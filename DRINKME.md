# CSS TEA

## Box sizing

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

## Rythmic cohesion

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

## Scalable units
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

## Responsive Images

* [Making images responsive](https://www.w3schools.com/css/css_rwd_images.asp)

```css
img {
    max-width: 100%;
    height: auto;
}
```

## Media

* [The media object saves hundred of lines of code](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/)
* [The media object, a bunch of ways](https://css-tricks.com/media-object-bunch-ways/)
* [The flag object](https://csswizardry.com/2013/05/the-flag-object/)

Implementation from [Solved by Flexbox](https://philipwalton.github.io/solved-by-flexbox/demos/media-object/)

```css
.Media {
  display: flex;
  align-items: flex-start;
}

.Media-figure {
  margin-right: 1em;
}

.Media-body {
  flex: 1;
}