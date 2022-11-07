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
![](https://michaelscottfulton.com/images/research/diver_detection/standard_examples.png "Faster-RCNN, YOLO, and SSD detectors.")
![](https://michaelscottfulton.com/images/research/diver_detection/detector.png "The Deep Diver Detector")
</div>

After this, I worked with another PhD student, Karin de Langis, on developing a new dataset for diver detection called VDD-C, improving on the DDD (Deep Diver Dataset).  
VDD-C consists of over 100,000 images of divers in video contexts, with all kinds of equipment, positions, multiple divers occluding one another, etc. 

<div align="center">
![](https://michaelscottfulton.com/images/research/diver_detection/vddc_dists_a.png "Diver Apperence Distributions")
![](https://michaelscottfulton.com/images/research/diver_detection/vddc_dists_b.png "Diver Position Distributions")
</div>

The increased rigerousness of this dataset improved the state of the art performance for diver detectors, simply by providing enough data to train with. 
However, we also explored the use of video detection methodologies on diver detection for the first time, and profiled common object detectors not only on their per-image accuracy, but on the extent to which they struggled in video contexts.

<div align="center">
![](https://michaelscottfulton.com/images/research/diver_detection/vddc_ddd.png "VDD-C vs. DDD")
![](https://michaelscottfulton.com/images/research/diver_detection/vddc_res.png "VDD-C Standard Result")
![](https://michaelscottfulton.com/images/research/diver_detection/stability.png "Stability Metrics")
</div>

I also worked for a time on extending the capabilities of diver detectors into predicting the future motion of divers. Undergraduate student Tanmay Agarwal, under my direction, adapated some LSTMs designed for pedestrian motion prediction to diver motion prediction, giving reasonbly accuracte predictions up to 2 seconds in the future.

<div align="center">
![](https://michaelscottfulton.com/images/research/diver_detection/lstm_training.png "LSTM Training Pipeline")
![](https://michaelscottfulton.com/images/research/diver_detection/lstm_preds.png "LSTM Diver Predictions")
![](https://michaelscottfulton.com/images/research/diver_detection/lstm_error.png "LSTM Error Rates")
</div>

Since that time, my work on diver perception has shifted from detection to body pose estimation (no publications as yet). 
I have been using DeepLabCut to develop a diver pose estimator which has allowed the development of higher-order algorithms for underwater HRI.

<iframe width="560" height="315" src="https://www.youtube.com/embed/m6-FUF4XOdg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>