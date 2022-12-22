---
title: "5G Core Network Testing: Let's Induce the Collision"
summary: "Framework that can execute not only guided fuzzing, but also various attack scenarios"
tags:
  - Cellular Network
date: "2022-08-09T00:00:00Z"

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
url_code: ""
url_pdf: "uploads/projects/procedure/mobisec22.pdf"
url_slides: "uploads/projects/procedure/Presentation.pdf"
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
  background-image: url("/uploads/projects/procedure/figure2.png");
  background-size: cover;
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

We implemented a framework based on Open5GCore, which runs the entities of 5G core network on the container managed by Kubernetes, to find the vulnerabilities of the 5G core network.
The framework consists of three main components: <b>Fuzzer</b> that continues testing on UE1 pod, <b>Controller</b> that captures packets on the host and relays them to the target, and <b>Analyzer</b> that analyzes the results of the test.

#### Fuzzer

The fuzzer running on the UE1 pod reads the input file and generates an attack scenario based on the file. Then, UE move to the target state and execute the test cases by communicating with other pod named gNB. After the test, it automatically change the scenario and repeat the test process.
The UE1 pod and gNB pod are easily transmit the packet using internal interface.

#### Controller

The controller is responsible for capturing messages sent to the core network and relaying them to the target network while monitoring br-ngc that is virtual network bridge. In this case, the packet for each test is stored in the form of a pcap while communicating with the UE.

#### Analyzer

The analyzer analyzes the logs stored in the form of json and displays them in the form of the CUI to determine whether the attack was successful or unsuccessful.

<div class="carousel-container">
  <div class="carousel my-carousel carousel--translate">
    <input class="carousel__activator" type="radio" name="carousel" id="F" checked="checked"/>
    <div class="carousel__controls">
      <label class="carousel__control carousel__control--backward" for="J"></label>
      <label class="carousel__control carousel__control--forward" for="G"></label>
    </div>
    <div class="carousel__track">
      <li class="carousel__slide">
        <p style="background-color: black; color:white; color: #fafafa; position: absolute; top: 5%; width: 100%; text-align: center; margin-top: -25px;">Figure 1. Analyzer example</p>
      </li>
    </div>
    <div class="carousel__indicators">
      <label class="carousel__indicator" for="F"></label>
    </div>
  </div>
</div>

### Libraries and frameworks

- UE, gNB emulator: C++, C, Kubernetes
- Packet capture & relay: Python (with scapy library)
- Analyzer: Python (with py_cui library)

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>
