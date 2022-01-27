## Float
The floating element is taken out of the normal layout flow of the document and stuck to the desired position say left, of its parent container. Any content that would come below the floated element in the normal layout flow will now wrap around it filling up the free space.

In the attached html and css files, we could add margin to the floating element and push the text away from it but we cannot add margin to the text to move it away from the element since the text run behinds the float. 
## Clearing floats
To stop an element from floating around a flot element, we can use ```clear``` property
It accepts 3 values:
* left: Clear elements floated to left.
* right: Clear elements floated to right.
* both: Clear any floated elements.
## Clearing boxes wrap around a float
if you want the box to wrap jointly around the floated item as well as the text of the first paragraph that wraps around the float, while also having the following content cleared of the box. This won't happen since the box is floated. [check out the html/css file for more info]
Two solve this problem we have 3 ways.
### The Clerfix Hack
Insert some generated content after the box that contains both float and content wrapped around it, then set the generated conent to clear both.

``` css
.wrapper::after{
    content:"";
    clear:both;
    display:block;
}
```
### overflow property
Another method to solve the problem is to set ```overflow:auto```.
``` css
.wrapper{
    overflow:auto;
}
```
### display: flow-root;
The best and the modern method to overcome this problem is using ```display:flex-kit```
``` css
.wrapper{
    display:flow-root;
}