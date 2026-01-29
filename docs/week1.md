## Week 1 - System Planning and Distribution Selection

#
# System Architecture Diagram 

<img width="466" height="151" alt="image" src="https://github.com/user-attachments/assets/3ab3a44d-be46-4e43-a659-a493a09d52e1" />

This architecture represents a dual-system setup where the Ubuntu Desktop virtual machine acts as the workstation used to remotely manage the Ubuntu Server virtual machine. The server runs in headless mode without a graphical interface and is administered securely over the network using SSH from the workstation.

----------------------------------------------------------------------------------------------------------------------



# Distribution Selection Justification comparing your chosen server distribution with alternatives?
Ubuntu Server 24.04 LTS was selected because it is stable, secure, and supported with long-term updates, making it suitable for a server environment. It provides regular security patches and includes built-in security features such as AppArmor. Compared to Debian, Ubuntu offers more up-to-date packages and easier access to documentation and community support, which is helpful for learning and troubleshooting. When compared to CentOS, Ubuntu has more predictable long-term support and is widely used in cloud and enterprise environments. Overall, Ubuntu Server offers a strong balance of stability, security, and ease of use.


   





# Workstation configuration decision justifying your choice of workstation option?
I chose an Ubuntu Desktop virtual machine as my workstation because it provides a full Linux environment with built-in SSH support and command-line tools needed to manage the server remotely. Using a separate desktop VM keeps the workstation isolated from the host machine, improving security and making the setup easier to control and replicate. It also reflects real-world practice, where administrators manage headless servers from dedicated systems. Although running an additional VM uses more resources, it provides better consistency, organisation, and a more professional setup for remote system administration.







#  adapter 1 and 2
adapter 1
<img width="1193" height="783" alt="image" src="https://github.com/user-attachments/assets/88c818da-9007-4481-9bc0-6124f3a4a52c" />

adapter 2
<img width="1161" height="787" alt="image" src="https://github.com/user-attachments/assets/4a3e4ceb-241f-489b-96b3-2d0c328b6d99" />

 Both virtual machines are configured with two network adapters: NAT and Host-only. The NAT adapter provides internet access so the systems can install updates and required packages, while the Host-only adapter creates a private internal network that allows secure SSH communication between the workstation and the server.



uname -a

<img width="1144" height="93" alt="image" src="https://github.com/user-attachments/assets/a7f43dcd-4977-4b0e-87d4-068a39a8334e" />




lsb_release -a
<img width="488" height="148" alt="image" src="https://github.com/user-attachments/assets/848696b4-8a15-4943-a328-98a7e1a1bde2" />


free -h
<img width="774" height="125" alt="image" src="https://github.com/user-attachments/assets/a4204538-feca-4488-8205-141866373de8" />



df -h
<img width="502" height="140" alt="image" src="https://github.com/user-attachments/assets/f3a79a4c-2b9d-4f87-b18c-dca9ffbeaef2" />





ip addr
<img width="531" height="254" alt="image" src="https://github.com/user-attachments/assets/f916cef3-53b7-4ee9-be9b-110ee344741c" />


The system now displays both a NAT IP address for internet access and a Host-only IP address for internal communication with the workstation. This confirms that the network configuration is working properly and both virtual machines can communicate within the isolated environment.














 
