---
layout: post
title: ShinyHunters - A Week of Data Breaches
subtitle: Learn more about the recent spate of data breaches
tags: APT Data ShinyHunters
---
> *“Until you have experienced something like this, you don't realise just what can happen, just how serious it can be.”*

---
## Newsworthy Breaches
Over the last few weeks, 2 major data breaches have hit the news, both [Santander](https://www.bbc.co.uk/news/articles/c6ppv06e3n8o) and [Ticketmaster](https://www.bbc.co.uk/news/articles/c899pz84d8zo). This is unusual, as these major breaches aren't common in the news. It's even more unusual that they have both been claimed by the same group of hackers. So let's dive into the details.

## Who
ShinyHunters, the group of hackers who are claiming responsibility for the attacks, got their name from a niche Pokémon community who search for unique, or shiny, Pokémon. Despite the somewhat innocent name, they have claimed many data breaches in the past, starting in 2020. These include:
- AT&T, 70 million records taken from the American mobile carrier in 2021. ([<ins>see here</ins>](https://gizmodo.com/a-notorious-hacker-gang-claims-to-be-selling-data-on-70-1847527860))
- Tokopedia, 91 million personal details breached from the Indonesian e-commerce company in 2020. ([<ins>see here</ins>](https://gizmodo.com/a-notorious-hacker-gang-claims-to-be-selling-data-on-70-1847527860))
- Microsoft, where the group claimed they had stolen 500GB of data from the tech giant's private GitHub repos in the same month as the Tokopedia breach. ([<ins>see here</ins>](https://techgenix.com/microsofts-github-account-breached/))

As it goes with many of these groups, sometimes referred to as APTs (Advanced Persistent Threats), not much is known about who exactly they are or where they operate from. It's likely an international affair, although we do know [one French member pleaded guilty](https://cyberwarzone.com/shinyhunters-22-year-old-member-pleads-guilty-to-cyber-extortion-causing-6-million-in-damage/) in the US to $6m in damamges as a result of some of these attacks. While we don't know exactly who they are, we do know their motivation: money.

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

## *Update - 03/06/2024*
Snowflake have created a [blog post](https://community.snowflake.com/s/question/0D5VI00000Emyl00AB/detecting-and-preventing-unauthorized-user-access) effectively denying responsibility for the attack. In short, they are suggesting that they haven't been directly attacked, and that the breaches were caused by customers not having Multi Factor Authentication (MFA) enabled. This has lead to unauthorised access to their accounts with the help of credentials that have been stolen in previous, unrelated breaches. 

It's still unclear what we are looking, but there are a few possibilities of what has happened:

1. **Snowflake has been breached** and they are yet to publicise this while they perform their investigations, potentially trying to reduce the reputational impact on the company

2. **Snowflake hasn't been breached** and each customer account takeover was independent and took advantage of failings on the customer's side (not enabling MFA)

3. **Snowflake's security policies are weak**, meaning that customers followed advice given and this lead to their accounts being breached. In this case, the liability wouldn't be as clear as the first two

Any of these are possible, but it is still bugging me *why Snowflake*? If the customer's details were already stolen, ShinyHunters could easily access so much more than just what is stored on Snowflake's servers, so why have they exclusively targeted this platform? I think there will be more details and questions answered as time goes on, but this process will likely be a long one. I'll try and keep this post updated.

## *Update - 10/06/2024*
I have always wondered how breaches like this are detected, especially in the case of breaches that aren't uncovered for some time. In one case, when Ticketmaster was breached in 2018, it was [Monzo](https://monzo.com/blog/2018/06/28/ticketmaster-breach/) seemed to spot it first. After various fraudulent transactions were reported to them in a small time frame, they investigated and found that all of those customers had used their cards on Ticketmaster at some point or another. They even found that someone had incorrectly input their details on Ticketmaster (incorrect expiry date), and a malicious actor had tried to use the incorrect details to make a transaction, further proving that Ticketmaster was the source of the breach.

Initially, Ticketmaster denied being breached and claimed to Monzo that they had found "no evidence of a breach and that no other banks were reporting similar patterns". Just over a week later, Ticketmaster publically announced they had been breached due to malware distrbuted to their internal networks via their customer support product.

Most breaches are detected after the threat actor makes a mistake, but what confirmed it here was not a mistake that was made not by the hacker, but by one of the victims. How ironic.

Thanks for reading. Any comments or questions? Head over to the contact page and send me a message.

> *"i hacked p much [all of these](https://www.snowflake.com/en/customers/all-customers/) so you could just list more of them"*