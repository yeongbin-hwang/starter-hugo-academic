---
title: "EVA: Emotion-based Video-conferencing Application for Enhanced Interactions in Online Platforms"
summary: "Course project in KAIST EE474 Introduction to Multimedia, Spring 2020"
tags:
  - AI
  - HCI
date: '2020-06-07T00:00:00Z'

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
url_slides: 'https://docs.google.com/presentation/d/e/2PACX-1vSFG6XvK4ByuNy8O7Rs5IR6TV8eeS12ec8l0hIehmWdP_aJzfa76CGbaCCIAcSz6g/pub?start=true&loop=false&delayms=3000'
url_video: 'https://youtu.be/S3Tn6Czs7Uc'

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

The emergence of COVID 19 has increased the demand for video conferencing applications; people are using the apps to conduct meetings and hang out with friends. There are several video conferencing applications available on the market, but Zoom is one of the most popular. However, despite its ease of use and broad functionality, the app does not offer certain features that consumers may find valuable on a daily basis: statistical analysis of audiences and entertainment features. The presenter may have difficulty tracking audience reactions during a video conference and getting feedback, since existing video conferencing applications are not equipped with any functions that track audience reactions. In addition, while large-scale video conferencing apps are becoming the primary method of communication, they do not offer entertainment features that could be useful for casual meetings. Consequently, we developed EVA, an emotion-based video conferencing application designed to make the video conference more enjoyable and interactive by detecting faces and emotions of participants. We utilize deep learning based techniques to enable EVA. For an enhanced user experience, our app offers emoji features and a fun mode based on detected emotions, as well as applying 3D face masks on a user's face. Furthermore, in order to make EVA interactive, we analyze the facial expressions of all participants in order to give the presenter an indication of how the audience is feeling, as well as to detect participants who are sleeping.

### Libraries and frameworks

**Backend**
- Flask
- TensorFlow
- Keras

**Frontend**
- React JS

<span style="color: gray">
<i>This is done as a course project in KAIST EE474 Introduction to Multimedia, Spring 2020.</i></span>