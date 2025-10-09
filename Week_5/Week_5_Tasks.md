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


