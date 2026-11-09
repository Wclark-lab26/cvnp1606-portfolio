## CVNP-1606 Week 11



## Ticket Information



Ticket ID: CVNP1606-W11-011



Submitted By: Jordan Lee, Nexus Support Services Lead Technician



Affected System: ACME tenant / multiple endpoints including Emily Park’s remote workstation

&#x20;

Request: Create compliance policy, document CA report-only logic, write security exception note template for noncompliant edge cases.



Business Impact: High — company data accessible from unmanaged devices violates ACME governance policy.



Initial Evidence: No compliance policy exists. CA policies not configured. Emily Park's device is Entra registered but not Intune-enrolled.



Required Outcome: Compliance policy created and documented, CA report-only policy logic explained, Hello/LAPS evidence note, security exception note template.



## Scenario



Riley Chen, ACME branch manager, has escalated a concern to Jordan Lee, Nexus Support Services Lead Technician: several ACME remote employees, including Emily Park, are signing in to Microsoft 365 from personal devices and endpoints that have not been through the Intune enrollment process. ACME’s IT governance policy requires that only compliant, managed devices access company data. Your job is to create or analyze a Windows compliance policy, connect it to Conditional Access logic in report-only mode, and document what would happen to a noncompliant device like Emily’s if the policy were enforced. You will also document Windows Hello for Business and LAPS as endpoint identity controls.



## Tools Used



\-Microsoft Edge



\-Microsoft Intune



\-Microsoft Entra







## Troubleshooting Narrative



1. 



* Microsoft Defender Antimalware



* Bitlocker



* Minimum OS version





\------------------------------------------------------------------------------------



* Bitlocker failed the test.



\------------------------------------------------------------------------------------



* Bitlockers failure could be cause by some problems such as a suspended bitlocker state or issues with the Intune framework.



\------------------------------------------------------------------------------------



2\. You'll see a sign in for your Azure account or a access denied due to a failure.



3\. Emily would need to be Intune enrolled on a device so that Intune can have full MDM and policy enforcement



4\. any member of the team causing a failure in their policy list



5\. when the business risk of adhering to the policy outweighs the security risk of violating it.



6\. Issue a "Report-Only" deployment strategy paired with group-based rollouts.



## What I can do now



I created a Windows compliance policy in Intune, connected it to a Conditional Access policy in report-only mode, and documented how noncompliant machines would affect ACME remote employees and what a security exception process requires of both evidence and outcome.



Ai usage:



Google Gemini assisted me in creating a outline for the laps-hello-note.

