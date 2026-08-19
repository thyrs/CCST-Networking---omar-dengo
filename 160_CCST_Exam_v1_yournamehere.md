



***The Packet Tracer file is only for Section B, Section C and Section D. Please don’t use it in other Sections.***

# Section A - IP addressing (8 PTS)

We have the following network setup topology:
 
All network documentation for the IP scheme was lost, leaving only the following IPS for you to find the network IP of each.
 
*	**San Jose**:
-	10.255.193.129/23
*	**Heredia**:
-	10.255.194.100/23
*	**San Juan**:
-	10.255.196.0/23
*	**Bogota**:
-	10.255.198.255/23
*	**Medellin**:
-	10.255.201.1/23

 
Then assign the IPs addresses as described below:
| Device  | Interface | IP address                        |
| ------- | --------- | --------------------------------- |
| Laptop1 | LAN       | The last usable IP from San Jose  |            
| PC1     | LAN       | The first usable IP from San Juan |            
| Laptop3 | LAN       | The last usable IP from Medellin  |            

2)	What is the IP of PC1? (1 pts)
- [ ] 10.255.199.1
- [ ] 10.255.192.1
- [ ] 10.255.196.1
- [ ] 10.255.197.1

3)	How many IPs does Bogota have in total? (1 pts)
- [ ] 508
- [ ] 514
- [ ] 510
- [ ] 512

4)	How many broadcast domains are in the topology? (1 pts) 
- [ ] 7
- [ ] 5
- [ ] 2
- [ ] 4

5)	What is the broadcast IP of Heredia? (1 pts)
- [ ] 10.255.193.255
- [ ] 10.255.195.255
- [ ] 10.255.194.255
- [ ] 10.255.196.255 
 
6)	What is the network IP for Medellin? (1 pts)
- [ ] 10.255.203.0	
- [ ] 10.255.202.0	
- [ ] 10.255.200.0	
- [ ] 10.255.201.0	

7)	Which of the following is the usable IPs range for Bogota? (1 pts)
- [ ] 10.255.198.1 - 10.255.200.254
- [ ] 10.255.197.1 - 10.255.198.254
- [ ] 10.255.197.1 - 10.255.199.254
- [ ] 10.255.198.1 - 10.255.199.254

8)	Which IP can’t be routed on a public network? (1 pts)
- [ ] 192.168.1.1
- [ ] 193.168.1.1
- [ ] 193.169.1.1
- [ ] 192.169.1.1

9)	If we remove MDE and connect Laptop3 directly to COL, without changing anything else, are we going to have connectivity from Laptop3 to Server0? (1 pts)
- [ ] Yes, we will be able to get connectivity
- [ ] No because it is necessary to get a switch to initiate ARP process
- [ ] No because layer 3 devices do not read layer 2 addresses
- [ ] No because the switch allows us to send the packet from Laptop 3 to COL via the default gateway


# Section B Analysis (6 PTS)

10)	A packet was sent from PC0 to Server0, which of the following options will properly complete the packet when it arrives at interface Gig0/1 on router CR? (2pts)
- [ ] Destination IP address 172.16.20.30 and source IP address 172.16.2.110
- [ ] Source IP address 172.16.2.110 and destination IP address 172.16.5.10
- [ ] Destination IP address 172.16.2.110 and source IP address 172.16.5.10
- [ ] Source IP address 172.16.2.110 and destination IP address 172.16.20.30

11)	A frame was captured:

| L2 address | L2 address | L3 address  | L3 address   | Data |
| ---------- | ---------- | ----------- | ------------ | ---- |
| -          | -          | 172.16.4.55 | 172.16.3.202 |      |

Which of the following options will properly complete the frame above? (2pts)
- [ ] Destination MAC address 0001.973d.7401 and source MAC address 000D.BD5A.0B1C
- [ ] Source MAC address 0001.973d.7403 and destination MAC address 0050.0FB6.03DA
- [ ] Source MAC address 0050.0FB6.03DA and destination MAC address 000D.BD5A.0B1C
- [ ] Destination MAC address 0001.973d.7403 and source MAC address 0050.0FB6.03DA 

12)	A frame going from PC0 to Laptop1 was capture on router PR, which option will properly complete the L2 addresses space? (2pts)

| L2 address | L2 address | L3 address   | L3 address | Data |
| ---------- | ---------- | ------------ | ---------- | ---- |
| -          | -          | 172.16.2.110 | 172.16.1.4 |      |

- [ ] Source MAC address 00E0.A344.07B6 and destination MAC address 0001.96DA.D211
- [ ] Destination MAC address 0060.474a.3602 and source MAC address 00E0.A344.07B6
- [ ] Source MAC address 0060.474a.3601 and destination MAC address 00E0.A344.07B6
- [ ] Destination MAC address 0060.474a.3601 and source MAC address 00E0.A344.07B6

# Section C Short-answer questions (12 PTS)

13)	If a new Router is added between Server0 and router CR and no further changes are performed, will Laptop1 be able to reach Server0? (3 pts)
14)	Currently all end devices have static IP configuration, what will happen if we change Laptop1 from its current position and connect it to MDE? (3 pts)
15)	Will the connection between SJO and CR go down if the auto-MDIX feature is disabled on SJO’s Gig0/1? (3 pts)
16)	What is the destination MAC address of a broadcast frame? (2 pts)
17)	What service can be used so that we don’t have to manually configure every end device’s IP? (1 pt)
 
# Section D Configuration (35 PTS)

19)	Configure PR, CR and BOG with their respective name and secure the access to the privileged mode with an encrypted password 1998 (6 pts)

20)	Secure the access through console for BOG, PR and CR with the password SEC-CON (6 pts)

21)	Configure a legal message for BOG, PR and CR (6 pts)

22)	Configure an SVI for BOG using the host IP 172.16.3.2/24. (2 pts)

23)	Configure PR, CR and BOG to accept SSH connection only and allow only 5 simultaneous sessions. (15 pts)

- Domain: latam.lab
- User: wanderer02
- Password: 0802
- Key size: 1500


---

