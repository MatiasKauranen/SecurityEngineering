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


# Task 3: BurpSuite
##  Subtask 1: Intercepting (0.25p)
To your github return repository, add a screenshot/screenshots of your edited post so that all the following information is visible.

-Listing of the last POST and GET request including timestamps and port  
**Week_4\Intercepting_POST_and_GET_requests.png** 

-Entire Edited POST request in Raw format
**Week_4\Intercepting_Edited_request.png** 

## Subtask 2: Repeater (0.25p)
Try to figure out how the dvwaSession cookie is generated by looking at the response after multiple repeats. Return a brief explanation on how a new cookie is generated and a screenshots where both Request and a corresponding Response is visible in Raw or Pretty format.

## Cookie generation
DVWA cookie seems to use UNIX time representation which calculates seconds from january 1st 1970.

Screenshot: **Week_4\Repeater.png**

## Subtask 3: Intruder (0.25p)
Inspect the results. Which bruteforce attemps were successful? Explain how did you come to this conclusion and what kind of evidence did you find from the responses? Return the explanation along with a screenshot where all 24 attempts are listed. If you find evidence of a successful attempt from the responses, include it in the screenshot.


## Explanation
I found successful brute force attack had welcome message in response for admin user: "Welcome to the password protected area admin"

Screenshot: **Week_4\Intruder.png**

## Subtask 4: Decoder (0.25p)
Return a screenshot of all the encoded and decoded results.  
Screenshot: **Week_4\Decoder.png**

## Subtask 5: thc-hydra (1p)

Return the following:

- Screenshot of the finished hydra command where atleast finishing time and last attempt are visible. Make sure the four letter password you used is visible:
**Week_4\Hydra.png**  
- How many minutes did the brute forcing process take?  
For 2 letter password it took 2 seconds, for 4 letter password (bart) it took 4 minutes. Every letter makes brute forcing exponentially harder.

- The full hydra command:
```
docker run --network="host" vanhauser/hydra -V -f -I -l admin -x 4:4:a "http-get-form://localhost/vulnerabilities/brute/:username=^USER^&password=^PASS^&Login=Login:H=Cookie:PHPSESSID=4q4iqquba85jjmq62q7b964pt2; security=low:F=Username and/or password incorrect."
```
