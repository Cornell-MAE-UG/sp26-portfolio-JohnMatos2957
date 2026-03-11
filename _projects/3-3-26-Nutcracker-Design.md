---
layout: project
title: Nutcracker Design
description: Macadamia Nut Cracker Problem
technologies: [None]
image: /assets/images/MacadamiaCracker.jpg
---

The objective of this problem was to create a nutcracker with sufficient dimensions in order to crack a macadamia nut, discuss how usable the designed nutcracker was, and to make a new nutcracker design utilizing a linear actuator.

Constraints and input parameters include the average load needed to crack a macadamia nut (~2180 N), the average size of a macadamia nut (20 mm diameter), and average grip strength of an adult (~300 N).

I started by calculating the lengths that the handle would need to be by using an arbitrary length of the macadamia nut from the hinge of 30 mm. By setting all moments about the hinge equal to zero, the length was equated to be ~188 mm.

Based on these dimensions, I stated that the nutcracker would be a bit long for daily use, as it is in total over 8 inches long. The arms of the nutcracker would be around 2 inches apart based on my design, so it is possible for someone to use this with just one hand, but two might be necessary for people with a weaker grip. A different system with more mechanical advantage would be optimal for daily use.

![Macadamia Actuator Cracker]({{ "/assets/images/MacadamiaActuatorCracker.jpg" | relative_url }}){: .inline-image-l}

The above Macadamia nut cracker was made with an IP65 Mini Linear Actuator, producing a force of approximately 751 Newtons with a stroke length of 1 inch, taking into account all the previous parameters such as size and strength needed to break the nut.

Using the moments about the hinge and an arbitrary nut distance of 30 mm from the hinge, I calculated the distance of the actuator to be around 9 cm, or around 3.5 inches from the hinge.

This design is much more usable than the previous one, as it is smaller and does not require any applied force from a user. All the force needed is generated from the linear actuator, allowing for people of all strengths to utilize it.