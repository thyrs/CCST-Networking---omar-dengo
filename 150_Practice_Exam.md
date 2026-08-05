# 190 practice exam

The Packet Tracer file is only for Section B, Section C and Section D. Please don’t use it in other Sections. (56 pts total)

## Section A ANDing and IP addressing (7 pts)

Your organization has the following network setup:
 
There was a recent change on the network of your organization, which resulted in the loss of all IP addressing documentation leaving behind only some IPs for each network configured.
 
*	Network A:	172.16.70.0/19

*	Network B:	172.16.100.100/21

*	Network C:	172.16.110.254/21

*	Network D:	172.16.116.255/21

*	Network E:	172.16.121.1/21


 

 The IP scheme is described on the table below:

| Device | Interface          | IP Address                   |
| ------ | ------------------ | ---------------------------- |
| LT1-N2 | LAN                | Last usable IP of Network A  |                     
| PC1-N3 | LAN                | First usable IP of network B |                     
| RT-01  | GigabitEthernet0/2 | First Usable IP of network C |                     

2.	How many broadcast domains is SW1-N2 part of?
 
- [ ] A. 3
- [ ] B. 2
- [ ] C. 1
- [ ] D. 9 

 
3.	What is IP of PC0-N1’s default gateway?
 
- [ ] A. 172.16.104.1 
- [ ] B. 172.16.64.1
- [ ] C. 172.16.0.1
- [ ] D. 172.16.80.1
 

4.	What is the IP of LT1-N2?
 
- [ ] A. 172.16.72.254
- [ ] B. 172.16.95.254
- [ ] C. 172.16.7.254
- [ ] D. 172.16.72.255
 

5.	PC1-N3 is connected to Amazon’s server, which is located on the internet, which IP will PC1-N3's packets have while traveling through the public networks?
 
- [ ] A. 172.15.96.1
- [ ] B. 172.16.96.1
- [ ] C. 172.17.96.1
- [ ] D. 172.18.96.1

6.	A technician needs to assign an IP and subnet mask to RT-03’s Gigabit Ethernet0/1 for a point-to-point connection to RT-04, which of the following should the technician use?
 
- [ ] A. Host IP 172.16.128.197 and subnet mask 255.255.255.254
- [ ] B. Host IP172.16.128.196 and subnet mask 255.255.255.252
- [ ] C. Host IP 172.16.128.198 and subnet mask 255.255.255.252
- [ ] D. Host IP 172.16.128.201 and subnet mask 255.255.255.254

 
7.	Which of the following usable host IPs belongs to network E?
 
- [ ] A. 172.16.126.255 /22
- [ ] B. 172.16.127.255 /21
- [ ] C. 172.16.127.254 /22
- [ ] D. 172.16.126.254 /21
 
 
# Section B Analysis (4 pts)
From the frames below answer a set of questions

L2 address	L2 address	L3 address	L3 address	Data
0030.a396.7001	00e0.8f12.6e02	?	?	
8.	Which of the following options will properly complete the frame above?

- [ ] A. Source 10.16.3.124 Destination 10.16.3.155
- [ ] B. Destination 10.16.3.123 Source 10.16.3.155
- [ ] C. Source 10.16.3.155 Destination 10.16.3.124
- [ ] D. Destination 10.16.3.155 Source 10.16.3.123


9.	A packet going from PC0-N1 to Server0 was captured on RT-01, which option will properly complete the Layer 2 addresses space?
L2 address	L2 address	L3 address	L3 address	Data
?	?	10.16.3.65	10.16.3.1	

- [ ] A. Source MAC address 000c.852c.0201 and destination MAC address 00e0.8f12.6e01
- [ ] B. Destination MAC address 00e0.8f12.6e01 and source MAC address 000c.852c.0201
- [ ] C. Source MAC address 000c.852c.0203 and destination MAC address 0001.969B.8853
- [ ] D. Destination MAC address 00e0.8f12.6e03 and source MAC address 000c.852c.0203 
 
# Section C Short-answer questions (18 pts)

10.	Why would an interface be on a “Administratively down” status? (2 pts)
R/

11.	PC1-N3 pinged Server0 and received a 100% success rate, does this mean that Server0's MAC address will be on PC1-N3's ARP table? (3 pts)
R/

12.	Will communication be possible from LT2-N4 to other networks if a new switch is added between RT-04 and SW3-N4 and no further changes are performed? (3 pts)
R/

13.	If RT-03 is removed and instead we directly connect RT-04 to RT-00 and no further changes are performed, will LT2-N4 and PC0-N1 still be able to communicate with Server0? (3 pts)
R/

14.	Which command should be used to display the ARP cache on a PC? (2  pts)
R/


15.	A technichian performed the following changes:
!- [Alt text](159_image.png)
 
When accessing the switch through Telnet, which password should be used?	(2 pts)
R/

16.	SW1-N2 received a frame containing the destination MAC address 00D0.582B.B8E8, and we captured the following information from the switch:
 
!- [Alt text](159_image-1.png)

What will SW1-N2 do with the frame? (3 pts)
R/ 


##  Section D
Configuration (27 pts)

17.	Configure the intermediary devices mentioned below with their respective name and secure the access to the privileged mode with the password cisco123 (6 pts)

18.	Secure the console access with the password class123 (3 pts)

19.	Configure __RT-00__ and __SW3-N4__ to accept SSH connections only , __SW0-N1__ should accept telnet connections only. (15 pts)

* Domain: NET.org
* User: Administrator
* Password: ADMIN08
* Key size: 1200

20.	Configure a legal message for the devices mentioned above. (3 pts)



Responses: https://forms.office.com/r/T2jjCRPiWT
