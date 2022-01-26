## List Styling
### List specific styles
There are three properties that can be set to a ```<ul>``` or an ```<ol>``` tag
* ```list-style-type```: sets the type of bulets to be used for the list
* ```list-style-position```: sets whether the bullets, at the start of each item, appear inside or outside the lists. Default value is generally ```outside```.
* ```list-style-image```: Allows you to use a custom image for the bullet, rather than a simple square or circle.

### Controlling List Counting
Sometimes you might want to count differently on an ordered list — e.g., starting from a number other than 1, or counting backwards, or counting in steps of more than 1.
### start
The ```start``` attribute allows you to start the list counting from a number other than 1.
``` html
<ol start="4">
  <li>Toast pita, leave to cool, then slice down the edge.</li>
  <li>Fry the halloumi in a shallow, non-stick pan, until browned on both sides.</li>
  <li>Wash and chop the salad.</li>
  <li>Fill pita with salad, hummus, and fried halloumi.</li>
</ol>
```
This would start the numbering of ```li``` items from 4.

### reversed
The ```reversed``` attribute will start the list counting down instead of up.
### value
The ```value``` attribute allows you to set your list items to specific numerical values.

> CSS counters are advanced tools for customising list counting and styling, but they are complex.