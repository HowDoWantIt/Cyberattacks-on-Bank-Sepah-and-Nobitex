Technical Analysis of Cyberattacks on Bank Sepah and Nobitex
By Ali Shadi, Senior Security Analyst at IDC7Sky

Attack on Bank Sepah:
Initial Access: Likely gained via insecure RDP endpoints or spear-phishing campaigns targeting staff.

Lateral Movement: Use of tools like Mimikatz to harvest administrator credentials and move laterally inside the network.

Data Wiping: Deployment of custom wiper malware to destroy databases and internal backups, causing service outages.

Attack on Nobitex Cryptocurrency Exchange:
Initial Infection: Staff machines were infected with infostealer malware such as RedLine or AgentTesla, which secretly harvested session cookies and credentials.

Session Hijacking: Attackers used stolen session tokens to bypass two-factor authentication (2FA) and gain access to administrative wallets.

Cryptocurrency Theft: Funds were transferred to burn addresses (wallets with lost or inaccessible private keys), making recovery impossible.

Common Vulnerabilities Exploited:
Lack of robust multi-factor authentication (MFA) and poor session management.

Flat network architecture without sufficient segmentation between critical systems.

Backup systems were either locally stored or accessible, making them vulnerable to deletion.

Flowchart of the Attack Process:
Reconnaissance & Initial Access
(via RDP, VPN vulnerabilities, or spear-phishing)

Lateral Movement
(using Mimikatz, Pass-the-Hash techniques)

Data Exfiltration & Wiping
(targeting databases and backups)

Infostealer Malware on Staff Devices
(installing RedLine, AgentTesla, etc.)

Session Hijacking
(reusing stolen tokens to bypass 2FA)

Cryptocurrency Transfer
(to burn addresses, irreversible)
