AzureAdJoined   : YES

WorkplaceJoined : NO

DomainJoined    : NO

MdmUrl          : (blank)







State: The machine is not registered on the BYOD path and the intune enrollment did not succeed 

Root Cause: The Entra account is not connected to the OS
Remediation: Login by going to Settings (Win+I) - Accounts - Work and school, then login

Verification: restart machine then run dsregcmd /status inside powershell

