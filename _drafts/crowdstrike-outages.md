---
layout: post
title: The CrowdStrike Outages
subtitle: How did one update cause so much damage?
tags: Crowdstrike BSOD Outage
published: False
---

> *"CrowdStrike is actively assisting customers affected by a defect in a recent content update for Windows hosts."*

---
## What is CrowdStrike?
Many people may not have heard of this company before now, but you've definitley interacted with a system that uses one of their products. CrowdStrike is a Cybersecurity company that provide various services such as endpoint security (antivirus), threat intelligence and post-attack response. With a market cap of around $74bn, this is a well known and trusted company. Notable customers include the Mercedes AMG Formula 1 team, many major banks including Chase Bank and Bank of America, and various worldwide airlines. Let's take a look at what has happened to bring all of these businesses to their knees.

## A Timeline
In the early hours of Friday morning, various emergency call centres and hospitals began to experience outages. As the morning went on, flights were grounded and public transport began cancelling routes. Around the same time, CrowdStrike released a statement to say they were "aware" of the outages.

As the day goes on, mnay businesses and organisations around the world begin experiencing outages that all link back to one piece of software: CrowdStrike Falcon. This is one of the enterprise antivirus software products that they offer, and is used by many companies across the world. But what exactly caused all of these outages?

## The Technical Stuff
The issue stems from one of the sensors that is attached to the software. The configuration was changed as part of an update and pushed out into production. This configuration caused an error within Windows, that caused a Blue Screen Of Death (BSOD) loop, where the computer would boot, crash and restart over and over. The issue with a problem like this is that it can't be fixed by issuing a quick patch over a software distribtion system, as the computer would have to boot properly in order to use them. Therefore, the current fix only works by manually perfoming an update. This is not practical for a whole host of reasons!

## What happens next?
Once the dust has settled and the majority of computers have returned to normal, it is unlikely much will happen externally to CrowdStrike. There is likely to be some interal reviews at CrowdStrike and some policy changes (as well as a loss in business!), but I doubt the company would be found liable for any damages, but that is yet to be seen.

Thanks for reading. Any comments feel free to let me know.

<img src="https://oliverb21.github.io/blog/img/posts/17_crowdstrike.png" alt="An XKCD comic about the CrowdStrike outages" text-align="centre" width="750"/>

*Image Source - XKCD*
