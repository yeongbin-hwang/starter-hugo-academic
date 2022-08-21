---
title: "5G core network testing: inducing the collision"
summary: "Guided fuzzing test that can detect the procedure collision"
tags:
  - Cellular Network
date: '2022-08-09T00:00:00Z'

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
url_code: ''
url_pdf: ''
url_slides: ''
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

From 5G, each network entity runs a container-based program. In the case of 5G Core Network, each network entity is implemented and managed using kubernetes. To test this, UE and gNB emulator were implemented using kubernetes, and the program for packet forwarding was made in python.

### Libraries and frameworks

- UE, gNB emulator: C++, C
- Entity management: Kubernetes
- Packet forwarding: Python

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>