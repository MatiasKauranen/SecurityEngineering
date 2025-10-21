 Task 1: Safety Concerns

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