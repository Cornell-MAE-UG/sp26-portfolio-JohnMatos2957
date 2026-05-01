---
layout: project
title: Nutcracker Design Pt. 2
description: Macadamia Nut Cracker Problem with Beam Bending
technologies: [None]
image: /assets/images/Revised-Design.jpeg
---

The objective of this problem was to find the areas where our original nutcracker design would deform the most due to an internal bending moment, and to design a cross section that would limit deformation to <2% of length and with an economical design.

Constraints and input parameters include the average load needed to crack a macadamia nut (~2180 N), the average size of a macadamia nut (20 mm diameter), which were all discussed and influenced the design in the previous problem.

In order to find the area of maximum deflection, I began with a simplified FBD of the beam which force was applied to. I also assumed that the original cross section of the beam was a circle with radius of 2 mm.

![Beam FBD]({{ "/assets/images/BeamAssumption.jpeg" | relative_url }}){: .inline-image-l}

In order to find M(x), i used sliced FBDs between AB and BC, treating A as x=0. I found M(x) in both situations, and then used the equation EIy''=M(x) and integrated using boundary conditions to find the equation for deflection.

For section AB, the boundary conditions were y(0)=0 and y(31.623)=0 since there were supports on both ends. For section BC, the BCs were y(31.623)=0 and y'(31.623)=y'(31.623), meaning that the value of the slope for section BC at point B was the same as section AB at point B since it is a continuous beam.

After applying these boundary conditions, i found the point were maximum delfection occured was at the end of the beam where the actuator applied it's load. Its x value was 91.78 mm.

Now, I had to design a new cross section for the beam so it wouldn't bend over 2% of its length. 2% of 91.78mm is 1.8356mm, so that was the maximum deflection that could happen at point C. Using the deflection equation found earlier for section BC, the deflection at point C under original conditions was 33.08 mm, which was much to high. The original I value was 12.566 mm^4, while the necessary I value is 226.469 mm^4.

I decided to design an I-beam to maximize the I value while minimizing area/mass to make it more efficient. I made the flange length "a," the flange and web widths "w," and the web length "a-2w" and calculated the area to be 2aw+w(a-2w). Using algebra, I calculated w for values of "a"=7, 8, 10, and 12. I found that "a" values that were greater than 8 had "w" values that were much less than 1 mm, which would technically make it more economical, but make it more prone to breaking or permanently bending since the metal would be so thin.

I settled on a=8 mm and w=0.956 mm as my final length and width.

![I-Beam]({{ "/assets/images/I-Beam.jpeg" | relative_url }}){: .inline-image-l}

Above is the final beam design.