### Week 8 (subnetting 1)
- Module 8: The IP protocol              
- Module 23: IPv4 Address Structure 
- Module 9: IPv4 and Network Segmentation
> Checkpoint Exam: Network Addressing                               



| __IPv4 Segmentation__                      |                                                   |
| ------------------------------------------- | ------------------------------------------------- |
| **Module 08**: The Internet Protocol        | 2.2.4                                             |
| * Octets and Dotted-Decimal Notation        | 2.2.5                                             |
| * Networks and Hosts                        |                                                   |
|                                             |                                                   |
| **Module 23**: IPv4 Address Structure       | 2.2.0 Identify IPv4 addresses and subnet formats. |
| * The Subnet Mask                           | 2.2.1 Subnet concepts                             |
| * Network, Host and Broadcast Addresses     | 2.2.2 Subnet Calculator (37.4.9)                  |
| * Subnet Calculator (37.4.9)                | 2.2.3 Slash notation                              |
|                                             | 2.2.4 Subnet mask                                 |
|                                             | 2.2.5 Broadcast domain                            |
|                                             |                                                   |
| **Module 9**: IPv4 and Network Segmentation | 2.3.0 Identify IPv6 addresses and prefix formats. |
| * Public and Private IPv4 Addresses         | 2.3.1 Types of addresses                          |
| * Types of addresses                        | 2.3.2 Prefix concepts                             |
|                                             |                                                   |
|                                             | 2.3.0 Identify IPv6 addresses and prefix formats. |
|                                             | 2.3.1 Types of addresses                          |
|                                             | 2.3.2 Prefix concepts                             |
|                                             |                                                   |
| __*21-23 Exam: Network Addressing*__        |                                                   |
|                                             |                                                   |





# Comparing the Subnet Mask and Prefix Length
```
| Subnet Mask     | 32-bit Address                      | Prefix Length |
|-----------------|-------------------------------------|---------------|
| 255.0.0.0       | 11111111.00000000.00000000.00000000 | /8            |
| 255.255.0.0     | 11111111.11111111.00000000.00000000 | /16           |
| 255.255.255.0   | 11111111.11111111.11111111.00000000 | /24           |
| 255.255.255.128 | 11111111.11111111.11111111.10000000 | /25           |
| 255.255.255.192 | 11111111.11111111.11111111.11000000 | /26           |
| 255.255.255.224 | 11111111.11111111.11111111.11100000 | /27           |
| 255.255.255.240 | 11111111.11111111.11111111.11110000 | /28           |
| 255.255.255.248 | 11111111.11111111.11111111.11111000 | /29           |
| 255.255.255.252 | 11111111.11111111.11111111.11111100 | /30           |
```

```
4th octect
|                 |     |     |     |     |     |     |     |     |
| --------------: | --: | --: | --: | --: | --: | --: | --: | --: |
|          SALTOS | 128 |  64 |  32 |  16 |   8 |   4 |   2 |   1 |
| Bits encendidos | /25 | /26 | /27 | /28 | /29 | /30 | /31 | /32 |
|         Mascara | 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |
|        Wildcard | 127 |  63 |  31 |  15 |   7 |   3 |   1 |   0 |
```
# IPv4 addresses 

>    Example 
192.168.2.38/24
255.255.255.0

Network address > 192.168.2.0
Broadcast Address > 192.168.2.255
First usable host > 192.168.2.1 (usually Default-gateway)
Last usable host > 192.168.2.254 (usually the SVI (Switch virtual interface))


# Routers Segment Broadcast Domains

* Switches propagate broadcasts out all interfaces except the interface on which it was received. 
* The only device that stops broadcasts is a router.
* Routers do not propagate broadcasts. 
* Each router interface connects to a broadcast domain and broadcasts are only propagated within that specific broadcast domain.
* A problem with a large broadcast domain is that these hosts can generate excessive broadcasts and negatively affect the network.
* The solution is to reduce the size of the network to create smaller broadcast domains in a process called subnetting. 
* Dividing the network address 172.16.0.0 /16 into two subnets of 200 users each: 172.16.0.0 /24 and 172.16.1.0 / 24. 
* Broadcasts are only propagated within the smaller broadcast domains when using subnetting. 

### Example
172.16.0.0 /16 > 
255.255.0.0 mask


|              |                |
| ------------ | -------------- |
| NETID        | 172.16.0.0     |
| broadcast    | 172.16.255.255 |
| 1st usable   | 172.16.0.1     |
| Last usable  | 172.16.255.254 |
| total usable | 65,534         |
|              |                |



```
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1   | 1   | 1   | 0   | 0   | 1   | 0   | 1   |
```


> https://www.calculator.net/ip-subnet-calculator.html



192.168.101.0/24
255.255.255.0

|                 |     |
| --------------- | --- |
| network address |     |
| broadcast       |     |
| 1st usable      |     |
| Last usable     |     |
| usable range    |     |

172.16.0.0/16
255.255.0.0
|                 |     |
| --------------- | --- |
| network address |     |
| broadcast       |     |
| 1st usable      |     |
| Last usable     |     |
| usable range    |     |


10.0.0.0/8
255.0.0.0
|                 |     |
| --------------- | --- |
| network address |     |
| broadcast       |     |
| 1st usable      |     |
| Last usable     |     |
| usable range    |     |


