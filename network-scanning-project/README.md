# Basic Network Scanning Using Nmap

## Objective
Identify open ports and services running on a target system.

## Tools Used
Nmap
Linux Bash

## Steps Performed

1. Identified target IP in local network
2. Performed basic scan

nmap <target-ip>

3. Performed service version detection

nmap -sV <target-ip>

4. Performed OS detection

nmap -O <target-ip>

## Results

Open ports discovered:

22 - SSH  
80 - HTTP  
443 - HTTPS  

## Learning Outcome

Understood how attackers and security analysts discover services running on a network host.
