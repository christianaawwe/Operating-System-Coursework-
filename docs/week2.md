## Week 2 – Security Planning and Testing Methodology
# Performance Testing Plan

The aim of this performance testing plan is to measure how the Ubuntu Server performs under normal and heavy workloads while being managed remotely from the Ubuntu Desktop workstation using SSH. All monitoring will be carried out using command-line tools to reflect real-world server administration.

#
First, baseline performance will be recorded while the server is idle. This provides a reference point to compare against later tests. The following commands will be used:

#
top to monitor CPU usage and running processes

free -h  to check memory usage

df -h   to view disk usage

uptime to check system load average

ping to measure network connectivity and latency

#
After the baseline has been recorded, workload testing will be performed in later weeks using stress and server applications. During these tests, the same monitoring commands will be run remotely via SSH and the results will be recorded in tables. This approach allows clear comparison between idle and loaded system performance.



#

| Security Control                    | Reason                                 | Risk Reduced          |
| ----------------------------------- | -------------------------------------- | --------------------- |
| SSH Hardening                       | Disable password login and root access | Brute force attacks   |
| Firewall (UFW)                      | Allow SSH only from workstation        | Unauthorised access   |
| Mandatory Access Control (AppArmor) | Restrict application behaviour         | Application exploits  |
| Automatic Updates                   | Install security patches automatically | Known vulnerabilities |
| User Privilege Management           | Use non-root admin users               | Privilege escalation  |
| Network Security                    | Use Host-only network for SSH          | External exposure     |



## Threat Model
Threat 1: SSH Brute Force Attack

Attackers may attempt repeated login attempts to gain access to the server.
Mitigation: Disable password authentication, enable SSH key-based login, and use fail2ban to block repeated failed attempts.

Threat 2: Privilege Escalation

An attacker could attempt to gain root access from a compromised user account.
Mitigation: Disable root login, use sudo access carefully, and apply the principle of least privilege.

Threat 3: Unauthorised Network Access

Open or unnecessary ports could expose the server to attackers.
Mitigation: Enable the UFW firewall, restrict SSH access to the workstation IP, and verify open ports using nmap.




## Week 2 Reflection
This week helped me understand the importance of planning security and performance before making system changes. Creating a security checklist and threat model made it clear how different risks can be reduced using layered security controls. Planning performance testing in advance also ensures results can be measured clearly and compared later. This preparation provides a strong foundation for implementing and evaluating security controls in the following weeks






