---
title: Week 02 - 2 ROS2
created: '2020-10-08T17:49:38.853Z'
modified: '2020-10-08T17:55:21.827Z'
---

# Week 02 - 2 ROS2
## ROS1 Characteristics
- A single robot
- Workstation-class computational resources on board
- No real-time requirements
- Excellent network connectivity required
- Applications in research, mostly academia
- Maximum flexibility

## ROS2 Use cases
- Teams of multiple robots
- Small embedded platforms
- Real-time systems
- Non-ideal networks
- Production environments
- Prescribed patterns for building and structuring systems

## ROS2 Arcitecture
| _ | ROS1 | ROS2 |
| --- | --- | --- |
| Application Layer | Master, Application | Application |
| Middleware Layer | Client Library, API, TCP/UDPROS | Client library, Abstract DDS Layer, DDS, API | 
| OS Layer | Linux | Linux / Windows / Max / RTOS |

## DDS vs OSI
| _ | _ |
| --- | --- |
| ROS 2 | Application |
| DDS | Presentation, Session |
| UDP/IP | Transport, Network |
| Ethernet | Data Link, Physical |

