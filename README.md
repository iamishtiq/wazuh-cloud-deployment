# Wazuh Cloud Deployment – SOC Lab

## Overview
This project demonstrates the deployment of a **Wazuh Cloud SIEM environment**, enrollment of a **Windows endpoint agent**, and validation of **log collection, alert generation, and File Integrity Monitoring (FIM)**.  

The lab was completed as **Task 5 of the WazuGuardix SOC Internship Program**, focusing on real-world **SOC Analyst (L1)** workflows using a cloud-based SIEM platform.

---

## Objectives
- Deploy a Wazuh Cloud environment  
- Enroll and configure a Windows agent  
- Verify agent connectivity and log collection  
- Generate authentication failure alerts  
- Configure and test File Integrity Monitoring (FIM)  
- Validate dashboard visibility and alerting  

---

## Environment & Tools

| Component | Details |
|---------|--------|
| SIEM Platform | Wazuh Cloud |
| Agent OS | Windows 10 (64-bit) |
| Virtualization | Oracle VirtualBox |
| Agent | Wazuh Windows Agent |
| Monitoring | Authentication logs, FIM |
| FIM Path | `C:\Users\Public` |

---

## Lab Walkthrough with Screenshots
### Wazuh Cloud Setup

![Wazuh Official Site](screenshots/fig01_wazuh_site.png)
*Accessing the Wazuh official website to start a free cloud trial.*

![Wazuh Cloud Signup](screenshots/fig02_signup.png)
*Creating a Wazuh Cloud account to deploy the SIEM environment.*

![Account Login](screenshots/fig03_login.png)
*Successful account verification and login into Wazuh Cloud.*

![Cloud Dashboard](screenshots/fig04_dashboard.png)
*Wazuh Cloud main interface after successful login.*

![Environment Creation](screenshots/fig05_environment_creation.png)
*Creating a new cloud environment and selecting the deployment region.*

![Environment Ready](screenshots/fig06_environment_ready.png)
*Wazuh Cloud environment deployed and marked as ready.*

---

### Wazuh Dashboard Access

![Wazuh Login](screenshots/fig07_wazuh_login.png)
*Secure login to access the Wazuh Dashboard.*

![Main Dashboard](screenshots/fig08_main_dashboard.png)
*Wazuh Dashboard providing visibility into agents and security events.*

---

### Agent Deployment & Enrollment

![Deploy Agent](screenshots/fig09_deploy_agent.png)
*Selecting Windows OS and viewing server details for agent deployment.*

![Installation Command](screenshots/fig10_install_command.png)
*Generated PowerShell command containing agent enrollment key.*

![Agent Installation](screenshots/fig11_agent_install_ps.png)
*Installing and starting the Wazuh agent using PowerShell.*

![Agent Active](screenshots/fig12_agent_active.png)
*Windows agent successfully connected and shown as active.*

---

### Log Collection & Alert Testing

![Failed Login Attempt](screenshots/fig13_failed_login.png)
*Simulated failed authentication attempt to generate security events.*

![Authentication Alert](screenshots/fig14_auth_alert.png)
*Authentication failure alert detected in Wazuh Dashboard.*

---

### File Integrity Monitoring (FIM)

![FIM Configuration](screenshots/fig15_fim_config.png)
*Configuring File Integrity Monitoring for the Public directory.*

![Agent Restart](screenshots/fig16_agent_restart.png)
*Restarting the agent to apply FIM configuration changes.*

![FIM Test](screenshots/fig17_fim_test.png)
*Creating files and folders to trigger FIM alerts.*

![FIM Alert](screenshots/fig18_fim_alert.png)
*File integrity alert successfully generated and visualized.*

## Documentation
- **Full Report (PDF):** `documentation/Wazuh_Cloud_Deployment_Report.pdf`
- **Screenshots:** `screenshots/` directory

---

## Key Results
- Wazuh Cloud environment deployed successfully  
- Windows agent enrolled and marked **Active**  
- Authentication failure events detected and logged  
- File Integrity Monitoring alerts generated correctly  
- Real-time SOC visibility confirmed via dashboard  

---

## Skills Demonstrated
- Cloud-based SIEM deployment  
- SOC monitoring and alert analysis  
- Endpoint security monitoring  
- File Integrity Monitoring (FIM)  
- Incident detection and validation  
- Wazuh dashboard operations  

---

## Author
**Ishtiaq Rashid**  
Aspirant SOC Analyst | Cybersecurity Enthusiast  
Pakistan  

---

## Conclusion
This project simulates real-world SOC analyst responsibilities by deploying and operating a cloud-based SIEM platform. It validates hands-on skills in detection, monitoring, and incident analysis using Wazuh Cloud, closely mirroring enterprise SOC operations.
