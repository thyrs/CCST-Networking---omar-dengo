
# 200 Subnetting

__IP calculator__:
> https://www.calculator.net/ip-subnet-calculator.html

### 4th octet
```
|     |     |     |     |     |     |     |     |                 |
| --: | --: | --: | --: | --: | --: | --: | --: | --------------: |
| 128 |  64 |  32 |  16 |   8 |   4 |   2 |   1 |          SALTOS |
| /25 | /26 | /27 | /28 | /29 | /30 | /31 | /32 | Bits encendidos |
| 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |            mask |
| 127 |  63 |  31 |  15 |   7 |   3 |   1 |   0 |        Wildcard |
```

Steps:

* identificar el "magic number" (Saltos)
1. magic number (Saltos) = ______
2. identificar el mask 
3. Hacer los saltos empezando desde el "0" en el octeto correspondiente
4. identificar a que network pertenece el ip address que me dieron y llenar el resto de lo que me piden
5. total usable host = "magic number" - 2 (on the 4th octect)
    * 2 ^ "numer_of_host_bits" -2 (2nd,3rd octect)

* 192.66.101.0/24

|              |     |
| ------------ | --- |
| NETID        |     |
| subnet mask  |     |
| broadcast    |     |
| 1st usable   |     |
| Last usable  |     |
| total usable |     |
|              |     |



* 192.66.101.31/25
|              |     |
| ------------ | --- |
| NETID        |     |
| subnet mask  |     |
| broadcast    |     |
| 1st usable   |     |
| Last usable  |     |
| total usable |     |



* 192.66.101.65/26
|              |     |
| ------------ | --- |
| NETID        |     |
| subnet mask  |     |
| broadcast    |     |
| 1st usable   |     |
| Last usable  |     |
| total usable |     |


* 192.66.101.125/27

|              |     |
| ------------ | --- |
| NETID        |     |
| subnet mask  |     |
| broadcast    |     |
| 1st usable   |     |
| Last usable  |     |
| total usable |     |


### 3er octet


|     |     |     |     |     |     |     |     |                 |
| --: | --: | --: | --: | --: | --: | --: | --: | --------------: |
| 128 |  64 |  32 |  16 |   8 |   4 |   2 |   1 |          SALTOS |
| /17 | /18 | /19 | /20 | /21 | /22 | /23 | /24 | Bits encendidos |
| 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |            Mask |
| 127 |  63 |  31 |  15 |   7 |   3 |   1 |   0 |        Wildcard |

172.16.100.35/18

1. magic number (Saltos) = __64__
2. identificar el mask = __255.255.192.0__
3. Hacer los saltos empezando desde el "0" en el octeto correspondiente
4. identificar a que network pertenece el ip address que me dieron y llenar el resto de lo que me piden
5. total usable host = "magic number" - 2 (on the 4th octect)
    * 2 ^ "numer_of_host_bits" -2 (2nd,3rd octect)



###	This IP 172.16.100.35/18 belongs to which of the following networks (NETID)

- [ ] a. 172.16.100.0
- [ ] b. 172.16.64.0
- [ ] c. 172.16.90.0
- [ ] d. 172.16.69.0
- [ ] e. 172.16.96.0

|              |     |
| ------------ | --- |
| NETID        |     |
| subnet mask  |     |
| broadcast    |     |
| 1st usable   |     |
| Last usable  |     |
| total usable |     |




### 2do octet
```
|     |     |     |     |     |     |     |     |                 |
| --: | --: | --: | --: | --: | --: | --: | --: | --------------: |
| 128 |  64 |  32 |  16 |   8 |   4 |   2 |   1 |          SALTOS |
|  /9 | /10 | /11 | /12 | /13 | /14 | /15 | /16 | Bits encendidos |
| 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |            Mask |
| 127 |  63 |  31 |  15 |   7 |   3 |   1 |   0 |        Wildcard |
```

## Subnetting Cisco CCNA -Part 1 The Magic Number
> https://www.youtube.com/watch?v=a84XIopJFXs

## Subnetting Cisco CCNA -Part 2 The Magic Number
> https://www.youtube.com/watch?v=84-zNmomYzk

## Subnetting Cisco CCNA -Part 3 The Magic Number
> https://www.youtube.com/watch?v=-kAhTal4bNk

## Subnetting Cisco CCNA -Part 4 The Magic Number
> https://www.youtube.com/watch?v=RGBA83J60H0

## [Método Fácil] Convertir de Binario a Decimal y > viceversa.
> https://www.youtube.com/watch?v=c-hyLLdDt7I

## Subneteo (Subnetting). Como crear subredes. > [FAVOR LEER DESCRIPCION]
> https://www.youtube.com/watch?v=sLWYpqjT0_Y&list=PLINy58Bvq5_IWqFOllj2qL53cjZ3JZie7

## Subneteo VLSM (VLSM Subnetting). Como crear > subredes con el método de VLSM : 
> https://www.youtube.com/watch?v=KsMXVnqQ3sg&t=1357s