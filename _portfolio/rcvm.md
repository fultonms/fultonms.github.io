---
title: "RCVM: Robot Communication Via Motion"
excerpt: "My method for robot-to-human communication using motion of AUVs."
excerpt-image: "research/rcvm/excerpt.gif   "
collection: research
relevant-pubs:
    ICRA-19: /publication/2019-05-01-icra-rcvm
    RSS-22: /publication/2022-07-01-rss-rcvm
    IROS-22: /publication/2022-11-01-iros-rrcvm
    THRI-21:  /publication/2021-11-01-thri-robot-communication-via-motion
---
Many AUVs use small digital displays to convey information to divers working collaboratively with them. However, these displays can be hard to read. 
To allow AUVs to communicate more freely, regardless of the relative position of divers, I created Robot Communication Via Motion (RCVM) for AUVs. 
The gestures of this communication method are called kinemes, and are shown below.

<div align="center">
    <img alt="A table demonstrating Aqua's kinemes." src="https://michaelscottfulton.com/images/research/rcvm/kinemes.png">
</div>

In an initial study, RCVM outperformed a light-based baseline method at all levels of education (None, names of kinemes, full training).

<div align="center">
    <img alt="A comparison of RCVM and a light-based baseline at different education levels." src="https://michaelscottfulton.com/images/research/rcvm/edu_comp.png">
</div>


Following this, we compared RCVM with a light-based communication method, a sound-based method, and a digital display. We also compared RCVM's effectiveness at different viewpoints and kineme content. 
We discovered that RCVM is more resistant to change in viewpoint than other methods.

<div align="center">
    <img alt="RCVM vs other systems" src="https://michaelscottfulton.com/images/research/rcvm/system.png">
    <img alt="RCVM vs other systems at a variety of viewpoints." src="https://michaelscottfulton.com/images/research/rcvm/viewpoints.png">
    <img alt="RCVM vs other systems with different content." src="https://michaelscottfulton.com/images/research/rcvm/content.png">
</div>

We also implemented all of these systems for a terrestrial robot and an aerial robot. The following confusion matrices include all of these systems.
<div align="center">
    <img alt="A confusion matrix for four different communication systems." src="https://michaelscottfulton.com/images/research/rcvm/multi_system_conf.png">
</div>

Sadman Sakib Enan has built on my work by developing a deep learning architecture which can recognize kinemes. I helped in this work by evaluating human transcription of robot-to-robot kineme conversations, to ensure that humans could also understand robot conversations, making the language universal.
<div align="center">
    <img alt="A diagram of RRCommNet, which can recognize kinemes." src="https://michaelscottfulton.com/images/research/rcvm/rrcom_net.png">
</div>
