---
title: Week 06 - Multi Agent Systems & Swarms
created: '2020-11-09T17:33:54.424Z'
modified: '2020-11-09T17:55:17.265Z'
---

# Week 06 - Multi Agent Systems & Swarms

## DAI
- Parallel AI
  + Distributed hardware architectures
  + Increase speed
- DPS
  + Very rigid, little flexibility
  + Sharing resources and knowledge
- MAS
  + Network of individual agents
  + Communicate and share to solve a problem that one could not solve on its own

## Agent definition
Flexible autonomous entity capable of perceiving the environment through the sensors connected to it. These act on the environment through actuators

## Agent characteristics
- Situatedness
  + Inputs because environment interaction act directly upon the environment through actuators
- Autonomy
  + Choose actions independently
- Inferential capability
  + Ability to work on abstract goal specifications
- Responsiveness
  + Perceive environment condition and respond timely
- Proactiveness
  + Exhibit a good response to opportunistic behavior
- Social behavior
  + Interact with external sources when needed for goal

## MAS benefits
- Speed increase
- Graceful degradation (Agents can fail)
- Scalability & flexibility
- Reduced cost
- Reusability

## MAS critical challenges
- Environment
  + Everyones envirment is being modified by everyone
- Perception
  + Limited sensing causes sub-optimal decision due to not knowing everything
- Abstraction
  + Not every agent experiences everything but need to learn from other's experiences
- Conflict resolution
  + Stem from lack of global view
- Inference
  + A conclusion based on evidence and reasoning is hard because the env is being changed by everyone

## MAS internal architecture
- Homogeneous
  + All agent have the same internal architecture
- Heterogeneous
  + Agents differ in ability structure and functionality

## MAS Agent organization
- Hierarchical
- Holonic
- Coalitions
- Teams (Similar to coalition but more together)

## MAS communication
- Local communication
  + No intermediator
- Blackboards
  + Data repository whoch provides efficient storage and retrieval

## MAS decision making
- Learning
  + Fixed
  + Adaptive (Active, reactive, based on consequence)
- Goals (Single, multiple)

### SMACH
Task level architecture for rapidly creating complex robot behavior. Building hierarchical state machines

## Swarms
Individual robot is not meaningful. Desired behavior emerges when there are many

### Pros of swarms
- Adaptability
- Robustness
- Scalability

### Cons of swarms
- Behaviour hard to predict and prove elegibility
- Current communication architectures don't match requirements
- Testing swarms is a big issue, often too risky
