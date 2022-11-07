---
title: "HREye: Emitted Light for AUV Communication and Gaze"
excerpt: "A new device and system for light-based robot communication, including a new capability for underewater robots: gaze indication"
excerpt-image: "research/hreye/excerpt.gif"
collection: research
relevant-pubs:
    arXiV-22: /publication/2022-09-15-arxiv-hreye
---
AUVs commonly use digital displays to communicate with divers. However, digital displays are hard to read at a distance or at an angle. 
In order to allow communication at further distances, we have previously proposed Robot Communication Via Motion, and now we present a light-based communication method called HREye.

<div align="center">
    <img alt="The HREye system operating on board LoCO" src="https://michaelscottfulton.com/images/research/hreye/loco_hreye.png">
    <img alt="The evolution of light-based communication for AUVs." src="https://michaelscottfulton.com/images/research/hreye/led_evolution.png">
</div>

Our HREye system was developed to take advantage of the long distances at which light can travel in adequate visibility underwater. We also wanted to take advantage of a wide array of colors and of the shape in which these lights are arranged. A sequence of light animations on the HREyes is called a luceme. 

<div align="center">
    <img alt="The active lucemes of HREye" src="https://michaelscottfulton.com/images/research/hreye/active_lucemes.png">
</div>

Active lucemes communicate a single piece of information, and perform only slightly less accurately than a digital display (OLED). Even people who haven't been trained on the meaning of lucemes can identify them with relative accuracy. 
<div align="center">
    <img alt="Comparison between HREye, Untrained HReye, and OLED conditions." src="https://michaelscottfulton.com/images/research/hreye/condition_compare.png">
    <img alt="Comparison between HREye and OLED for communicaiton phrases." src="https://michaelscottfulton.com/images/research/hreye/per_luceme.png">
</div>

However, HREyes are capable of more than just active lucemes. In ocular mode, an HREye can mimic the blinking and gaze directions of a human eye.
<div align="center">
    <img alt="The ocular lucemes of the HREye device" src="https://michaelscottfulton.com/images/research/hreye/ocular_lucemes.png">
</div>

The chart below shows that people can identify the gaze direction of ocular lucemes, with a small amount of error (average 21◦).
<div align="center">
    <img alt="Results of gaze indication using HREye." src="https://michaelscottfulton.com/images/research/hreye/ocular_results.png">
</div>

