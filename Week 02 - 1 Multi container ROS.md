---
title: Week 02 - 1 Multi container ROS
created: '2020-10-05T19:20:14.028Z'
modified: '2020-10-05T19:35:55.846Z'
---

# Week 02 - 1 Multi container ROS
## Coupled vs Decoupled
Coupled means everything is one big blob, whereas in decoupled systems, when something goes down, the rest is able to stay up

## Multiple containers = Decoupled applications
Each container should have 1 concern!

\+
- Improved overview
- Better isolation
- Easier maintenance
- More robust
- More dynamic
- Better security

\-
- More containers
- Possible performance hit
- More tooling needed

## Docker compose
Get app running in one command: `docker-compose up`
Example: `docker-compose.yml`
```yaml
version: '3.5'
services:
  master:
    image: 'ros:noetic-ros-core'
    container_name: master
    hostname: master
    environment:
      - 'ROS_HOSTNAME=master'
    command: roscore
```
Get logs with `docker logs`
Close with `docker-compose down`

## Docker swarm
Docker on multiple computers
Multiple docker hosts act as manager and workers or both. 
- Can run services (spawn containers)
- Can facilitate an overlay network on all nodes

