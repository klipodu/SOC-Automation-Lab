# SOC-Automation-Lab

## Objective
The primary objective of this SOC home lab is to provide oneself with a hands-on experience in setting up, configuring, and operating a Security Operations Center in a simulated environment.
I was inspired by myDFIR found [here](https://www.youtube.com/watch?v=XR3eamn8ydQ&ab_channel=MyDFIR)

### Skills Learned

- Home lab using virtualization
- Incident Response Training
- Case management and reporting
- Automation
- Integration Testing
- Threat Intelligence Enrichment
  
### Tools Used

- Wazuh, Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Shuffle, Security Orchestration Automation and Response (SOAR).
- theHive, Case management and Incident reporting
- VirtiualBox

## Overview

<img src="https://github.com/klipodu/SOC-Automation-Lab/blob/main/SOC-Automation-Project-Wrokflow.png?raw=true" alt="Image Alt">

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

[Shuffle](https://github.com/klipodu/SOC-Automation-Lab/blob/main/Shuffle-Configure.txt)

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

