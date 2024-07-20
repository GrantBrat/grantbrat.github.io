---
layout: post
title: Current Home Network Setup
tags: 
- IT
- Home
- Project
- Sec
math: true
toc: true
date: 2024-04-04 15:32 +0800
---
Current setup for the time being is this simple home network.


## Current Home Setup


The main router serves as the firewall, wireless modem and router to the rest of the network. It then assigned IP addresses to all the wireless devices connected via the 2.3GHz or 5GHz bands. These are assigned Dynamically via DHCP. I think I may need to fix something with this soon as at times, a new device being added to the bands are getting an incorrect IP altogether. They can talk with the router fine, but cannot receive any internet without manually assigning a static IP. May be vendor issue with that brand of Router.

![Image](/assets/home_net.png)

Two cameras are connected to a main hub device that is then connected to the router. These cameras can be accessed outside of network via vendor app. Very handy, may find a way to later save the videos onto file server at some point. Can only save data to local storage on camera.

The ghetto switch is just an old router that I have plugged in Ethernet from the main router to make some more ports open for the Static IPs of the Server and W10 Workstation. Turns out, If you just connect incoming Ethernet to  the router on one of the open ports and NOT in the "Internet" port, then it will just feed a connection without having to configure any forwarding from the second router to the first! Makes my life easier as I don't have any other configurations to make to the other devices downstream from this point. 
## Future Plans

- Add a firewall or Pi hole to filter internet traffic through and manage.

- Get proper switch with more then 1GB networking 

- Get a server rack that can hold proper networking devices/ look cool