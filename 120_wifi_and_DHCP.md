### Week 12  
- Module 03: Wireless and Mobile Networks
- Module 04: Build a Home Network    
- Module 11: Dynamic Addressing with DHCP

> Checkpoint Exam: Build a Small Network
> Checkpoint Exam: The Internet Protocol
> Checkpoint Exam: ARP, DNS, DHCP and the Transport Layer

| __DHCP & ICMP__                                        |                            |
| ------------------------------------------------------ | -------------------------- |
| Module 03: Wireless and Mobile Networks      (lectura) | 3.2.0                      |
|                                                        | 3.2.1                      |
|                                                        | 3.2.2                      |
|                                                        | 3.2.3                      |
|                                                        | 3.2.4                      |
|                                                        |                            |
| Module 04: Build a Home Network                        | 6.3.0                      |
| * SSID                                                 | 6.3.1                      |
| * "Ethernet-LAN ports" vs "internet-WAN ports"         | 6.3.2                      |
| > __*4.4.4 PT - Configure a Wireless Router*__         | 6.3.3                      |
| * MAC address filtering                                | 4.5.2                      |
|                                                        |                            |
| Module 11: Dynamic Addressing with DHCP                | 1.5.7 DHCP                 |
| * Static vs Dynamic Address Assignment                 |                            |
| > __*11.2.3 PT - DHCP on a Wireless Router*__          |                            |
|                                                        |                            |
| Module 29: ICMP                                        | 1.5.9 ICMP                 |
| * ICMPv4 and ICMPv6 Messages                           | 5.3.1 ping                 |
| * Traceroute                                           | 5.3.2 ipconfig/ifconfig/ip |
|                                                        | 5.3.3 tracert/traceroute   |
|                                                        |                            |



# Static IPv4 Address Assignment

- __How to change IP address in Win10__: Settings > Network & Internet > change adapter option > right click in the NIC > 

* __IP address__ - This identifies the host on the network.
* __Subnet mask__ - This is used to identify the network on which the host is connected.
* __Default gateway__ - This identifies the networking device that the host uses to access the internet or another remote network.


# DHCP Servers:
```
┌───────┐                       ┌────────┐
│ My PC │          ┌──┬─────────┤  DHCP  │
└───────┴──────────┤SW│         │ SERVER │
                   └──┘         └────────┘
```
* Steps to Obtain a Lease

- DHCP Discover (DHCPDISCOVER) CLIENT
- DHCP Offer (DHCPOFFER) SERVER
- DHCP Request (DHCPREQUEST) CLIENT
- DHCP Acknowledgment (DHCPACK) SERVER

(port UDP numbers 67 server 68 client)


## APIPA (Automatic provisioning of IP Address)

* When DHCP fails: Link-local is assinged
* APIPA is (169.254.0.1 to 169.254.255.254) having 65,534 usable IP addresses, with the subnet mask of 255.255.0.0.
* An ip address is always used so PCs on same broadcast domain can comunicate 

# Configure DHCP on a Wireless Router

__DHCP internal server (GUI):__
    - Setup > Basic setup > DHCP server Settings

# ICMP

Host reachability
Destination or Service Unreachable
Time exceeded


# 29.2.5 Traceroute - Test the Path