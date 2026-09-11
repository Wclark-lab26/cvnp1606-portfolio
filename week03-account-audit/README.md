## CVNP1606 - Week 3

## Ticket Information

Ticket ID: CVNP1606-W03-003

Submitted by: Jordan Lee, Nexus Support Services Lead Technician.

Request: Create seasonal staff and kiosk accounts with appropriate privilege levels, audit local group membership, and document the access rationale.

Buisness: High - seasonal staff cannot start work without accounts; kiosk is in active use with no access controls in place.

Initial Evidence: No seasonal or kiosk accounts exist. Existing local Administrators group membership has not been audited.

Required Outcome: Standard accounts created and verified, UAC behavior tested, group membership exported, and a written memo explaining the least-privilege decisions.

## Scenario 

ACME is onboarding a group of seasonal staff who need Windows access to complete their work but must not have administrator rights on their machines. ACME also has a shared kiosk machine in the break room that needs a restricted standard account so visitors and temporary employees cannot make system changes or access other users' files. Your job is to create and configure the required accounts, audit local group membership, and write a short memo explaining how the access decisions were made.

## Tools used

- Settings app

-User Account Control (UAC)

-Computer Managment


## PowerShell Commands Used

-  Get-LocalUser

-  Get-LocalGroupMember -Group "Administrators

-  New-LocalUser

-  Add-LocalGroupMember

## Documentation

- Screenshots

- GitHub
