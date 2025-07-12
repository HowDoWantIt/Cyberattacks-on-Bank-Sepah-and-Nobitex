# Technical Analysis of Cyberattacks on Bank Sepah and Nobitex

*By Ali Shadi, Senior Security Analyst at IDC7Sky*

---

## Attack on Bank Sepah

1. **Initial Access:** Likely gained via insecure RDP endpoints or spear-phishing campaigns targeting staff.  
2. **Lateral Movement:** Use of tools like **Mimikatz** to harvest administrator credentials and move laterally inside the network.  
3. **Data Wiping:** Deployment of custom **wiper malware** to destroy databases and internal backups, causing service outages.

---

## Attack on Nobitex Cryptocurrency Exchange

1. **Initial Infection:** Staff machines were infected with **infostealer malware** such as RedLine or AgentTesla, which secretly harvested session cookies and credentials.  
2. **Session Hijacking:** Attackers used stolen session tokens to bypass two-factor authentication (2FA) and gain access to administrative wallets.  
3. **Cryptocurrency Theft:** Funds were transferred to **burn addresses** (wallets with lost or inaccessible private keys), making recovery impossible.

---

## Common Vulnerabilities Exploited

- Lack of robust **multi-factor authentication (MFA)** and poor session management.  
- **Flat network architecture** without sufficient segmentation between critical systems.  
- Backup systems were either locally stored or accessible, making them vulnerable to deletion.

---

## Flowchart of the Attack Process

1. **Reconnaissance & Initial Access**  
   (via RDP, VPN vulnerabilities, or spear-phishing)  
2. **Lateral Movement**  
   (using Mimikatz, Pass-the-Hash techniques)  
3. **Data Exfiltration & Wiping**  
   (targeting databases and backups)  
4. **Infostealer Malware on Staff Devices**  
   (installing RedLine, AgentTesla, etc.)  
5. **Session Hijacking**  
   (reusing stolen tokens to bypass 2FA)  
6. **Cryptocurrency Transfer**  
   (to burn addresses, irreversible)

---

*Prepared by Ali Shadi, IDC7Sky*
