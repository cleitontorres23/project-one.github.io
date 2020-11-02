---
title: "Load Balancer"
date: 2020-09-24T20:49:00-03:00
draft: true
author: "Cleiton S. Torres"
---

Load balancer in Layer 4 and Layer 7

This is the first of series of knowledge tops about technologies and stuffs. I hope you enjoy the journey.

In technology, a load balancer distributes connections from clients between a set of servers . A server load balancing (SLB)is designed for pools of application servers within a single site or local area network (LAN)

one of the most important difference between Network layer and application layer is the algorithms in how they’re able to analyze incoming traffic.

Examples of network layer algorithms include: Round robin, Weighted round robin , Least connections, Weighted least connections , Source IP hash (we can talk about it later)

What is LAYER 4
Based on traffic routing, such as IP address and destination ports . Considering layer 4 (TCP) and below. 
Caring only about the network-layer information  contained within the packets it is directing this way and that

What is LAYER 7
Based on network traffic and HTTP protocol , from the network layer to the application layer.
Provides the ability to route HTTP and HTTPS traffic based upon rules.

Long story short..
Application Load Balancer works at the Application Layer (Layer 7 of the OSI model) and the network load balancer works at layers 3 & 4 (network and transport layers).

Is different, period.


Another difference between the two is important because network load balancing cannot assure availability of the application, in other words, it can just correctly complete the three-way TCP handshake and an application load balancer goes much deeper, is capable of determining availability based on successful HTTP GET of a particular page.


![loadbalancer](loadbalancer.png) 


