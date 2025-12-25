# Screenshots

This folder contains visual evidence of the Splunk Universal Forwarder configuration and log ingestion process.

## Files Included

### **1. forwarder_status.png**
Shows the Splunk Universal Forwarder restarting successfully using:
```
/opt/splunkforwarder/bin/splunk restart
```
Indicates that the forwarder is installed and running without errors.

---

### **2. inputs_conf.png**
Displays the contents of:
```
/opt/splunkforwarder/etc/system/local/inputs.conf
```
Confirms that `/var/log/auth.log` is being monitored and forwarded to the `linux` index.

---

### **3. outputs_conf.png**
Shows the configuration in:
```
/opt/splunkforwarder/etc/system/local/outputs.conf
```
Verifies that the forwarder is sending logs to the Splunk indexer on port `9997`.

---

### **4. splunk_results.png**
Screenshot of Splunk Search UI with:
```
index=linux
```
Confirms that logs from the Linux server have successfully arrived and are being indexed.

---

These screenshots support the main project and validate that log forwarding works end-to-end.

