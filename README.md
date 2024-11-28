<h1>Dubergofo - Creating Firewall Rules on Windows and Linux</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Hi everyone, welcome to my first cybersecurity tutorial. In this tutorial, we’ll learn about creating and managing firewall rules on both Windows and Linux. Firewalls are a critical part of securing our systems, and knowing how to configure them is a fundamental skill for any IT or cybersecurity professional.
<br />

<h2> Topics covered in this tutorial</h2>


- <b>What Are Firewalls?</b>
- <b>Brief overview of firewall concepts.</b>
- <b>How to create rules on Windows and Linux.</b>
- <b>Testing and validating configurations.</b>

<h2>Environments Used </h2>

- <b>Windows Server 2022</b>
- <b>Kali Linux 2024.1</b> 

<h2>Program walk-through:</h2>

### What Are Firewalls?

A firewall is a network security device or software application designed to monitor and control incoming and outgoing network traffic based on pre-defined security rules. It acts as a barrier between a trusted internal network (e.g., your home or organizational network) and untrusted external networks (e.g., the internet), filtering traffic to block unauthorized access and mitigate cyber threats.

### Type of Firewalls 


- Packet-Filtering Firewalls: Inspect individual packets of data based on rules for source/destination IP, ports, and protocols.
- Stateful Inspection Firewalls: Track the state of active connections to make more informed filtering decisions.
- Proxy Firewalls: Act as intermediaries, filtering traffic at the application layer and hiding the internal network from the outside.
- Next-Generation Firewalls (NGFWs): Combine traditional firewall functions with advanced features like intrusion prevention, application awareness, and threat intelligence.

### Why Firewalls Are Needed?

- Protecting Against Unauthorized Access: Firewalls prevent unauthorized users or malicious actors from accessing sensitive resources on a network by filtering connections based on IP addresses, ports, or protocols.

- Blocking Malicious Traffic: They identify and block malicious traffic, such as malware, phishing attempts, and other exploits, safeguarding the integrity of the network and its devices.

- Enforcing Security Policies: Organizations use firewalls to enforce internal security policies, such as restricting access to certain websites, applications, or services.

- Mitigating Attacks: Firewalls help detect and mitigate various types of cyberattacks, including Distributed Denial of Service (DDoS), Man-in-the-Middle (MITM) attacks, and brute force attempts.

- Segmenting Networks: Firewalls enable network segmentation by isolating sensitive areas (e.g., databases, IoT devices) from less secure zones, reducing the impact of potential breaches.

- Facilitating Monitoring and Logging: Firewalls log traffic data, which is essential for monitoring suspicious activity, conducting audits, and performing forensic analysis after an incident.

### Creating Firewall Rules on Windows

- Step 1: Access Windows Firewall
  - Navigate to Control Panel → System and Security → Windows Defender Firewall → Advanced Settings.
  - Explain the Inbound Rules and Outbound Rules tabs.

- Step 2: Create an Inbound Rule
  -  Example: Allow SSH traffic on port 22.
  -  Steps:
     1. Click Inbound Rules → New Rule.
     2. Select Port and click Next.
     3. Choose TCP or UDP, enter 22, and click Next.
     4. Allow the connection, and click Next.
     5. Specify profiles (Domain, Private, Public) and click Next.
     6. Name the rule (e.g., “Allow SSH”) and click Finish.
 
- Step 3: Test the rule
  - Open a terminal or SSH client and attempt to connect.
  - If blocked, adjust the rule or check the firewall logs for debugging.
 
- Step 4: Modify or delete a Rule
  - Demonstrate how to disable or remove a rule if needed.

### Creating Firewall Rules on Linux

- Step 1: Introduce ufw (Uncomplicated Firewall)
  - Install (if needed): sudo apt install ufw
  - Enable the firewall: sudo ufw enable
 
- Step 2: Allow Traffic on Port 80 (Web Server)
   - Command: sudo ufw allow 80/tcp.
   - Explanation: This allows HTTP traffic to your system.

- Step 3: Block Traffic from a Specific IP Address
  - Command: sudo ufw deny from 192.168.1.100.
  - Explanation: This blocks traffic from a specific malicious IP
 
 - Step 4: Check Active Rules
   - Command: sudo ufw status verbose
   - Verify that the rules are correctly applied.

 - Optional: Use iptables for Advanced Configuration
   - Example:
      - sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT


<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
