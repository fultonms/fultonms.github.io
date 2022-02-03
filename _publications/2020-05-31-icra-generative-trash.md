---
title: "A Generative Approach Towards Improved Robotic Detection of Marine Litter"
collection: publications
permalink: /publication/2020-05-31-icra-generative-trash
excerpt: 'A method for generating synthetic images of underwater trash, improving detector performance by providing more examples.'
date: 2020-05-31
venue: 'IEEE International Conference on Robotics and Automation (ICRA)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9197575'
citation: 'J. Hong, M. Fulton and J. Sattar, "A Generative Approach Towards Improved Robotic Detection of Marine Litter," 2020 IEEE International Conference on Robotics and Automation (ICRA), 2020, pp. 10525-10531, doi: 10.1109/ICRA40945.2020.9197575.'
bibtex: 'https://fultonms.github.io/files/bibtex/2020-irca-generative.bib'
---
## Abstract
This paper presents an approach to address data scarcity problems in underwater image datasets for visual detection of marine debris. The proposed approach relies on a two-stage variational autoencoder (VAE) and a binary classifier to evaluate the generated imagery for quality and realism. From the images generated by the two-stage VAE, the binary classifier selects "good quality" images and augments the given dataset with them. Lastly, a multi-class classifier is used to evaluate the impact of the augmentation process by measuring the accuracy of an object detector trained on combinations of real and generated trash images. Our results show that the classifier trained with the augmented data outperforms the one trained only with the real data. This approach will not only be valid for the underwater trash classification problem presented in this paper, but it will also be useful for any data-dependent task for which collecting more images is challenging or infeasible.