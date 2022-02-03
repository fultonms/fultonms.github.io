---
title: "Predicting the Future Motion of Divers for Enhanced Underwater Human-Robot Collaboration"
collection: publications
permalink: /publication/2021-10-01-iros-prediction
excerpt: 'A method for predicting the future motion of divers using LSTMs.'
date: 2021-10-01
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9636374'
citation: 'T. Agarwal, M. Fulton and J. Sattar, "Predicting the Future Motion of Divers for Enhanced Underwater Human-Robot Collaboration," 2021 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2021, pp. 5379-5386, doi: 10.1109/IROS51168.2021.9636374.'
bibtex: 'https://fultonms.github.io/files/bibtex/2021-iros-prediction.bib'
---
## Abstract
Autonomous Underwater Vehicles (AUVs) can be effective collaborators to human scuba divers in many applications, such as environmental surveying, mapping, or infrastructure repair. However, for these applications to be realized in the real world, it is essential that robots are able to both lead and follow their human collaborators. Current algorithms for diver following are not robust to non-uniform changes in the motion of the diver, and no framework currently exists for robots to lead divers. One method to improve the robustness of diver following and enable the capability of diver leading is to predict the future motion of a diver. In this paper, we present a vision-based approach for AUVs to predict the future motion trajectory of divers, utilizing the Vanilla-LSTM and Social-LSTM temporal deep neural networks. We also present a dense optical flow-based method to stabilize the input annotations from the dataset and reduce the effects of camera ego-motion. We analyze the results of these models on scenarios ranging from swimming pools to the open ocean and present the model’s accuracy at varying prediction lengths. We find that our LSTM models can generate predictions with significant accuracy 1.5 seconds into the future and that stabilizing LSTM models significantly improves trajectory prediction performance.