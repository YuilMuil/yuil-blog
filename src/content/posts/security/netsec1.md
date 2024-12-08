---
title: An overview of Networks and Network Security - Part 1
published: 2024-12-08
description: [SECURIOUS 블로그 첼린지] A basic overview of Network Fundamentals and a incomplete introduction to basic Network Security concepts and terminology.
tags: [English, 네트워크 보안, 개념, 날피]
category: Security
draft: false
---

# What this post is about
This post will cover the basics of Network Fundamentals and basic Network Security concepts and terminology.

# Table of Contents
- Network Fundamentals
- Network Security Systems

# Network Fundamentals
## Packet Switching
Packet Switching is the concept in which the data you send are split into smaller blocks of data called 'Packets' and each packet has it's own metadata(Destination IP, Sender IP, Packet/Sequence Number etc) along with it's own write. After the split data are received at the destination, it is then reconstructed into the original data before it was split, by combining each packet in order using the metadata as a reference.

## Shared Media Ethernet
A method of sharing a single bandwidth with all users in a end-point, akin to a high-way for cars. The problem with this method is that bandwidth for every client added is split and reduced, and for each client that is added, the risk of Collision occuring is increased.

## Segments & Bridges
A bridge splits the LAN into a smaller shared segment, where each segment is like a mini shared media ethernet. This method can reduce the risk of Collision and prevents the bandwidth from being spread out between clients.

## Transmission Methods
- Unicast(Point to Point)
This method sends the same packet from server to client N times, with each request being sent to each unique client.

- Broadcast(Point to Multipoint)
It sends the same packet to every client connected at once.

- Multicast(Point to Multipoint)
It sends the same packet to every client within a certain group at once.

## Types of networks

- WAN(Wide Area Network)
The biggest network unit used. Size of network ranges from 100km to 1000km and usually denotes a country or continent. (Fun fact: The Internet is the world's largest WAN)

- MAN(Metropolitan Area Network)
The second biggest network unit used. Size ranges from 10km to 100km and usually denotes a city.

- LAN(Local Area Network)
The msot often used network unit. Size ranges from 10m~1km and usually denotes Room, Building, Campus.

## OSI 7 Layer
Also known as the Open Systems Interconnection Reference Model, it is the Layered standard model for telecommunications developed by the International Organization for Standardization (ISO).

### Pros
- There are 7 layers which allows interoperability of different vendors by creating standards which are agreed upon for all vendors for each layer.
- If management is divided into each level via Encapsulation, it is easier to resolve problems by splitting them from one big problem into 7 smaller problems.

### Layers
The layers consists of Application, Presentation, Session, Transport, Network, Data Link, Physical. For each layer, there is a header added which is completed at Data Link layer, then the data is sent via the Physical Link layer, which then the receiver reads each layer which is then ultimately sent to the client.

## Telecommunications equipment for each layer
- L2 Switch: Only reads until the Data Link layer to check the MAC Address for which it sends the packet to the client connected to the switch with that MAC address saved within it's MAC Address Table.

- L3 Switch: Same as L2 Switch, but it reads until the Network Layer to check where the destination IP is, in which it redirects to that host.

- L4 equipment: Checks the Transport layer, which it can check the port information.

- L7 equipment: Checks up until the Application layer, in which it can see the data being sent in it's intended form.

- Hub(L1 equipment): Connects network devices at the physical layer. It gets all signals and sends to every network devices in every port(Repeater) and shares the entire bandwidth. Because it is a 'dumb machine' in the context that it simply gets a signal and shares it with every device, it doesn't require any smart features or settings unlike routers.

- Switch(L2 equipment): As an L2 equipment, it reads the packet 'Frame' and reads the destination MAC Address to filter and send via broadcasting to the intended client. Switches is mostly based on bridge technology and uses address tables which is much faster than bridge's method of software frame reading methods. Switches support more ports than bridges and allow equal bandwidth for all connected devices.

- Router(L3 equipment): As a L3 equipment, each router port has it's own segment. It reads the packets destination IP address and makes use of broadcasting to the corresponding port segment, preventing traffic from leaking out to other unintended clients. It also make use of routing tables which keep track of each network address and port segments.

## Addresses
- IP Address: IPv4(32 bits), IPv6(128bits). Each segment has it's own unique address in a router.
- MAC Address: 48 bits. The address used when network equipments communicate with each other.

# Network Security Systems

## Basic Terminology
- Spoofing: Using the weakness of TCP/IP packet structure, modify the values within the packet to falsify information to gain unauthorized system permissions which can then be leveraged to steal information.
- Sniffing: Take a look at other network node traffic.
- Snooping: Taking look at important information within a network in a way that was not intended.

## Threat Concepts
- Interception(Sniffing)
- Modification(Spoofing)
- Interruption(DDoS)
- Fabrication(Authentication Falsification)

## Basic Concepts
- Backbone Network: In a large area, connect and group multiple networks to allow them to communicate with each other. A good example of this is KREONET(Korea Research Environment Open NETwork).

- Client/Server Network