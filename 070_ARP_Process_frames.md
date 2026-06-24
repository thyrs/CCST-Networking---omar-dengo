

### Week 7 (frames)
- Module 13: The ARP Process         
- Module 24: Address Resolution      
- Module 29: ICMP
> Checkpoint Exam: Communication Between Networks
> Checkpoint Exam: Configure Cisco Devices


| __Frames__                                 |                                            |
| ------------------------------------------ | ------------------------------------------ |
| **Module 13:**  The ARP Process            | 4.5 CCST Explain basic switching concepts. |
| * ARP                                      | 4.5.1 MAC address tables                   |
|                                            |                                            |
| **Module 24:** Address Resolution          |                                            |
| * ARP Table                                |                                            |
| > *24.1.10 Lab - ARP Traffic in Wireshark* |                                            |
| * frames practice                          |                                            |
|                                            |                                            |
| **Module 29:** ICMP                        | 1.5.9 ICMP                                 |
| * ICMPv4 and ICMPv6 Messages               | 5.3.1 ping                                 |
| * Traceroute                               | 5.3.2 ipconfig/ifconfig/ip                 |
|                                            | 5.3.3 tracert/traceroute                   |



**Module 24:** The ARP Process   

1. Cuanto el paquete es para una red remota, la PC se lo manda a su DGW (Default GateWay)

2. En el viaje, la "IP ADDRESS" __NO CAMBIA__, pero el MAC ADDRESS va cambiando en cada salto(router)


# Module 29: ICMP

```sh
ping 8.8.8.8
# test reachability to "8.8.8.8" 
ping dns.google
# test reachability to "dns.google" 

ipconfig
# check PC's ip configuration (Windows OS)


tracert 8.8.8.8
# test reachability to "8.8.8.8" (Windows OS)
tracert 8.8.8.8
# test reachability to "8.8.8.8" (Linux OS)
tracert dns.google
# test reachability to "dns.google" (Windows OS)

```

### 3 Possible options:
* Host reachability
* Destination or Service Unreachable
* Time exceeded

# 29.2.5 Traceroute - Test the Path