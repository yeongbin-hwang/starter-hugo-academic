---
title: "PitchPerfect: Tinder for Amateur Music Lovers"
summary: "Course project in KAIST CS473 Introduction to Social Computing, Fall 2020"
tags:
  - HCI
date: '2020-12-23T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ""
  focal_point: Smart

links:
  - icon: 
    icon_pack: 
    name: Demo
    url: https://sanghyeon-lee.github.io/PitchPerfect/
url_code: 'https://github.com/SangHyeon-Lee/PitchPerfect'
url_pdf: ''
url_slides: 'https://docs.google.com/presentation/d/e/2PACX-1vRDYC3LR6Tq_lkYYPBD48LEr5Aon09gRfOqTyKlDu03NLQHvMrNR3vNACWvQZYgZpeCF0U9EM-6Nehl/pub?start=true&loop=false&delayms=3000'
url_video: 'https://youtu.be/0H4-MHTlwbI'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

A conductor is a messenger for the composer, and musicians’ duty is to PitchPerfect provides an easy-to-use interface to achieve two goals: (1) help amateur musicians find suitable collaborators and (2) provide tools for managing music collaboration projects. To achieve the first goal, PitchPerfect has project summary pages (Figure1) that provide an overview of the project and personal profile pages (Figure2) for other users to get a sense of what kind of musician that person is. We designed those pages to contain all information necessary for the users to make an informed decision, such as parts involved in a music or musical preferences. At the same time, we used standard symbols and recurring designs throughout our interface to deliver such information concisely and clearly. For example, we introduce the proficiency emoticons 🐣 for level1, 🐥 for level2, 🐦 for level3) in the signup process and use them in personal profile pages. Also, when displaying a project, the same or slightly modified design (white rectangle with round corners with music title, required parts, and proficiency tag inside) is used in all pages so that the user can naturally associate that design component with a project. In our survey, we asked the users to rate how helpful the project summary page and personal profile page were in finding a suitable project to join on a Likert scale of 1-5. Out of the 20 users that participated in our survey, 15 users rated 4 or above for the project summary page, and 17 users rated 4 or above for the personal profile page. To achieve the second goal, we designed novel UI components to provide communication tools for music collaboration. Two most unique tools are: shared annotatable sheet music (Figure3 and Figure4) and moveable pins with threads (Figure3 and Figure5). During music collaboration, musicians often add annotations to play in sync (ex. down bow annotation for all violinists to slide their bows in the same direction) and make modifications to music (ex. adding a crescendo to measure 1). These annotations and changes are difficult to communicate through text but can be easily communicated with shared annotatable sheet music. Musicians also often discuss certain parts at length for various reasons (ex. that part is important, that part does not harmonize well...etc). The moveable pins are designed to aid such discussion. To make the pins point to the part in question, team members can freely adjust the location of pins and the location changes are reflected the next time any member enters the sheet music page. Also, to keep those discussions independent, each pin is connected to its own discussion thread. In our survey, we also asked the users to rate how helpful such tools were in collaboration with team members on a Likert scale of 1-5. Out of the 20 users that participated in our survey, 14 users rated 4 or above for shared annotatable sheet music and 18 users rated 4 or above for moveable pins with linked threads. Moreover, one user commented “this interface will open a new paradigm of music collaboration.” 
