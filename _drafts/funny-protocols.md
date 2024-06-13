---
layout: post
title: The Funny Side of Communcation Protocols
subtitle: We've all heard of IP or HTTPS, but what about IPoAC, or IMPS?
tags: Funny Protocols OSI
published: False
---
>*"This memo describes an experimental method for the encapsulation of IP datagrams in avian carriers.  This specification is primarily useful in Metropolitan Area Networks."*

## Introduction
There are many protocols and standards that ensure that the systems we use and run every day can communicate and exchange data effectively. But not all of these communication protocols are created equally. Today I'm going to look at some of the funny, interesting and bizzare protocols that have been formally registered over the years. I've also noted the Request For Comment (RFC) number, for easy reference

## IPoAC - IP on Avian Carrier ([RFC 1149](https://www.rfc-editor.org/rfc/rfc1149))
IPoAC, also known as Internet Protocol on Avian Carrier discusses how an IP datagram could be transported via a bird. Hexadecimal is used to encode the data, and it is secured to the bird in the form of a small scroll. The bird would find it's way to the recipient, and deliver the data to be decoded and displayed as a normal TCP/IP packet would. It is also noted in the RFC that "storms can cause data loss". Updates have been provided, including a [Quality of Service update](https://www.rfc-editor.org/rfc/rfc2549) detailing improvements to the operation and performance, and an [update to the IPv6 specification](https://www.rfc-editor.org/rfc/rfc6214)

## HTCPCP - HyperText Coffee Pot Control Protocol ([RFC 2324](https://www.rfc-editor.org/rfc/rfc2324))
A modifcation of HTTP, this protocol is designed for use with coffee pots. Instead of using a POST request to cause an action, the BREW request will cause the coffee pot to fire up. Started pouring milk and want to indicate you've got enough? The WHEN request has you covered. However, try and brew coffee using a teapot with this method and get a 418 "I'm a teapot response! The original RFC has been update to include teapots, that can be found at [HTCPCP-TEA](https://www.rfc-editor.org/rfc/rfc7168)

## IMPS - Infinite Monkey Protocol Suite ([RFC 2795](https://www.rfc-editor.org/rfc/rfc2795))
This set of protocols is designed to look after and monitor the monkeys from the infinite monkey theorem. The RFC talks about various aspects including communication with the monkeys, and ensuring their welfare with food and sleep. This was released on April Fool's day in 2000.

## IPv4 Security Flag ([RFC 3514](https://www.rfc-editor.org/rfc/rfc3514))
This memo from April 1st 2003 aims to improve and streamline security in IPv4 messgaes. It details a flag that can be set in the header known as the "evil bit". If the bit is set to 0, the packet is not malicious and can be passed through the network. If the bit is set to one, it can be assumed that the packet is malicious and should be blocked by a firewall. This allows simple and streamlined security for businesses and organisations, although unforntunatley would also involve trusting every single person connected to the internet...

## TELNET Randomly-Lossy Transmission Mode ([RFC 748](https://www.rfc-editor.org/rfc/rfc748))
Release in 1978, this memo describes a new configuration for Telnet. It allows the user to simulate poor network conditions, by randomly dropping packets as they are transmitted. In theory, this would allow the user to test their applications and connections in the poor conditions while maintaining a full internet connection.

## Conclusion
THanks for reading. If there are any other funny protocols or systems that you've found, head over to the contact page to let me know!

>*"This memo describes a protocol suite which supports an infinite number of monkeys that sit at an infinite number of typewriters in order to determine when they have either produced the entire works of William Shakespeare or a good television show."*