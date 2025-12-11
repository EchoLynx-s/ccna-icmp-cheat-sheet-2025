# CCNA – ICMP (Module 13)

Quick-reference notes for NetAcad CCNA – **Module 13: ICMP**.  
Focus is on how ICMPv4 and ICMPv6 support reachability tests and error
reporting, and how to use **ping** and **traceroute** to troubleshoot networks.

I use this repo to revise:

- The role of **ICMP** in IP networks (not a transport protocol, but a control protocol).
- Common **ICMPv4 / ICMPv6 message types**: echo, destination unreachable, time exceeded.
- How to interpret ping results (success, timeouts, unreachable messages).
- How to run **systematic ping tests** (loopback → gateway → remote host).
- How **traceroute** works and what each hop/time-out means.
- Typical **connectivity troubleshooting workflows** using ICMP.

  
---

## Table of Contents

- [Module 13 Overview](#module-13-overview)  
- [Module Map](#module-map)  

- [13.0 Introduction](#130-introduction)  
  - [13.0.1 Why should I take this module?](#1301-why-should-i-take-this-module)  
  - [13.0.2 What will I learn in this module?](#1302-what-will-i-learn-in-this-module)  

- [13.1 ICMP Messages](#131-icmp-messages)  
  - [13.1.1 ICMPv4 and ICMPv6 Messages](#1311-icmpv4-and-icmpv6-messages)  
  - [13.1.2 Host Reachability](#1312-host-reachability)  
  - [13.1.3 Destination or Service Unreachable](#1313-destination-or-service-unreachable)  
  - [13.1.4 Time Exceeded](#1314-time-exceeded)  
  - [13.1.5 ICMPv6 Messages](#1315-icmpv6-messages)  
  - [13.1.6 Check Your Understanding – ICMP Messages](#1316-check-your-understanding--icmp-messages)  

- [13.2 Ping and Traceroute Tests](#132-ping-and-traceroute-tests)  
  - [13.2.1 Ping – Test Connectivity](#1321-ping--test-connectivity)  
  - [13.2.2 Ping the Loopback](#1322-ping-the-loopback)  
  - [13.2.3 Ping the Default Gateway](#1323-ping-the-default-gateway)  
  - [13.2.4 Ping a Remote Host](#1324-ping-a-remote-host)  
  - [13.2.5 Traceroute – Test the Path](#1325-traceroute--test-the-path)  
  - [13.2.6 Packet Tracer – Verify IPv4 and IPv6 Addressing](#1326-packet-tracer--verify-ipv4-and-ipv6-addressing)  
  - [13.2.7 Packet Tracer – Use Ping and Traceroute to Test Network Connectivity](#1327-packet-tracer--use-ping-and-traceroute-to-test-network-connectivity)  

- [13.3 Module Practice and Quiz](#133-module-practice-and-quiz)  
  - [13.3.1 Packet Tracer – Use ICMP to Test and Correct Network Connectivity](#1331-packet-tracer--use-icmp-to-test-and-correct-network-connectivity)  
  - [13.3.2 Lab – Use Ping and Traceroute to Test Network Connectivity](#1332-lab--use-ping-and-traceroute-to-test-network-connectivity)  
  - [13.3.3 What did I learn in this module?](#1333-what-did-i-learn-in-this-module)  
  - [13.3.4 Module Quiz – ICMP](#1334-module-quiz--icmp)  

---

## Module 13 Overview

> **Goal:** Understand how ICMP supports IP by providing **error reporting** and
> **reachability testing**, and be able to use `ping` and `traceroute` to
> systematically test and troubleshoot network connectivity.

---

## Module Map

| Topic                         | Focus                                                        |
|-------------------------------|--------------------------------------------------------------|
| 13.1 ICMP Messages            | ICMPv4/v6 message types, echo, unreachable, time exceeded   |
| 13.2 Ping and Traceroute      | Using ICMP-based tools to test reachability and paths       |
| 13.3 Practice and Quiz        | Hands-on labs + final ICMP review                           |

---
