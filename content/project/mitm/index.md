---
title: "MitM simulater: Modifying packets between users"
summary: "Simulator for verifying our attack in real environment"
tags:
  - Cellular Network
date: '2020-12-09T00:00:00Z'

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

MitM environment was built in LTE network to verify vulnerabilities found through formal verification. In the case of Fake gNB and Fake UE, it was executed through srsRAN, and a program to relay messages between the two entities was made using python.

### Libraries and frameworks

- Fake UE and Fake eNB: C++, C
- MitM simulator: Python

<span style="color: gray">
<i>This is done, Fall 2020.</i></span>