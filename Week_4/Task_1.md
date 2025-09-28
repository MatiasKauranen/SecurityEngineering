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