---
title: "Large Scale Evaluation of Secure Headers in Wild"
summary: "Investigation on HTTP response headers to find insecure websites"
tags:
  - Web
date: "2022-12-09T00:00:00Z"

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
url_code: "https://github.com/yeongbin-hwang/secure-headers"
url_pdf: ""
url_slides: "uploads/projects/secureHeaders/Presentation.pdf"
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

We assume that malicious javascript is inserted into the server and reflected to the client browser by a cross-site scripting (XSS) attack. Then, we want to know whether the browsers successfully detect and prevent the XSS's implications by analyzing secure headers in HTTP response headers.
In this work, we investigate the actual usage of secure headers and conduct a large-scale evaluation. For this, we first compare the secure header collected on different days and identify which fields and websites are vulnerable. Also, we analyze the websites that can be vulnerable due to a mismatch, which is the difference between a website's request and browser support for a secure header for each browser.

### Libraries and frameworks

- Crawler (HTTP response): Python
- Crawler (Browser support option): Javascript (nodejs)

<span style="color: gray">
<i>This is done as a course project in KAIST IS542 Web Service Security and Privacy, Fall 2022.</i></span>
