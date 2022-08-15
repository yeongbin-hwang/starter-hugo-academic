---
title: "EVA"
summary: "Course project in EE474 Mobile Computing and Systems for Intelligent Living, Spring 2020"
tags:
  - AI
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
url_code: 'https://github.com/elianakim/EE595_BeatSaver'
url_pdf: 'uploads/ee595_report.pdf'
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

A conductor is a messenger for the composer, and musicians’ duty is to fully understand the conductor’s messages through gestures and produce unified music in a musical ensemble. However, in many cases where the conductor is absent, musicians inevitably resort to their faint memories or abstract note-taking to infer the conductor’s instructions. To revamp this limitation, we propose BeatSaver that converts conducting gestures to metronome beats. Musical details that a conductor instructed are recorded in beats and dynamics so that musicians can refer to even when they are practicing on their own. BeatSaver consists of Time Signature Classifier, Beat Detector, and Musical Dynamics Classifier, which we prove their effectiveness through real-world experiments. BeatSaver is lightweight and practical as it only utilizes Arduino Nano 33 BLE Sense attached to the conducting baton and an external server to extract the details after the practice session, making it easily applicable in the wild.