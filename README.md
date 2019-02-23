# css-cheat-sheet
My cheat sheet for CSS

### Terminology 
* descendants - children + grandchildren + ... of
* children - only first level

### Important tips
* the browser is "reading" the CSS from top to bottom (cascade) - two identical selectors with different properties, the bottom one will win
* 

### Selectors
* #container - ID selector
* .container - class selector
* span - element selector
* span, div, p - multiple elements selector
* #container p - select '''p''' that is the descendant of '''#container'''
* #container > p - select '''p''' that is the child od '''#container'''

### Selector specific points
* ID - 100 points
* classes - 10 points
* elements - 1 point
* !important - overrides everything (try not to use this, rather write nice and clean code!)
