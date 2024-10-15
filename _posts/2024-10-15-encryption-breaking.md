---
layout: post
title: Did someone just break encryption?
subtitle: Chinese researchers use quantum technology to break RSA
tags: Encryption Data Quantum
---

> *"Quantum Annealling Public Key Cryptographic Attack Algorithm Based on D-Wave Advantage"*

---
## What's Encryption
As the internet has developed and grown, the need has arisen more and more for the ability to send messages and information without others being able to see it. This is where encryption came into play, allowing people to exchange information over digital systems that would otherwise be able to be intercepted by a malicious party.

But you may be thinking, surely a system like this has existed since before computers were a thing? And yes! You're right! The earliest example we know of encyption being used is Ancient Egypt, where symbols were replaced so only those with the key were able to understand the heiorglyphs that had been written. Other examples of encryption in history are the Caeser Cipher (which he actually used!) and Enigma, used by the germans in WW2. These ciphers range in complexity from being simple enough for small children to understand (sprl aopz!), to needing large teams of mathematicians years to solve the puzzle (ammk ubcr!)

## Modern Encryption
Most modern systems use assymetric encryption, allowing the user to both securely send information and verify the author. The gold stanard of this at the moment is RSA-4096, which has been securely used since 1977. This is manifested in most people's lives as a token that they use to authenticate themselves before logging into a system. Another common encryption method is AES, which is often used to protect data at rest.

RSA uses the idea that you can multiply 2 very large numbers together easily to achieve a result, but it is very difficult to find the two numbers that were initially multiplied from that result. This will become important shortly

## So, what's happened?
A team of researchers in China have claimed that they have been able to break simple RSA. There are many rewards and bounties on the solution to breaking this encryption, posted by hackers and companies alike, which they may well have been working towards. This process has been completed using quantum computing. Quantum computers in short, are much more powerful than whatever you are reading this on, and can be used to solve difficult mathematical equations very efficiently. In the case of RSA, this means being able to find the 2 numbers that were multiplied much easier than with traditional computers.

However, there is a catch. The version of RSA that they used to complete this research was much simpler than the one that is normally used (22 bit compared to much longer ones normally used). While this is a start, it will likely provide an excellent jumping point for people looking to research into this field in the future. We can only wait and see how this develops.

Thanks for reading!

> *"Quantum computing presents an exciting yet formidable challenge to cryptographic security"*