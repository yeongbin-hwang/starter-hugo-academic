---
title: "Private SNS"
summary: "Clone coding that implements SNS service like Instagram"
tags:
  - Web
date: '2022-07-09T00:00:00Z'

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
url_code: 'https://github.com/yeongbin-hwang/instaclone-backend'
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
In the case of the frontend server to create my own sns, the code was imported and used from <u>[github](https://github.com/manikandanraji/instaclone-frontend)</u>, and the backend server linked thereto was implemented and completed by myself.

There are no functions such as post modification, friend tag, and notification in the existing frontend code, so the frontend part of that part is added, and most of the functions used by the instagram are supported.

### Libraries and frameworks

- Database: mysql
- Backend server: node.js, express
- Image storage server: cloudinary
- Deploy: AWS lightsail
- Load & unit testing: jest

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>