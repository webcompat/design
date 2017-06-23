# Layout Grid system

Our Layout System is based on a 3x1 grid and the flow of the containers is defined for 3 different resolutions:
Desktop, Tablet, Mobile

Desktop: min-width 900px + 19px margin + 30 px padding
Tablet: min-width 585px + 15px margin + 25px padding
Mobile: min-width 270px + 9px margin + 15px padding

Please note that the margins and paddings are *2 for both sides.

The min-width for a container is 270px, next is 585px, next step 900px.

All containers are responsive.

All modules for the living style guide as well as webcompat.com will be build upon that Grid System.

The Living Style Guide (LSG) can be found in the [docs/](https://github.com/webcompat/design/tree/master/docs) folder of this repository and is published as [gh-pages](http://webcompat.github.io/design/ ). 


## Technology

After creating a POC with CSS Grid, we've decided against CSS Grid. There are too many trade offs like 
e.g. need of usage for media queries as we want the span of a column to change with a specific resolution or the browser 
support at the moment and the need for pollyfills / hacky workarounds.

As CSS Flexbox is more established and solves e.g. the span of a column change out of the box, we've decided to go with 
this technology.
