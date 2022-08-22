---
title: "Emergency alarm: Bodyguard Implementation in BLE"
summary: "Course project in KAIST EE595 Mobile Computing and Systems for Intelligent Living, Fall 2021"
tags:
  - Mobile Computing
date: '2021-12-09T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ""
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: 'https://github.com/yeongbin-hwang/mobile_project'
url_pdf: 'uploads/projects/mobile/Documentation.pdf'
url_slides: 'uploads/projects/mobile/Presentation.pdf'
url_video: ''

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

We tried to detect dangerous situations through smartwatch. We created a service that detects two potentially dangerous situations through the IMU(Inertial Measurement Unit) sensor present in all smartwatches and sends them to the phone to alert the user. To show the feasibility of the service, we tested it using Arduino Nano 33 BLE Sense, and through this, the accuracy of voice and gesture recognition was measured to be 92 or 93%, implying that it will perform well when applied to real-world scenarios.

### Libraries and frameworks

- Classifier: Google colab
- Emergency detection algorithm: arduino
- Communication with BLE: Python

<span style="color: gray">
<i>This is done, Fall 2021.</i></span>