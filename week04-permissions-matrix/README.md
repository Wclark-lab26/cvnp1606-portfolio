\## CVNP-1606 Week 4



\## Ticket Information



Ticket ID: CVNP1606-W04-004



Submitted By: Jordan Lee, Nexus Support Services Lead Technician



Affected System: ACME-W11-BASELINE (acting as file server)



Request: Build the HR payroll share with group-based NTFS and share permissions, test effective access from multiple account contexts, and deliver a documented permissions matrix with ACL evidence.



Business Impact: High - payroll data is sensitive. Incorrect permissions expose confidential records or lock out staff who need access to do their jobs.



Initial Evidence: No HR share exists. Default Everyone Full Control is present on the test share created during initial server setup.



Required Outcome: A secured HR share with group-based permissions, ACL evidence before and after, access test results from the HR-Staff account context, and a permissions matrix that could be handed to a peer or auditor.



\## Scenario



HR is moving payroll files to a dedicated shared folder on the ACME file server. Three groups need different levels of access: HR-Managers require Full Control so they can manage the folder and its contents, HR-Staff need Read and Write access to work with payroll files daily, and Audit-Readonly needs Read-only access for compliance review. No other users should be able to access the share. The current default Everyone permission on the parent share must be removed before the share goes live.





\## Tools Used



\-Powershell



\-Computer Management





\## Troubleshooting Narrative



1. Access could have been lost if improperly done

2. I checked to see if all of the made groups had their proper restrictions in place

3. I ran threw the code several times to see if their restrictions held up 



4\. I would run through the code again to make sure I had all of the details and permissions correctly set up 



5\. I logged into the hr-staff-test account to see if I could add anything and I could not



6\. All Accounts that could reach the file were able to and had the correct permissions when in a specific group





\## What I can do now 



I built a secure HR share folder at ACME, assigned group-based NTFS and share permissions, tested access from multiple account, contexts and interactions, and documented the permissions for each model so a peer or auditor could verify it. 





