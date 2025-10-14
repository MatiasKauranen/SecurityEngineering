# Week 6
## Task 1: Secure Running Environment?
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
