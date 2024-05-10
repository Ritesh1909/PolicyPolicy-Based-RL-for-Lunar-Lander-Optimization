# Policy-based Reinforcement Learning on LunarLander-v2

This repository contains the implementation and analysis of Policy-based Reinforcement Learning algorithms applied to the OpenAI Gym's LunarLander-v2 environment. The project focuses on the REINFORCE algorithm and various actor-critic methods, exploring their effectiveness in solving complex control tasks with high-dimensional state spaces.

## Abstract

We implement and analyze Policy-based algorithms on OpenAI Gym’s LunarLander-v2 environment, including the REINFORCE algorithm and variants of the actor-critic algorithm. The study involves experimenting with different values for multiple parameters to compare how these algorithms perform under varied settings.

## Introduction

The Lunar Lander environment presents a physics-based simulation aimed at optimizing rocket landings using principles derived from Pontryagin’s maximum principle. This project provides an in-depth analysis of the simulation’s action and observation spaces, along with the reward mechanisms that guide the learning algorithms.

## Environment Setup

The environment uses PyGame for rendering, providing a visual representation of the simulation where different landing scenarios can be tested and analyzed.

### Action Space

The action space consists of four discrete actions:
- Do nothing
- Fire the left orientation engine
- Fire the main engine
- Fire the right orientation engine

### Observation Space

The observation space is an 8-dimensional vector including the lander's x and y coordinates, velocities, angle, angular velocity, and boolean indicators for leg contact.

### Rewards

Rewards are structured to promote precise navigation and safe landing, with penalties for using too much fuel and rewards for maintaining stability and making safe landings.

## Algorithms Implemented

### REINFORCE

A Monte Carlo variant of policy gradient methods focusing directly on optimizing the policy used by the agent.

### Actor-Critic Methods

These methods combine elements of policy-based and value-based approaches to improve learning efficiency and stability, involving:
- Standard Actor-Critic
- Actor-Critic with Bootstrapping
- Actor-Critic with Baseline Subtraction

