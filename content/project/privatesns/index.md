---
title: "Infrastructure of My Own Instagram"
summary: "Clone coding that implements SNS service like Instagram"
tags:
  - Web
date: "2023-01-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: "https://github.com/yeongbin-hwang/instaclone-backend"
url_pdf: ""
url_slides: ""
url_video: ""

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
.carousel__activator:nth-of-type(2):checked ~ .carousel__slide:nth-of-type(1) {
  transition: opacity 0.5s, transform 0.5s;
  top: 0;
  left: 0;
  right: 0;
  opacity: 1;
  transform: scale(1);
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__controls:nth-of-type(1) {
  display: block;
  opacity: 1;
}
.carousel__activator:nth-of-type(2):checked ~ .carousel__indicators .carousel__indicator:nth-of-type(1) {
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
  background-image: url("/uploads/projects/privatesns/figure1.png");
  background-size: contain;
  background-position: center;
}
.carousel__slide:nth-of-type(2),
.carousel--thumb .carousel__indicators .carousel__indicator:nth-of-type(2) {
  background-image: url("/uploads/projects/privatesns/figure2.png");
  background-size: contain;
  background-position: center;
}
<style>
body{
  font-size: 14pt;
  margin-left: 12%;
  margin-right: 12%;
  /* margin-bottom: -100px; */
}

@media only screen and (max-width: 768px) {
 body {
  font-size: 12pt;
  /* text-align:center; */
  margin-left: 0%;
  margin-right: 0%;
 }
}
</style>

### Project summary

In the case of the frontend server to create my own sns, the code was imported and used from <u>[github](https://github.com/manikandanraji/instaclone-frontend)</u>, and the backend server linked thereto was implemented and completed by myself.

There are no functions such as post modification, friend tag, and notification in the existing frontend code, so the frontend part of that part is added, and most of the functions used by Instagram are supported.

I implemented the backend, frontend, and database as containers, respectively, and applied docker-compose and Kubernetes to set up a network for communication.

<div class="carousel-container">
  <div class="carousel my-carousel carousel--translate">
    <input class="carousel__activator" type="radio" name="carousel" id="F" checked="checked"/>
    <input class="carousel__activator" type="radio" name="carousel" id="G" />
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="F"></label>
      <label class="carousel__control carousel__control--forward" for="G"></label>
    </div>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="F"></label>
      <label class="carousel__control carousel__control--forward" for="G"></label>
    </div>
    <div class="carousel__track">
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure 1. ERD</p>
      </li>
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure 2. Swagger</p>
      </li>
    </div>
    <div class="carousel__indicators">
      <label class="carousel__indicator" for="F"></label>
      <label class="carousel__indicator" for="G"></label>
    </div>
  </div>
</div>

### Libraries and frameworks

- Backend server: node.js, express
- API specification: swagger
- Load & unit testing: jest
- Database: mysql, redis
- Image storage server: cloudinary
- Deploy: Kubernetes, Docker, github actions, argoCD

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>
