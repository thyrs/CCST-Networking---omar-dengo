# Intro to Wireshark: Basics + Packet Analysis!        
https://www.youtube.com/watch?v=jvuiI1Leg6w


### IP Address:

- ip.addr
- ip.src
- ip.dst

### MAC Addres:

- eth.addr
- eth.dst
- eth.src

### Protoco:

- dns
- dhcp
- http


# Comparison Operators:

### Equals: == or eq
* ip.addr eq 192.168.1.1 
* ip.addr == 192.168.1.1 

### And: && or and
* tcp.port == 22 && ip.addr == 192.168.1.1
* tcp.port == 22 and ip.addr == 192.168.1.1

### Or: || (double pipe) or or
* http.request || http.response
* http.request or http.response


# Filtering examples
```sh
http.request
# Display all HTTP requests.

http.request || http.response
# Display all HTTP request and responses.

ip.addr == 127.0.0.1
# Display all IP packets whose source or destination is localhost.

tcp.len < 100
# Display all TCP packets whose data length is less than 100 bytes.

http.request.uri matches “(gif)$” 
# Display all HTTP requests in which the uri ends with “gif”.

dns.query.name == “www.google.com” 
# Display all DNS queries for “www.google.com”
```




# Investigating Lost Packets With Wireshark

https://www.youtube.com/watch?v=mQ8CbakZLFU

Internet Protocol Version 
    > Identification (apply as a columm)

then under:

Transmission Control Protocol
    > [SEQ/ACK analysis]
        > [This is an ACK to the segment in frame: 8]



