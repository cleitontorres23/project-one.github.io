---
title: "Load Balancer"
date: 2020-11-07T10:57:09-03:00
draft: false
---

Load balancer in Layer 4 and Layer 7

This is the first of series of knowledge sequences about technologies and stuffs. I hope you enjoy the journey.

WHAT IS LOAD BALANCER?

In technology, a load balancer distributes connections from clients between a set of servers to provide the best possible application performance. A server load balancing (SLB)is designed for pools of application servers within a single site or local area network (LAN)

one of the most important difference between Network Load Balancer - L4 and Application Load Balancer - L7 is the number of layers who each one can reach.

These differences is based on the various layers in the Open Systems Interconnection (OSI) Reference Model. An L4 load balancer works at the transport layer, using the TCP and UDP protocols to manage transaction traffic. An L7 load balancer works at the application layer (the highest layer in the OSI model, and makes its routing decisions based on more detailed information such as the characteristics of the HTTP/HTTPS header.

![osi.jpg](/project-one.github.io/osi.jpg)

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

![loadbalancer.png](/project-one.github.io/loadbalancer.png)
