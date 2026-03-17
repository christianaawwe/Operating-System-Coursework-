
**1) Open terminal and type**

<img width="1017" height="603" alt="image" src="https://github.com/user-attachments/assets/325b6375-a02a-432b-a741-4cc2bc15085f" />


The system packages were updated to ensure the server is running the latest security patches before performing the security audit.

-----------------------------------------------------------

**hostnamectl**

<img width="820" height="370" alt="image" src="https://github.com/user-attachments/assets/f663fe68-aba6-4902-be1f-4bf6d72d6553" />

**uname -r**

<img width="802" height="85" alt="image" src="https://github.com/user-attachments/assets/fd347e3d-1c0b-475a-a840-192339192683" />


System information was retrieved to identify the operating system, kernel version, and system configuration prior to the security audit.

----------------------------------------------------------------------------

**ip a**

<img width="894" height="601" alt="image" src="https://github.com/user-attachments/assets/f14505eb-f3af-4fdc-b913-6a3a7f4974f1" />

The network configuration of the system was examined to identify the active network interfaces and IP address used for network security testing.

----------------------------------------------------------------------------

**sudo lynis audit system**

<img width="829" height="281" alt="image" src="https://github.com/user-attachments/assets/1f48a407-e5ae-4d03-92b2-f4a6e5f1f58a" />


An initial Lynis security audit was performed to analyse the current security configuration and identify vulnerabilities or weaknesses in the system.

----------------------------------------------------------------------------
**Hardening Index**

<img width="405" height="152" alt="image" src="https://github.com/user-attachments/assets/7043e086-1f10-4199-a85a-ccdd997e42de" />

The initial Lynis audit produced a hardening index score representing the current level of system security before remediation.

----------------------------------------------------------------------------
**sudo ufw status**


<img width="896" height="235" alt="image" src="https://github.com/user-attachments/assets/4ad3b5d0-b54c-467e-a09a-82c8184ca75b" />

The firewall status was checked to determine whether the system had active network protection.

--------------------------------------------------------------------------
**sudo ufw allow 22
sudo ufw allow 80
sudo ufw allow 443**


<img width="894" height="204" alt="image" src="https://github.com/user-attachments/assets/beed6fdb-cd75-45b0-b4aa-a83b20f45213" />


**sudo ufw enable
sudo ufw status**

<img width="890" height="389" alt="image" src="https://github.com/user-attachments/assets/00c40ca8-19f0-43f7-8a7f-d81c6d46c3ae" />

The firewall (UFW) was enabled and configured to allow only essential services including SSH (22), HTTP (80), and HTTPS (443), reducing the system attack surface.

----------------------------------------------------------------------------

**Show these lines in the SSH config file.**

<img width="815" height="580" alt="image" src="https://github.com/user-attachments/assets/e9b1b554-265f-4a6d-97e9-45ac5c477893" />


The SSH configuration was hardened by disabling root login and password authentication to reduce the risk of brute force attacks.

----------------------------------------------------------------------------

**Verify SSH Root Login is Blocked**

<img width="882" height="178" alt="image" src="https://github.com/user-attachments/assets/95b990c2-676a-47ef-bd25-62d13da3a6a9" />

SSH root login was tested and successfully blocked, confirming that the security configuration prevents direct root access.

---------------------------------------------------------------------------

**Perform Network Security Scan**

<img width="867" height="281" alt="image" src="https://github.com/user-attachments/assets/5e0dc27d-e906-4c5e-9de2-a1f615ca2e1d" 
  />

An Nmap scan was performed to identify open ports and services running on the system.

---------------------------------------------------------------------------
**Perform Service Detection Scan**

<img width="890" height="96" alt="image" src="https://github.com/user-attachments/assets/f8382ced-fd7e-4b65-bd1f-53a5e59c65f8" />


The Nmap service detection scan identified the services running on each open port, confirming that only necessary services are exposed.

----------------------------------------------------------------------------

**Check Running Services**

<img width="894" height="678" alt="image" src="https://github.com/user-attachments/assets/920c88fd-4235-467a-9e37-76af020bc9a7" />

Running services were reviewed to identify active system services and verify that only required services are running.

---------------------------------------------------------------------------

**Verify User Access Control**

<img width="879" height="51" alt="image" src="https://github.com/user-attachments/assets/f04d3645-5d6f-4b03-ac58-ff0bda43da97" />

User accounts and group memberships were reviewed to verify access control and ensure only authorized users have administrative privileges.

----------------------------------------------------------------------------

**Run Lynis Again (After Fixes)**


<img width="893" height="515" alt="image" src="https://github.com/user-attachments/assets/edd91b1b-4d25-4f43-97c4-940a2aa7bb9a" />




After applying security improvements, the Lynis audit was executed again to measure improvements in the system's security hardening score.

----------------------------------------------------------------------------
**Improved Score**


<img width="868" height="36" alt="image" src="https://github.com/user-attachments/assets/6f6e4718-1216-4ca3-bdff-eabf3b127188" />



The final Lynis hardening index increased after implementing recommended security measures, demonstrating improved system security.

The security audit demonstrated improvements in system hardening through firewall configuration, SSH security enhancements, and service review.

----------------------------------------------------------------------------

