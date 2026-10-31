## CVNP-1606 Week 5



## Ticket Information



Ticket ID: CVNP1606-W05-005



Submitted By: Riley Chen, ACME Branch Manager (via Nexus helpdesk)



Affected System: ACME-BRANCH-WS01



Request: Diagnose application freezing during the first 10 minutes post-login. Identify the bottleneck, apply one safe remediation, and provide before and after metrics.



Business Impact: High - Riley hosts client-facing meetings; freezes disrupt video calls and presentations.



Initial Evidence: No HR share exists. Default Everyone Full Control is present on the test share created during initial server setup.



Initial Evidence: User reports 10-15 second freezes when switching apps, worst in first 10 minutes after login. No recent hardware changes reported.



Required Outcome: A documented performance remediation with before-metrics, a change note, after-metrics, and a portfolio README that a peer technician could follow to verify the fix.



## Scenario



You are a junior technician at Nexus Support Services. Riley Chen, ACME's branch manager, has submitted a helpdesk ticket reporting that her meeting workstation freezes for 10 to 15 seconds when switching applications. The problem is worst during the first 10 minutes after login. Your lead has asked Nexus to investigate the endpoint, identify the bottleneck using evidence, apply one safe remediation, and document the before and after state so the fix can be reviewed or replicated by another technician.





## Tools Used



\-Powershell



\-Task manager



\-Resource monitor





## Troubleshooting Narrative



1. I set all high impact applications to enabled. The business impact


2\. I checked Task manager first, that shows all the wake up applications all together.


3\. My hypothesis was that Microsoft explorer was the main issue causing the slow down on wake up and I check task manager for that





4\. I disabled Microsoft explorer in the Startup apps section in task manager. Microsoft explorer does not become unusable if disabled on wake up





5\. I restarted the machine and used the Get-Process command to show that the cpu has been brought down and the machine is running faster



6\. I'd use the Get-Process command again to see what application is bringing down the machine, and look inside of the resource monitor





## What I can do now



I Identified the issues with a slow Windows 11 endpoint using Task Manager, Resource Monitor, and PowerShell evidence, identified a startup bottleneck, applied a safe solution, then wrote down and screenshotted the before and after state for a branch manager's machine.



No ai was used

