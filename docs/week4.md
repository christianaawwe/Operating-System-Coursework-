


## Testing connectivity

<img width="740" height="218" alt="image" src="https://github.com/user-attachments/assets/18839d5f-c3a4-40ee-ad2c-fc554bfe52f4" />

 tests the network connection between the workstation and the server. The ping command is used to confirm that the server is reachable over the network.



## ssh keygen
<img width="761" height="361" alt="image" src="https://github.com/user-attachments/assets/61eb5cab-eba7-488c-869f-439bc060df7d" />
 
 generates a secure SSH key pair on the workstation. The private key stays on the workstation, while the public key is used for authentication.





## To generate key

<img width="858" height="558" alt="image" src="https://github.com/user-attachments/assets/cc14e5e7-21de-437e-a40d-d5521057d886" />

step generates an SSH key pair for secure authentication. The key pair includes a private key, which remains on the workstation, and a public key, which is shared with the server.


## adding key
<img width="833" height="332" alt="image" src="https://github.com/user-attachments/assets/b6ddf6eb-adf1-41c4-91f4-947e95b5a71b" />

This step adds the workstation’s public SSH key to the server. The key is stored in the server’s authorized_keys file to allow secure access. This enables passwordless login and improves overall server security.





## before editung ssh config file
<img width="882" height="721" alt="image" src="https://github.com/user-attachments/assets/ca55cdf2-4019-47e7-9923-4275860e93da" />

Before editing the SSH configuration file, the current SSH connection is verified to ensure access to the server is working. This helps prevent accidental lockout during configuration changes




## after editing ssh config file 

<img width="591" height="118" alt="ssh editing config file " src="https://github.com/user-attachments/assets/7fdaf93f-c4b5-4145-89f1-a736fdd8b856" />
#
<img width="395" height="352" alt="after editing ssh config file 2" src="https://github.com/user-attachments/assets/cfbe6952-0f70-4aa9-9890-594f947806ae" />
After editing the SSH configuration file, the SSH service is restarted to apply the changes. This ensures that the new security settings, such as key-based authentication, take effect.






ssh login without password requirement
#
 <img width="359" height="32" alt="ssh login without pasword" src="https://github.com/user-attachments/assets/dc4ef3ab-89ab-4bd6-ba93-4a525e6e32d8" />

 ssh login with key authentication
















## Enable UFW on the SERVER


<img width="803" height="137" alt="image" src="https://github.com/user-attachments/assets/f323ede8-fbcc-444f-a0ef-a6412d1a1217" />

Once enabled, UFW starts enforcing the configured firewall rules. This provides an additional layer of protection by controlling incoming and outgoing network traffic.







## Allow SSH ONLY from the workstation
<img width="855" height="48" alt="image" src="https://github.com/user-attachments/assets/7cc1f3a2-781f-4aba-a1f3-f3d5ed11b4e0" />
This step configures the firewall to allow SSH access only from the workstation IP address. All other SSH connection attempts are blocked by default. This ensures that remote access to the server is restricted to a single trusted system.







##  Deny everything else

<img width="656" height="88" alt="image" src="https://github.com/user-attachments/assets/6e9c3df6-6320-43b1-adeb-6b24b1db6bb0" />

This step blocks all other incoming network connections to the server. Only explicitly allowed traffic, such as SSH from the trusted workstation, is permitted.









##  allow
<img width="631" height="70" alt="image" src="https://github.com/user-attachments/assets/c929bd47-02f4-4ac1-9ef3-509fcbcf1b24" />

This step allows SSH access to the server from the trusted workstation IP address. The firewall rule ensures that only this specific machine can connect using SSH. This helps secure the server by limiting access to known and trusted sources.








## Check firewall rules

<img width="674" height="243" alt="image" src="https://github.com/user-attachments/assets/cbf925c3-be33-4afa-b76a-eb01747744ac" />
This step checks the current firewall configuration on the server. It confirms that SSH access is only allowed from the trusted workstation IP.



## ANY OTHER IP should not be allowed


<img width="514" height="75" alt="image" src="https://github.com/user-attachments/assets/852de424-7f4d-42a0-8fc7-55ee1a2e5383" />

This step ensures that SSH access is restricted to one trusted workstation only. The firewall is configured to block SSH connections from any other IP address.





## Create a new user server

<img width="787" height="437" alt="image" src="https://github.com/user-attachments/assets/d4e03772-7590-435b-9e63-f7c8d29132c6" />

creates a new user account on the server for administration purposes. The user is created as a standard, non-root account to reduce security risks.






## Give admin

<img width="310" height="14" alt="image" src="https://github.com/user-attachments/assets/82b02e42-40cc-4967-833c-53a128aeafe0" />





<img width="599" height="45" alt="image" src="https://github.com/user-attachments/assets/b13153fb-e098-4d7c-b112-9b55d8fc7b93" />

assigns administrative privileges to the adminuser account. The user is added to the sudo group, allowing them to run administrative commands when required. This avoids direct root login and improves system security.




## Verify sudo access

<img width="241" height="26" alt="image" src="https://github.com/user-attachments/assets/35653cc9-9c5c-4704-8753-54e1dae7a4f4" />
#

<img width="266" height="38" alt="image" src="https://github.com/user-attachments/assets/168bf50b-1dbb-4a2d-867b-e9e3011e0c92" />

verifies that the adminuser account has administrative privileges. The sudo command is used to run an administrative command without logging in as the root user. This confirms that privilege management is correctly configured and follows the principle of least privilege.

## Adminuser login via ssh

<img width="383" height="63" alt="image" src="https://github.com/user-attachments/assets/78366b0d-944b-4843-8661-9b78408964e2" />

 shows logging into the server remotely using the adminuser account over SSH. Using a non-root account improves security and follows best practice. Administrative tasks are only carried out when needed using sudo.

#

##  Remote Administration Evidence via SSH

<img width="368" height="306" alt="image" src="https://github.com/user-attachments/assets/cbbfd741-99d0-4ba9-8f51-3b2ab5a7b32d" />

#

<img width="329" height="129" alt="image" src="https://github.com/user-attachments/assets/f4164c54-72cd-4be7-bbea-76c807099a26" />

##
This command establishes a secure SSH connection using a non-root administrative account. This demonstrates best practice by avoiding direct use of the root account.




