# Home Router (autonomos AP)
```txt
         ┌───┐
         │ISP│
         └─┬─┘
           │
Internet   │
Interface  │
        ┌──┴───┐            ┌─────┐
        │ HOME │gi0/1       │ PC01│
        │ROUTER├────────────┤ADMIN│
        └──────┘         fa0└─────┘


        ┌──────┐
        │ WIFI │
        │LAPTOP│
        └──────┘
```
## Basic Setup:

- "Internet interface" > WAN Port > (ISP) *
- gig1 > LAN Ports > (LOCAL NETWORK) > PC
- connect PC and ask dhcp address
- access broswer on PC > 192.168.0.1 (default gateway)
- username: admin 
- password: admin

## Configuration options:

### 1. Change SSID (Wifi Name)
    Wireless > Basic Wireless Settings >2.4 or 5.0 > Network Name (SSID)
    Example: mywifi
    *Save settings

### 2. Add Wifi password
    Wireless >  Wireless Security > Security mode > 
    (Default) : WPA2 personal, 
    encryption: (Default) AES
	Example: wifipass
    *Save settings
    
### 3. Change user and password to access router - OPTIONAL
    Administration > Management > Router Access
    Example: routerpass
	*Save settings

### 4. Change outside ip address (internet interface) - OPTIONAL
    Setup > Basic Setup > Internet setup > Internet connection type (default DHCP)
    *Save settings

## How to connect laptop to Wifi on packet tracer

    1. Laptop > Physical tap
        A. Turn off the Laptop 
        B. Drag and drop the ethernet adaptor to the left
        C. Drag and drop the WPC300N adaptor to the Laptop
        D. Turn on Laptop 
    
    2. Desktop > PC wireless > Connect > Select wifi name > enter password and Connect.


## How to connect smartphone and table to a Wifi network

* Open Smartphone/table > Config tab > Interface wireless0 > change SSID(wifi name) > select "WPA2-PSK" > add wifipassword > make sure "encryption type" is correct



# Menu of topics

## How to configure: 

* **DHCP internal server**
    - Septup > Basic setup > DHCP server Settings
---
* **Wifi security configuration**
    - Wireless > Wireless Security
---
* **Guest network**
    - Wireless > Guest Network
---
* **Mac filtering**
    - Wireless > Wireless MAC Filter 
---
* **Program Wifi avilability**
    - Wireless > advance Wireless Settings Enable WIFI:
---
* **Block URL, apps using ports**
    - Access restrictions >
---
* **Open ports for gaming and especial apps**
    - Aplicacions & gaming
---
* **DMZ**
    - Aplicacions & gaming > DMZ
---
* **QoS**
    - Aplicacions & gaming > DMZ
---
* **Change router password**
    - Adminstration > Router access
---
* **Save config and restore it.**
    - Adminstration > BackUP and Restore
---
## CMD
* C:\>ipconfig /release 
* C:\>ipconfig /renew