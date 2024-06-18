---
layout: post
title: Aircraft Communication Security
subtitle: Is ADS-B suitable in the modern world?
tags: ADS-B Aerospace
---

>*" What about danger, one may enquire? Danger is one of the attractions in flying"*

---
## Introduction
In today's world, airports and aircraft are one of the most secure places you can be. With the amount of checks and detectors someone must go through before getting in the plane, you'd struggle to get 101ml of liquid onto your flight. But, do these security policies apply to the digital communications in aerospace as well? Let's explore ADS-B.

## What is ADS-B?
Automatic Dependant Surveillance-Broadcast, more commonly known as ADS-B, is one of the systems that aircraft use to broadcast information to the ground,for systems such as Air Traffic Control (ATC). This broadcast includes key pieces of information, such as location, direction, speed and height, and other information about the flight including it's source, destination and flight number. ATC can use this information to see where planes are in the sky and plan their arrivals into the airport. There are also various websites that allow enthusiasts to view this information on a map, such as [FlightRadar](https://www.flightradar24.com/) and [ADS-B Exchange](https://globe.adsbexchange.com/). However, this technology has one key flaw: it's completely open. No encryption, no authentication, no certification. Let's see why that is important.

## Shopping List
- HackRF One  or Similar - £263
- Simple Antenna - £11
- Various FOSS Tools - Free
- Guide on the internet - Free (No, I'm not linking it here but a quick Google will show you what you're looking for)

For less than £300 (prices correct as of 10/06/2024), anyone could buy, build and deploy an ADS-B spoofing station. They would be able to broadcast fake information about a plane in the sky and falsify all of the information I listed above. While this wouldn't have much impact at low power in a small village far away from anything, imagine the damage that could be caused by someone with a laptop sat outside Heathrow Airport at peak times, adding planes to the queue of those waiting to land. While ATC does have systems to fall back on in the case of disruption like this, the initial chaos caused would be enough to cause significant financial and physical disruption.

## How to mitigate this problem
At the moment, ADS-B is the standard. However, there is a potential solution that could reduce or prevent the likelihood of packets being spoofed.
This would be to provide certification to the communication. Much like the web has Certificate Authorities (CAs), aircraft authorities such as IATA or the CAA could issue certificates to airlines/aircraft companies, who could then issue certificates to their planes. This would allow each ADS-B communcation to be signed with this certificate, so receiving stations on the ground (ATC, enthusiasts) would be able to verify that authenticity of the broadcasts being recieved.

## Conclusion
It's likely we will see this system (or something similar) come into effect in the next few years. However, this is yet to be seen. If you have any ideas of how the system could be improved, drop me an email. Thanks for reading!

> *“The sky is not the limit, it's just the beginning.”*