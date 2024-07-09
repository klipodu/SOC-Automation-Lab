# SOC-Automation-Lab

## Objective
The primary objective of this SOC home lab is to provide oneself with a hands-on experience in setting up, configuring, and operating a Security Operations Center in a simulated environment.
I was inspired by myDFIR found [here](https://www.youtube.com/watch?v=XR3eamn8ydQ&ab_channel=MyDFIR)

### Skills Learned

- Security Monitoring and Threat Detection
- Incident Response
- Security Automation and Orchestration (SOAR)
- Linux Administration
- Understanding of Security Concepts
- Open-Source Technologies
  
### Tools Used

- Wazuh, Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Shuffle, Security Orchestration Automation and Response (SOAR).
- theHive, Case management and Incident reporting
- VirtiualBox

## Overview

<img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SOC-Automation-Project-Wrokflow.png?raw=true" alt="Image Alt">

-----------------------------------------
### Technical Skills
-----------------------------------------

**SIEM & Log Management:** Wazuh provided hands-on experience with Security Information and Event Management (SIEM) tools. <br>
I learned to collect logs, configure alerts, and analyze security events.
<br><br>

**Security Monitoring & Threat Detection:** Through Wazuh, I gained proficiency in identifying suspicious activity and potential threats by analyzing logs and understanding security rules.
<br><br>

**Sysmon Configuration & Endpoint Security:** Sysmon exposed me to endpoint security concepts and the configuration of a popular endpoint monitoring tool.<br>
This allowed me to understand how detailed system activity is captured for threat detection.
<br>

**Linux Administration:** Setting up these tools often involved working with a Linux environment.<br>
I gained experience with package management, system configuration, and basic troubleshooting on Linux.
<br><br>

**Security Automation (SOAR):** Shuffle introduced me to Security Orchestration, Automation, and Response (SOAR) tools.<br>
I learned to automate tasks like enriching alerts and creating incident cases.

-----------------------------------------
### Analytical Skills
-----------------------------------------

**Incident Response:** TheHive taught me the incident response process, including investigating alerts, collecting evidence, containing threats, and taking remediation steps.
<br><br>

**Workflow Optimization:** Integrating Shuffle with Wazuh and TheHive allowed me to understand how to automate incident response workflows, improving efficiency in handling security incidents.
<br><br>

**Problem-Solving & Critical Thinking:** Troubleshooting alerts, identifying root causes of security incidents, and taking corrective actions honed my problem-solving and critical thinking skills.
<br><br>


-----------------------------------------
### Configure the servers and endpoints to communicate to each other
-----------------------------------------

[TheHive]

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Cassandra.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Cassandra.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-ElasticSearch.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-ElasticSearch.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Permissions.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Permissions.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Login.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure-Login.png?raw=true" alt="Image Alt" width="200" height="100">
</a>


[Wazuh]

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Configure-Login.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Configure-Login.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Add-Agent.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Add-Agent.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard-Home.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard-Home.png?raw=true" alt="Image Alt" width="200" height="100">
</a>

<a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard.png?raw=true" alt="Image Alt" width="200" height="100">
</a>



-----------------------------------------
### Genereate Telemetry & Ingest into Wazuh
-----------------------------------------

[Telemetry and Ingest]

<div style="display: flex; justify-content: space-around;">
    4.1 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Sysmon.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Sysmon.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
    4.2 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Ossec.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Ossec.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
    4.3 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Events-Sysmon.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Events-Sysmon.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
    4.4  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Mimikatz.png?raw=true">
           <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Mimikatz.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
</div>
<br>

<div style="display: flex; justify-content: space-around;">
     4.5 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Filebeats.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Filebeats.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
     4.6 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Mimikatz.png?raw=true">
           <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Mimikatz.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
   4.7  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule.png?raw=true">
           <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
   4.8  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule-Trigger.png?raw=true">
            <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule-Trigger.png?raw=true" alt="Image Alt" width="200" height="100">
         </a>
  </div>

-----------------------------------------
### Connect Shuffle (SOAR)
-----------------------------------------

[Shuffle]

<div style="display: flex; justify-content: space-around;">
    5.1 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
    5.2 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-ChangeMe.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-ChangeMe.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
     5.3 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true" alt="Image Alt" width="200" height="100">
        </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
      5.4 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Execution.png?raw=true">
             <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Execution.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
      5.5 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true">
            <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
      5.6 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true">
           <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
      5.7 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Hash.png?raw=true">
             <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Hash.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
      5.8 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Regex.png?raw=true">
           <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Regex.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
      5.9 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal.png?raw=true">
             <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
      5.10 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal-Web.png?raw=true">
              <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal-Web.png?raw=true" alt="Image Alt" width="200" height="100">
          </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
        5.11  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-User-Accounts.png?raw=true">
                <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-User-Accounts.png?raw=true" alt="Image Alt" width="200" height="100">
              </a>
        5.12  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Firewall-Rules-TheHive.png?raw=true">
                <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Firewall-Rules-TheHive.png?raw=true" alt="Image Alt" width="200" height="100">
              </a>
        5.13  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Alert.png?raw=true">
                 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Alert.png?raw=true" alt="Image Alt" width="200" height="100">
              </a>
        5.14  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SquareX-Email.png?raw=true">
                  <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SquareX-Email.png?raw=true" alt="Image Alt" width="200" height="100">
              </a>
</div>
<br>
  5.15 <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Workflow.png?raw=true">
          <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Workflow.png?raw=true" alt="Image Alt" width="200" height="100">
      </a>

