## Implicit and Explicit Grid
explicit grid is the one created using ```grid-template-columns``` and ```grid-template-rows```.
implicit gird is created when the content is placed outside that gird, such as into our rows.

to size the tracks of implicit grid, you can use ```grid-auto-rows``` and ```grid-auto-columns``` properties.

## repeat() function
while setting up the columns grid, you need to to make 10 columns of same size. To achieve this, you can use 
```grid-template-columns: repeat(3,1fr)```.

## The minmax() function
sizing the tracks won't be very useful if we add content into those tracks that is taller than 100 pixels, in which case it would cause an overflow.
The ```minmax()```` function lets us set a minimum and maximum size for a track, for example, ```minmax(100px, auto)```. The minimum size is 100 pixels, but the maximum is auto, which will expand to accomodate more content.

## As many columns as will fit
Somtimes to create as many columns as will fit into the container, we use ```grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));```