---
title: "ADROC: Autonomous Diver-Relative Operator Configuration"
excerpt: "A method for diver approach by AUVs using monocular vision."
excerpt-image: "research/adroc/excerpt.gif"
collection: research
relevant-pubs: 
    ICRA-22: /publication/2022-05-01-icra-adroc
---
The ability of an AUV to navigate relative to a diver is essential for effective diver-AUV interaction.  In order for a robot to communicate with a diver, the robot must be able to position itself in front of a diver, at an appropriate distance from the diver. Our method, autonomous diver-relative operator configuration (ADROC), achieves this using only monocular vision as input. 

<div align="center">
![A diagram which displays ADROC guiding an AUV to a diver, in two examples. In the left example, there is no search process while the AUV searches for a while in the right image.](https://michaelscottfulton.com/images/research/adroc/figure1.png "Figure 1")
</div>

Our method is capable of approaching a diver from a distance (up to 15m has been tested), searching for a diver when one is not initially seen, and adjusting its position relative to the diver in the x, y, and z dimensions. An overview of ADROC is shown below, with the overall algorithm on the right and the state machine which governs the searching/approaching/final position behavior on the left. The diver detector (bounding boxes) and body pose estimator ( 2d body skeleton keypoints) both provide information to the diver-relative position estimator, which generates a center point for the diver, as well as a ratio between the current distance to the diver and the ideal distance. This ratio is referred to as pseudodistance. Finally, the approach controller manages the thruster outputs to move the center point of the diver into the center of the image and reach a psuedodistance of 1.0. Once these conditions are met, the robot has approached the diver successfully.

<div align="center">
![A flowchart displaying the ADROC algorithm](https://michaelscottfulton.com/images/research/adroc/flowchart.png "Flowchart")
</div>

ADROC has been evaluated in a number of closed water experiments (open water trials have been prevented thus far by the COVID-19 pandemic). In 162 approach attempts, ADROC achieved successful approaches in 132 cases. We attempted approaches in clear and cloudy water, from distances of 3, 6, and 9 meters, and from initial angles of 0, 45, and 90 degrees, on a total of 9 divers. Aggregate results are visible below, along with two cases of ADROC approach graphed in terms of the center point and pseudodistance errors used as inputs the PID approach controller.

<div align="center">
![A table of ADROC results. Overall success rate 81.5 percent. Experiment 1 (clear pool), 88.9 percent, Experiment 2 (cloudy pool), 66.7 percent. Success rate decreases as initial distance increases, from 92.6 percent at 3 meters to 68.5 percent at 9 meters. ](https://michaelscottfulton.com/images/research/adroc/table2.png "Table 2")
![A diagram which displays two examples of ADROC approaches in terms of the pseudo distance and center point error. In one example, the error falls until the end. In the other, there are some issues and the error never falls low enough.](https://michaelscottfulton.com/images/research/adroc/figure5.png "Figure 5")
</div>