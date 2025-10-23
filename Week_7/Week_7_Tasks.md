# Task 1: Safety Concerns

In terms of medical equipment and automotive industry mentioned in the Lecture 13, consider the following:

    Why are new safety concerns sometimes overlooked?
    What are events that trigger sudden change?

250 words maximum, cite if you use external sources

Security Engineering Lecture 13: Safety and Security

## Safety Concerns

## Why are new safety concerns sometimes overlooked?
Vendors often try to blame users for product safety concerns, thus claiming that the issue is 'user error'. Vendors want to deny responsibility for these security concerns to avoid legislative consequences. In the case of infusion pumps, the issue was with different and non-standardized user interfaces that made human mistakes more likely to happen. Having a standardized system would make these accidents less likely to occur. Oftentimes, these large companies have significant political or lobbying power to slow down the process of standardization. After all, these companies would lose a lot of money if they had to change their manufacturing methods or if their inventory in warehouses became obsolete due to being non-standard.

## What are events that trigger sudden change?
Incentives to improve safety are not working; therefore, security scares are the driving force behind sudden changes in security concerns. A security scare in which it was proven that pacemakers could be taken over via the RF channel proved that security scares can bring a lot of attention to safety concerns and lead to quick changes. Overall, progress is still very slow.

# Task 2: Static and Dynamic Analyzers

Explain the difference between static and dynamic analyzers. Explain what the advantages are of using these tools during production. Pick one of the Static or Dynamic testing methods mentioned in the Lecture 14 and write a brief description of it.

250 words maximum, cite if you use external sources

Security Engineering Lecture 14: Assurance and Sustainability

## Static and Dynamic Analyzers
Static analyzer runs before the code is run, making these compile time tools. Static analyzers such as Lint tools help to reduce amount of bugs, syntax errors, type mismatches, unused variables and other potential code vulnerabilities, if used early in the project. Dynamic analyzers run over the code, meaning that they work during the runtime. They are very good for catching issues such as memory leaks, buffer overflow and other exceptions.

## Linters
Linters such as ESLint are static analyzers. These linters try to spot potential programming issues or in other words 'code smell' before the code is run. These linters should find potential issues despite them not having any syntax errors since that code could become buggy in the future. Linters should be used early on to prevent any potential issues in future. Linters are also useful tool to enforce custom rules to match the 'house style' if there are multiple people working on the project.

# Task 3: Security Certification
Consider the different incentives (both 'Good' and 'Bad' incentives) for Security Certification of a product from the following points of view:

    Potential End User/Buyer of the product
    Certifying authority (both vendor funded and non-profit)
    Manufacturer/designer of the product

400 words maximum, cite if you use external sources

(EXPLANATIONS)

    Vendor funded = Applicant pays the certifying authority for the certification process
    Non-profit = Applicant does not have to pay directly for the certification process

Security Engineering Lecture 15: Governance and Regulation Security Engineering Lecture 16: Ian Levy, NCSC - Protecting a country for fun and profit


## Potential End User/Buyer of the product
### Good Incentives
Certificates provide assurance of product security to the end user. This increases confidence and trust that the product properly protects sensitive data. Certified products simplify risk calculations. A certified vendor appears more professional and reliable.
### Bad Incentives
Certificates can bring a false sense of security and they don’t guarantee safety. Certificates also increase product prices since obtaining these certificates isn’t free.

## Certifying authority (both vendor funded and non-profit)
### Good Incentives
Successful certificates build reputation and credibility. Certificates provide revenue to the certifying authority in the form of certifications, renewals, and audits. Trust in certificates encourages the use of better security practices. This increases market demand for certificates when companies want to certify their products.
### Bad Incentives
In a vendor-funded model, the certifying authority may be more interested in making the applicant pass to keep them as a customer rather than make them fail and potentially lose them. This conflicting interest puts profits over security. This reduces demand for certificates when their credibility decreases. Non-profit certifying authorities don’t have the same issue; however, their challenge is the administrative burden since they do it for non-profit purposes.

## Manufacturer/designer of the product
### Good Incentives
Certification gives an advantage over competitors who don’t have certificates. Certificates increase the overall security of the manufacturer due to the policies they bring. Certificates can also protect the company in case of security breaches since these certificates are proof that the company has put effort and resources into their security.
### Bad Incentives
Certificates bring high recurring costs to the company since they require annual renewals to stay up to date. This also requires a lot of effort from the IT department to maintain the certificates, preventing them from working on other projects. In less regulated industries, certificates have a lower return on investment. Certificates can also lead to false assurance and ignorance of the security of other systems.

# Task 4: NIS2 & RED

There are currently three European Union Directives that will affect current and future products and services. These Directives are:

    Cyber Resilience Act (CRA)
    Radio Equipment Directive (RED)
    Revised Directive on Security of Network and Information Systems (NIS2)

Traficom has collected information regarding all three quite concisely providing a good starting point for familiarizing on the subject

    (CRA) https://www.kyberturvallisuuskeskus.fi/en/toimintamme/saantely-ja-valvonta/kyberkestavyyssaados-cyber-resilience-act-cra
    (RED) https://traficom.fi/en/news/new-information-security-requirements-eu-improve-information-security-wireless-devices
    (NIS2) https://www.kyberturvallisuuskeskus.fi/en/our-activities/regulation-and-supervision/nis2-european-union-cybersecurity-directive

PICK ONE, Either CRA, RED or NIS2 and answer the following questions

    Concisely explain the main goal of the directive?
    Which types of products does it concern?
    Which types of organizations does it concern?
    What kind of cybersecurity measures have to be implemented for a product/organization to comply with the directive?
    When (Date) do organizations/products need to comply with the directive?
    What are possible penalties?
    Your own thoughts: How does this benefit you/society overall. Are there positive and negative aspects?

You can answer directly to each bullet point with few sentences

## Cyber Resilience Act (CRA)
### Concisely explain the main goal of the directive?
The main goal of the directive is to improve the security of products and software sold in the EU market. These directives aim to ensure that products have fewer vulnerabilities.
### Which types of products does it concern?
All products with a digital element that can connect to other devices via a network.
### Which types of organizations does it concern?
It concerns manufacturers, importers, and other vendors who sell these products in the EU.
### What kind of cybersecurity measures have to be implemented for a product/organization to comply with the directive?
Measures include secure default settings, automatic security updates, prevention of unauthorized access, confidential storage, minimization of data, and securing key functionalities.
### When (Date) do organizations/products need to comply with the directive?
Notified bodies: 11 June 2026, vulnerability reporting: 11 September 2026, and full product compliance with essential cybersecurity requirements: 11 December 2027.
### What are possible penalties?
No specific penalties are listed, but most likely the product or software would be withdrawn from the EU market.
### Your own thoughts: How does this benefit you/society overall. Are there positive and negative aspects?
Hopefully, this increases overall cybersecurity for devices and software in the EU market and abroad, as manufacturers aim to enter the EU market. However, small businesses may struggle with these policies due to costs, and if handled poorly, slow EU bureaucracy could hinder innovation across the tech market in the EU.