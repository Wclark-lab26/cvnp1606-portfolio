## CVNP-1606 Week 7



## Ticket Information



Ticket ID: CVNP1606-W07-007



Submitted By: Alex Torres, ACME Office Manager



Affected System: HP LaserJet (shared office printer), USB headset (audio device)



Request: Investigate driver state after Windows Update, restore device function, and document the change with a rollback plan.



Business Impact: High - printer is shared by the office; headset is needed for scheduled calls today.



Initial Evidence: Both devices stopped working on Tuesday after Windows Update completed. No changes were made by users.





Required Outcome: At least one device restored to working state, hardware inventory collected, change documented with before/after state, and a written rollback plan in case the fix causes additional problems.



## Scenario



You are a junior technician at Nexus Support Services. ACME's office manager, Alex Torres, reports that last Tuesday's Windows Update knocked out two devices in the main office: the HP LaserJet printer and a USB headset used for calls. Both need to be working before end of day. Your lead has asked you to investigate the driver state, make a safe remediation decision, and document the change with a rollback plan so another technician could reverse it if needed.





## Tools Used



\-Powershell



\-Run



\-Device Manager





## Troubleshooting Narrative



1. The printer had lost connection due to a wifi issue.



2\. I opened run and used devmgmt.msc to open the Device manager.



3\. I looked to see if I could rollback the connection but could not.



4\. I reinstalled the driver and scanned for hardware and it came back fixed.



5\. I ran the Get-Pnpdevice command and saw it was good.



6\. it supported the printer so people could use it again and if it does drop again I know what will fix it.





## What I can do now



I identified a driver regression after a Windows Update, rolled back and or repaired the printer driver safely, and wrote a change note and rollback plan so the team could reverse the fix if it caused new problems and for future use if the problem appears again.



No ai was used

