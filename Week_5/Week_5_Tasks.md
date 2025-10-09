# Week 5
# Task 1: Bring your own devices
Following link containing NIST:s security recommendations for workplace bring your own device. On the page 12 is listed following 9 threat events, and your job is to make one A4 sized poster or otherwise shortly summarize what each listed threat event means based on the document or your own research.
## Intrusive application practices
Intrusive application practices refers to application which collects users personal information and data without their knowledge or consent. Criminals often use these kinds of applications to harvest sensitive data for reselling, targeted ads, or other malicious purposes.
## Account credential theft through phishing
Credential phishing is spesific type of phishing which aim is to gain access to victims username and password. Attacker uses phised credentials to gain unauthorized  access to accounts such as email, business resources or other valuable accounts.
## Outdated phones
Outdated phones pose a security threat for multiple reasons: outdated OS, insecure configs, elevation of privileges, unauthorized device profiles and compromised devices. Best way to prevent these kinds of vulnerabilities is to have phone with latest OS and security updates.
## Sensitive data transmissions
Sensitive data should only be transmitted through secure channels. Using unencrypted Wifi or unauthorized apps can pose a security threat via data exposure or interception.
## Brute-force attacks to unlock a phone
Brute-force attack refers to attacker trying to guess password to unlock phone. If password it too short or too easy to guess, attacker may gain access to stolen phone. It's advised to use strong or biometric password to secure your devices.
## Application credential storage vulnerability
This vulnerability refers to situation in which device stores credentials in plain text or other unsecure forms which could potentially be stolen via physical or remote access.
## Unmanaged device protection
Unmanaged device protection refers to security risk in which unmanaged devices have access to company resources. Unmanaged devices usually lack sufficient security measures or tools to protect these valuable resources.
## Lost or stolen data protection
This risk refers to situation in which valuable data is stored on device which can be lost or stolen. These devices therefore have to be secured to prevent potential data loss or leak. This kind of risk can be mitigated for example by using cloud only storage and avoiding storing on local storage.
## Protecting enterprise data from being inadvertently backed up to a cloud service
This risk refers to situation in which sensitive corporate data is unintentionaly uploaded to public or personal cloud. This risks data privacy and violates compliance. Storing on public/personal cloud can also cause data leaks.

# Task 2: attacks on CPU execution
spectre and meltdown are two original side channel attacks discovered in 2017 that target cpu, and over the years more have been discovered. This wikipedia article list some of them. Pick 3 of them to research about how exactly each exploits the system,their differences, which systems they targeted and how they can be mitigated.

Answer in max 300 words. You are free to use tables or otherwise make to comparison easier to read if you wish.

## Foreshadow
Foreshadow is a vulnerability, which was first discovered in january 2018. Foreshadow is a speculative execution attack on Intel processors. It targets sensitive data on PC's and third-party clouds. It's similiar to Spectre vulnerability which affects both Intel's and AMD's processors. However Foreshadow doest not affect AMD processors which is best way to mitigate the vulnerability. Newer Intel processors also mitigate this vulnerability. There are two versions of this vulnerability:

Original version (CVE-2018-3615): Targets data from SGX enclaves  .

Second version (CVE-2018-3620 and CVE-2018-3646): Targets VMs, hypervisors, OS kernel memory and System Management Mode (SMM) memory.

## Microarchitectural Data Sampling (MDS)
Microarchitectural Data Sampling or MDS for short are set of vulnerabilities, which was first discovered by Intel's researchers in 2018. These vulnerabilites are in Intel x86 microprocessors that use hyper-threading. Vulnerability causes data leak across protection boundaries which should be secure. However there are many variants of MDS and not all processors are affected by all variants. Old processors have this weakness, however new processors have mitigations againts this vulnerability.

## Load Value Injection (LVI)
Load Value Injection or LVI for short, is vulnerability discovered in march 2020. LVI attacks Intel's Software Guard Extension or SGX for short. It's development of well known Meltdown vulnerability. Unlike Meltdown, LVI can inject data values and is resistant to countermeasures used against Meltdown. There is mitigation guide by Intel which recommends using compiler technology to protect vulnerable parts in code.

# Task 3: Securing OS
Following is a list of some of the more common vulnerabilities and attack vectors existing in operating systems.

Malware and Viruses  
Exploiting Software Vulnerabilities  
Phishing and Social Engineering  
Drive-by Downloads  
Zero-Day Exploits  
USB/Removable Media Attacks  
Password Cracking  

Make short write up about each that answers following questions

What harm can it cause to you?  
How OS of your choosing (Windows, Mac, Linux) can mitigate it?  
Function of the OS itself or external tools?

## Malware and Viruses  
Malware is software designed to cause harm. Virus is type of malware which replicates itself to spread to new files. Can erase or corrupt files or steal valuable data as credentials to your accounts. Can also encrypt files (ransomware). Windows Defender offers protection with windows updates. Real-time scanning offers added security.

## Exploiting Software Vulnerabilities   
Softwares can have vulnerabilities which attacker can expose. Attacker can execute code to gain access to other parts of the system which can compromise whole system. Windows updates mitigate vulnerabilities and Windows Sandbox offers isolated environment to run risky software.

## Phishing and Social Engineering  
Phishing and Social Engineering try to exploit human nature and psychology to get victim to give sensitive data. It can cause stolen credentials, fradulent transcations and unauthorized access. OS and external tools offer little help against these types of attack and best defence is phishing training.

## Drive-by Downloads
This attack causes silent infection by visiting malicious website. Attacker uses browser or browser plugins to download malicious data without user noticing. This can cause data leakage and system takeover. Windows offers SmartScreen to block harmful downloads and Windows Defender Application Guard for untrusted sites.  

## Zero-Day Exploits  
Attack which exploits unknown or patchless vulnerabilities. These attacks can bypass defences and compromise system without being detected. OS offers little to mitigate these attacks but external tools and quick patches are important.

## USB/Removable Media Attacks  
In this attack physical USB drive is used to auto execute malicious code to gain access to device. Best ways to mitigate is to use OS controls to turn auto play off for usb devices. There are also external tools which scan usb devices before execution.

## Password Cracking  
It's brute-force attack trying to guess victims credentials. This attack can give account information and unauthorized access to the attacker. Windows offers various tools to enforce strong passwords such as policies and MFA. There are also external tools such as password managers to mitigate these attacks.

# Task 4: Logging
Log files are records of events or actions that occur in a system, application, or program. Logs are essential for troubleshooting, debugging, and analyzing the behavior of software or hardware.

Find answers to following questions:

1. What kind of information would be saved into following types of log files

- Application logs
- Event logs
- Service logs
- System logs

2. Where in each of the common Operating Systems those logs would be stored (Windows, Mac, Linux(changes per distro so provide in answer which you are using)

3. What kind of threats could you notice by monitoring each log file?  
4. How would you go about monitoring logs on your personal computer?  

remember to list sources for information you use!

## Application logs
Application logs are records of events generated by the application. They hold data such as error messages, user inputs, events, and application spesific data. In Windows you can browse application logs in Event Viewer. Application logs can reveal malicious application behaviour such as trying to access sensitive data or unexpected behaviour.

## Event logs
On Windows event logs is a record of events related to system, security and all applications stored on the device. There are four common event types: system, application, setup and security. Location on Windows is: C:\WINDOWS\system32\config\ folder. Monitoring event logs you could spot threats such as unauthorized activity and external threats.

## Service logs
Service logs refer to logs containing information about system services or background processes. These can be viewed via Event Viewer. Crashes or restarts of critical services may indicate malicious intent.

## System logs
Windows system logs are records which hold important events related to operation system's operations. These logs include information about shutdown and startup processes, system errors and hardware events. In Event Viewer you can scroll through system spesific logs. These logs can reveal suspicious activity such as unknown USB insertions, suspicious events and unexpected hardware changes.

## How would you go about monitoring logs on your personal computer?
Easiest way to monitor logs on Windows is to use Event Viewer. Using Event Viewer user can view events of system, applications, security and much more. There are also many safe external tools to monitor ones PC. Process Monitor is an advanced monitoring tool for Windows which has many useful features such as filtering and comprehensive event properties.


Sources:

[What is an Application Log? ](https://www.crowdstrike.com/en-us/cybersecurity-101/observability/application-logs/)   

[Complete guide to application logging](https://newrelic.com/blog/best-practices/how-to-manage-an-application-log) 

[What is Windows Event Log?](https://www.solarwinds.com/resources/it-glossary/windows-event-log) 

[Ultimate Guide — Windows Logging Basics](https://hassen-hannachi.medium.com/ultimate-guide-windows-logging-basics-1d7ef9f4e512) 

[How to view and access Windows system logs?](https://www.manageengine.com/products/eventlog/kb/how-to-view-and-access-windows-system-logs.html) 

[Process Monitor v4.01](https://learn.microsoft.com/en-us/sysinternals/downloads/procmon) 