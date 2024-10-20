# Day-30-Fortifying-Windows-Server-Security

Congratulations on reaching DAY 30! Today's focus on implementing security controls for Windows Server is a crucial step in fortifying your server against breaches. Based on the findings from the challenge, here are several security controls we implemented:

## Security Controls Implemented

1. **Limit RDP Access**
   - Restrict RDP access by:
     - Allowing RDP only from trusted IP addresses or through a VPN.
     - Using firewalls to block RDP access from unauthorized networks.

2. **Schedule Regular Maintenance Windows**
   - Ensure automatic updates are enabled to receive the latest security patches and system updates without manual intervention.
   - Regularly check for updates, especially for critical security patches and zero-day vulnerabilities.
   - Create scheduled maintenance windows for patch management to apply updates without disrupting business operations.
   - Test updates before deployment.

3. **Use Strong Password Policies**
   - Implement strong password policies that require complex passwords and regular password rotations to mitigate brute-force attacks and account lockouts.

4. **Deploy Endpoint Detection and Response (EDR)**
   - Keep Elastic Defend (Elastic EDR) active to detect and block malware, monitor suspicious activities, and ensure host isolation where possible.

5. **Enforce Least Privilege for Accounts**
   - Apply the principle of least privilege, ensuring that user accounts and services have only the minimal permissions necessary to perform their tasks.

6. **Enable Windows Firewall and Define Rules**
   - Configure Windows Firewall to block unnecessary ports and services while allowing only legitimate traffic. Define strict inbound/outbound rules based on business needs.

7. **Regularly Patch and Update the Server**
   - Ensure that your Windows Server is up-to-date with the latest security patches and updates, especially those addressing known vulnerabilities (e.g., SMB or RDP-related).

8. **Audit Logs and Set Up Centralized Logging**
   - Configure audit policies to log important security events (e.g., logins, failed authentication attempts).
   - Use Elastic Stack or any SIEM tool to centralize logs for better visibility and incident response.

9. **Network Segmentation**
   - Implement network segmentation to isolate sensitive areas of your infrastructure, limiting lateral movement in case of a breach.

10. **Enable Multi-Factor Authentication (MFA)**
    - MFA adds an additional layer of security beyond passwords, especially useful for securing RDP and administrative accounts.

11. **Enforce PowerShell Script Execution Policy: (Signed Scripts Only)**
    - Modify the Local Group Policy to allow only signed PowerShell scripts to run.

By applying these controls, your Windows Server will be significantly harder to breach, with better detection and response capabilities to thwart any attacks. Stay vigilant, keep refining your strategies, and you’ll have a rock-solid defense in place!

