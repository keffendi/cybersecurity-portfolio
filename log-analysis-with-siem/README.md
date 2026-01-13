## Log Analysis with SIEM
**Platform:** TryHackMe

### Practice Scenario

As a SOC Level 1 Analyst on shift, I received an alert about a suspicious network connection on port 5678 from the host WIN-105. My task was to investigate the activity using Windows logs in the SIEM and determine whether it was suspicious or required escalation.

![WindowsLogs](WindowsLogs.png)

### Questions 1 & 2 – Destination IP and Initiating Process

**Questions:**  
- Which IP address was the connection established with?  
- Which process initiated this suspicious connection?

**Investigation approach:**  
I checked the network logs for port 5678 on WIN-105 to find the destination IP and the process that initiated the connection.

![IPaddress](IPaddressProcess.png)

### Question 3 – MD5 Hash of Malicious Process

**Question:**  
What is the MD5 hash of the malicious process from the previous question?

**Investigation approach:**  
I filtered 'sharepoint.exe' to check for the MD5 hash

![Hashes](Hashes.png)

### Question 4 – Scheduled Task Name

**Question:**  
What is the name of the scheduled task that was created on the system?

**Investigation approach:**  
I looked at the details from the previous event and checked the Windows logs to find the name of the scheduled task.

![Office365](Office365.png)
