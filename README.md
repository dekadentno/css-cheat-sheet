# css-cheat-sheet
My cheat sheet for CSS

### Terminology 
* descendants - children + grandchildren + ... of
* children - only first level

### Important tips
* the browser is "reading" the CSS from top to bottom (cascade) - two identical selectors with different properties, the bottom one will win
* 

### Selectors
* ```#container``` - ID selector
* ```.container``` - class selector
* ```span``` - element selector
* ```span, div, p``` - multiple elements selector
* ```#container p``` - select ```p``` that is the descendant of ```#container```
* ```#container > p``` - select ```p``` that is the child od ```#container```
* ```h2 + p``` - adjacent selector, the one that comes directly after the ```h2```
* ```input[type="text"]``` - attribute selector
* ```span:hover``` - dynamic pseudo selector (behavior) - hover, presses, checked etc
* ```ul:nth-child(5)``` - structural pseudo selector (parent-child relationship) - 5th li tag, element without children etc.
* ```*``` - universal selector (mostly used to override default styles)

### Selector specific points
* ID - 100 points
* classes - 10 points
* elements - 1 point
* !important - overrides everything (try not to use this, rather write nice and clean code!)

# CSS properties
### Font size
* absolute - px
* relative - em, percentages - used when making responsive design

```css
.container {
  font-size: 12px;
}
article {
  font-size: 14px;
}
article h2 {
  font-size: 2em; /* inherit font size from article and miltiple it by 2 */
}
article p {
  font-size: 50%; /* inherit font size from article and take 50% of size */
}
```

### Font family
Note: some families already exist on user's computer. Remember to use the font family stack for fallbacks.
```css
.container {
  font-family: arial, helvetica, sans-serif; /* if arial is not available, use helvetica etc. */
}
```

### Text decoration
```css
/* text-decoration: inerhit line-through none underline overline inherit; */
.container {
  text-decoration: underline;
}
```
