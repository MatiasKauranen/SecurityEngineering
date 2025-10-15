# Week 6
# Task 1: Secure Running Environment?
It is important to understand the differences and security capabilities of the concepts listed below. Choose two out of the four concepts and write a short explanation of them and their respective security capabilities and incapabilities.

Focus on giving a good overview of the security limits for the concepts.

TPM  
Enclave  
**Container**  
**Virtualization**  

Max 300 words excluding sources.

## Container
Container is a unit of software application, that packages code and all dependencies it requires, so that the program runs fast and reliably in various computing environments. Container is lightweight, and it holds all required to run the application, such as: code, runtime, system tools, system libraries and settings.

Applications are safer in containers, since they have isolation capabilites. Isolation reduces risk, that malicious software gets out of the container, and infects other parts of the code. Containers also reduce attack surface, since containers only include absolutely neccessery components to run the applications. 

Containers are however not without risks. Applications and container images can have vulnerabilities, which could be exploited, such as outdated libraries, unpatched software and untrustworthy registries. Other risks include: Container breakout attack, insecure configurations and network security issues.

Sources:

[Use containers to Build, Share and Run your applications](https://www.docker.com/resources/what-container/)

[100% Transparency and Five Pillars](https://www.docker.com/blog/100-transparency-and-five-pillars/)

[Top 10 Container Security Issues](https://www.sentinelone.com/cybersecurity-101/cloud-security/container-security-issues/)



## Virtualization
Virtualization is a technology, which makes it possible to create multiple virtual environments from single physical machine. This makes resource usage more efficient, by distributing them across computing environments. Virtualization offers multiple benefits such as: resource efficiency, easier management, small downtime, quick provisioning, disaster recovery and cost-effectiveness.

Virtualization offers multiple security benefits: better control, application and network isolation, easier to keep OS and applications up to date, and smaller attack surface via Hypervisor.

Despite all benefits, virtualization poses some security concerns. VM Sprawl is caused by abandoning used VM's without proper decomissioning which can leak sensitive data due to vulnerable and unmanaged VM's. Malware can also infect VM's, and then spread to other environments. Bad VM configuration choices, such as file share between environments can cause vulnerabilities to malware and viruses. API's can also be risk to virtualized environments since they offer additional paths for attackers.


[What is virtualization? ](https://www.ibm.com/think/topics/virtualization)

[Virtualization Security: A Comprehensive Overview](https://www.liquidweb.com/blog/virtualization-security/)

[8 Most Important Virtualization Security issues](https://www.liquidweb.com/blog/virtualization-security-issues-and-risks/)


# Task 2: Supply Chain Attacks

In this task we are looking at the difficulties handling supply chain attacks, specifically detecting and responding.

For this scenario you are working for a networking hardware and software company, and you're tasked with securing their supply chain. The company manufactures and sells routers with their own software and other various networking accessories B2B and B2C. Some parts for the routers have to be outsourced and manufactured outside company.

Research and write a report on concrete actions you could implement on the supply chain, trying to make sure the product is not being tampered or researched with malicious intent. Keep in mind, that the supply chain includes third party tools, code and update providing, as well as other companies maintaining firmware. Your supply chain must include at least four actors including your company. You should analyze the points of concerns in the report.

Provide reasoning for your choices and analyze what potential problems and additional actions these choices might require from your company.

Probable actors in such supply chains include, but are not limited to:

    Employees, in-house and outsourced
    Transportation companies
    Retail companies
    Storage facilities
    Part suppliers

Example supply chain

Some concepts to help you get started:

    NDR (Network Detection and Response)
    UBA (User Behavioral Analytics)
    EDR (Endpoint Detection and Response)
    TPM (Trusted Platform Module)

Real-life cases for inspiration:

    SolarWinds
    Routers, servers and networking equipment from the USA | Notice the second page accessible at the bottom of the article

Minimum 500 words,
Maximum 4 visual representations,
Each visual representation is minus 50 words off the total required.

For example a report with 3 visuals requires 350 words.
The visuals must be useful for the report, ex. company logos do not count.

# Supply Chain Attacks

Protection from supply chain attacks has to take into account various factors, in which the first step starts from our own company. We have to be sure that our employees, whether they're in-house or outsourced, are to be trusted. Thorough background checks decrease the risk of insiders who could tamper with our products. An insider could potentially add backdoors or malicious software unnoticed. Additional security measures such as code reviews, signed commits, role-based access, and zero-trust principles could combat this risk. NDAs ensure that our ex-employees are held accountable if they leak sensitive information to our competitors or other parties. Even innocent employees could pose a security threat if they're not properly trained. Therefore, we must ensure that our employees are familiar with common security risks such as phishing and malware.

Part suppliers offer another surface for attackers. A supplier can have an insider who can modify chips with backdoors and malware. It's important to have a reliable supplier who has all security aspects under control. An unreliable supplier could provide counterfeit chips with vulnerabilities or provide chips that could potentially have vulnerabilities in their firmware. We should do randomized inspections on the parts we use.

The next step in our supply chain is the manufacturer. Like in our own company and supplier company, insiders pose a significant threat also in this step. They could tamper with our hardware, such as installing malicious firmware or physically modifying our devices. Extensive inspections and testing should make it less likely that tampered products get out of the production line. Completed products should be packaged and sealed in a way that prevents tampering.

Transportation is not without risks for the supply chain. The company should use only reliable transportation companies that can transport high-security products. Transport companies that hire drivers without proper background checks could compromise the supply chain. We must use tamper-resistant packages and serial numbers in our products, which can indicate if our supply chain is compromised. Other measures, such as GPS tracking for our high-value shipments, could increase security. These measures should make it less likely that compromised and modified products can move in the supply chain without being detected.

Even if our products are physically safe in secure transport, they can still be vulnerable to third-party software on which our product depends. Unsupported, unupdated, or abandoned libraries could cause vulnerabilities. There must be policies that ensure these unreliable libraries are replaced before they cause any issues. Compromised dependencies and packages offer another surface for attackers if not kept under control. All used dependencies should be verified to prevent unverified packages from compromising our supply chain. Using open-source code can be vulnerability, since attacker can use known vulnerabilities.

The last step in our supply chain is retail. A malicious retailer could tamper with our products before they reach our customers. They could attempt to install modified firmware or configurations. We should add security measures to make this less likely. Using our tamper-proof packaging could alert our customers to compromised products. We could also add a portal for customers to check their products’ authenticity after purchasing. This should prevent retail from selling counterfeit products in our name.

Words: 530


Sources:

[Supply chain attack](https://en.wikipedia.org/wiki/Supply_chain_attack) 

[Supply Chain Attack: How It Works and 5 Recent Examples](https://www.oligo.security/academy/supply-chain-attack-how-it-works-and-5-recent-examples)  

[What is a supply chain attack?](https://www.cloudflare.com/learning/security/what-is-a-supply-chain-attack/) 

[Supply Chain Attacks: The Bump in the Night That Keeps Us Awake](https://www.sep2.security/supply-chain-attacks/) 


