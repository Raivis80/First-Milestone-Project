
## ***Testing***

### **Table of contents**

1. [Testing website responsiveness](#Testing-website-responsiveness)
1. [Testing Functions and Links](#Testing-Functions-and-Links)
1. [Further Testing](#Further-Testing)
1. [W3C Validation](#W3C-Validation)
1. [Bugs and Issues](#Bugs-and-Issues)
1. [Fixed Bugs and Issues](#Fixed-Bugs-and-Issues)
1. [Back to README.md](README.md)

# [&#8686;](#Testing)

## ***Testing website responsiveness***

### **Testing Navigation responsiveness:**
    
NavBar is responsive to most viewport sizes. 

I'm using bootsrap5 components and flexBox components for NavBar responsiveness.

I'm using display Property "Fixed". As you scroll it will remain fixed at the top of the browser's viewport.

![responsivedesign](assets/project-files/testing/responsive-test/testing-nav.gif)
#
### **Testing Home page responsiveness:**
   
For "home Page" for font responsiveness I'm using CSS property "min & max", that is responsive to all other browser sizes.

![responsivedesign](assets/project-files/testing/responsive-test/home-testing.gif)
#
### **Testing About page responsiveness:**
    
I'm using FlexBox design for responsive "About us" page design.

I'm using CSS FlexBox property "order" for tablet and mobile device elements reordering.

I'm using FlexBox declaration "flex-direction: row;"for desktop device elements and for mobile devices I'm using "flex-direction: column;" for elements.

![responsivedesign](assets/project-files/testing/responsive-test/about-page.gif)
#
### **Testing gallery responsiveness:**

For "gallery" responsiveness I'm using Bootstrap Grid system.

I'm using media queries with CSS declaration "display: none;" to hide some of the images for mobile devices.

![responsivedesign](assets/project-files/testing/responsive-test/gallery-testing.gif)
#
### **Testing Review and Contact form responsiveness:**

For "review area" responsiveness I'm using Bootstrap Grid system.

I'm using CSS declaration "max-width: 600px;" for "Contact form" to make it responsive.

![responsivedesign](assets/project-files/testing/responsive-test/testing-review-and-contact-form.gif)
#
### **Testing footer responsiveness:**

I'm using FlexBox system for the Footer responsiveness. 

I'm using CSS Media query technique with FlexBox CSS declaration "flex-item :order" to rearrange Element order for mobile devices.

![responsivedesign](assets/project-files/testing/responsive-test/footer-testing.gif)

# [&#8686;](#Testing)
## ***Testing Functions and Links***

### **Testing NavBar:**

 I'm using link for NavBar brand element and when I click on it the page reloads.
 
 The NavBar features navigation menu to navigate the site pages. The menu links all the pages on the site.
 
 For mobile devices I'm using drop down menu Navigation and it is activated using bootstrap grid properties such as: "d-none d-sm-block" to hide or display navigation menu items and media queries.
 
 Navbar also features links to the social media platforms. I'm using font awesome for the link icons. I'm using a target="_blank" attribute to links to open social media links in a new browser tab.

![responsivedesign](assets/project-files/testing/nav-link-test.gif)
#
### **Testing "op picks" feature:**

"Top Picks" Feature was designed to overlap each image using negative margin and CSS property z-index.

Pseudo-class "hover" was used with transition effects "rotate, translate and scale" for each card to create visual effect such as scale and rotate 6deg on mouse-over.

![responsivedesign](assets/project-files/testing/top-picks-test.gif)
#
### **Testing thumblail gallery:**

The gallery configuration designed to have smaller images for Thumbnails when clicked on opens full size images in a new tab. 

![responsivedesign](assets/project-files/testing/gallery-test.gif)
#
### **Testing contact-form:**

Contact form was tested ifr input element functioning correctly. 

And if all of the input fields "required" attribute functioning correctly.
 
![responsivedesign](assets/project-files/testing/contact-form-test.gif)
#
### **Testing Footer links:**

Footer features links to the social media platforms. 

I'm using font awesome for the link icons. 

Also Footer features eMail link and contact phone Link.

I'm using a target="_blank" attribute to links to open links in a new browser tab.

![responsivedesign](assets/project-files/testing/footer-test.gif)

# [&#8686;](#Testing)
## **Further Testing:**
-  Tested on Chrome, Opera and Firefox desktop version browsers and on Iphone 11 Safari, huawei p30 Pro chrome and android browser.
-  Chrome DevTools was used to Test variety of devices such as Desktop, Laptop, iPhone7, iPhone 8 & iPhoneX for responsiveness.
-  Testing was done to ensure that all Links were linking correctly.

# [&#8686;](#Testing)
## **W3C Validation**
  The W3C Markup Validator and W3C CSS Validator Services were used to validate every page of the project to ensure there were no syntax errors in the project.

-   [W3C Markup Validator](assets/project-files/validators/HTML-Vaalidator.pdf)
-   [W3C CSS Validator](assets/project-files/validators/CSS-Validator.pdf)

# [&#8686;](#Testing)
## **Bugs and Issues:**
*hide scroolBar for the browser*
- W3C CSS Validation Warning: "::-webkit-scrollbar is an unknown vendor extended pseudo-element" *Hide scrollbar for Chrome*   
    
   Code is still in use for aesthetics. In order to Validate CSS, solution is not to use the following code:
    
    "html::-webkit-scrollbar display: none;"

- W3C CSS Validation Warning: "-ms-overflow-style is an unknown vendor extension"  *Hide scrollbar for IE, Edge*

    Code is still in use for aesthetics. In order to Validate CSS, solution is not to use the following code:
    
    "html::-webkit-scrollbar display: none;"

*Input Form Autofill and input form custom background color*

- W3C CSS Validator Warning: "::-webkit-input-placeholder is an unknown vendor extended pseudo-element" *Custom input form placeholder font color*
    
    This code is in use for aesthetics, to match website color sheme. In order to Validate CSS, solution is not to use the following code:
    
    ".contact--form input::-webkit-input-placeholder"

- W3C CSS Validator Warning: "-webkit-background-clip is an unknown vendor extension" *Custom input form background color*
   
    This code is in use for aesthetics, to match website color sheme. In order to Validate CSS, solution is not to use the following code: 
    
    "background-clip: text;"

- W3C CSS Validator Warning: "-webkit-text-fill-color is an unknown vendor extension" *Custom input form background color*
    
    This code is in use for aesthetics, to match website color sheme. In order to Validate CSS, solution is not to use the following code: 
    
    "-webkit-text-fill-color: rgb(255, 255, 255);"

# [&#8686;](#Testing)
## **Fixed Bugs and Issues**


- W3C CSS Validation ERROR: - "Property scrollbar-width doesn't exist : none" *Hide scrollbar for Firefox browser*
    
    In order to Validate CSS, solved this issue by Removeing following declaration from CSS: 
    
    "scrollbar-width: none;"

- W3C CSS Validation ERROR:  "input:-webkit-autofill	text is not a background-clip value : text" *Input Form autocomplete custom background colour* 
    
    In order to Validate CSS, solved this issue by Removeing following code from CSS:
    
    "-webkit-background-clip: text;"

- W3C CSS Validation Warning: "-moz-max-content is an unknown vendor extension" Mozilla Firefox css property maximum width fit content

    In order to Validate CSS, Solved this issue by replacing it with the following CSS declaration:

    "width: max-content;"  Text will not wrap with this declaration but it works in my case.


 - Custom colors, position and width was used for the Boostrap NavBar. Most of the Bootstrap NavBar components was redesigned and replaced. 
 - Drop-down menu, bootstrap toggle hamburger menu was replaced with font awesome "bars" icon to match website color Scheme.                                      
 - Issue with CSS Declaration "width: fit-content;" does not work on Firefox browser. I Googled for "fit-content aternative" and CSS Declaration "width: max-content;" and it worked.  Text does not wrap, but in my case it is accetable and Solution works.
 - I had an issues with content overflow on the right side on mobile devices. Using Chrome DevTools I was able to detect that most of the time there was an issues with bootstrap grid system paddings. Using CSS Declaration "padding: 0;" I was able to resolve most of them.
 - Issue with contact form custom background color and placeholder text color to match the website color sheme. Solution was found [here](https://stackoverflow.com/questions/2781549/removing-input-background-colour-for-chrome-autocomplete) with W3C CSS Validation warnings.
 - Issue with text block element, underline allignment on "contact us" page for tablet devices. underline missalignment was solved using "min-height" CSS declaration for text block elements.
 - Issue with "Contact Us" page: as the viewport decreased in width, one of 3 images shifted below two top images, width for the image below was wider than two images above as they where compressing and image below was expanding. I've solved the issue using media queries and for the single image i was using margins left, right as viewpost decrease the image compressed same rate as two top images.

 # [&#8686;](#Testing)