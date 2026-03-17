**Update the System**




<img width="1165" height="720" alt="image" src="https://github.com/user-attachments/assets/3505acc3-e822-498a-a2c7-d5a04c267a33" />


The system packages were updated to ensure the server is running the latest security patches before performing the security audit.




--------------------------------------------------------------



<img width="1200" height="691" alt="image" src="https://github.com/user-attachments/assets/755c99a0-e67e-4cdf-b1d9-da27bfa52434" />


Lynis and Nmap were installed. Lynis is used for system security auditing and hardening analysis, while Nmap is used for network security assessment and port scanning.

------------------------------------------------------------------------------


**Display System Information**
**hostnamectl**
<img width="696" height="337" alt="image" src="https://github.com/user-attachments/assets/f3181501-623d-45cf-a4ad-d3e6b372b6f7" />

System information retrieved using the hostnamectl command to identify the operating system, hostname, and system configuration before performing the security audit.

**uname -r**
<img width="490" height="47" alt="image" src="https://github.com/user-attachments/assets/b3f585d0-833b-44a3-a5dc-8da741c6de5e" />

System and kernel information obtained using the hostnamectl and uname -r commands to verify the operating system environment prior to the security audit.



----------------------------------------------------------------------------------------------------------

**ip a output**
<img width="1115" height="514" alt="image" src="https://github.com/user-attachments/assets/e8cf2e30-2bfb-4078-b8c3-69b9afa7fc30" />

The network configuration of the system was examined to identify the active network interfaces and IP address used for network security testing.



-------------------------------------------------------------------------------------------------------------------


**Run the First Lynis Security Audit**

<img width="1054" height="640" alt="image" src="https://github.com/user-attachments/assets/a7d03f98-f768-46f3-ace7-d16f9557cd70" />

<img width="1144" height="672" alt="image" src="https://github.com/user-attachments/assets/69d2f55c-9eca-4b7f-b470-1072cc374c0e" />


An initial Lynis security audit was performed to analyse the current security configuration and identify vulnerabilities or weaknesses in the system.



----------------------------------------------------------------------------------------------------------------------


**Hardening Index**


<img width="505" height="87" alt="image" src="https://github.com/user-attachments/assets/3c04dea8-a683-4a2a-bd7b-cac011c871c3" />


The firewall status was checked to determine whether the system had active network protection.


---------------------------------------------------------------------------------------------------------------



**Enable Firewall and Allow Required Ports**





