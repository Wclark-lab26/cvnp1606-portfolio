\## Section A: Windows Hello for Business







\## What it replaces



Windows Hello for Business completely replaces traditional reusable passwords and vulnerable local PINs for network and cloud authentication. Unlike standard Windows Hello, which only unlocks a single local device, WHfB replaces the need to transmit password hashes across the network, acting as a full replacement for legacy Active Directory passwords during authentication.



\## How it works



WHfB is a specialized distributed two-factor authentication system that relies on a strong cryptographic key pair bound to a specific device's Trusted Platform Module (TPM) security chip.



• Provisioning: When a user sets up WHfB, a unique asymmetric key pair (or certificate) is generated inside the hardware TPM. The private key never leaves the TPM, while the public key is registered with the organization's identity provider (such as Microsoft Entra ID or Active Directory).



• Authentication: To log in, the user provides a gesture—either a biometric scan (facial recognition or fingerprint) or a local PIN. This gesture acts strictly as a local "release mechanism" to unlock the private key inside the TPM. The TPM then signs a cryptographic challenge sent by the authentication server. The server verifies the signature using the registered public key, granting access without ever seeing or storing the user's gesture or a password.



Why it is stronger than a password or local PIN



• Asymmetric Cryptography: Traditional passwords can be guessed, phished, or intercepted. WHfB uses a private-public key pair; because the server only holds the public key, a breach of the authentication server does not compromise user credentials.

• Hardware-Bound Possession Factor: Unlike a standard password or a basic Windows PIN that might be stored in software, the WHfB credential is physically tied to the device's hardware TPM. Even if an attacker learns a user's WHfB PIN, it is completely useless to them unless they physically steal that exact computer.



• Anti-Phishing Defenses: Because authentication relies on a cryptographic challenge-response specific to the device and the registered identity provider, users cannot be tricked into typing their WHfB credentials into a fake phishing website.





\## Section B: Windows LAPS







\## What problem it solves



Windows LAPS solves the critical security risk of static, identical local administrator passwords across an organization's endpoints. Historically, IT departments set the same local admin password on every workstation for easy troubleshooting. If an attacker compromises a single machine and extracts that local admin password, they can easily log into every other machine on the network, performing unchecked lateral movement.

How rotation works

Windows LAPS automatically manages, rotates, and secures the password of a specified local administrator account on each machine.



1\. Centralized Policy: Administrators configure a LAPS policy via Group Policy or Microsoft Intune, defining password complexity, length, and age requirements.



2\. Local Generation \& Storage: The built-in LAPS operating system component on the client machine automatically generates a random, complex password that meets the policy.



3\. Secure Backup: The client machine securely uploads this unique password directly to a protected attribute in Active Directory or Microsoft Entra ID.



4\. Scheduled Rotation: Once the password age expires (e.g., every 30 days), or immediately after an authorized admin reads and uses the password, the local LAPS agent automatically triggers a rotation, generating a brand-new password and updating the directory.



\## Why it specifically matters for ACME’s cashier kiosk machines



• Physical Exposure Risks: Cashier kiosks sit in public, high-traffic retail environments where they face an increased risk of physical tampering. If a malicious actor attempts to boot a kiosk into a recovery environment or exploit local access, LAPS ensures they cannot use a guessed corporate-wide "master" local admin password to gain control.



• Blast Radius Containment: Kiosks are highly vulnerable to targeted local attacks. If a single cashier kiosk is compromised via a physical USB exploit or local vulnerability, Windows LAPS guarantees that the local administrator password discovered on that specific machine is completely random and unique. The attacker cannot use it to compromise adjacent registers, back-office servers, or ACME's wider corporate network.



• Automated Remediation for Disconnected Devices: Kiosk environments frequently experience network shifts or reboots. LAPS operates natively within the Windows OS framework, ensuring that local administrative access remains strictly managed and auditlocked without requiring manual IT oversight for every individual cash register.

