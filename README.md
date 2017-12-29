# Portfolio website

Portfolio website for my Front-End Web Development module

P14165711

### Module information

CTEC3905 Front-End Web development

## Contents

1. Website idea
2. Wireframe and protoype designs
3. Mobile first responsive design
4. Semantic elements
5. Advanced CSS styling (Flex box)
6. JavaScript
7. API
8. User Testing
9. Validation
10. GitHub
11. Personal Development

## Website idea

When we were first given this assignment for this module my first idea was to create a portfolio website. I came up with this idea as i thought i could use it in the future. Upon completion of my website i realised that i had developed more in depth development skills so will likely re develop and design my website to create a better version for suture use.

## Wirerframe and prototype designs

The following images show initial sketches that were created to show the general desired layout of my site

### Mobile view

<img src="https://preview.ibb.co/fYL5Wb/IMG_1034.jpg" alt="IMG_1034" border="0">


### Desktop view

<img src="https://preview.ibb.co/n1gqxG/IMG_1033.jpg" alt="IMG_1033" border="0">

(The tablet view was to be the same as the dektop view but with scaling added using a media query to ensure that responsive design was achieved)

## Mobile first responsive design

As stated in the assignment brief the website was to be developed using the mobile first approach to responsive design. this was achieved using the follwoing media queries

/*styling for tablets*/
@media screen and (min-width: 650px){

/*styling for desktop*/
@media screen and (min-width: 1020px){

the follwoing link is my reason for the decided break points: http://tangledindesign.com/deciding-what-responsive-breakpoints-to-use/

Other resource: https://www.impactbnd.com/examples-of-effective-mobile-website-design

## Semantic elements

For this module we were required to use correct HTML5 semantic elements, this includes the use of tags such as nav, article and section

An example of the use of these can be seen below:

<section id="maintext">
    <article id="statement">
      <p>Hi! I am gradute student who has just graduated with a Bsc in computing. My goal is to be a web developer
      and specialise in HTML, CSS and JavaScript.<br><br> This site is a place for me to showcase both current and past work
    of mine.</p>
    </article>
  </section>
  
 Resource: https://webflow.com/blog/html5-semantic-elements-and-webflow-the-essential-guide
  
## Advanced CSS styling

For this section we were tasked to use advanced features of CSS for our styling. For this i used the FlexBox techique for layout. At the start of development i was positioning images using the position tag in the stylesheet, but i was having issues with the layout altering with added content so i changed the the use of flex box. 

This can be seen below:

.flexbox {
  display: flex;
  width:60%;
  margin-top:12%;
  margin-left:.5%;

}

#flex-item2 {
  width:35%;
  height: 300px;
  padding:5px;
  display: block;
}

Resource: https://css-tricks.com/snippets/css/a-guide-to-flexbox/
### Animations

I also used keyframes in order to acheive a typing effect on my mobile view of the website, this can be seen below:

@keyframes typing {
  from { width: 0 }
  to { width: 100%}
}

@keyframes blink-caret {
  from, to {border-color: transparent}
  50% { border-color: orange}

}

Resource: https://css-tricks.com/snippets/css/typewriter-effect/

## JavaScript

I used javascript in this website to acheive the hamburger navigation for the mobile website and also for the API. The java script for the hamburger nav bar can be seen below:

(function(){

  let menuButton = document.getElementById("menu");
  let navMenu = document.getElementById("nav-menu");

  menuButton.addEventListener("click", toggleMenu);

  let toggle = false; // hidden at first
  function toggleMenu(){
    if (toggle) { // true: it's visible
      navMenu.classList.remove("show-menu"), // hide it
      toggle = false
    }
    else { // false: it's hidden
      navMenu.classList.add("show-menu"), // show it
      toggle = true
    }
  }

})();

## API

Unfortunatly i didnt get to experiment as far as i had hoped with the use of API's but i did manage to include one on my site and to get it fully working, i also had to alter some of the styling for this in order to make it work for my site

## User testing

For this i asked friends to view the website on their mobile phones, i asked them to do this to test the responsive design of the website. They game me feedback and improvements were made. Unfortunatly, i forgot to screenshot the evidence for this.

I also decided it would be good to get someone to use the website who does not have any technical knowledge of how websites are developed etc so i asked my sister to use the website and give me feedback, evidence of this can be seen below:

<img src="https://preview.ibb.co/nJvu7G/IMG_1030.jpg" alt="IMG_1030" border="0">

## Website usability

### Information Architecture and PARC

I tried to implement the use of as many techniques taught to use about information architecture and PARC througout the design of my website. Maintaining a constant layout across all pages and also using colours to tie things in.

Resource: https://www.usability.gov/what-and-why/information-architecture.html

### Navigation

I also tried to make the navigation simple yet effective, i wanted to make sure it was easy for any user to get aorund the website with ease. This was also acheived by implementing a site map at the bottom of the site.

Resource: 

## Validation

I ran my website pages through the W3schools HTML validator, the W3Schoolcs CSS validator and also the accessability validator. There were no errors on any of the validators only warnings which were to do with article elements not having a header element.

accessability validator:

<img src="https://preview.ibb.co/hBGsSG/Capture.png" alt="Capture" border="0">

CSS validator:

<img src="https://image.ibb.co/kQsXSG/Capture1.png" alt="Capture1" border="0">


## GitHub

Right from the begginning of development i had my site on GitHub this allowed me to track development and also allows me to roll back if there was ever any issues with my code after a push. Unfortunatly, i forgot to use branches for testing ideas


## Personal Development

During this module i have learnt many new skills when it comes to writing correct HTML and CSS techniques.; I have greatly increased my knowledge in the use of semantic elements and even more so in the use of advanced CSS feature to help me achieve the desire laqyouts and effects i desire

I also developed some basic skills in the use of JavaScript and JSON use. This is something that i would like to further develop on in the future.

My confidecne with the use of GitHub to clone repos etc for my work has also greatly increased during the module.

## Things not fully achieved

There were things that i was not happy with for the website, i was not 100% happy with the responsive design and had issues with this changing after every commit to git hub. It would be okay before a commit and then it wouldnt work as it should once cloned again.

I was also unable to get the "position:Fixed" CSS attribute to work for the footer for some reason


