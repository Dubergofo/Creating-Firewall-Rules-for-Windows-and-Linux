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
