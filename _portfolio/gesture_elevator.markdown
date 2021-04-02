---
layout: post
title: Gesture Elevator
description: 2020
img: /img/gesture_elevator.jpg
---

Developed for the course "Physical Interaction" at KTH Royal Institute of Technology.

<div class="video-container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/qu5Mt_bnD24" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<br />
We set out to build a concept of a touchless elevator, that can be controlled through hand gestures. This design is especially relevant in COVID-19 times, as it allows to avoid touching buttons in public places. Also, it was a great opportunity for us to explore hand gesture interaction.


We have created a prototype of a gesture-based control system for a small elevator model. The elevator itself is made out of laser cut MDF, with a servo motor attached to the back, that controls it through a nylon thread and a pulley system.


The servo motor is connected to an Arduino, which acts on data from a Leap Motion Controller. The gesture interpretation is done in a Java application running on a computer before passing it to the Arduino.


We indicate what floor the user selects by an arrow indicator that moves across a semicircle, and yellow leds, similar to old fashioned floor indicators.