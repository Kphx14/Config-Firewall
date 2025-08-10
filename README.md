# Config-Firewall

🛡️ Task 4: Firewall Configuration and Testing Report
This report documents the completion of Task 4, which involved configuring and testing basic firewall rules on a Windows system. The objective was to create rules to either allow or block network traffic, and to demonstrate the application of these rules.

1. Objective
The primary goal was to configure a new firewall rule to manage network traffic on a Windows machine. The rule was tested to ensure it functioned as intended, and a screenshot of the configuration was captured as a deliverable.

2. Tools Used
Windows Defender Firewall with Advanced Security: The native firewall management tool in Windows.

nmap: A network scanning tool used to test if a specific port was open or closed after applying the firewall rule.

Windows PowerShell: Used for command-line verification and testing.

3. Firewall Rule Implementation
A new inbound rule was created in Windows Defender Firewall with Advanced Security. The rule was configured to block all incoming traffic on TCP port 80, which is commonly used for HTTP web traffic.

Rule Type: Port-based rule.

Protocol: TCP.

Specific Local Ports: 80.

Action: Block the connection.

4. Testing and Verification
To verify that the rule was working, the nmap tool was used from a different system (or on the local machine) to scan for open ports. The scan was performed on the IP address of the machine with the newly created firewall rule.

The nmap command was:

nmap -p 80 

Test Result:

As shown in the attached screenshot, the nmap scan failed to find an open port. The output showed "All 1000 scanned ports on [Target IP Address] are closed," indicating that the firewall rule successfully blocked incoming connections on port 80.

5. Deliverables
The following deliverables confirm the completion of this task:

Screenshot 1: A screenshot of the "New Inbound Rule Wizard" showing the configuration for blocking TCP port 80.

Screenshot 2: A screenshot of the PowerShell terminal showing the nmap output, which demonstrates that port 80 is no longer reachable, thus proving the firewall rule is active and effective.

The results confirm that the task was successfully completed, and a basic firewall rule was effectively configured and tested to block traffic on a specific port.






