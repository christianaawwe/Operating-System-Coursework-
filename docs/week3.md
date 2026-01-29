## Week 3 – Application Selection for Performance Testing
Application Selection Overview

The purpose of this week is to select applications that stress different parts of the operating system. Each application is chosen to test a specific system resource such as CPU, memory, disk, or network performance. This allows clear analysis of how the operating system behaves under different workload types.


| Workload Type      | Application       | Reason for Selection                                      |
| ------------------ | ----------------- | --------------------------------------------------------- |
| CPU-intensive      | stress-ng         | Generates high CPU load to test processor scheduling      |
| Memory-intensive   | stress            | Allocates large amounts of RAM to test memory management  |
| Disk I/O-intensive | dd                | Tests disk read and write performance                     |
| Network-intensive  | iperf3            | Measures network bandwidth and throughput                 |
| Server application | Apache Web Server | Simulates a real server workload handling client requests |


Each application targets a different operating system subsystem, allowing structured performance evaluation.

## Installation Documentation (SSH Only)

All applications were installed on the Ubuntu Server remotely using SSH and the apt package manager.

CPU Stress Tool
sudo apt update
sudo apt install stress-ng
This installs a tool used to generate CPU load.





Memory Stress Tool
sudo apt install stress
This tool is used to allocate memory and test RAM usage.







Disk I/O Testing
sudo apt install coreutils
The dd command is included in core system utilities and is used for disk performance testing.






Network Performance Testing
sudo apt install iperf3
This tool measures network speed between the workstation and server.







Server Application
sudo apt install apache2
Apache is installed to simulate a real server workload.







## Expected Resource Profiles
stress-ng (CPU Test)

Expected to increase CPU usage close to 100% and raise the system load average. This tests how the OS schedules CPU processes.



## stress (Memory Test)

Expected to significantly increase RAM usage and test how the OS handles memory allocation and pressure.



## dd (Disk I/O Test)

Expected to increase disk read and write activity, testing the file system and disk I/O performance.



## iperf3 (Network Test)

Expected to increase network throughput and measure bandwidth between the workstation and server.



## Apache Web Server

Expected to consume moderate CPU and memory while responding to client requests, simulating a real-world server environment.







## Monitoring Strategy

During each test, system performance will be monitored remotely from the workstation using SSH. The following commands will be used:

top = to monitor CPU usage

free -h = to track memory usage

df -h = to  observe disk usage

uptime = to record system load

ping = to check network latency

Results will be recorded before, during, and after each test to allow clear comparison.


## Week 3 Reflection

This week highlighted how different applications place different demands on the operating system. Selecting tools that target specific system resources makes performance testing more structured and meaningful. This preparation will allow clearer analysis and comparison of system behaviour during performance testing in later weeks.






