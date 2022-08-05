 # Basic-Biography-Web-Application
This is my first bio app about Leonardo Da Vinci biography. I applied CSS Background Patterns skills, Flexbox skills, \
and media queries skills to this web app.\
\
\
##CSS Background Patterns skills\
Patterns are a fantastic way to add a significant effect to a website architecture. They also don\'92t require an excessive amount of effort.\
Background patterns increase the attractiveness of a website.\
The first thing that needs to be mastered in order to create patterns using CSS is the linear-gradient function that CSS3 provides. \
The linear-gradient function can be used in several ways, by tweaking multiple properties, but the most basic usage is the one wherein we specify \
the starting color and the ending color like so:\
background: linear-gradient(<starting-color>, <ending-color>, ...<other-colors>);\
###Basic patterns\
####Two-color symmetric gradient\
The intermediate colors are filled in between depending on the size of the div. We are not specifying any dimensions here, so the two colors meet at the center:\
background: linear-gradient(#e66465, #9198e5);\
####Two-color asymmetric gradient\
Along with the color value, we can provide a percentage value which represents the color stop point for that color in percentage units. In that case, that much percentage of the area is taken by that solid color and the remaining with the rest of the colors.\
background: linear-gradient(#e66465 80%, #9198e5);\
####Two-color solid pattern\
If we provide percentage values to both the colors, instead of a gradient, we get a solid color combination of this kind. Where the first solid color spans from 0 to 80 percent and the second one from 80 to 100.\
background: linear-gradient(#e66465 80%, #9198e5 80%);\
####Two-color directional pattern\
There is a slight variation of this function which also lets us configure the direction in which the pattern gets generated. For instance, supplying a to right value as the first argument makes the pattern appear from left to right instead of the default top to bottom. Other valid values are: to left, to top, to bottom, to bottom left, etc.\
background: linear-gradient(to right, #e66465, #9198e5);\
####Multi-color patterns\
Just like the previous examples that used two colors, we can supply as many numbers of colors we like and get those beautiful gradients just as easily. Here is an example:\
background: linear-gradient(#3f87a6, #ebf8e1, #f69d3c, #561423);\
Also, in addition to specifying the direction using the to syntax that we used before, there are other ways of achieving the same result.\
Supplying an angular value as the first argument means the gradient gets rotated accordingly. Supplying an angular value of 180 degrees keeps the pattern as is.\
background: linear-gradient(30deg, #3f87a6, #ebf8e1, #f69d3c, #561423);\
The second method is a fraction to the turn units, like 0.25turn.\
background: linear-gradient(0.33turn, #3f87a6, #ebf8e1, #f69d3c, #561423);\
###Intermediate patterns\
####Vertical bars\
background-color: #00ccd6;\
background-image: linear-gradient(90deg, transparent 50%, rgba(255,255,255,.5) 50%);\
background-size: 20px;\
####Checkerboard pattern\
background-color: #e66464;\
background-image: linear-gradient(to right, transparent 50%, rgba(255, 255, 255, 0.5) 50%),\
linear-gradient(to bottom, transparent 50%, rgba(255, 255, 255, 0.5) 50%);\
background-size: 20px 20px;\
####Polka Dot pattern\
body \{\
  background-image: radial-gradient(red 20%, transparent 20%),\
      radial-gradient(yellow 20%, transparent 20%);\
  background-color: green;\
  background-position: 0 0, 50px 50px;\
  background-size: 100px 100px;\
\}\
\
\
##CSS Flexbox Layout Module
The flex container becomes flexible by setting the display property to flex: 
.flex-container \{\
  display: flex;\
\}\
The row value stacks the flex items horizontally (from left to right):\
.flex-container \{\
  display: flex;\
  flex-direction: row;\
\}\

## Media Queries

Responsive Flexbox
.flex-container \{\
  display: flex;\
  flex-direction: row;\
\}\
\
/* Responsive layout - makes a one column layout instead of a two-column layout */\
@media (max-width: 800px) \{\
  .flex-container \{\
    flex-direction: column;\
  \}\
\}\
}
