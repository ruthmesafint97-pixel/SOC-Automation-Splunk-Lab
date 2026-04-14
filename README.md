1. Reconnaissance
   
I used Zenmap to identify the attack surface. 

![Port Scan](01_Recon_Port_Scan.jpg)

![Topology](02_Recon_Network_Topology.jpg)

3. Exploitation
   
Executing a brute-force attack using Hydra on port 8000.

![Hydra Attack](03_Exploit_Hydra_BruteForce.jpg)

5. Detection & Analysis
   
Splunk captured the telemetry and visualized the spike in malicious activity.

![Traffic Spike](04_Detection_Traffic_Spike.jpg)

![Event Distribution](05_Analysis_EventCode_Distribution.jpg)

![Forensics](06_Forensics_Failed_Logins_Raw.jpg)


Challenges Overcome:

Firewall Obstacles: Initially, the Windows host based firewall blocked all incoming traffic from the Kali VM but I successfully resolved this by elevating privileges and using PowerShell as an Administrator to modify the firewall profile.
