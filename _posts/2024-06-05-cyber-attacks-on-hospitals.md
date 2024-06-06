---
layout: post
title: Why do Hackers Target Hospitals?
subtitle: A brief anaylsis, inspired by the recent London cyber attack
tags: Healthcare Hackings
---
> *"This is a harsh reminder that this sort of attack can happen to anyone at any time and that, dispiritingly, the individuals behind it have no scruples about who their actions might affect."*

## The Context
Earlier today, BBC News reported that various London hospitals had been hit with a cyber attack. So, I'm going to take a brief look into the attack to find out what happened, and try and find out more about why someone would attack a hospital.

## What Happened
To no suprise, this appears to be a ransomware attack. The main source of information appears to be [a statement from the NHS](https://www.england.nhs.uk/london/2024/06/04/nhs-london-statement-on-synnovis-ransomware-cyber-attack/), stating that the ransomware attack began on Monday, and has been effecting non-emergency care for some patients attending hospitals in London. The ransomware has hit the IT systems of a company called Synnovis, who provide pathology lab services to the NHS in south east London. Interestingly they have also posted their [own statement](https://www.synnovis.co.uk/news-and-press/synnovis-cyberattack), which contains an interesting detail. This is very much a boilerplate cyber statement, apart from one quote towards the bottom:

> The incident is being reported to law enforcement and the Information Commissioner, and we are working with the National Cyber Security Centre and the Cyber Operations Team.

According to the [Information Commissioner's website](https://ico.org.uk/media/for-organisations/documents/2614816/responding-to-a-cybersecurity-incident.pdf), cyber attacks only have to be reported to them in the case of a data breach. While they may be taking precautions, it is possible that this ransomware attack has also gone hand in hand with a data breach, which would be particularly concerning for a company handling sensitive patient information. Aside from this, there is no other mention of a data incident, so this may not be the case.

## Why
As the name "**ransom**ware" would imply, it is almost certain that the motivation behind this attack is money. Often, ransomware is distributed without much regard, as if you send out 10 attacks you're more likely to get a payout if you attack just one.

Additionally, Ransomware as a Service (RaaS) is on the rise. Instead of needing technical expertise to put together a sophisticated ransomware attack, cyber criminals are renting or selling their software, allowing anyone to hold a business to ransom for the right price (often 15-20% of the revenue).
## Update - 06/06/2024
The attack has been claimed by Qilin, a Russian group of cyber criminals. The group has been operating since October 2022, and, offers a RaaS service as described above. They also seem to be more opportunistic than targeted, so the advice being given at the moment is to ensure that your systems are robust to ransomware attacks. This attack has interestingly come at a time when western countries have started giving Ukraine more freedom on how they are using their arms.

Interestingly, they also have a history of exfiltrating data alongside the ransomware. This is not always the case with ransomware, but allows the criminals to sell the data on the dark web if they don't receive payment for it, allowing a second source of income for the group. Whether this, if anything, will surface on the dark web is yet to be seen. A detailed dive into this group, which is definitely worth a read, can be found at [Group-IB's blog](https://group-ib.com/blog/qilin-ransomware), where they went as far as infiltrating the group itself. Some key points from their post:

![A graphic detailing information about the Qilin ransomware group](https://oliverb21.github.io/blog/img/posts/08_qilin_profile.png)

*Image source - Group-IB*

## Conclusion
Thanks for reading. If anything further information comes out, I'll make sure to update this post.

> *"Cyber-attacks can have significant and substantial cascading impacts as we are seeing in this unfolding situation where critical health services are being impacted."*