# Network Security Hands-on Labs

This file documents beginner network security labs performed using Nmap and Wireshark.

--------------------------------------------------

LAB 1 – Network Scanning using Nmap

Objective
Identify active hosts, open ports and running services on a network.

Tool Used
Nmap

Steps Performed

1. Opened terminal in Linux environment.

2. Checked the IP address of the system.

Command used

ip a

or

ifconfig

3. Verified that the target system is reachable.

Command used

ping <target-ip>

4. Performed a basic network scan.

Command

nmap <target-ip>

This scan checks the most common 1000 TCP ports.

5. Performed service version detection.

Command

nmap -sV <target-ip>

This identifies the versions of services running on open ports.

6. Performed operating system detection.

Command

nmap -O <target-ip>

Observations

Open ports discovered included:

22/tcp – SSH  
80/tcp – HTTP  
443/tcp – HTTPS

Service version detection revealed web server and SSH services running on the host.

Learning Outcome

Learned how network scanning tools identify exposed services on a system.  
This technique is commonly used during the reconnaissance phase of security assessments.

--------------------------------------------------

LAB 2 – Packet Analysis using Wireshark

Objective

Capture and analyze network traffic to understand communication between devices.

Tool Used

Wireshark

Steps Performed

1. Opened Wireshark and selected the active network interface (Wi-Fi or Ethernet).

2. Started packet capture.

3. Generated network traffic by opening a web browser and visiting a website.

4. Stopped packet capture after sufficient packets were collected.

5. Applied filters to analyze specific protocols.

Filters used

dns  
http  
tcp

6. Inspected DNS packets to observe domain name resolution.

Example observation

Standard query A example.com

7. Inspected HTTP packets to analyze client-server communication.

Right clicked on packet and selected

Follow → TCP Stream

Observations

Observed DNS requests resolving domain names to IP addresses.

HTTP packets showed GET requests sent from client to server and corresponding responses.

Learning Outcome

Understood how data travels across a network and how packet analysis can help identify suspicious network behavior.
