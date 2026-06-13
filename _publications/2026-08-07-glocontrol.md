---
title: "GloControl: Global Teleoperation of Robots for Disaster Response Using WebRTC over Internet"
collection: publications
category: underreview
permalink: /publication/2026-global-control
excerpt: 'A global control system for disaster response robot.'
date: 2026-08-07
venue: 'International Performance Computing and Communications Conference (IPCCC)'
header:
  teaser: "glocontrol-demo.gif"
paperurl: 'https://arxiv.org/abs/YOUR_ID'
citation: 'Chao He and Da Hu. (2026). &quot;GloControl: Global Teleoperation of Robots for Disaster Response Using WebRTC over Internet. &quot; <i>****</i>.'
---

## Abstract
Global teleoperation of robots in disaster response scenarios demands low-latency, infrastructure-independent communication capable of functioning without local network infrastructure, which is often destroyed or unavailable at disaster sites. Existing teleoperation systems rely on specialized hardware, VPN tunnels, or dedicated servers, and few formally characterize end-to-end latency under real-world conditions. In this paper, we present GloControl, a WebRTC-based system that unifies live video feedback and motion control commands within a single WebRTC session via the Janus media server, leveraging the WebRTC data channel for real-time robot control. By utilizing WebRTC's built-in NAT traversal via ICE, STUN, and TURN, the system is operable from anywhere on Earth where Internet connectivity is available via 5G or LEO satellite networks such as Starlink, requiring only a standard web browser on the operator side. We deploy and evaluate GloControl on a Yahboom Rosmaster-X3-Plus robot equipped with a NVIDIA Jetson NX, and characterize end-to-end latency across seven test configurations spanning operator, cloud server, and robot locations across China and the United States, including an intercontinental link of 13{,}327\,km. Control latency, measured via a ping-pong scheme over the WebRTC data channel, ranges from 133\,ms (same-city) to 283\,ms
(intercontinental), and end-to-end video latency is 183\,ms (same-city) and approximate 330 ms (intercontinental). Cloud server placement is identified as the dominant latency design variable, and a Seattle-based server is shown to outperform Hong Kong and Tokyo servers for China-to-USA teleoperation. These results confirm the feasibility of WebRTC over 5G and Starlink as a viable transport for real-time disaster response robot teleoperation deployable where fixed network infrastructure cannot be assumed. Our project is availabel at https://github.com/Saturn-Chao-He/glocontrol.

## Method Overview

<div style="text-align: center;">
  <img src="/images/glocontrol-arc.png" 
       alt="GloControl system architecture" 
       width="700">
  <p><em>Figure 1: GloControl system architecture. (The robot streams live
video and receives motion commands through a cloud-hosted Janus
WebRTC server over the Internet. The operator requires only a
standard web browser. Internet connectivity can be provided by
5G or Starlink, enabling operation
in infrastructure-denied disaster environments.)</em></p>
</div>

<br>

<div style="text-align: center;">
  <img src="/images/glocontrol-robot.png" 
       alt="Disaster response robot" 
       width="500">
  <p><em>Figure 2: Disaster response robot is holding medicine and gauze and ready to deliver.</em></p>
</div>

<br>

<div style="text-align: center;">
  <img src="/images/glocontrol-ui.png" 
       alt="GloControl operator interface" 
       width="700">
  <p><em>Figure 3: GloControl operator interface. (Left: live video  from the robot camera and bitrate cap control. Right: motion control buttons and real-time control latency display.)</em></p>
</div>

<br>

<div style="text-align: center;">
  <img src="/images/glocontrol-rtt.png" 
       alt="RTT" 
       width="400">
  <p><em>Figure 4: RTT ping-pong scheme over the data channel. (both timestamps recorded on the operator clock, no clock synchronization required.)</em></p>
</div>

<br>

<div style="text-align: center;">
  <img src="/images/glocontrol-video_latency.png" 
       alt="Video latency" 
       width="500">
  <p><em>Figure 5: The pipeline of video stream processing and transmission.</em></p>
</div>

<br>

## Results

<div style="text-align: center;">
  <img src="/images/glocontrol-map.png" 
       alt="Map" 
       width="700">
  <p><em>Figure 6: Cities on the map in this experiment. (blue: operator, red: cloud server, green: robot.)</em></p>
</div>

<br>

<div style="text-align: center;">
  <img src="/images/glocontrol-stopwatch.png" 
       alt="Stopwatch" 
       width="500">
  <p><em>Figure 7: End-to-end highest latency and lowest latency for video reviewer in the same city (T7). (up: highest 259 ms, bottom: lowest 124 ms, mean: 183 ms.)</em></p>
</div>


## Demo Video

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/PIzeexqpmoQ" 
  title="Global control of robot demo" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; 
         encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

## Citation
```bibtex
@article{he2026glocontrol,
  author  = {Chao He and Da Hu},
  title   = {GloControl: Global Teleoperation of Robots for Disaster Response Using WebRTC over Internet},
  journal = {****},
  year    = {2026}
}
```
