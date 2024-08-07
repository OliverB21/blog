---
layout: post
title: How the FBI Hacked Thomas Crooks' Phone
subtitle: The ethics and methods behind breaking into personal devices
tags: hacking encryption
---

> *"It's possible to guess the identity behind an ad ID with a frightening level of accuracy"*

---
## The Context
As I am sure I don't need to reiterate, a 20 year old Thomas Crooks attempted to take the life of former US president Donald Trump. However, in a world where "military grade encryption" is becoming the norm, are there any military grade tools that can break it? Let's find out how the FBI were able to access the shooter's mobile phone. This article is inspired by Seytonic's video, that you can check out [here](https://www.youtube.com/watch?v=I6mlaPLPcXU).

## Cellebrite and the phone's journey
After they secured the phone, FBI agents in Pennsylvania failed to break into the phone. This is likely due to having minimal tools and expertise in the locality. These tools may include basic encryptions crackers and resources that require minimal knowledge. Having no success, the phone made it's way from Pennsylvania to Virginia, where specialised staff were able to crack the phone in a mere 40 minutes! But how exactly did they do this?

Cellebrite is a digital forensics company based in Israel. Their product, Cellebrite InsEYEts claims that it is able to access 5x more devices, 60% more information and do all of that twice as fast. What they are comparing this to is unclear, but what is clear is that they are an industry standard for cracking and accessing mobile phones. This explains why they were able to access the shooter's phone so quickly.

## How do tools like this work?
In a word, it's unclear. This company wouldn't have a product without the ability to break these devices open, so the chances of them revealing this IP is 0. The chances are, they have a team of ethical hackers who work on finding zero day exploits in the devices and operating systems provided, in order to add the capabilities to their product. A graph did leak, however, of the devices that they support, and there is an interesting range. There doesn't necessarily seem to be a correlation between particular brands and OSes, i'd reccommend checking out the video linked above for more detail.

## Tracking the phone before the event
There is some controversy however, around the method the FBI have used to track his location. Apps that track your location are able to sell this data to data brokers, who are then able to do just about whatever they want with it, including selling it on to advertising agencies to serve ads based on where you go. This data is theoretically anonymous, being linked only to you "ad-id" that is assigned to you, but this is very easily unscrambled. The example that Seytonic gives in [this video](https://www.youtube.com/watch?v=qySOODYdboI) is that there isn't going to be many people that go from your place of work to your home as often as you do!

You may have these apps on the very same device you are reading this article on! The best way to prevent this from happening is **regularly review permissions** on your phone to make sure services don't have access to more information that they need, and consider setting up a **DNS sinkhole**, to prevent tracking URLs being accessed by your device.

## Conclusion
Overall, I don't think this process puts any pressure on data privacy laws, nor has it revealed any new information in the world of cyber security. Forensic devices are regulated by laws and can't be used willy-nilly by law enforcement. However, this event may raise some eyebrows in the information security world, we will have to wait and see. Thank you for reading.

> *"The aim of marketing is to know and understand the customer so well the product or service fits him and sells itself."*