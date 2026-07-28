# 123_DHCPv6_theory

# AOM flags (auto, other, managed)

| Automatic  | Other info   | with DHCPv6  |
| ---------- | ------------ | ------------ |
| ____0_____ | ______1_____ | ______0_____ |

```.ios
interface fa0/0
 !automatic is default
 ipv6 nd other-config-flags
 ipv6 nd managed-config-flag
```


## Router Advertisement (RA): 
> Router explain how the host will configue its ipv6 address(Link-local address, GUA)
> It is unique per interface


## Router Solicitation (RS):
> host manda mensaje preguntando quien es el router de la red


### Automatic:

- 1st option = WIN:randomly Generated

- 2nd EUI-64 >> (mac-address-48bits)

0030.F21B.4CB7
FF:FE > en medio del MAC address
2001:DB8:1234:ACAD//:230:F2FF:FE1B:4CB7
        64bit               64bit
0030.F21B.4CB7

|      |      |      |      |
| :--: | :--: | :--: | :--: |
|  0   |  0   |  3   |  0   |
| 0000 | 0000 | 0011 | 0000 | da vuelta al 7mo bit
| 0000 | 0010 | 0011 | 0000 |
|  0   |  2   |  3   |  0   |


| 64bit              | 64bit              |
| ------------------ | ------------------ |
| 2001:DB8:1234:ACAD | 230:F2FF:FE1B:4CB7 |


| Original MAC     | 0030.F21B.4CB7      |
| ---------------- | ------------------- |
| Final 64bit IPV6 | 0230:F2FF:FE1B:4CB7 |


Final full ipv6 address : 2001:DB8:1234:ACAD:230:F2FF:FE1B:4CB7


# Stateless Address Autoconfiguration (SLAAC)


# Stateless >> no se lleva registro
> 1st automatic: EUI-64 Process or Randomly Generated
> 2nd automatic but DHCPv6-server will give more info (ei.DNS)

# Statefull >> lleva registro
> 3rd DHCPv6 server will provide all the info


show ipv6 interface
> host use stateless autoconfig for address

__DAD > Duplicate Address Detection__


### IPV6 NO USA ARP (broadcast) ... USA Neighbor Advertisement(NA) y Neighbor solicitation (NS)

These are two common IPv6 assigned multicast groups:

__ff02::1 All-nodes multicast group__ - This is a multicast group that all IPv6-enabled devices join. A packet sent to this group is received and processed by all IPv6 interfaces on the link or network. This has the same effect as a broadcast address in IPv4. The figure shows an example of communication using the all-nodes multicast address. An IPv6 router sends ICMPv6 RA messages to the all-node multicast group.
__ff02::2 All-routers multicast group__ - This is a multicast group that all IPv6 routers join. A router becomes a member of this group when it is enabled as an IPv6 router with the ipv6 unicast-routing global configuration command. A packet sent to this group is received and processed by all IPv6 routers on the link or network.