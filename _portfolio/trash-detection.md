---
title: "Trash Detection"
excerpt: "Deep learning methods for detection of underwater debris"
excerpt-image: "research/trash_detection/excerpt.gif"
collection: research
relevant-pubs: 
    ICRA-19: /publication/2019-05-01-icra-rcvm
    ICRA-20: /publication/2020-05-31-icra-generative-trash
---
With my fellow PhD student Jungseok Hong, I have developed a dataset for underwater trash, and performed an evaluation of standard object detection methods using that data.
Our initial work focused on making a trash dataset for community use, which we did achieve with the <a href="https://conservancy.umn.edu/handle/11299/214366">Trash-ICRA19 dataset</a>. We later released the <a href="https://conservancy.umn.edu/handle/11299/214865">TrashCan dataset</a>.


<div align="center">
    <img alt="This table shows the accuracy and inference time results for the original trash paper." src="https://michaelscottfulton.com/images/research/trash_detection/trash_metrics.png">
    <img alt="This figure shows some detections of trash by a variety of networks." src="https://michaelscottfulton.com/images/research/trash_detection/trash_results.png">
</div>

After this exploration into the availability of trash data, we determined that the data scarcity issues inherent in underwater trash detection were an enormous hinderance to progress on the topic.
To attempt to address this, we created a two-stage variational autoencoder (VAE) which generates images of plastic bags and plastic bottles. We also demonstrated that the addition of these generated images could improve trash classification tasks. It is out hope that further generative or low-data efforts can help to solve the trash detection problem, allowing AUVs to contribute to cleaning up the horrible pollutions of the Earth's oceans.

<div align="center">
    <img alt="This image shows the structure of our two-stage Varitional Autoencoder." src="https://michaelscottfulton.com/images/research/trash_detection/trash_vae.png">
    <img alt="This figure shows some examples of generated trash data." src="https://michaelscottfulton.com/images/research/trash_detection/vae_results.png">
</div>