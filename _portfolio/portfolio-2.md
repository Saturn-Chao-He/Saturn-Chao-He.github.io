---
title: "LiWarn: A LiDAR-Based 3D Object Tracking and Speed Violation Warning System for Construction Site Safety"
excerpt: "In-vehicle edge device voice warning slow down when speed limits are exceeded. (marked in red on system) <br/><img src='/images/warn.png' width='500'>"
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
tracking, and real-time speed violation and proximity warning in construction site 
environments. Five state-of-the-art 3D object detection methods are 
evaluated: PointPillars, SECOND, PointRCNN, Part-A2, and PV-RCNN. 
The best-performing model is integrated with a Kalman filter-based 
multi-object tracker for continuous speed estimation, and an edge 
computing alert pipeline that delivers audible warnings to vehicle 
operators via NVIDIA Jetson and ChipIntelli CI1302 voice chips when 
speed limits are exceeded or worker within proximity limit of vehicle. A GPS-based vehicle-to-track binding 
mechanism enables targeted per-vehicle alerts without requiring 
additional infrastructure beyond a single LiDAR sensor.

![demo](/images/warn.png)
*Figure 1: In-vehicle edge device voice warning "slow down" when speed limits are exceeded (marked in red on system) and warning "attention, person nearby" when the worker within the proximity limit of vehicle.*


## Demo Video 1

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/4AwM3QyL0vg" 
  title="speed warning system demo 1" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; 
         encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>


## Demo Video 2

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/0CKKnBfNn78" 
  title="proximity warning system demo 2" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; 
         encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

## Demo Video 3

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/XuNE9SLx9VA" 
  title="speed warning system demo 3" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; 
         encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

## Demo Video 4

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/-HgY7wCSlL0" 
  title="proximity warning system demo 4" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; 
         encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

