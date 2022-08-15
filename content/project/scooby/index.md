---
title: "Scooby: AI-interactive Speech Practive Platform for Non-native English Speakers"
summary: "Course project in KAIST CS492 Human-AI Interaction, Fall 2020"
tags:
  - AI
  - HCI
date: '2020-12-23T00:00:00Z'

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
url_code: 'https://github.com/choch-o/Scooby'
url_pdf: ''
url_slides: 'uploads/projects/scooby/scooby_slides.pdf'
url_video: 'https://youtu.be/HyknwxEhZF4'

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
Despite the variety of existing AI pronunciation practicing models, there is no AI-interactive platform for non-native English speakers to evaluate and practice English pronunciation skills with __personalized scripts__ . To solve this problem, we propose Scooby, a AI powered platform where users input their scripts, practice the pronunciation and receive the feedback from AI to further improve the English speech skills. Unique features of Scooby include ii) enabling a user's __personal text input__, ii) visualizing the speech-to-text results with __wrongly spoken parts colored__, iii) providing sophisticated __phonetic-level analysis__ from AI, iv) __scoring the user speeches__.
The platform has intuitive, visually appealing interface. Overall users' usability score is 4.2/5.0 with users making comments as following:

> "It is helpful because it gives syllable level feedback, and makes it easier to correct myself."

> "I like the way the program allows the users to see the correct pronunciation so that they can practice the correct way to pronounce words."

### Libraries and frameworks

**Backend**
- Django framework
- SpeechAce API (https://docs.speechace.com/)
- Google Cloud STT and TTS engines:
    - google-api-python-client
    - google-cloud-speech
    - google-cloud-texttospeech
    - some other google libraries
- Audio processing libraries:
    - SoundFile
    - pydub
    - simpleaudio

**Frontend**
- ReactJS
- Grommet - for styling UI components
- Axios - REST framework
- React Redux

