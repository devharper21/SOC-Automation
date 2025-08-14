# SOC Automation

## Objective

Design and implement an automated Security Operations Center (SOC) environment to detect, analyze, and respond to simulated security incidents. The project aimed to integrate multiple cybersecurity tools into a cohesive workflow, reducing manual investigation time and demonstrating the power of Security Orchestration, Automation, and Response (SOAR) in threat management.

### Skills Learned

- EDR configuration, monitoring, and alert handling.
- SOC workflows: detection, triage, investigation, and automated remediation.
- Playbook creation for SOAR-based automated actions.
- Threat intelligence integration using APIs.
- Hands-on experience simulating and analyzing endpoint threats.
- Security tool integration and API-based data exchange.

### Tools Used

- **Vultr** – Endpoint detection, investigation, and live forensics.
- **Wazuh** – SIEM for centralized log collection and alerting.
- **TheHive** – Incident and case management platform.
- **Shuffle** – SOAR platform for automation and enrichment workflows.
- **VirusTotal** – Threat intelligence API for IOC enrichment.

## Steps
1. **Environment Setup**
   - Built a virtual lab using VirtualBox and Ubuntu servers.
   - Installed and configured Vultr as the EDR solution to monitor endpoint activity.
2. **SIEM Integration**
   - Deployed Wazuh Manager on a dedicated server.
   - Configured Velociraptor and endpoint logs to be forwarded to Wazuh for alert generation.
3. **Incident Management Integration**
   - Integrated Wazuh with TheHive via webhook for automatic case creation.
   - Created structured case templates in TheHive for consistent triage.
4. **SOAR Workflow Automation**
   - Used Shuffle to create automated workflows that:
    - Receive alerts from Wazuh.
    - Query VirusTotal for IOC enrichment.
    - Add enrichment results to TheHive cases.
    - Notify via email or Slack of critical incidents.
5. **Attack Simulation & Testing**
   - Conducted simulated endpoint attacks using Metasploit and PowerShell scripts.
   - Validated that:
       - Velociraptor detected malicious activity.
       - Wazuh generated alerts and sent them to TheHive.
       - Shuffle enriched cases with threat intel and automated notifications.
6. **Documentation & Publishing**
   - Documented full setup instructions, configurations, and workflow exports.
   - Uploaded project files, diagrams, and screenshots to GitHub for portfolio showcase.

   
*Ref 1: Network Diagram*

![image](https://github.com/user-attachments/assets/17529d05-8562-4c17-a0ad-480ca0fd7e43)


