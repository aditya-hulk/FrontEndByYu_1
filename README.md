# Section-1
# 5. How does internet actually works?
# Section-2
# 11. What is HTML?

# Section-3
# 13. What are webpages?
![alt text](image.png)![alt text](image-1.png)
### A website contain multiple webpages. We provide link between multiple pages in a website.
![alt text](image-2.png)
# 14. The Html boiler plate.
![alt text](image-3.png)
### Doctype declaration
<! DOCTYPE html> -- doctype declaration  
- Aap konse type ka doctype use kar rahe ho 
![alt text](image-4.png)
### Root of Doc is html
- we use language for read out website
![alt text](image-5.png)
### About Head tag
![alt text](image-6.png)
- Head doesn’t include any content that user  can see
- Meta tag – for charcter set encoding of the web page
- UTF-8 jo character aapke use ho rahe hai wo website mein  display ho correctly
    -  kuch Charaset mein emoji allow nhi hai
    - kuch mein multiple, division ye sysmbol allow nhi hai
### About Body
- Body tag mein aall of the website content goes here
    -  like text,  images etc
![alt text](image-7.png)![alt text](image-8.png)
### About shortcut
! + Enter shortcut 
- but remember
    - ye sirf .html website ke liye kaam karta
### Some other stuff
![alt text](image-9.png)
- This line keep your html compatible with internet explorer

![alt text](image-10.png)
- How you display/render website when it first open
# 28. Project portfolio webiste
jazz this up - to make sth more intresting and attractive
# 29. Hosting your website
![alt text](image-11.png)
### About Web hosting?
 - It is basically a process of Making your website available anywhere on the internet.
 #### 1. Local Developement
 ![alt text](image-12.png)
 #### 2. Hume Webhosting ke liye isse dalna honga webserver par
 ![alt text](image-13.png)
 ### Git Hub
 ![alt text](image-14.png)
 #### 1. About uploading the content
 ![alt text](image-15.png)![alt text](image-16.png)![alt text](image-17.png)
 - About index.html  
    - ye lower case hi hona chahiye
    - index.html ki karya karenga,home.html ya etc nahi
- About folder
    - folder drag nhi karna sirf content
    - nhi to kaam nhi karenga
- Then clk on commit change
### Now Branch change
![alt text](image-18.png)![alt text](image-19.png)![alt text](image-20.png)
- Change to main branch
    - clk on save
    - then refresh it 
    - it will take some time

![alt text](image-21.png)
https://aditya-hulk.github.io/html-portfolio/
# 30 Capstone project
- Banda ye web devloper hai
- apne portfolio mein bata raha hai, 
    - ki maine falana company ke sath kaam kiya
- client hier karte waqt uski achievements dekhenga 
- That's exactly the capstone project

![alt text](image-25.png)
### Use git hub for that
![alt text](image-26.png)![alt text](image-27.png)
![alt text](image-28.png)
# 31 Instruction
![alt text](image-22.png)![alt text](image-23.png)![alt text](image-24.png)

# Section-7 Intermediate CSS
# 43. The Cascade Specificity and Inheritance
### Hume yaha ye dekhenge ki Yadi aapke element par 1 se jyada rule apply ho rahe hai, toh exactly konsa rule uske liye applicable honga.
![alt text](image-29.png)
### Observe:
![alt text](image-30.png)
- Yadi hum pool ko observe kare
- so top level rule i.e No 2 ye sarvapratham apply honga
- But water level niche jate jate Number-1 rule ye applicable honga.
- and user ko No-1 rule dikhenga
### ***Category which define level of Importance***
![alt text](image-31.png)
### ***Position***
![alt text](image-32.png)
#### yaha blue override karenga red color ko since wo niche apply hai.
![alt text](image-33.png)
#### Yaha green applicable honga, since lower down position par hai. So In position rule, lower down position has more importance.
### ***Specificity***
 ![alt text](image-34.png)
 - So Id selector has more importance than above selectors.
 ### ***Type***
 ![alt text](image-35.png)
 ### ***Importance***
 ![alt text](image-36.png)
 ### ***Hierarchy***
 ![alt text](image-37.png)
 -  Importance has higher priority than anything above.
 - Then type, then speicificity and last Position
 ### Ab yadi mix-match mein chije aayi so aapko ye chart dhyan mein rakhna honga
 ![alt text](image-38.png)
 - Yeh code mein specificity category mein id selector dikh raha hai
 - aur yaha type category  inline css hai
- type category ye specificity category se important hai
- so in this case inline css ka rule applicable honga.
- so color will be green 
# 44. Combining CSS Selectors
### ***Group rule for CSS Selectors***
- yadi aapko ek se jyada selectors par same rule apply karna hai 
    - tab ye Group rule apply kare.

![alt text](image-39.png)
- for differntiating multiple selectors use comma
### ***Child rule for CSS slectors***
- ye rule direct desendents par applicable hota.
    - mane direct child ko aapko target karna ho tab child rule apply kare.

![alt text](image-40.png)
```html
<body>
  <div class="flag">
    <p>The Flag</p>
    <div>
      <div>
        <p>of Laos</p>
      </div>
    </div>
  </div>
</body>
````
- Upar eg mein Parent div ke direct child kon konse hai
    - p para tag
    - div tag
### So in order to target this we can use this Child rule.
```html
.flag > div{
    background-color=green;
}
```
#### Important tips regarding Child rule Selector
![alt text](image-41.png)
- so here 1st seletor is parent 
- 2nd selector is child 
- this rule is applicable for direct children
    - not on grand chidren or great grand chidren.
- This relation only 1 generation deep
### ***Descendent Rule for CSS selectors***
![alt text](image-42.png)![alt text](image-43.png)![alt text](image-44.png)
- provide space in multiple selectors
```html
<body>
  <div class="flag">
    <p>The Flag</p>
    <div>
      <div>
        <p>of Laos</p>
      </div>
    </div>
  </div>
</body>
```
#### Yadi aapko target karna hai paragraph tag ko wo bhi of Laos wali so we apply this rule.

```html
 .flag  div div p{
      color: yellow;
    }
```
### ***Chaining Rule for CSS Selectors***
![alt text](image-45.png)![alt text](image-46.png)
#### Important note
#### uprokta tag ko khangale so hume usme 3 selecotor mil rahe hai
![alt text](image-47.png)
#### So chain rule applicable karte waqt sarvapratham element selector aayenga uske baad class/id selector
### Why?
#### Aapne yadi pehle class selector likhe aur uske baad element selector
![alt text](image-48.png)
#### Ab ye class selector .big and element selecotor i.e h1 ko separate nhi padenga aur .bigh1 ye combine kar padenga
#### so ye ab dhundenga is name ki class jo milengi nhi, isiliye in chain rule use this concept.
### ***Combining combiners***
![alt text](image-49.png)
#### Aap differnt combination like 
- parent-child with desendents etc combine kar sakte
```html
<body>
  <div class="flag">
    <p>The Flag</p>
    <div>
      <div>
        <p>of Laos</p>
      </div>
    </div>
  </div>
</body>
```
#### yaha hum parent-child aur desendents selector combine kar rahe hai.
```html
.flag  > div div p{
      color: yellow;
    }
```
# 45. CSS positioning
### When developer dosen't understand the concept of positioning Then this haapen's.
![alt text](image-50.png)
### Types of positioning
![alt text](image-51.png)
### For understanding positioning go to this website
https://appbrewery.github.io/css-positioning/
### ***Static Positioning***
![alt text](image-52.png)![alt text](image-53.png)![alt text](image-54.png)
- static positon lagane ki jarurat nhi padti
- by default applicable hoti hai.
- aap isme kuch aur element add karo wo prvious element ke niche aa javenga
### ***Relative positioning***
![alt text](image-55.png)
#### Pehle by default static position kaise thi
![alt text](image-56.png)
#### After htting relative position button
![alt text](image-57.png)
#### Remember
![alt text](image-58.png)
- Relative to supposed location
- static position par image aise thi..
- relative par left aur top se differntiate ho gyi.
### Note:
- Static position ye html ki default positon hoti hai
- Mane ab aapko position lagana hai so bacha relative aur absolute
### ***Absolute position***
![alt text](image-59.png)
### 1. Position relative to nearest position anscestor
![alt text](image-60.png)
### 2. But yadi anscestor ki position set nhi hai, tab wo web page ke top left corner par aa javenga
![alt text](image-61.png)
### Observe: Yaha itne sare ansector hai, kahi bhi position set nhi hai; that's why come to top corener
![alt text](image-62.png)![alt text](image-63.png)
- So top se 50px aur left se 50px push hua hai
### ***Z-Index***
#### konsa element top par avenga here that's we specify in z-index
![alt text](image-64.png)
#### About z-axis
![alt text](image-65.png)
#### Now provide z-index
![alt text](image-66.png)
#### Eg- Abhi ye abosolute block sab ke upar dominate kar raha hai
![alt text](image-67.png)
#### hum iski z-index property negative kar dete
![alt text](image-68.png)
#### Note: har element ka Z-index 0 hota hai
### ***Fixed position***
![alt text](image-69.png)
#### Diff in Absolute and Fixed
- absolute position is top left of web page
- fixed postion is top left of browser window
- ye position fixed hi rehti kitna bhi scroll karlo, but absolute  position  fixed nhi rehti.
#### Aaap top left bhi kar sakte ho
![alt text](image-70.png)
#### aap margin bhi add kar sakte ho
![alt text](image-71.png)
#### Note:
The position is actually separate from the margin, which in turn is separate from the padding,
which in turn is separate from the width and the height.
### ***How to create a circle in CSS***
#### Create a rectangle
![alt text](image-72.png)
#### Use border radius property - yaha thoda tild hua
![alt text](image-73.png)
#### aaple logo
![alt text](image-74.png)
#### circle
![alt text](image-75.png)
### Program solution
- Now notice these numbers that I've given here 150px, 250px,
- basically they are half, 250 is half of 500
and 150 is half of 300.
- Essentially, I wanted the top left corner of this circle to be right in the middle of the rectangle.
- Alternatively to setting these pixel values, you could have also set it to 50% from the top and 50%
from the left.
- It would achieve exactly the same thing.

# Section-8 Advanced CSS
# 48. CSS Display
![alt text](image-77.png)
### Here we basically focus on website layout.
![alt text](image-78.png)
### what happen when display value is inline.
![alt text](image-80.png)
### About Display property
![alt text](image-81.png)
### What happen when display having block value?
![alt text](image-82.png)
### What happen when display having inline value?
![alt text](image-83.png)
### What happen when display having inline-block value?
![alt text](image-84.png)![alt text](image-85.png)
### What happen when display having none value?
![alt text](image-86.png)
### Go to this website
https://appbrewery.github.io/css-display/ 
### In website we have follwing things.
![alt text](image-87.png)
#### Regarding block u can change height and width
![alt text](image-88.png)
#### for inline - nothing is going to change
![alt text](image-89.png)
#### Regarding inline-block
##### U can change height and width but same line par chalenga
![alt text](image-90.png)
##### Par element ki width badh gyi to next line par javnega
![alt text](image-91.png)
# 49. CSS Float
![alt text](image-92.png)![alt text](image-93.png)![alt text](image-94.png)
### Use float property to wrap text around 
#### via float:left
![alt text](image-95.png)
#### via float:right
![alt text](image-96.png)
### About image and paragraph element
![alt text](image-97.png)![alt text](image-98.png)
### About clear property
![alt text](image-99.png)
#### aapko footer par float property set nhi chaiye
![alt text](image-100.png)
### What happen if you apply float property 
![alt text](image-101.png)
#### Observation: Abhi image ke baju mein paragrapy aur footer dono float ho rahe hai. But hume footer ko float nhi karwana. 
### use clear property
![alt text](image-102.png)
### Eg: Target
![alt text](image-103.png)
#### float:left aur float:right se dono ek mek se alag ho javenge.
![alt text](image-104.png)
#### aur clear:both se footer niche aavenga
![alt text](image-105.png)
## Note: For Wrapping text around use float and for designing ke liye flexbox/grig/bootstrap etc.
# 50. How to create a responsive website.
## What do you mean by responsive website.
![alt text](image-106.png)![alt text](image-107.png)
### Go to this website
https://tastybasics.nl/
- humme isse chota-bada kare
- ye website responsive na hone ke wajah se alag dikh raha hai.
### 4 tarike se responsive website banate aati.
![alt text](image-108.png)
#### 1) Media query
![alt text](image-109.png)![alt text](image-110.png)
#### 2) via CSS Grid
![alt text](image-111.png)![alt text](image-112.png)![alt text](image-113.png)![alt text](image-114.png)![alt text](image-115.png)
- Grid ye 2D layout par apply hota hai.
#### 3) via Flexbox
![alt text](image-116.png)![alt text](image-117.png)![alt text](image-118.png)![alt text](image-119.png)

- Flexbox is good for creating 1D layout
- gist:=
    - the main point or part
- yaha sab ratio or proportion mein hai,
    - so width change ho javengi dynamically
    - ie responsive website.
#### 4) BootStrap framework
![alt text](image-120.png)![alt text](image-121.png) ![alt text](image-122.png)![alt text](image-123.png)![alt text](image-124.png)

# 51. Media Queries
![alt text](image-125.png)![alt text](image-126.png)
### via eg
![alt text](image-127.png)![alt text](image-128.png)
### regarding max width
![alt text](image-129.png)![alt text](image-130.png)
### regaridng min-width
![alt text](image-131.png)
### Combination
![alt text](image-132.png)![alt text](image-133.png)
### About device
![alt text](image-134.png)![alt text](image-135.png)


# Section-9 Flexbox
# 54. Display Flex
![alt text](image-136.png)
- Semantically :  
  - in a way that is connected with the meaning of words, शब्दार्थ
  - when people are talking about code being semantically correct :->  
	- i.e they're referring to the code that accurately describes something.

- Fidly : 
  - requiring close attention to detail 
- coveting-
	 - लालच
- Tweak 
  - CHANGE SLIGHTLY
  - to change something slightly, especially in order to make it more correct, effective, or suitable: 
### ***Designing website layout***
![alt text](image-137.png)![alt text](image-138.png)![alt text](image-139.png)![alt text](image-140.png)![alt text](image-141.png)
### ***Problem in floats***
![alt text](image-142.png)
### ***When to use floats and when to use flexbox.***
![alt text](image-143.png)
## ***Design a website layout via flexbox.***
![alt text](image-144.png)
### ***Note***
![alt text](image-145.png)![alt text](image-146.png)![alt text](image-147.png)
## ***2 version of Flexbox container***
## 1) flex
![alt text](image-148.png)
## 2) inline-flex
![alt text](image-149.png)
# 55. Flex Direction
![alt text](image-150.png)
### ***In Html***
![alt text](image-151.png)
### ***In FlexBox***
![alt text](image-152.png)![alt text](image-153.png)
## About Axis
###  ***When flex-direction:row*** 
![alt text](image-154.png)
### ***When flex-direction:column***
![alt text](image-155.png)
***Note: All this stuff is important for customization***
## ***Different behaviour of flex-basis property;***
### ***1) When flex-direction:row and flex-basis:100px***
![alt text](image-156.png)
### ***2) When flex-direction:column and flex-basis:100px***
![alt text](image-157.png)
## ***Note:***
- Flex-basis aur other property they are flexing along with main axis
- Flex-direction : row 
  - So flex-basis  ye width set karta
- Flex-direction:column
  - So flex-basis ye height set karta
# 56. Flex-Layout
![alt text](image-158.png)
## ***Note:***
- Jo bhi property aapko lagana hai usse sarvapratham check karlo
  - ki Wo property Parent par lagni hai 
  - ya ki child par
### ***About terminology Parent-child***
![alt text](image-159.png)
## ***Properties***
### ***1) Order***
![alt text](image-160.png)![alt text](image-161.png)![alt text](image-162.png)![alt text](image-163.png)
### ***2) flex-wrap***
![alt text](image-164.png)
### ***The defualt behaviour of flexbox***
![alt text](image-165.png)
### ***when flex-wrap:wrap***
![alt text](image-166.png)
### ***when flex-wrap:wrap and flex-wrap:wrap-reverse***
![alt text](image-167.png)![alt text](image-168.png)
- ***sort of meaning:***
  - in a way
### ***3)	Justify-content property:***
- ***justify content meaning :***
  - The justify-content property aligns the flexible container's items when the items do not use all available space on the main-axis (horizontally).
  - सिद्ध करना
### ***About justify content**
![alt text](image-169.png)
### ***About axis***
![alt text](image-170.png)
### ***In details***
![alt text](image-171.png)![alt text](image-172.png)![alt text](image-173.png)![alt text](image-174.png)
- ***godsend meaning:***
  - something very lucky or helpful 
### ***3)align-item property***
![alt text](image-175.png)
- abhi row based flexbox hai yadi column-based-flexbox hua
  - so main axis at vertical
  - and cross axis at horizontal
- align item:
  - ye property parent mane container par apply hoti hai.
  - na ki child mane flexItems par
### ***About viewport height***
![alt text](image-176.png)![alt text](image-177.png)
### ***Eg regarding align-items***
![alt text](image-178.png)![alt text](image-179.png)
![alt text](image-181.png)
### Note:
![alt text](image-180.png)![alt text](image-182.png)
### ***About align-self property***
![alt text](image-183.png)![alt text](image-184.png)
- Overwhelmed:
  - If something overwhelms someone or something, it is too much, or almost too much, for them to manage
  - घबराया हुआ व्याकुल
### ***4)	Align-content***
![alt text](image-185.png)![alt text](image-186.png)![alt text](image-187.png)![alt text](image-188.png)![alt text](image-189.png)
## ***CSS flexbox cheatsheet***
https://css-tricks.com/snippets/css/a-guide-to-flexbox/
## ***Eg Understand***
https://appbrewery.github.io/flex-layout/
## ***Eg practice***
![alt text](image-190.png)
https://appbrewery.github.io/flexboxfroggy/
# 57. Flex- sizing


# Section-11
# 64. What is bootstrap?
![alt text](image-191.png)
### ***Why it became so popular?***
- Isme pre-made CSS files di hoti hai. 
  - Aap unhe apne project mein include karo
  - aur bootstrap ke pre-built components and styling use karo.
- Bootstrap also provide 12-column layout system.
  - That make really easy to create responsive website.
- ***Ye Felxbox ke upar bana hai.***
### Eg
![alt text](image-192.png)![alt text](image-193.png)![alt text](image-194.png)
### ***How to use bootstrap***
![alt text](image-195.png)![alt text](image-196.png)
### ***What is CDN?***
- full form is  content delivery network
- This are little hubs across the world and it knows where the user is located.
- So jab bhi aap apni website load karonge aur aap try to access the particular css file jske andar
Sare bootstrap ka code hai.
- Ye closest location to server provide Karenga. Jaha se content aapko mil javenga.
### Other things
![alt text](image-197.png)![alt text](image-198.png)
### another one
![alt text](image-199.png)
## ***Note*** 
- jab bhi hume bootstrap ki style sheet ko override karna hai.
- 1) inline stylesheet
- 2) internal style sheet <style tag ke andar mein provide karo 
- 3) aur yadi external style sheet hai.
   Tab bootstrap ke link ke niche mein apni link provide karo.



