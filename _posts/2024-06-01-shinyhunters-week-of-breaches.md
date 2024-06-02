---
layout: post
title: ShinyHunters - A Week of Data Breaches
tags: APT Data ShinyHunters
---
> *“Until you have experienced something like this, you don't realise just what can happen, just how serious it can be.”*

## Newsworthy Breaches
Over the last few weeks, 2 major data breaches have hit the news, both [Santander](https://www.bbc.co.uk/news/articles/c6ppv06e3n8o) and [Ticketmaster](https://www.bbc.co.uk/news/articles/c899pz84d8zo). This is unusual, as these major breaches aren't common in the news. It's even more unusual that they have both been claimed by the same group of hackers. So let's dive into the details.

## Who
ShinyHunters, the group of hackers who are claiming responsibility for the attacks, got their name from a niche Pokémon community who search for unique, or shiny, Pokémon. Despite the somewhat innocent name, they have claimed many data breaches in the past, starting in 2020. These include:
- [AT&T](https://gizmodo.com/a-notorious-hacker-gang-claims-to-be-selling-data-on-70-1847527860), 70 million records taken from the American mobile carrier in 2021.
- [Tokopedia](https://www.wired.com/story/shinyhunters-hacking-group-data-breach-spree/), 91 million personal details breached from the Indonesian e-commerce company in 2020.
- [Microsoft](https://techgenix.com/microsofts-github-account-breached/), where the group claimed they had stolen 500GB of data from the tech giant's private GitHub repos in the same month as the Tokopedia breach.

As it goes with many of these groups, sometimes referred to as Advanced Persistent Threats (APTs), not much is known about who exactly they are or where they operate from. It's likely an international affair, although we do know [one French member pleaded guilty](https://cyberwarzone.com/shinyhunters-22-year-old-member-pleads-guilty-to-cyber-extortion-causing-6-million-in-damage/) in the US to $6m in damamges as a result of some of these attacks. While we don't know exactly who they are, we do know their motivation: money.

## Why
Groups that undertake large scale data breaches like these rarely have a motivation that isn't money. Cyber criminals that aim to disrupt for the sake of activism, revenge or pretty much any other motivation aside from nation state actors won't have the funding or skills to pull of attacks on this scale. So the why? Certainly money.

## What
So what exactly did they do this time? Over the last week, across the two attacks, they have exfiltrated over 800m staff and customer records from Ticketmaster and Santander. You'd think (and hope!) that your bank will have some of the best cyber security of any company that you interact with. Interestingly, it is being claimed by [Hudson Rock](https://www.hudsonrock.com/blog/snowflake-massive-breach-access-through-infostealer-infection), a security research company, that the breach is a result of a lapse of security in a cloud hosting service known as [Snowflake](https://www.snowflake.com/en/), which both of the affected companies use. In their exclusive interview with ShinyHunters, they claim that it is not just the two companies that they have breached, and that they have more than they are letting on. They suggested looking at [Snowflake's customer page](https://www.snowflake.com/en/customers/), which currently contains household names such as Mastercard, Disney and Pfizer. Unfortunately, there is no Internet Archive cache of this page to see whether Santander or Ticketmaster were on that list...

![A sceencapture from a Russian forum, listing the Santander details for sale](https://oliverb21.github.io/blog/img/posts/01_snowflake_breach_infostealer_1.png) 
*Image Source - Hudson Rock*

## How
This is where it gets interesting. Systems that hold significant amounts of data such as this are going to be effectively impenetrable, until you look to the weakest link in any computer system: **the human**. Remember the French citizen I mentioned was arrested earlier? Their specialism? Phishing and social engineering. According to the above linked report, the member, and likely the group as a whole, specialises in creating convicing replicas of login websites and emails, targeted to convince employees to inadvertently enter their login details. This is likely how the group managed to breach Snowflake, and from there gain access to their customer's systems.

Anyone can send a fake email, but they are often clumsy and easy to spot. It takes skill to set up cloned web servers and emails, to get as close to what the target will expect as possible. If the person notices something off, particularly in digital fields, they'll likely dismiss it at best and report it at worst. However, if the login page looks exactly the same as the one they have used every day for the last 2 years, it suddenly becomes very easy to hand over your details to a threat actor.

## So, what's next?
It's likely, over the next few weeks, more breaches that the group have performed will pop up, and investigations will begin into how such major breaches could have occurred. To keep yourself safe from breaches like this, make sure that your data is only being stored by companies that need it, and learn your rights around your data. Also, check out the [https://haveibeenpwned.com/](haveibeenpwned.com/) project, aiming to teach people about personal data, and find out if your email or password have appeared in any major breaches.

Thanks for reading
> *"i hacked p much [all of these](https://www.snowflake.com/en/customers/all-customers/) so you could just list more of them"*