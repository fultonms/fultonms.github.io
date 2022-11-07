---
title: "Diver Detection Detection"
excerpt: "Deep learning methods for detection of divers"
excerpt-image: "research/diver_detection/excerpt.gif"
collection: research
relevant-pubs: 
    RAL-19: /publication/2019-05-01-ral-diver-following
    IROS-21: /publication/2021-10-01-iros-vddc
---
The task of diver detection is challenging, but key to underwater human-robot interaction. For an AUV and a diver to effectively collaborate, the AUV must know the diver's location.
My earliest work on this subject was under the direction of my fellow PhD student Md. Jahidul Islam, developing a novel diver detection algorithm and comparing it to other commonly used methods.

<div align="center">
    <img alt="This figure shows the network architectures of Faster RCNN, YOLO, and SSD." src="https://michaelscottfulton.com/images/research/diver_detection/standard_examples.png"></img>
    <img alt="This figure shows the network architecture of the Deep Diver Detector." src="https://michaelscottfulton.com/images/research/diver_detection/detector.png"></img>
</div>

After this, I worked with another PhD student, Karin de Langis, on developing a new dataset for diver detection called VDD-C, improving on the DDD (Deep Diver Dataset).  
VDD-C consists of over 100,000 images of divers in video contexts, with all kinds of equipment, positions, multiple divers occluding one another, etc. 

<div align="center">
    <img alt="This figure shows that VDD-C has a much higher variety of diver appearences." src="https://michaelscottfulton.com/images/research/diver_detection/vddc_dists_a.png"></img>
    <img alt="This figure shows that VDD-C has a much wider diver position distribution" src="https://michaelscottfulton.com/images/research/diver_detection/vddc_dists_b.png"></img>
</div>

The increased rigerousness of this dataset improved the state of the art performance for diver detectors, simply by providing enough data to train with. 
However, we also explored the use of video detection methodologies on diver detection for the first time, and profiled common object detectors not only on their per-image accuracy, but on the extent to which they struggled in video contexts.

<div align="center">
    <img alt="This table shows that VDD-C trained models outperform those trained on DDD, and that the VDD-C test set is more challenging." src="https://michaelscottfulton.com/images/research/diver_detection/vddc_ddd.png"></img>
    <img alt="This table shows standard metrics for VDD-C trained models, with SSD and YOLO models doing quite well." src="https://michaelscottfulton.com/images/research/diver_detection/vddc_res.png"></img>
    <img alt="This table shows temporal stability for VDD-C trained models, demonstrating that while SSDs are the best at single images, for temporal stability, YOLO works better." src="https://michaelscottfulton.com/images/research/diver_detection/stability.png"></img>
</div>

I also worked for a time on extending the capabilities of diver detectors into predicting the future motion of divers. Undergraduate student Tanmay Agarwal, under my direction, adapated some LSTMs designed for pedestrian motion prediction to diver motion prediction, giving reasonbly accuracte predictions up to 2 seconds in the future.

<div align="center">
    <img alt="This figure shows the training pipeline of the diver prediction LSTMS." src="https://michaelscottfulton.com/images/research/diver_detection/lstm_training.png"></img>
    <img alt="This figure shows some examples of predicted diver trajectories." src="https://michaelscottfulton.com/images/research/diver_detection/lstm_preds.png"></img>
    <img alt="This figure shows diver prediction error rates, demonstrating that predictions under 2 seconds in the future are possible, but not necessarily accurate" src="https://michaelscottfulton.com/images/research/diver_detection/lstm_error.png"></img>
</div>

Since that time, my work on diver perception has shifted from detection to body pose estimation (no publications as yet). 
I have been using DeepLabCut to develop a diver pose estimator which has allowed the development of higher-order algorithms for underwater HRI.

<iframe width="560" height="315" src="https://www.youtube.com/embed/m6-FUF4XOdg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>