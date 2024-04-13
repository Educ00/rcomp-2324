# Building 2 

## 1. Imagens do Layout do packet tracer

### 1.1 Imagem do layout do building2

![buildinng2_report.png](..%2F..%2F..%2F..%2Fbuildinng2_report.png)

### 1.2 Imagem do campus

![Campus.png](..%2F..%2F..%2F..%2FCampus.png)

## 2. Descriçao do edificio

    End user outlets on the ground floor: 90 nodes  
    End user outlets on floor one: 120 nodes
    Wi-Fi network: 220 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 50 nodes
    VoIP (IP-phones): 110 nodes

### 2.1 Subnet e Subnet Mask

| Building |    Subnet    |     Mask      |
|:--------:|:------------:|:-------------:|
|    2     | 172.23.196.0 | 255.255.252.0 |

### 2.2 VLAN's

| Building | Vlan Id |   Name    | Nodes |         Ip          |      Mask       |
|:--------:|:-------:|:---------:|:-----:|:-------------------:|:---------------:|
|    2     |   390   |  B2-WIFI  |  220  |  172.23.196.0 / 24  |  255.255.255.0  |
|    2     |   391   | B2-OUT-F1 |  120  |  172.23.197.0 / 25  | 255.255.255.128 | 
|    2     |   392   |  B2-VOIP  |  110  | 172.23.197.128 / 25 | 255.255.255.128 |
|    2     |   393   | B2-OUT-F0 |  90   |  172.23.198.0 / 25  | 255.255.255.128 |
|    2     |   394   |  B2-DMZ   |  50   | 172.23.198.128 / 26 | 255.255.255.192 |

### 2.3 IPv4 adress space

- **IPv4 address space:** 172.23.192.0/20




