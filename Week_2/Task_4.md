# Task 4: Wazuh

## What rule descriptions did you get?
"Integrity checksum changed."  
"File deleted."

## What are the MITRE ATT&CK techniques(include ID) Wazuh reports for these events?
Integrity checksum changed, ID:550, Tactic: Impact, Rule: T1565.001  
File deleted, ID=553, Tactic: Defense Evasion, Impact, Rule: T1070.004, T1485  

## What is the reported MITRE techniques for deleting files or directories inside monitored directories?
T1070.004 = Indicator Removal: File Deletion  
T1485 = Data Destruction 

## Explain in your own words where, when and why should these systems be used, would they be helpful in banking.
These system should be used to monitor most important files and folders of a system for unauthorized modifications. They are helpful in banking since they protect sensitive data such as account numbers and balance and prevent frauds. If something important changes for fradulent reasons then security can react fast.

## Add a screenshot of your integrity monitoring events tab.
Week_2\Integrity_Monitoring.png  
Week_2\MITRE_ATT&CK_Events.png
