# **Linux Log Forwarding to Splunk**

This mini-project demonstrates how to forward Linux system logs to Splunk Enterprise using the Splunk Universal Forwarder.  
It includes installation, configuration, and verification using SPL queries.

---

## **Project Overview**

The goal is to send Linux system logs (such as `/var/log/auth.log`) to a Splunk Enterprise instance for monitoring and analysis.

This includes:

- Installing the Splunk Universal Forwarder  
- Configuring inputs (log sources)  
- Configuring outputs (Splunk receiver)  
- Verifying ingestion in Splunk with SPL  

---

## **Repository Structure**

Splunk-Log-Forwarding/
│
├── screenshots/
│ ├── forwarder_status.png
│ ├── inputs_conf.png
│ ├── outputs_conf.png
│ └── splunk_results.png
│
├── Configuring_Linux_to_Forward_Logs_to_Splunk.pdf
│
└── README.md


---

## **Steps Performed**

### **1. Linux Setup**
- Installed Ubuntu Server in a virtual machine  
- Enabled SSH  
- Configured UFW firewall rules
  
---

### **2. Install Splunk Universal Forwarder**

Example commands:

```bash
dpkg -i splunkforwarder.deb
/opt/splunkforwarder/bin/splunk start --accept-license

Enable Forwarder on boot:
/opt/splunkforwarder/bin/splunk enable boot-start

3. Configure Log Forwarding
inputs.conf
[monitor:///var/log/auth.log]
index = linux
sourcetype = linux:auth

outputs.conf
[tcpout]
defaultGroup = default-autolb-group

[tcpout:default-autolb-group]
server = <Splunk_Server_IP>:9997


[tcpout:default-autolb-group]
server = <Splunk_Server_IP>:9997

Restart the forwarder:
/opt/splunkforwarder/bin/splunk restart

4. Verify Logs in Splunk

Example SPL queries:
index=linux
index=* 
| dedup host source sourcetype 
| table host source sourcetype
If events appear, the forwarder is configured correctly.

---

Notes

This is a small SIEM onboarding lab meant to demonstrate basic Splunk data forwarding.
It provides practical experience with:

Splunk Universal Forwarder

inputs.conf and outputs.conf

Log ingestion pipeline

Basic SPL querying
