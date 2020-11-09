---
title: "Load Balancer"
date: 2020-11-07T10:57:09-03:00
draft: false
---

Load balancer in Layer 4 and Layer 7

This is the first of series of knowledge sequences about technologies and stuffs. I hope you enjoy the journey.


WHAT IS LOAD BALANCER?

Before starting talking about what Load Balancer is, let's talk about layers. 

Layer is the OSI Model method to destribute and organize the application path to come up into your website.

This picture below shows you how is that works properly.


![osi.jpg](/project-one.github.io/osi.jpg)


Now you understand how the drill is, let's talk about Load Balancer. Load balancer as its name suggests it distributes (balance) all the connections (loads) from clients to the servers improving the application performance. A server load balancing (SLB) is designed for pools of application servers. One of the differences between Network Load Balancer(layer 4) and Application Load Balancer(layer 7) is the number of layers who each one can reach.

A load balancer layer 4 works at the transport layer and only until there, using the TCP and UDP protocols to manage transaction traffic and the load balancer layer 7 works at until the top of application layer, it means that it can offer more funcionalities than layer 4.


Some examples of network layer algorithms include: Round robin, Weighted round robin , Least connections, Weighted least connections , source IP hash (we can talk about it later)

Long story short about layer 4 and 7..

SLB layer 4 is based on traffic routing, such as IP address and destination ports . Considering layer 4 (TCP) and below. 
Caring only about the network-layer information in his package without check the inside content.


SLB layer 7 is Based on network traffic and HTTP protocol , from the network layer to the application layer.

One of the capacity of the Application Delivery Controller is provides the ability to route HTTP and HTTPS traffic based upon rules, checking inside the inside content of all packages, making this SLB more intelligent than others. 


Is different, period.

SLB Layer 7 provide you the possibility to make redirect base on URLs and headers, peculiar treatment for frequent
clients and occasional visitors, Intelligent load balancing between application servers, firewalls

![loadbalancer.png](/project-one.github.io/loadbalancer.png)
