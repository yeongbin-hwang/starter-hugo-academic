---
title: "Comparsion between state machines"
summary: "Analyzer, Fuzzer: build state machines in LTE"
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
url_code: 'https://github.com/yeongbin-hwang/Analyzer'
url_pdf: 'uploads/projects/statemachine/URP_report.pdf'
url_slides: 'uploads/projects/statemachine/URP_presentation.pdf'
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

<u>[srsRAN](https://github.com/srsran/srsRAN)</u> implements each cellular network identity with software so that LTE network can be accessed using SDR equipment. I tried to find vulnerabilities by conducting fuzzing tests on LTE networks. Based on this project, I implemented the following functions to conduct a fuzzing test. 
- First, implements a code that converts to it so that it can be recognized by srsRAN when given the form of the message to be tested.
- Second, a function capable of logging the result value while repeatedly executing the test by changing the input value was implemented.
- Third, implement a CLI based analyzer that analyzes stored result values.

### Libraries and frameworks

- UE simulator: C++, C
- Message Generator, Analyzer: Python

<span style="color: gray">
<i>This is done, Spring 2021.</i></span>