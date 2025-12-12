---
layout: project
title: MAE 4272 Blade Design
description: Design Project
technologies: [Autodesk Fusion, MATLAB]
image: /assets/images/blade-with-parameters.png
---


For this project, we were asked to design a small-scale wind turbine blade capable of maximizing aerodynamic power while remaining structurally safe and within all operational limits. The goal was to create a blade that performed reliably under a realistic Weibull wind distribution while staying below stress and RPM constraints, ultimately balancing efficiency, safety, and manufacturability.

![Our blades with parameters]({{ "assets/images/CAD-Rendering.png" | relative_url }}){: .inline-image-r style="width: 200px"}

Our design process centered on selecting a target angle of attack, choosing an appropriate airfoil, and defining chord and twist distributions that would maintain efficient lift along the span. Using a MATLAB model adapted from Lab 5, we targeted a 6° operating angle of attack and used NACA 4412 data to shape the aerodynamic profile before linearizing the geometry from root to tip. Each iteration refined lift generation while keeping stresses within limits and aiming for an operating speed near 1500 RPM, with CAD confirming the feasibility of each update.

The blades were tested across wind speeds ranging from 8 to 16 Hz by allowing the turbine to spin freely before gradually applying load through the torque brake. This produced full RPM–torque curves for each speed, and LabVIEW measurements of rotational speed, torque, and power allowed us to generate power curves, identify peak power, and compare expected versus actual performance.

![Power Curves]({{ "/assets/images/power-curve.png" | relative_url }}){: .inline-image-r style="width: 200px"}

My contribution focused on developing the MATLAB code used to define blade parameters and analyze the experimental data. I processed torque and RPM measurements, computed power across wind speeds, and identified peak operating points that helped evaluate how closely the final blade aligned with our predictions.
