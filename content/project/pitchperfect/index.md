---
title: "PitchPerfect: Tinder for Amateur Music Lovers"
summary: "Course project in KAIST CS473 Introduction to Social Computing, Fall 2020"
tags:
  - HCI
date: '2020-12-23T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ""
  focal_point: Smart

links:
  - icon: 
    icon_pack: 
    name: Demo
    url: https://sanghyeon-lee.github.io/PitchPerfect/
url_code: 'https://github.com/SangHyeon-Lee/PitchPerfect'
url_pdf: ''
url_slides: 'https://docs.google.com/presentation/d/e/2PACX-1vRDYC3LR6Tq_lkYYPBD48LEr5Aon09gRfOqTyKlDu03NLQHvMrNR3vNACWvQZYgZpeCF0U9EM-6Nehl/pub?start=true&loop=false&delayms=3000'
url_video: 'https://youtu.be/0H4-MHTlwbI'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
<style>
body{
  font-size: 14pt;
  margin-left: 12%;
  margin-right: 12%;
  /* margin-bottom: -100px; */
}

.carousel {
  height: 500px;
  width: 600px;
  overflow: hidden;
  text-align: center;
  position: relative;
  padding: 0;
  list-style: none;
}
.carousel__controls,
.carousel__activator {
  display: none;
}
.carousel__activator:nth-of-type(1):checked ~ .carousel__track {
  transform: translateX(0%);
}
.carousel__activator:nth-of-type(1):checked ~ .carousel__slide:nth-of-type(1) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(1):checked ~ .carousel__controls:nth-of-type(1) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(1):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(1) {
  opacity: 1;
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__track {
  transform: translateX(-100%);
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__slide:nth-of-type(2) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__controls:nth-of-type(2) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(2) {
  opacity: 1;
}
.carousel__activator:nth-of-type(3):checked ~ .carousel__track {
  transform: translateX(-200%);
}
.carousel__activator:nth-of-type(3):checked ~ .carousel__slide:nth-of-type(3) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(3):checked ~ .carousel__controls:nth-of-type(3) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(3):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(3) {
  opacity: 1;
}
.carousel__activator:nth-of-type(4):checked ~ .carousel__track {
  transform: translateX(-300%);
}
.carousel__activator:nth-of-type(4):checked ~ .carousel__slide:nth-of-type(4) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(4):checked ~ .carousel__controls:nth-of-type(4) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(4):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(4) {
  opacity: 1;
}
.carousel__activator:nth-of-type(5):checked ~ .carousel__track {
  transform: translateX(-400%);
}
.carousel__activator:nth-of-type(5):checked ~ .carousel__slide:nth-of-type(5) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(5):checked ~ .carousel__controls:nth-of-type(5) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(5):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(5) {
  opacity: 1;
}
.carousel__control {
  height: 30px;
  width: 30px;
  margin-top: -15px;
  top: 50%;
  position: absolute;
  display: block;
  cursor: pointer;
  border-width: 5px 5px 0 0;
  border-style: solid;
  border-color: #bebebe;
  opacity: 0.35;
  outline: 0;
  z-index: 3;
}
.carousel__control:hover {
  opacity: 1;
}
.carousel__control--backward {
  left: 10px;
  transform: rotate(-135deg);
}
.carousel__control--forward {
  right: 10px;
  transform: rotate(45deg);
}
.carousel__indicators {
  position: absolute;
  bottom: 20px;
  width: 100%;
  text-align: center;
}
.carousel__indicator {
  height: 15px;
  width: 15px;
  border-radius: 100%;
  display: inline-block;
  z-index: 2;
  cursor: pointer;
  opacity: 0.35;
  margin: 0 2.5px 0 2.5px;
}
.carousel__indicator:hover {
  opacity: 0.75;
}
.carousel__track {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  padding: 0;
  margin: 0;
  transition: transform 0.5s ease 0s;
}
.carousel__track .carousel__slide {
  display: block;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
}
.carousel__track .carousel__slide:nth-of-type(1) {
  transform: translateX(0%);
}
.carousel__track .carousel__slide:nth-of-type(2) {
  transform: translateX(100%);
}
.carousel__track .carousel__slide:nth-of-type(3) {
  transform: translateX(200%);
}
.carousel__track .carousel__slide:nth-of-type(4) {
  transform: translateX(300%);
}
.carousel__track .carousel__slide:nth-of-type(5) {
  transform: translateX(400%);
}
.carousel--scale .carousel__slide {
  transform: scale(0);
}
.carousel__slide {
  height: 100%;
  position: absolute;
  overflow-y: auto;
  opacity: 0;
}
/**
  * Theming
*/

.carousel-container {
  display: inline-block;
}
.my-carousel {
  border-radius: 5px;
  margin: 30px;
}
.carousel__slide {
  overflow: hidden;
}
.carousel--thumb .carousel__indicator {
  height: 30px;
  width: 30px;
}

.carousel__indicator {
  background-color: #bebebe;
}
.carousel__slide:nth-of-type(1),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(1) {
  background-image: url("/uploads/projects/pitchperfect/figure1.png");
  background-size: cover;
  background-position: center;
}
.carousel__slide:nth-of-type(2),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(2) {
  background-image: url("/uploads/projects/pitchperfect/figure2.png");
  background-size: cover;
  background-position: center;
}
.carousel__slide:nth-of-type(3),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(3) {
  background-image: url("/uploads/projects/pitchperfect/figure3.png");
  background-size: cover;
  background-position: center;
}
.carousel__slide:nth-of-type(4),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(4) {
  background-image: url("/uploads/projects/pitchperfect/figure4.png");
  background-size: cover;
  background-position: center;
}
.carousel__slide:nth-of-type(5),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(5) {
  background-image: url("/uploads/projects/pitchperfect/figure5.png");
  background-size: cover;
  background-position: center;
}

@media only screen and (max-width: 768px) {
 body {
  font-size: 12pt;
  /* text-align:center; */
  margin-left: 0%;
  margin-right: 0%;
 }

  .carousel {
    height: 400px;
    width: 400px;
    overflow: hidden;
    text-align: center;
    position: relative;
    padding: 0;
    list-style: none;
  } 
}

</style>

### Project summary
A conductor is a messenger for the composer, and musicians’ duty is to PitchPerfect provides an easy-to-use interface to achieve two goals: (1) help amateur musicians find suitable collaborators and (2) provide tools for managing music collaboration projects. To achieve the first goal, PitchPerfect has project summary pages (Figure1) that provide an overview of the project and personal profile pages (Figure2) for other users to get a sense of what kind of musician that person is. We designed those pages to contain all information necessary for the users to make an informed decision, such as parts involved in a music or musical preferences. At the same time, we used standard symbols and recurring designs throughout our interface to deliver such information concisely and clearly. For example, we introduce the proficiency emoticons 🐣 for level1, 🐥 for level2, 🐦 for level3) in the signup process and use them in personal profile pages. Also, when displaying a project, the same or slightly modified design (white rectangle with round corners with music title, required parts, and proficiency tag inside) is used in all pages so that the user can naturally associate that design component with a project. In our survey, we asked the users to rate how helpful the project summary page and personal profile page were in finding a suitable project to join on a Likert scale of 1-5. Out of the 20 users that participated in our survey, 15 users rated 4 or above for the project summary page, and 17 users rated 4 or above for the personal profile page. To achieve the second goal, we designed novel UI components to provide communication tools for music collaboration. Two most unique tools are: shared annotatable sheet music (Figure3 and Figure4) and moveable pins with threads (Figure3 and Figure5). During music collaboration, musicians often add annotations to play in sync (ex. down bow annotation for all violinists to slide their bows in the same direction) and make modifications to music (ex. adding a crescendo to measure 1). These annotations and changes are difficult to communicate through text but can be easily communicated with shared annotatable sheet music. Musicians also often discuss certain parts at length for various reasons (ex. that part is important, that part does not harmonize well...etc). The moveable pins are designed to aid such discussion. To make the pins point to the part in question, team members can freely adjust the location of pins and the location changes are reflected the next time any member enters the sheet music page. Also, to keep those discussions independent, each pin is connected to its own discussion thread. In our survey, we also asked the users to rate how helpful such tools were in collaboration with team members on a Likert scale of 1-5. Out of the 20 users that participated in our survey, 14 users rated 4 or above for shared annotatable sheet music and 18 users rated 4 or above for moveable pins with linked threads. Moreover, one user commented “this interface will open a new paradigm of music collaboration.” 


<div class="carousel-container">
  <div class="carousel my-carousel carousel--translate">
    <input class="carousel__activator" type="radio" name="carousel" id="F" checked="checked"/>
    <input class="carousel__activator" type="radio" name="carousel" id="G"/>
    <input class="carousel__activator" type="radio" name="carousel" id="H"/>
    <input class="carousel__activator" type="radio" name="carousel" id="I"/>
    <input class="carousel__activator" type="radio" name="carousel" id="J"/>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="J"></label>
      <label class="carousel__control carousel__control--forward" for="G"></label>
    </div>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="F"></label>
      <label class="carousel__control carousel__control--forward" for="H"></label>
    </div>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="G"></label>
      <label class="carousel__control carousel__control--forward" for="I"></label>
    </div>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="H"></label>
      <label class="carousel__control carousel__control--forward" for="J"></label>
    </div>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="I"></label>
      <label class="carousel__control carousel__control--forward" for="F"></label>
    </div>
    <div class="carousel__track">
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure 1. Project Summary Page</p>
      </li>
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure 2. Personal Profile Page</p>
      </li>
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure3: Shared Sheet Music Page</p>
      </li>
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure4: Annotation Page</p>
      </li>
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure5: Thread Discussion Page</p>
      </li>
    </div>
    <div class="carousel__indicators">
      <label class="carousel__indicator" for="F"></label>
      <label class="carousel__indicator" for="G"></label>
      <label class="carousel__indicator" for="H"></label>
      <label class="carousel__indicator" for="I"></label>
      <label class="carousel__indicator" for="J"></label>
    </div>
  </div>
</div>

### Libraries and frameworks

- Vue.js
- Firebase
- HTML and CSS

<span style="color: gray">
<i>This is done as a course project in KAIST CS473 Introduction to Social Computing, Fall 2021.</i></span>