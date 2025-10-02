# Week 4

# Task 1: Side-channels
Excluding speculative CPU attacks such as Meltdown or Spectre, choose an example of a side-channel attack and explain the following information about it:

- Brief explanation of what side-channel the attack uses and how

- What systems does it affect?

- What information is leaked via the side channel?

- Is there a documented case of it being used in a real life attack?

- Has it been fixed? If yes, how it was fixed?

You are not expected to produce an essay. Direct answers to questions above are sufficient. List sources and keep the answer concise at max 300 words not including sources.

# Electromagnetic attack
## Brief explanation of what side-channel the attack uses and how
Electromagnetic attack uses electromagnetic radiation or radio waves to measure victims devices and try to imitate devices internal signals. Commonly used to try obtain secret keys via cryptographic operations.
## What systems does it affect?
All electronic devices emit electromagnetic waves, which can potentially be exploited. These devices include devices such as: smart cards, computers and phones.
## What information is leaked via the side channel?
Cryptographic secrets, user inputs, timing data and other sensitive data which could be exploited to gain access to unauthorized information.
## Is there a documented case of it being used in a real life attack?
Well known case was when researcher Wilm van Weck demonstrated weakness in CRT displays using electromagnetic side-channel attack in 1985. This case was one of the first unclassified analysises of this kind of attack.
## Has it been fixed? If yes, how it was fixed?
There are many counter measures for electromagnetic attacks. One of the most important methods to battle these kinds of side-channel attacks is to make it more difficult to read electromagnetic signals. Protecting the chip and reducing signal strenght help reduce the range of the signals since most electromagnetic attacks require the attacker to be close proxmimity.

Sources:

[What is a side-channel attack? ](https://www.techtarget.com/searchsecurity/definition/side-channel-attack)  
[EM Side-Channel Attacks on Cryptography ](https://www.allaboutcircuits.com/technical-articles/em-side-channel-attacks-on-cryptography/)  
[Van Eck phreaking](https://en.wikipedia.org/wiki/Van_Eck_phreaking)  
[Electromagnetic attack](https://en.wikipedia.org/wiki/Electromagnetic_attack)  


# Task 2: Slow Loris
HOX! Consider Slow Loris as a type of attack rather than the 'slowloris' program itself

Seek information about the Slowloris Denial-of-Service attack and answer to the following questions:

- How does it work?

- Why is it unique while compared to the other high bandwith DDoS attacks?

- What are the effects of the attack?

- How can you mitigate/prevent the effects of the attack?

- Are there any notable instances of this style of attack being performed?

You are not expected to produce an essay. Direct answers to questions above are sufficient. List sources and keep the answer concise at max 300 words not including sources

#  Slowloris Denial-of-Service
## How does it work?
Slowloris is a DoS attack (denial-of-service). It's used to maliciously slow or shut down service or device. Usually it includes overwhelming service/device with large amount of requests which shouldn't be possible in normal traffic.
## Why is it unique while compared to the other high bandwith DDoS attacks?
Slowloris attack operates in application layer, it's aim it to make multiple HTTP request and keep them active as long as possible using partial request headers which will not complete and prenvent timeout. It uses low amount of bandwidth compared more traditional high bandwidth consuming DDoS attacks.
## What are the effects of the attack?
Eventually targeted server runs out of resources since it can't finish pending requests which causes denial-of-service.
## How can you mitigate/prevent the effects of the attack?
Having measures such as implementing IP adress limitations, having maximum connection time for clients and restricting slow transfer speeds should mitigate these types of attacks. Many cloud providers also offer variety of tools for these kinds of attacks.
## Are there any notable instances of this style of attack being performed?
In 2009 Slowloris attack was used against sites run by the goverment of Iran during presidential election. This type of attack was chosen for it's low usage of bandwidth.

[What is a denial-of-service attack?](https://www.cloudflare.com/learning/ddos/glossary/denial-of-service/)  
[What is a Slowloris DDoS attack?](https://www.cloudflare.com/learning/ddos/ddos-attack-tools/slowloris/)  
[Slowloris (cyber attack)](https://en.wikipedia.org/wiki/Slowloris_(cyber_attack))


