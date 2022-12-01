---
title: "Comparative analysis between state machines"
summary: "Build fine-grained state machines and analyze the difference between state machines"
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

We assume that if handling of invalid messages between each networks is different, this may lead to implementation vulnerabilities.
Therefore, we implements the framework that automatically builds the state machine of network using the UE side log.
The framework is implemented on top of <u>[srsRAN](https://github.com/srsran/srsRAN)</u> project.
The srsRAN implements each cellular network entity with software so that LTE network can be accessed using SDR equipment.
Based on this open-source project, we implemented the following modules and programs.
- First, module that converts config file to internal structure so that it can be recognized by srsRAN when given the form of the message to be tested.
- Second, module capable of logging the result value while repeatedly executing the test by changing the input file.
- Third, CLI based analyzer that analyzes stored result values.
- Fourth, program that builds the state machine based on stored log.

### Libraries and frameworks

- UE simulator: C++, C
- Analyzer: Python (with py_cui library)
- State machine generator: Python (with transitions library)

<span style="color: gray">
<i>This is done, Spring 2021.</i></span>