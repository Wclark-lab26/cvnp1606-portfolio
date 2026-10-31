

|Group Name|NTFS Permission|Share Permission|Effective Network Access|Test Result|
|-|-|-|-|-|
|HR-Managers|Full Control|Full Control|Full Control|Full Access|
|HR-Staff|Read/Write|Read-Only|Read-Only|Read-Only|
|Audit-Readonly|Read-Only|Read-Only|Read-Only|Read-Only|







Audit-Readonly is only allowed to read and not modify because Audit-Readonly is a base level entry point for all new users and that creates issues if they are allowed to modify files due to being able to change text and or delete information. Everyone was also removed from the share due to a similar reason, being that everyone can see it and this is private information for a company like ACME.

