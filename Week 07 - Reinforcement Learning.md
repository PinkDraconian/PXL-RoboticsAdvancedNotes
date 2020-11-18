---
title: Week 07 - Reinforcement Learning
created: '2020-11-18T11:50:15.382Z'
modified: '2020-11-18T12:31:21.780Z'
---

# Week 07 - Reinforcement Learning

## What is reinforcement
Consequence applied that will strengthen future behavior whenever it's preceded by a stimulus

## Law of effect
Responses with satisying effect are more likely to occur again than responses with a discomforting effect

## Operant conditioning
Associative learning process where strength of behavior is modified by reinforcement or punishment

## Skinner box
Box with levers and lights, if the rat uses the right lever when a light comes on, he gets rewarded, else, punished

## Operant conditioning: consequences
1. Positive reinforcement
  - Lever -> Gets food pellet
2. Negative reinforcement
  - Lever -> noise turns off
3. Positive punishment
  - Punishment
4. Negative punishment
  - Taking away a child toy
5. Extinction
  - Remove the reward from an action

## Operant conditioning: Applications
- Addiction and dependence
- Animal training
- Applied behavior analysis
- Behavioral economics
- Gambling
- Entertainment

## Knowledge acquisition bottleneck
If you dont learn, you're just putting all knowledge into a system, such as AI has been doing. It has a ceiling to the capabilities.

## what is RL?
Area of machine learning concerned with how software agents take actions in an environment in order to maximize reward

## RL examples
- Games
- Fly stunt manouvres in helicopter
- Control power station
- Investment portofolio
- Make robots walk

## RL Rewards
- Scalar feedback signal
- Indicates how well agent is doing at step t
- Agent wants to maximise cumulative reward

## RL Sequential decision making
- Maximise total future reward
- Long term consequences to actions
- Reward may be delayed
- Sacrifice immediate reward for long-term reward

## RL History
Sequence of observations, actions and rewards

## RL environment state vs agent state vs Markov state
- Environment private representation
  + What the env uses to pick next reward
  + Usually not visible to agent
- Agent internal representation
  + Info the agent uses for next action
  + Can be any function of history
- Markov state (Information state)
  - All useful info from history
  + Markov when Future is independant of the past given the present

## MDP vs POPMDP
- Fully observable env vs partially observable
- Agent state = env state = info state vs. agent state not env state

## Major RL agent components
Explain using maze
- Policy: behavior function
- Value function: How good each state is
- Model: Agents representation of env

## Modeling, inference and learning paradigm
- Modeling: Taking the world and building a simplified model
- Inference: Operate on model, ask questions
- Learning: Start without params and apply learning alg to fill in params

## Intelligence of models
- Reflex (Fixed set of computations, Deep NN)
- States (Plan, think ahead)
  + Search problem (you control everything)
  + Markov decision processes (Against nature)
  + Adversarial games (Against opponent)
- Variables (Sudoku, scheduling)
- Logic

## Categorizing RL agents
- Value based
- Policy based
- Actor critic (Value and policy)
- Model free
- Model based

## Q-Learning
For a finite MDP, find optamal policy for every state 

## RL Learning vs planning
- Rules are unknown vs known
- Pick actions and see result vs perfect model in brain

## RL: Exploration vs exploitation
Find more info about env vs. exploit known information

## RL: Prediction vs control
Evaluate vs optimise the future

## RL Problems
- Credit assignment problem: problem of detmining the actions that lead to a certain outcome
- Sparse reward problem: Flip pancake, long before getting reward (You only learn when rewarded)
- Reward shaping: Adapt reward function to guide agent towards task
- Agent alignment problem: Agent exploits reward system in unwanted way
- Unintended behavior: Walking without touching legs: flip over
