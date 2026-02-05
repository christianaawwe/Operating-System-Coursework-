


## Verify AppArmor Is Installed and Enabled






<img width="674" height="154" alt="image" src="https://github.com/user-attachments/assets/0cd3f9f9-3e21-44e4-bd3a-97ec85007bcc" />



This confirms AppArmor is active on the system.






## Check Which Profiles Are Enforced








<img width="592" height="435" alt="image" src="https://github.com/user-attachments/assets/dab2f064-f27e-4804-8c0f-4751bdc9c2b2" />







## Report Access Control Status




<img width="738" height="312" alt="image" src="https://github.com/user-attachments/assets/a088864c-ca57-4134-9b35-ae836b8e40c1" />



This shows which applications are being restricted by AppArmor.



## Show Access Control Tracking (Logs)




<img width="1202" height="269" alt="image" src="https://github.com/user-attachments/assets/1dedbb72-8762-47a2-be25-0d949925be3e" />

This proves that AppArmor events are being logged and tracked.





------------------

## Configure Automatic Security Updates:
Install automatic updates package


<img width="963" height="571" alt="image" src="https://github.com/user-attachments/assets/625497e5-3250-4259-a256-3dae5429af8b" />
This installs the tool used to apply security updates automatically.






## Enable automatic security updates


<img width="1218" height="744" alt="image" src="https://github.com/user-attachments/assets/c2cddc0f-a38a-4dec-98d4-06e3e04197b8" />
This enables automatic installation of security updates.






##    Verify automatic updates configuration


<img width="734" height="71" alt="image" src="https://github.com/user-attachments/assets/b0d8ca12-745a-4fa1-a6c9-aee36bb47a20" />

confirms that automatic security updates are enabled.




## Show update activity log


<img width="1215" height="643" alt="image" src="https://github.com/user-attachments/assets/106206e5-f74f-4f7f-9e3f-c17a63222c28" />



This proves that automatic updates are active and being logged.


 The configuration file confirms that updates are enabled, and log files provide evidence that update activity is being recorded. This ensures the server receives security patches automatically.



--------------------------------------------
## Fail2Ban

Fail2Ban is installed
<img width="697" height="230" alt="image" src="https://github.com/user-attachments/assets/8dd86906-f715-4840-a14d-4e45c5c2acfd" />





## Fail2Ban is running and monitoring SSH


<img width="832" height="122" alt="image" src="https://github.com/user-attachments/assets/48597653-caf5-47c3-b716-ce96617bc1f9" />
--------------------------------     











-----------------------------------------------
## Create a remote monitoring script (`monitor-server.sh`) that runs on your workstation,connects via SSH, and collects performance metrics from the server.


<img width="580" height="27" alt="image" src="https://github.com/user-attachments/assets/cd6154f1-940e-405d-86bf-fdfbd658c79f" />


this tells you the file status and changes made to the file.




creating security baseline
<img width="1219" height="660" alt="image" src="https://github.com/user-attachments/assets/149e5b21-b31e-4f59-b17a-7fcfd841403d" />




## running security baseline and showing output
<img width="859" height="733" alt="image" src="https://github.com/user-attachments/assets/db68fab1-6f8d-4410-ae6d-33ffce282f5b" />





## shows it running and its status

<img width="1090" height="642" alt="image" src="https://github.com/user-attachments/assets/0f584d7c-74c3-4234-9a35-1df2c8c12ecb" />




------------------------------------------------
## Create a remote monitoring script (`monitor-server.sh`) that runs on your workstation,connects via SSH, and collects performance metrics from the server.


<img width="676" height="29" alt="image" src="https://github.com/user-attachments/assets/2ef90b27-42eb-441f-bef8-3e90240bc3da" />

making moneterig script




## inside the script
<img width="785" height="303" alt="image" src="https://github.com/user-attachments/assets/ab4c5eea-a031-4ea3-bf0b-975a28d2e7e5" />


## output
<img width="897" height="572" alt="image" src="https://github.com/user-attachments/assets/5419793a-ad32-4da5-88a9-bc492a719c76" />



# Week 5 Reflection

In Week 5, I focused on improving the security and monitoring capabilities of the server. I configured automatic security updates to ensure the system receives important patches without manual intervention, which reduces the risk of vulnerabilities over time. I also implemented Fail2Ban to detect and block repeated unauthorised login attempts, adding an extra layer of protection against brute-force attacks.

Creating security and monitoring scripts helped me understand how security controls can be verified and monitored efficiently using automation. This week highlighted the importance of continuous security management rather than one-time configuration. Overall, these tasks improved my confidence in managing and securing a Linux server in a professional and practical way.

