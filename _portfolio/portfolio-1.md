---
title: "5G Video transmission of remote driving for harbor container truck or mine truck"
excerpt: "Real-time 5G/WebRTC video transmission system for autonomous truck remote takeover. <br/><img src='/images/harbor.png' width='500'>"
collection: portfolio
---

## Overview
This project is part of the Harbor Autonomous Container Trucks solution. When a truck's 
autopilot fails, the remote driving platform takes over. I independently built the full 
5G/WebRTC video transmission pipeline — from the truck's domain controller (NVIDIA Jetson 
Orin) through an Aliyun cloud relay to the remote driving platform rendering 8 GMSL camera streams in real time.

![180 Wide View](/images/harbor.png)
*Figure 1: Remote driving for container truck.*

![180 Wide View](/images/mine.png)
*Figure 2: Remote driving for mine truck*

## Key Contributions
**1 Preliminary research**
- Compiling and developing of WebRTC source code; deploying WebRTC stream media server

**2 System Design**
- Authored architecture design, testing manual, and development documentation

**3 Development**
- WebRTC video push client for truck (NVIDIA Jetson Orin, ARM64)
- WebRTC stream media server for cloud relay
- WebRTC video pull and rendering module for remote driving platform

**4 Optimization**
- GPU/CUDA-accelerated video decoding and rendering
- End-to-end latency: **50 ms** (local network), **150 ms** (5G same city), **250 ms** (global)
- 180° wide-view front camera via video stitching of two front cameras

![180 Wide View](/images/180.png)
*Figure 3: 180° stitched front camera view*

**5 Result**
- Delivered a complete 5G public network video transmission product comparable to 
  Tencent's solution
- Full system designed, implemented, and deployed independently

## Tech Stack
Nvidia Jetson, embedded system, WebRTC, CUDA, C++, OpenCV, Websockets, Cloud server, Visual Studio, VS code, QT, Linux
