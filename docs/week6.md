## In this phase, performance testing was carried out to analyse how the operating system behaves under different workloads. Baseline performance was recorded first, followed by load testing using different applications. CPU, memory, disk, network, and system responsiveness were monitored using command-line tools. The results were analysed to identify bottlenecks, and system optimisations were applied and tested to measure improvements.

------------------------------
## CPU & Memory Stress Tools

<img width="1208" height="380" alt="image" src="https://github.com/user-attachments/assets/187cc756-5751-495d-bf27-d3fb112e7688" />

Used for:

CPU usage testing

Memory pressure testing




## Network Performance Tool
<img width="1221" height="764" alt="image" src="https://github.com/user-attachments/assets/7c361bc4-a653-4b38-88c2-b32bebfd2177" />
Used for:

Network throughput testing

Latency analysis with ping





## uptime
<img width="710" height="54" alt="image" src="https://github.com/user-attachments/assets/8a4770ac-35ee-4478-b1a7-f2c2fee7eb33" />



## Memory usage at rest

<img width="938" height="187" alt="image" src="https://github.com/user-attachments/assets/c5861b47-cd6d-46c1-a2a3-c9771de2b847" />


## Disk usage

<img width="919" height="86" alt="image" src="https://github.com/user-attachments/assets/8d16301d-d212-4ea0-86ad-9ec2072f303e" />


##  System responsiveness

<img width="684" height="162" alt="image" src="https://github.com/user-attachments/assets/3263e937-76e7-453b-86b2-2a36ddecf37a" />




| Metric       | Baseline Value |
| ------------ | -------------- |
| CPU Load     | 0.08 ,0.18   |
| Memory Used  | 412MB     |
| Disk Used    | 3.4g      |
| Load Average | 0.18,0.13,0.08    |



## CPU Load Test

<img width="744" height="186" alt="image" src="https://github.com/user-attachments/assets/68e73dcc-ba43-4180-bd6a-1d6334ce2ca6" />




| Test       | CPU Load (1 min) |
| ---------- | ---------------- |
| Baseline   | 0.18             |
| CPU Stress |0.01      |


<img width="787" height="73" alt="image" src="https://github.com/user-attachments/assets/335f4c78-09a4-4df8-9b14-5a80de349abf" />


#
## running stress vm
<img width="721" height="64" alt="image" src="https://github.com/user-attachments/assets/ad4c87f3-3c46-4359-b465-770c3fd5e5af" />



#

the memory user has gone up significantly and the load average slitly went up
<img width="776" height="309" alt="image" src="https://github.com/user-attachments/assets/ce3ab4bd-1bff-4a6d-b08d-8a268782556a" />




  ##
  
During memory stress testing, memory usage increased from approximately 500 MB at baseline to around 1 GB under load. This shows that the system successfully allocated additional memory when required without instability. The load average increased slightly from 0.18 to 0.28, indicating a small rise in overall system activity, but CPU usage remained relatively low, showing that the workload was primarily memory-intensive rather than CPU-bound.




#
## Disk I/O Test

<img width="671" height="74" alt="image" src="https://github.com/user-attachments/assets/d9cacdd4-04a2-422b-bccd-1bdeb3027ed7" />


| Test     | Disk Write Speed |
| -------- | ---------------- |
| Disk I/O | 390 MB/s    |


#

## ping server ip
<img width="718" height="315" alt="image" src="https://github.com/user-attachments/assets/bb61b614-296d-46b7-b1da-dfb2158f5b84" />

This command was used to measure network latency between the workstation and the server. The output shows the minimum, average, and maximum round-trip time in milliseconds. The average latency value was recorded to evaluate how quickly network packets travel between both systems.

#



## iperf3 -s
<img width="209" height="11" alt="image" src="https://github.com/user-attachments/assets/c6d2ab15-53ec-442b-acb2-993a1b91be61" />

Starting Iperf3 - This command starts the server in listening mode so that it can receive network performance tests. It prepares the server to accept incoming connections from the workstation for throughput measurement. This allows controlled testing of network bandwidth within the isolated environment.
#


## Iperf3 output
<img width="425" height="220" alt="image" src="https://github.com/user-attachments/assets/c9e30a46-b225-45e4-ace4-f45563128912" />

This command was executed on the workstation to test network throughput to the server. It measures how much data can be transferred per second between the two systems. The final throughput value in Mbits/sec was recorded to assess network performance.


#
These commands together provide quantitative measurements of network latency and throughput, which are essential for analysing network performance in a server environment.








