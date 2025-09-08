# Splunk SIEM Lab – Windows Event Log Monitoring

## Overview
This project demonstrates hands-on experience with Splunk Enterprise for Security Information and Event Management (SIEM).  
The goal was to implent Windows Event Logs, create security-focused dashboards, configure alerts, and implement SOC analyst workflows to enhance the security operations of the organization.

## Data Sources
- **Windows Event Logs** from a forwarder:
  - Security
  - System
  - Application

## Key Features
- **Dashboards**  
  - Authentication activity (Event ID 4624 – logon, 4625 – failed logon)  
  - Privilege escalation (4672, 4717)  
  - Credential use (4648, 4798, 4799)  
  - Kerberos / cryptographic events (5058, 5059, 5061, 5379, 5382)  
  - System changes (4616 – time change, 4732 – group membership)
  
- **Alerts**  
  - Real-time and scheduled alerts for suspicious activity (e.g., failed logon spikes, time changes, privilege use).
 
- **Drilldowns**  
  - Click-through on panels to pivot into raw event data for deeper investigation.
  
- **Visualizations**  
  - Bar charts, line graphs, pie charts with custom colors.  

### Search Queries (SPL)
- Example query to detect failed logon attempts (EventCode 4625).  
![SPL Query](screenshots/spl_query.jpg)

### Dashboards

- Event Counts (all Windows logs)  
![Event Counts](eventcounts.jpg)

- Failed Logons by User  
![Failed Logons](logonattempts.jpg)

- Privileged Logons (EventCode 4672)  
![Privileged Logons](explicitcredentials.jpg)


### Alerts
- Configured real-time alert for failed logons (EventCode 4625).  
![Alert Setup](screenshots/alert_setup.png)
 

## Learning Outcomes
- Built a SIEM workflow from scratch.  
- Implemented detection and alerting on Windows security events.  
- Developed dashboards for SOC analyst monitoring.  
- Proven hands-on experience with Splunk search (SPL), alerting, and dashboard customization.  

---

### Author
Olusegun Soares – Cybersecurity Enthusiast  
[LinkedIn Profile](#) | [GitHub Profile](#)
