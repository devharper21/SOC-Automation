# SOC Automation

## Objective

Design and implement an automated Security Operations Center (SOC) environment to detect, analyze, and respond to simulated security incidents. The project aimed to integrate multiple cybersecurity tools into a cohesive workflow, reducing manual investigation time and demonstrating the power of Security Orchestration, Automation, and Response (SOAR) in threat management.

### Skills Learned

- SOC workflows: alert triage, incident correlation, and response automation.
- Log ingestion, parsing, and security event correlation.
- Creating automated playbooks for incident investigation.
- Integrating SIEM, SOAR, and case management systems.
- Threat intelligence enrichment and API integration.
- Hands-on experience with alert lifecycle management.

### Tools Used

- **Wazuh:** SIEM platform for log management and threat detection, as demonstrated in the series.
- **TheHive:** Incident response platform for managing and tracking security incidents.
- **Shuffle:** Workflow automation tool for orchestrating and connecting various security tools.

## Steps
1. **Environment Setup**
   - Built a virtual lab using VirtualBox and Ubuntu servers.
   - Installed and configured Wazuh Manager and Wazuh agents on test endpoints.
2. **Log Collection & Detection**
   - Ingested logs from multiple sources (Windows event logs, Linux syslogs, and simulated attack traffic).
   - Configured Wazuh rules to detect suspicious activities such as brute-force attempts, malware signatures, and privilege escalations.
3. **Incident Management Integration**
   - Connected Wazuh alerts to TheHive via webhook/API for automated case creation.
   - Mapped alert fields to incident fields in TheHive for structured triage.
4. **Automation & Playbook Design**
   - Used Shuffle to create automated workflows that:
    - Parse Wazuh alerts.
    - Query external threat intelligence sources (VirusTotal, AbuseIPDB, etc.).
    - Enrich incident cases in TheHive with IOC context.
    - Automatically assign cases to analysts.
5. **Testing & Validation**
   - Simulated attacks using tools like Kali Linux and Metasploit.
   - Verified alerts triggered in Wazuh, cases created in TheHive, and enrichment executed via Shuffle.
6. **Documentation & GitHub Publishing**
   - Created step-by-step project documentation, diagrams, and screenshots.
   - Uploaded configuration files, playbooks, and workflow exports to GitHub for portfolio demonstration.

   
*Ref 1: Network Diagram*

![image](https://github.com/user-attachments/assets/17529d05-8562-4c17-a0ad-480ca0fd7e43)


