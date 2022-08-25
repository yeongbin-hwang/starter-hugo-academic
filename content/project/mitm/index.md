---
title: "MitM simulater: Modifying packets between user and network"
summary: "Simulator for verifying our attack scenarios in real environment"
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
url_pdf: 'https://patentimages.storage.googleapis.com/04/a7/f6/7c254830d6c656/US20220124504A1.pdf'
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

MitM(Man in the Middle) environment was built in LTE network to verify vulnerabilities found through formal verification. This MitM simulator executes the attack scenario we want and determines whether the network or user is functioning normally for it. This allows us to validate attacks on vulnerabilities found using formal analysis. As shown in the figure above, the simulator is largely composed of <b>fake eNB</b>, <b>fake UE</b>, and <b>controller</b>. In the case of Fake eNB and Fake UE, it was implemented based on <u>[srsRAN](https://github.com/srsran/srsRAN)</u>, and we implemented a controller that parses and transfers a scenario input in the form of xml and uses it to relay or tamper messages.

### Libraries and frameworks

- Fake UE and Fake eNB: C++, C
- Controller: Python

<span style="color: gray">
<i>This is done, Fall 2020.</i></span>