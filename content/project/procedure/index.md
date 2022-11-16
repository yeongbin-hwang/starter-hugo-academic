---
title: "5G core network testing: let's induce the collision"
summary: "Framework that can execute not only guided fuzzing, but also various attack scenarios"
tags:
  - Cellular Network
date: '2022-08-09T00:00:00Z'

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
url_pdf: 'uploads/projects/procedure/mobisec22.pdf'
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

We implemented a framework based on open5gcore to test the vulnerabilities of the 5G core network. The framework consists of three main components: a <b>Fuzzer</b> that continues testing on UE1 pod, a <b>Controller</b> that captures packets on the host and relays them to the target, and an <b>Analyzer</b> that analyzes the results of the test.

#### Fuzzer
The fuzzer running on the UE1 pod receives the input we want to test and generates various scenarios and sends them to the core network. After the test, change the scenario and send a message to the network and save the results in json format.

#### Controller
The controller is responsible for capturing messages sent to the core network and relaying them to the target network while monitoring br-ngc. In this case, the packet for each test is stored in the form of a pcap while communicating with the UE.

#### Analyzer
The Analyzer analyzes the logs stored in the form of json and displays them in the form of the CLI to determine whether the attack was successful or unsuccessful.

### Libraries and frameworks

- UE, gNB emulator: C++, C, Kubernetes
- Packet capture & relay: Python

<span style="color: gray">
<i>This is done, Fall 2022.</i></span>