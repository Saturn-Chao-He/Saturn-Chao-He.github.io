---
title: "LiWarn: A LiDAR-Based 3D Object Tracking and Speed Violation Warning System for Construction Site Safety"
excerpt: "In-vehicle edge device voice warning "slow down" when speed limits are exceeded. (marked in red on system) <br/><img src='/images/warn.png' width='500'>"
collection: portfolio
---

## Overview
Construction sites are among the most hazardous 
working environments, where speeding vehicles pose significant safety 
risks to workers and equipment. Traditional manual monitoring methods 
are labor-intensive, prone to human error, and unable to provide 
real-time situational awareness or automated intervention.
This work presents LiWarn, 
a LiDAR-based system for automated 3D object detection, multi-object 
tracking, and real-time speed violation warning in construction site 
environments. Five state-of-the-art 3D object detection methods are 
evaluated: PointPillars, SECOND, PointRCNN, Part-A2, and PV-RCNN. 
The best-performing model is integrated with a Kalman filter-based 
multi-object tracker for continuous speed estimation, and an edge 
computing alert pipeline that delivers audible warnings to vehicle 
operators via NVIDIA Jetson and ChipIntelli CI1302 voice chips when 
speed limits are exceeded. A GPS-based vehicle-to-track binding 
mechanism enables targeted per-vehicle alerts without requiring 
additional infrastructure beyond a single LiDAR sensor.

![demo](/images/warn.png)
*Figure 1: In-vehicle edge device voice warning "slow down" when speed limits are exceeded. (marked in red on system)*

[Demo 1](https://youtu.be/4AwM3QyL0vg)


[Demo 2](https://youtu.be/XuNE9SLx9VA)

