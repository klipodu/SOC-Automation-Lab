# SOC-Automation-Lab

## Objective
The SOC Automation Lab project explores how automation enhances incident response, accelerates threat detection, and streamlines SOC workflows.
Focus is to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. 
This hands-on experience teaches how to setup a SOC envrionment using Wazuh, Shuffle, and theHive.

### Skills Learned

- Home lab using virtualization
- Responsive capabilites
- Case management and reporting
- Automation
- Incident response
  
### Tools Used

- Wazuh, Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Shuffle, Security Orchestration Automation and Response (SOAR).
- theHive, Case management and Incident reporting
- VirtiualBox

## Overview

<img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SOC-Automation-Project-Workflow.png?raw=true" alt="Image Alt" width="741" height="525">

-----------------------------------------
### Install the components to set up in the cloud
- Windows 10 w/Sysmon
- Wazuh Server
- TheHive Server
-----------------------------------------

- [Windows 10 w/Sysmon](https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Install.txt)

  After downloading VirtualBox, check the hash using PowerShell <br>
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Hash-Check.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Hash-Check.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>


  VitrualBox is now setup <br>
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>

- [Wazuh Server](https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Install.txt)

  SSH into Wazuh Server<br>
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-SSH.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-SSH.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>   

  Wazuh Homepage<br>
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard-Home.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Dashboard-Home.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>

  
- [TheHive Server](https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Install.txt)

   SSH into TheHive<br>
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-SSH.png?raw=true">
    <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-SSH.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>

-----------------------------------------
### Configure the servers and endpoints to communicate to each other
-----------------------------------------

[TheHive](https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Configure.txt)

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


[Wazuh](https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Configure.txt)

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

[Telemetry and Ingest](https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry.txt)

<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Sysmon.png?raw=true">
        4.1 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Sysmon.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Ossec.png?raw=true">
        4.2 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Ossec.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Events-Sysmon.png?raw=true">
        4.3 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Events-Sysmon.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Mimikatz.png?raw=true">
        4.4 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/VirtualBox-Windows10-Mimikatz.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
</div>
<br>

<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Filebeats.png?raw=true">
      4.5 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Filebeats.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>
  
   <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Mimikatz.png?raw=true">
    4.6  <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Mimikatz.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>
  
   <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule.png?raw=true">
    4.7  <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>
  
  <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule-Trigger.png?raw=true">
   4.8   <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Wazuh-Telemetry-Custom-Rule-Trigger.png?raw=true" alt="Image Alt" width="200" height="100">
  </a>
</div>

-----------------------------------------
### Connect Shuffle (SOAR)
-----------------------------------------

[Shuffle](https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Configure.txt)

<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true">
        5.1 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-ChangeMe.png?raw=true">
        5.2 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-ChangeMe.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true">
        5.3 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Execution.png?raw=true">
        5.4 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Execution.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true">
        5.5 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true">
        5.6 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-URL.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Hash.png?raw=true">
        5.7 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Webhook-Hash.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Regex.png?raw=true">
        5.8 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Regex.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal.png?raw=true">
        5.9 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal-Web.png?raw=true">
        5.10 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-VirusTotal-Web.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
</div>
<br>
<div style="display: flex; justify-content: space-around;">
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-User-Accounts.png?raw=true">
        5.11 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-User-Accounts.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Firewall-Rules-TheHive.png?raw=true">
        5.12 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/Firewall-Rules-TheHive.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Alert.png?raw=true">
        5.13 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/TheHive-Alert.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
    <a href="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SquareX-Email.png?raw=true">
        5.14 <img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SquareX-Email.png?raw=true" alt="Image Alt" width="200" height="100">
    </a>
</div>
<br>

