## CVNP-1606 Week 9



## Ticket Information



Ticket ID: CVNP1606-W09-009



Submitted By: Jordan Lee, Nexus Support Services Lead Technician



Affected System: Multiple ACME endpoints



Request: Work the four-ticket queue, prioritize by business impact, and document each resolution or escalation with full evidence.



Business Impact: High — multiple employees unable to work or experiencing degraded performance.



Initial Evidence: Four open tickets with mixed symptoms; see Lab Tasks for ticket details.





Required Outcome: ticket-pack.md with all four tickets addressed, evidence for each, and prioritization rationale.



## Scenario



Jordan Lee, Nexus Support Services Lead Technician, has briefed the team: ACME is having its busiest support day of the quarter. Four tickets just opened simultaneously. Each touches a different skill area from the first eight weeks. Your job is to triage the queue, prioritize by business impact, work each ticket using the correct tools and documentation standards, and close or escalate each one with full evidence. Before you start: confirm you can reach ACME systems from each affected machine — a fully isolated endpoint blocks both the fix and your ability to verify or document it.





## Tools Used



\-Powershell



\-Task Manager



\-Resource Monitor



\-Device Manager



\-Computer Managment



\-Event Viewer



\-Task Scheduler





## Troubleshooting Narrative



1. The most significant issue I encountered was the driver failure, due to the driver being installed on other machines and that firmware might act up on other machines and might need a total rollback for all of them.



2\. I checked to see what was causing the error through Device Manager, and found out that due to a issue with a firmware update it cause the device to become unusable



3\. I looked into the Device Manager, to see if any drivers were having issues



4\.    

&#x20;  p1: enabling the account



&#x20;  p2: rolling back firmware



&#x20;  p3: Port 445 is closed or blocked, it must be reopened for issue to be resolved



&#x20;  p4: Memory usage was high on device and after updating the required drivers caused it 	to use less 





5\. I ran through all of the tests again to prove that they were functioning again, even after a restart



6\. 

&#x20;  p1: Fixed lock out issue so they could log in and begin their job



&#x20;  p2: Firmware issues causing sound problems before important video calls are fixed by 	rolling back drivers



&#x20;  p3: Network issues caused by port 445 being closed and needing to be reopened



&#x20;  p4: Multiple issues with a slowing machine due to an older version of Windows Antivirus 	needing an update 





## What I can do now



I triaged a four-ticket mixed Windows support queue, prioritized by business impact, and resolved or escalated each ticket with documented evidence applying all production standards from Weeks 1 through 8.



No ai was used

