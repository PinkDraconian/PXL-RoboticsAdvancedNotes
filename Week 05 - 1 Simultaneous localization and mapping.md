---
title: Week 05 - 1 Simultaneous localization and mapping
created: '2020-11-01T19:30:48.542Z'
modified: '2020-11-05T10:09:17.444Z'
---

# Week 05 - 1 Simultaneous localization and mapping
## Estimation methods
- Recursive Bayes Filters
Allow robots to continuously update their most likely position
  + Kalman
  + Extended Kalman
  + Particle

## Localization methods
- Relative
  + Odometry
    - Use of motion sensors to change position over time. Errors continuously increase. Errors (Skidding, ...)
  + Inertial Navigation
    - Navigation device that uses accelerometers and gyroscopes to calculate, by dead reckoning, the position, orientation and velocity of a moving object without external references.
- Absolute
  + Beacons
  + Vision system

## Dead reckoning
The process of calculating one's current position by useing a previously determined position, or fix, and advancing that position based upon known or estimated speeds over elapsed time and course

## Visual Odometry
Determining equivalent odometry information using sequential camera images
- Monocular and sterio
- Feature based and direct
- Visual inertial

### Visual odometry algorithm
1. Acquire input images
2. Image correction (Image processing)
3. Feature detection
4. Check flow field vectors for potential tracking errors and remove outliers
5. Estimation of camera position
6. Periodic repopulation of trackpoints to maintain coverage across the image

## Egomotion
3D motion of a camera withing an environment (Camera in car)

## SLAM Applications
- Automatic car piloting
- Rescue takss
- Plantary, aerial, oceanic, ... explotation
- Augmented reality
- Visual surveillance systems
- Medicine

## Introceptive vs exteroceptive
- Relative vs absolute position measurements

## Acoustic sensors
Use time of flight to measure location (Sonar, ultrasonic)

## Laser rangefinders
ToF and phase-shift techniques to measure position. High speed and high accuracy

## Visual sensors
- Monocular
- Stereo
- RGB-D

## SLAM Maps
- Feature maps
  - Sparse number of objects to represent a map
- Occupancy grids

## Sparse vs Dense methods for visual SLAM
- Sparse: Small selected subset of image frame
- Dense: All pixels

## Feature-based vs Direct methods for visual SLAM
Extract features vs tracking photometric (Intensity differences)

## Loop closure
- Final refinement step
- Process of observing the same scene by non-adjacent frames and adding a constraint between tehm, reducing the drift in the pose estimation
- Feature descriptors to find previous frame
### Issues with loop closure
- False positive (Perceptual aliasing). 2 places are perceived as the same
- False negative (Perceptual variability). One place is perceived as 2 different places (Shadows for example)

## Back-end optimization
- Drift is inevitable
- Camera pose optimization
- Bundle adjustment (Graph optimization)
