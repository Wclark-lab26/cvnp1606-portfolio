## CVNP-1606 Week 10



## Ticket Information



Ticket ID: CVNP1606-W10-010



Submitted By: Jordan Lee, Nexus Support Services Lead Technician



Affected System: ACME-W11-PILOT01 / ACME Intune tenant

&#x20;

Request: Prepare pilot Intune enrollment — create device groups, enroll test endpoint, verify join state with dsregcmd, and design pilot rollout plan for all 50 ACME endpoints.



Business Impact: Medium-High — ACME cannot begin cloud-first rollout until pilot process is validated.



Initial Evidence: No Intune enrollment or Entra join in place. Device groups not yet created.



Required Outcome: Enrolled endpoint with verified join state, documented tenant setup, and pilot group design memo.



## Scenario



Riley Chen, ACME branch manager, has informed Jordan Lee, Nexus Support Services Lead Technician, that ACME is shifting to a cloud-first device management model. All new endpoints will be Entra joined and Intune-enrolled rather than joined to the on-premises domain. Jordan has assigned you to prepare the pilot enrollment process: set up the required device groups, enroll one test endpoint, verify its join and management state, and design the pilot group structure for a phased rollout to the rest of ACME.



## Tools Used



\-Microsoft Edge



\-Microsoft Intune



\-Microsoft Entra



\-Powershell







## Troubleshooting Narrative



1. Trying to set up the AzureID



2\. I looked through both Entra and Intune to see if there were any warnings or issues with groups or users.



3\. To see if the account had a working subscription for Entra and Intune and seeing if it was enabled.



4\. Logging in using the AzureID login inside of settings.



5\. I ran dsregcmd /status.



6\. Updates for the groups would not work correctly and only some people would be getting the correct material.





## What I can do now



I enrolled a Windows endpoint into Entra ID and Intune and Azure, joined and managed the current status with dsregcmd, and designed a four-wave pilot rollout plan to help ACME migrate 50 endpoints to cloud-first management.



No ai was used

