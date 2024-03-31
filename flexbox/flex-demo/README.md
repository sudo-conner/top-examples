this is a follow along coding example from 'interneting is hard' about flexbox.
this guide covered flex containers and items, alignments, distribution, grouping, wrapping, ordering and more.

### some notes:
* display: flex; to make an element into a flex container; don't forget to add flex to each container
    * before we learned block, inline and inline-block
* justify-content: center; to center the items in your flex container
    * some other options are flex-start, flex-end, space-around, space-between
* align-items: center; to center items vertically
    * flex-start, flex-end, stretch, baseline
* flex-wrap: wrap; to wrap flex items down to another row instead of the row just going off screen
* flex-direction: column; to turn a flex row into a flex column instead. ie vertical
    * justify-content and align-items become switched when using column since the alignment axis is rotated
    * row-reverse and column-reverse can reverse the order of flex items, this is done on a row by row basis so the last item in a row will become the first in that row. not last item in the container becomes first on the first row.
    * order property can also be used to change order of flex items. default is 0, larger values move items to the end. This works across the whole container, not just the row that item happens to fall into

* align-self can be used for items within a container and will override the alignment set by align-items in the rules for the container
* flex property can be given to items to change how quickly they grow compared to other items in the container
    * flex property is shorthand for: flex-grow, flex-shrink, and flex-basis
    * flex-grow if only one number is given to flex, ie: flex: 1;, it is flex-grow
    * flex-shrink, number value for how much an item will shrink relative to other items
    * flex-basis, can be a %, px, or other length unit. specifies the length of the item
    * flex: auto; same as 1 1 auto
    * flex: initial; same as 0 1 auto
    * flex: none; same as 0 0 auto
