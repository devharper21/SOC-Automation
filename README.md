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

   
*Ref 1: Project Playbook*
<img width="1033" height="831" alt="0" src="https://github.com/user-attachments/assets/26d64653-43d5-47d9-b27b-871237ab4b70" />

*Ref 2: Installing LimaCharlie on Windows Server*
<img width="1918" height="529" alt="unnamed" src="https://github.com/user-attachments/assets/2bc22bda-d264-4de6-a312-43087e2d46bb" />

*Ref 3: Confirmation of Installation and successful event logs*
<img width="1918" height="820" alt="unnamed" src="https://github.com/user-attachments/assets/084a667a-3967-48de-98b9-64d54cb13cb2" />
<img width="1915" height="814" alt="unnamed" src="https://github.com/user-attachments/assets/2f69a0ec-9642-4094-a319-63653c5daf7c" />

*Ref 4: Confirmation of LaZagne.exe was ran in PowerShell and stated creating a detection rule*
<img width="1918" height="819" alt="unnamed" src="https://github.com/user-attachments/assets/3cf40855-66c6-467d-aad1-8a57fbc4ae45" />
<img width="1794" height="675" alt="unnamed" src="https://github.com/user-attachments/assets/227c4844-9fb3-4ef5-aece-0593c402a9f1" />
<img width="1771" height="451" alt="unnamed" src="https://github.com/user-attachments/assets/73ab36fc-3d96-43e8-b0ad-87b6318d92ed" />

*Ref 5: Testing to confirm if the newly created rules were successful by copying an event from the Timeline section in LimaCharlie and pasting it in the Target Event section*
<img width="1390" height="669" alt="unnamed" src="https://github.com/user-attachments/assets/f0a7a9e3-43e5-49d9-bc8b-2753c3a35d39" />
<img width="1416" height="412" alt="unnamed" src="https://github.com/user-attachments/assets/0e4b37db-2b83-4db3-a00b-058fe5a59f48" />

*Ref 6: Ran the LaZagne.exe installation again to see if the rule detects it and was successful*
<img width="1489" height="568" alt="unnamed" src="https://github.com/user-attachments/assets/941d9fba-74b7-4913-a10b-50f00600cd3d" />
<img width="1918" height="697" alt="unnamed" src="https://github.com/user-attachments/assets/1a24fe75-3fe0-4b27-b730-375e494f97fa" />

*Ref 7: Created a Slack server so the alerts from LimaChart will flow into the alerts channel*
<img width="1918" height="823" alt="unnamed" src="https://github.com/user-attachments/assets/12033fbf-f65b-4e7e-8ce5-2f465cc6e7db" />

*Ref 8: Created a storyboard on Tines connecting each aspect of my playbook*
<img width="872" height="911" alt="0" src="https://github.com/user-attachments/assets/66fb0525-453d-4fc5-97d7-4c9744fb3a52" />

*Ref 8a: User Prompt page*
<img width="979" height="748" alt="unnamed" src="https://github.com/user-attachments/assets/4a24b724-9324-414b-85f0-c0b1b56d3693" />

*Ref 8b: Confirmation of isolating the Windows Server and Slack notification if the user selects "Yes" on the User Prompt*
<img width="1915" height="820" alt="unnamed" src="https://github.com/user-attachments/assets/604c808a-4f1c-4971-bd7a-37369bdf040b" />
<img width="1923" height="825" alt="unnamed" src="https://github.com/user-attachments/assets/c19b4515-7b87-4f56-8fc3-c2e4b0c4745b" />

*Ref 8c: Confirmation of isolating the Windows Server and Slack notification if the user selects "No" on the User Prompt*
<img width="1918" height="826" alt="unnamed" src="https://github.com/user-attachments/assets/4e7b1086-b8e0-45e7-8b3e-ed002bfad10b" />












