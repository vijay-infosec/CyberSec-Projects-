---

## **Screenshots**

### **1. Splunk Forwarder Status**
This screenshot shows the Splunk Universal Forwarder restarting successfully after configuration changes.

![Forwarder Status](screenshots/forwarder_status.png)

---

### **2. inputs.conf Configuration**
This confirms that log monitoring is enabled for `/var/log/auth.log` and assigned to the `linux` index.

![inputs.conf](screenshots/inputs_conf.png)

---

### **3. outputs.conf Configuration**
The forwarder is configured to send logs to the Splunk indexer on port `9997`.

![outputs.conf](screenshots/outputs_conf.png)

---

### **4. Logs Successfully Ingested in Splunk**
Search results for `index=linux` confirm that logs are being received and indexed by Splunk Enterprise.

![Splunk Results](screenshots/splunk_results.png)

---
