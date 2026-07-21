### Week 13  
- Module 36: Troubleshoot Common Network Problems                               
- Module 37: Network Support           
- Module 18: Network Design   
> Checkpoint Exam: Cisco Devices and Troubleshooting Network Issues
> Module 37: Module Exam

| __16__                                             |                                                                                                                   |
| -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Module 36: Troubleshoot Common Network Problems    | 5.1.0 Demonstrate troubleshooting methodologies                                                                   |
|                                                    | and help desk best practices, ticketing, documentation, and information gathering.                                |
| * Structured Troubleshooting Methods               | 5.1.1 Policies and procedures                                                                                     |
|                                                    | 5.1.2 accurate and complete documentation                                                                         |
|                                                    | 5.1.3 prioritization                                                                                              |
|                                                    |                                                                                                                   |
|                                                    | 3.4.0 Demonstrate how to set up and check network connectivity on Windows, Linux, Mac OS, Android, and Apple iOS. |
| Module 37: Network Support                         | 3.4.1 Networking utilities on Windows, Linux, Android, and Apple operating systems;                               |
| * Cisco Discovery Protocol (CDP)                   | 3.4.2 how to run troubleshooting commands;                                                                        |
| * Packet Capture and Protocol Analysis (Wireshark) | 3.4.3 wireless client settings (SSID, authentication, WPA mode)                                                   |
| * RDP                                              |                                                                                                                   |
| * linux                                            | 5.2.0 Perform a packet capture with Wireshark and save it to a file.                                              |
| * Windows                                          | 5.2.1 Purpose of using a packet analyzer                                                                          |
| * Apple                                            | 5.2.2 saving and opening a .pcap file                                                                             |
|                                                    |                                                                                                                   |
|                                                    | 5.4.0 Differentiate between different ways to access and collect data about network devices.                      |
|                                                    | 5.4.1 Remote access (RDP, SSH, telnet)                                                                            |
|                                                    | 5.4.2 VPN                                                                                                         |
|                                                    | 5.4.3 terminal emulators                                                                                          |
|                                                    | 5.4.4 Console                                                                                                     |
|                                                    | 5.4.5 Network Management Systems                                                                                  |
|                                                    | 5.4.6 cloud-managed network (Meraki) 37.6.5                                                                       |
|                                                    | 5.4.7 scripts                                                                                                     |
|                                                    |                                                                                                                   |
| Module 18: Network Design                          | 4.2.0 Use a network diagram provided by an engineer to attach the appropriate cables.                             |
| * Fault Tolerance                                  | 4.2.1 Patch cables                                                                                                |
| * Scalability                                      | 4.2.2 switches and routers                                                                                        |
| * Quality of Service                               | 4.2.3 small topologies                                                                                            |
| * Hierarchical Network Design                      | 4.2.4 power                                                                                                       |
|                                                    | 4.2.5 rack layout                                                                                                 |


# Troubleshooting Methodologies

## 36.1.3 Gather Information
When a problem is first discovered in the network, it is important to verify it and determine how much of the network is affected by it. After the problem is confirmed, the first step in troubleshooting is to gather information. The following checklist provides some of the important information you should check.

### Nature of problem

- End-user reports
- Problem verification report
- Equipment

* Manufacturer
* Make / model
* Firmware version
* Operating system version
* Ownership / warranty information
* Configuration and Topology

- Physical and logical topology
- Configuration files
- Log files
- Previous Troubleshooting

* Steps taken
* Results achieved

## Troubleshooting with Layered Models

| #   | mnemonic | OSI MODEL    | TCP/IP MODEL | *   | DATA UNIT NAME (PDU) | mnemonic     |
| --- | -------- | ------------ | ------------ | --- | -------------------- | ------------ |
| 7   | aviso    | App          |              | *   |                      |              |
| 6   | previo   | Presentation | App          | *   | Data                 | Dificilmente |
| 5   | sin      | Session      |              | *   |                      |              |
| 4   | trabajan | Transport    | Transport    | *   | Segment              | Salir        |
| 3   | no       | Network      | Network      | *   | Packet               | Parecen      |
| 2   | datos    | Data-link    | Data-link    | *   | Frames               | Flamantes    |
| 1   | pendejos | Physical     | Data-link    | *   | Bits                 | Bijotes      |


* Bottom-Up
* Top-Down
* Divide-and-Conquer
* Follow-the-Path
* Substitution, change cable
* Comparison, other device working?
* Educated Guess




# 36.2.1 Common Layer 1 Problems

* Device power turned off
* Device power unplugged
* Loose network cable connection
* Incorrect cable type
* Faulty network cable
* Faulty wireless access point
* 
* Nothing is plugged into the port.
* There is an issue with the wired or wireless connection.
* A device or port has failed.
* There is a cabling issue.
* The wireless router is improperly configured, for example, a port was administratively shut down.
* The wireless router has a hardware fault.
* The device does not have power.

# 36.3.1 Causes of Wireless Issues

- Not all wireless standards are compatible. 
- Each wireless conversation must occur on a separate, non-overlapping channel. 
- The strength of an RF signal decreases with distance. 
- RF signals are susceptible to interference from outside sources, including other devices functioning on the same frequency. 
- APs share the available bandwidth between devices. 
- Authentication and Association Errors

# 36.4 Common Internet Connectivity Issues

- DHCP Server Configuration Errors
- Check Firewall Settings
- Divide and Conquer with ping
- The tracert Command
- The netstat Command
- The nslookup Command

 # Sources of Help

* Documentation 
* Online FAQs (Frequently Asked Questions) 
* Internet searches 
* Colleagues 
* Last option: ask team lead




 <!-- 2 dias -->

## 37.1 Troubleshooting Process

### 1 Identify the Problem

- Ask direct questions to gather information.
    * Do not use industry jargon.
    * Do not talk down to the customer.
    * Do not insult the customer.
    * Do not accuse the customer of causing the problem.
    * Open-Ended and Closed-Ended Questions
        - WH questions. (when, who, what, how, why)

- Diagnostic tools
    * Beep Codes
    * Event Viewer
    * Device Manager
    * Task Manager

### 2 Establish a Theory of Probable Cause

- List of the most common reasons for the error. 
- If necessary, conduct internal (__Data base__) or external (internet) research based on the symptoms.

### 3 Test the Theory to Determine the Cause

* Testing your theories of probable causes one at a time
* Create a list of possible solutions and implement them one at a time. 
* If you implement a possible solution and it does not correct the problem, reverse the action you just took and then try another solution. 
* Continue this process until you have found the appropriate solution.

### 4 Establish a Plan of Action to Resolve the Problem and Implement the Solution

* Prioritize solutions starting with the easiest and fastest to implement

### 5 Verify Full Functionality and, If Applicable, Implement Preventive Measures

* Verifying full system functionality 
* Ensure that you have not created another problem while repairing the computer. 
* Whenever possible, have the customer verify the solution and system functionality.


### 6 Document Findings, Actions, and Outcomes


 * Explain the problem and the solution to the customer verbally and in writing.
 * Have the customer test the solution and try to reproduce the problem.
 * Include the following information in the documentation:
    > Description of the problem
    > Steps to resolve the problem
    > Components used in the repair
    > Outcome

# 37.2.2 Network Topologies and Descriptions
|       |                             |                                                                      |
| ----- | --------------------------- | -------------------------------------------------------------------- |
| LAN   | Local Area Network          | Pertenece a un solo duen'o, limitado a un area geografica            |
| WAN   | Wide Area Network           | Conjunto de redes de uso colectivo                                   |
| MAN   | Metropolitan Area Network   | A Nivel de ciudad                                                    |
| CAN   | Controller Area Network     | Peer to peer comunication                                            |
| PAN   | Personal Area Network       | Personal (10m o menos)                                              |
| WLAN  | Wireless Local Area Network | Wireless= Pertenece a un solo duen'o                                 |
| VLANs | Virtual LANs                | segment the ports on a single switch as if it were multiple switches |
| WMN   | wireless mesh network       | uses multiple access points to extend the WLAN                       |
| VPN   | virtual private network     | securely connect to another network over an insecure network         |
|       |                             |                                                                      |

# 37.2.6 Wi-Fi the IEEE 802.11 WLAN standards.

# 37.2.9 Network Baseline > Estudio, estadisticas del rendimiento y estado promedio de la Red

# 37.2.10 Cisco Discovery Protocol (CDP) Overview

R1# show cdp neighbors
Capability Codes: R - Router, T - Trans Bridge, B - Source Route Bridge
                  S - Switch, H - Host, I - IGMP, r - Repeater, P - Phone,
                  D - Remote, C - CVTA, M - Two-port Mac Relay
  
Device ID        Local Intrfce     Holdtme    Capability  Platform  Port ID
S1               Gig 0/0/1           179         S I      WS-C3560- Fas 0/5

 <!-- 2do dia -->

# 37.4 Troubleshoot Endpoint Connectivity

* Windows Network Setup
    > in Windows 10, you can access the IP address details from the Network and Sharing Center > interface > Details

ipconfig 
<!-- view the IP addressing information on a Windows host -->

ipconfig /all
<!-- used to view additional addressing details  -->

* Linux Network Setup

ifconfig
<!-- is used to display addresses and their properties. It can also be used to add or delete IP addresses. -->

* MacOS Network Setup
    > In the GUI of a Mac host, open Network Preferences > Advanced to get the IP addressing information,

ifconfig 
<!-- command can also be used to verify the interface IP configuration a shown in the output. -->

*  Setup and Verify Networking in iOS
    > You can also verify the IPv4 and IPv6 addressing information including the default gateway (router) on an Apple IOS device, as shown in the figure. To do so, go to Settings > Wi-Fi > Select the information icon (i) to the right of the active Wi-Fi network name (SSID).


### 37.5.2 Packet Capture and Protocol Analysis (Wireshark)

# Wireshark Comparison Operators:

## Equals: == or "eq"
ip.addr eq 192.168.1.1 
ip.addr == 192.168.1.1 

## And: && or "and"
tcp.port == 22 && ip.addr == 192.168.1.1
tcp.port == 22 and ip.addr == 192.168.1.1

## Or: || (double pipe) or "or"
http.request || http.response
http.request or http.response


# Wireshark Filtering examples

* http.request
    - Display all HTTP requests. 

* http.request || http.response
    - Display all HTTP request and responses. 

* ip.addr == 127.0.0.1
    - Display all IP packets whose source or destination is localhost. 

* tcp.len < 100
    - Display all TCP packets whose data length is less than 100 bytes. 

* http.request.uri matches “(gif)$” 
    - Display all HTTP requests in which the uri ends with “gif”. 

* dns.query.name == “www.google.com” 
    - Display all DNS queries for “www.google.com”.


### 37.5.5 Measuring Network Throughput

> Ejemplo manguera

* Bandwidth: 
    > is the capacity at which a medium can carry data.

* Latency: 
    > Amount of time, including delays, for data to travel from one given point to another

* Throughput: 
    > The measure of the transfer of bits across the media over a given period of time

* Goodput: 
    > The measure of usable data transferred over a given period of time

### 37.6.2 Remote Access with Telnet, SSH, and RDP

* Telnet TCP port 23. >> TERMINAL
* SSH TCP port 22. >> TERMINAL
* Remote Desktop Protocol (RDP) TCP port 3389 >> GUI (GRAFIC USER INTERFACE)


## VPN

* Site-to-Site VPN > conectar dos edificios (redes) de manera segura
* Remote-Access VPNs > conectar usuarios individuales a una red privada

## Network Management Systems


* Simple Network Management Protocol (SNMP)
* Cisco Meraki

## Scripts, Automation, and Programmability

> A scripting language such as Python can be used to create programs that automate network management processes, thus creating management and operational efficiencies while saving on the costs associated with manual network management.

## Review frames 2




