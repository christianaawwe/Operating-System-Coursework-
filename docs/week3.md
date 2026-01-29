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



Installation Documentation (SSH Only)

All applications were installed on the Ubuntu Server remotely using SSH and the apt package manager.

CPU Stress Tool
sudo apt update
sudo apt install stress-ng
This installs a tool used to generate CPU load.














