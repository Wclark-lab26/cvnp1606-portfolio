## CVNP-1606 Week 8



## Ticket Information



Ticket ID: CVNP1606-W08-008



Submitted By: Riley Chen, ACME Branch Manager



Affected System: ACME-W11-POS01

&#x20;	

Request: Investigate unexpected overnight reboots, build an event log timeline, and produce a written root-cause analysis.



Business Impact: High — insurance audit requires documented cause within 48 hours.



Initial Evidence: Event ID 6008 (unexpected shutdown) present in System log. No user was logged in at time of reboot.



Required Outcome: Event timeline, exported log evidence, and written root-cause analysis with escalation note



## Scenario



Riley Chen, ACME Branch Manager, has submitted an urgent support request. The cashier workstation ACME-W11-POS01 rebooted twice overnight with no one logged in. Riley needs documented cause for an insurance audit — guesses are not acceptable.



Your job as a Nexus Support Services technician is to investigate the Windows event logs, build a chronological event timeline, and write a defensible root-cause analysis that Riley can present to the auditor.





## Tools Used



\-Run



\-Powershell



\-Event Manager





## Root-Cause Analysis



Hypothosis:	The evidence on each of the events show that the machine has been incorrectly rebooting without powering down first.



Supporting Evidence:	With each and every restart, there is a incorrect rebooting event that occurs.



Alternative causes considered:	Other problems with the pc can cause a incorrect reboot due to not functioning correctly.



Escalation note: If the machine starts automatically restarting itself due to error codes or issues with hardware, contact tech officials.









## Troubleshooting Narrative



1. To investigate overnight reboots with the event ID of 6008 (unexpected shutdown) present in System log.



2\. I opened run and used eventvwr.msc to open Event Manager, sorted it down to events only using critical and error tags then sorted those by codes 41 and 6008 using powershell. I then took those event ID's and codes and sorted them chronologically.



3\. I found both 41 and 6008 event ID's, showing improper shut down and restarting.



4\. The machine is rebooting itself due to the improper shut down.



5\. Issues with the hardware could cause improper shut downs and restarts as well, as the pc is trying to fix itself.



6\. Once the machine starts giving crashes and starts shutting down during service.





## What I can do now



I used Event Viewer and Get-WinEvent to investigate unexpected reboots, built an event timeline with each event put into chronological order to show it clearer, and wrote a root-cause analysis that gave ACME's branch manager documented evidence for an insurance audit



No ai was used

