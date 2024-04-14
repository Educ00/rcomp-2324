# Project 1 - Sprint 2 - Building 3 #

### 1. IPv4 addresses ###

#### 1.1. Building 3 ####
    End user outlets on the ground floor: 110 nodes
    End user outlets on floor one: 130 nodes
    Wi-Fi network: 200 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 45 nodes
    VoIP (IP-phones): 180 nodes


### 2. VLANs ###

 | Vlan Id |   Name    | Nodes |         IP          |      Mask       |
|:-------:|:---------:|:-----:|:-------------------:|:---------------:|
|   395   |  B3-WIFI  |  200  |  172.23.200.0 / 24  |  255.255.255.0  |
|   396   |  B3-VOIP  |  180  |  172.23.201.0 / 24  |  255.255.255.0  |
|   397   | B3-OUT-F1 |  130  |  172.23.202.0 / 24  |  255.255.255.0  |
|   398   | B3-OUT-F0 |  110  |  172.23.203.0 / 25  | 255.255.255.128 |
|   399   |  B3-DMZ   |  45   | 172.23.203.128 / 26 | 255.255.255.192 |


### 3. Building 3 simulation ###

![buildinng3.png](./Building3.png)
