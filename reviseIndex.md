

# Section-8
# 48 CSS Display
### About display property
- display:block
    - Entire page ki width leta
    - u can change height and width of an element.
- display:inline
    - element ke content ke hisab se width leta
    - same page par rehta
    - u can't change height and widht of an element.
- display:inline-block
    - multiple element same line par hi chalenge
    - u can set height and width of an element
    - but particular element ki width badh gyi to next line par aa javenga.
- display:none
    - element ko hide karta web-page se.
# 49. CSS Float
- Wrap text around ke liye use kare float property
    - float:left
    - float:right
- ek mek se separate karne ke liye use
    - float:left and float:right
    - so dono element exactly separate ho javenge.
- Clear property
    - Yadi aapko float nhi karwana particular element so use clear property
    - clear:left
    - clear:right
    - clear:both
# 50. How to create a responsive website.
- Theory knowledge
# 51. Media Queries
- Adding breakpoints to define responsive layout.
- Breakpoints bole toh condition in media query
    - isse bada ya chota screen-size hua tab hum kya kare.
- max-width:600px
    - maximum width is upto 600px
    - screen-size <= 600px
- min-width:600px
    - minimum width is 600px
    - screen-size >=600px
- Combination
    - hum combine kar sakte minimum and maximum width
- Devise
    - Printing mein landscape orientatino dene ke liye use hota hai.
    - but not recommended.

# Section-9 Flexbox
# 54. Display Flex
- Layout via Html
- Layout via CSS
    - Via absolute positioning
    - Problem with Absolute positioning
- Float
- When to use flexbox and when to use float.
- Design a website via flexbox
- 2 version of flexbox container.
    - Inline-flex
    - flex
# 55. Flex-Direction
- Flex direction  :   row/column
- Main-axis   (
    - flex-direction:row 
        - then  main-axis is at horizontal axis
        - and element goes from left to right
	- flex-direction:column 
        - then main-axis is at vertical axis
        - and element goes from top-bottom
- Cross-axis  
    -  (it is perpendicular to main-axis)
	- ( behviour you predict)
- Flex-basis – 
    - (increase width 
        - Fd:row  main-axis horizon)                         
    - (increase height
        -   FD-col  mani-axis vertical
# 56. Flex-Layout
-	***About parent child terminology****
    -   Parent mane container
    -   Child mane flexitems
- 1)***Order property***
    -	Applicable on child mane flexitem
- 2)***flex-wrap property***
    - The default behaviour of flexbox
    - Flex-wrap: wrap/wrap-reverse/nowrap
    -  About it’s axis
-	3)***justify-content property***
    -   About axis
    -   Justify-wrap: flex-start/flex-end/center/space…
-	4)***align-item property***
    - About viewport height
    -   Align-item: flex-start/flex-end ….
    -	About align-self property
-	5)***align-content***
    -   Align-content:flex-start …..
    -   Diff between align-item and align-content

# Section-11
# 64. What is bootstrap?
- ***Why bootstrap became so popular?***
    - Pre-made css jisse pre-build component aur styling use kar pave
    - 12 column layout sys
- ***Konse framework ke upar bana hai bootstrap?***
	- Flexbox 
- ***What is CDN?***
	- Little hub  across world.. Jo content jaldi rendere karave.
- ***How to use bootstrap?***
	- Include it’s link in head section
    - and regarding functionality include script before /body tag
- ***How to override bootstrap css?***
	- Inline
	- Internal 
	- External par ye bootstrap ke link ke niche include karna tabhi work karnega.
# 65. BootStrap layout
## Feature of Bootstrap:
- 12 col layout system.
- Autofit
- Bootstrap container is used for creating responsive website
- Sized col
- boostrap breakpoints
- multiple breakpoint
- mix and match
# 65. Bootstrap components