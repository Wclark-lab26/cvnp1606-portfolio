As we transition our Conditional Access (CA) policy to full enforcement, this memo details the precise user workflow and the operational value of our phased rollout.



1\. User Experience: When you open Outlook on your personal laptop, the CA policy intercepts your sign-in and evaluates the device's status. It checks whether the laptop is marked compliant in Intune. Because the device is not enrolled, the policy blocks access and displays an error page.



2\. Technician Response: the helpdesk technician will explain that the personal device must be enrolled in Intune and pass compliance checks before access is restored. If enrollment is not feasible, the technician will initiate the official security exception process.



3\. Value of Report-Only Mode: Keeping the policy in report-only mode first is the right strategy because it answers critical operational questions before users face disruption. It allows us to quantify affected users and validate the remediation path without blocking active workflows.

