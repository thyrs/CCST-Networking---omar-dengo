# 036 Verduras Homework 

cree un nuevo packet tracer y arme este topology:

## Addressing table

| Device    | Interface | IP              | Subnet Mask   |
| --------- | --------- | --------------- | ------------- |
| Zanahoria | vlan 1    | 192.168.253.253 | 255.255.255.0 |
| Apio      |           | 192.168.253.10  | 255.255.255.0 |
| Lechuga   |           | 192.168.253.20  | 255.255.255.0 |
| Tomate    | vlan 1    | 192.168.253.254 | 255.255.255.0 |
| Pepino    |           | 192.168.253.30  | 255.255.255.0 |
| Chile     |           | 192.168.253.40  | 255.255.255.0 |


```https://asciiflow.com/
                                             ┌──────────┐
                                      ┌──────┤ PC Pepino│
┌─────────┐                           │      └──────────┘
│ PC apio ├───────┐                   │
└─────────┘       │                   │
               ┌──┴─────────┐  ┌──────┴──┐
               │SW Zanahoria├──┤SW Tomate│
               └──┬─────────┘  └──────┬──┘
                  │                   │
┌───────────┐     │                   │     ┌─────────────┐
│ PC Lechuga├─────┘                   └─────┤ Server Chile│
└───────────┘                               └─────────────┘
```

* Todos los dispositivos se pueden hacer ping entre ellos y tambien se le puede accessar remotamente a los Switches(telnet o SSH)

