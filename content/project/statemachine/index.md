---
title: "Comparsion between state machines"
summary: "Analyzer, Fuzzer: build state machine in LTE"
tags:
  - Cellular Network
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

We tried to find vulnerabilities by conducting fuzzing tests on LTE networks. The UE simulator for testing was implemented based on srsRAN, and the analyzer for analyzing the results was implemented in the form of Ubuntu CLI using python.

### Libraries and frameworks

- UE simulator: C++, C
- Message Analyzer: Python

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>