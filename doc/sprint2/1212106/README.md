# Sprint 2 - Building 4 #


### 1. IPv4 addresses ###
#### 1.1. Backbone ####
    Backbone: 200 nodes

#### 1.2. Building 4 ####
 
    End user outlets on the ground floor: 120 nodes
    End user outlets on floor one: 150 nodes
    Wi-Fi network: 190 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 40 nodes
    VoIP (IP-phones): 170 nodes


### 2. VLANs ###

| Building | Vlan Id |   Name    | Nodes |         Ip          |      Mask       |
|:--------:|:-------:|:---------:|:-----:|:-------------------:|:---------------:|
|    4     |   400   |  B4-WIFI  |  190  |  172.23.204.0 / 24  |  255.255.255.0  |
|    4     |   401   |  B4-VOIP  |  170  |  172.23.205.0 / 24  |  255.255.255.0  | 
|    4     |   402   | B4-OUT-F1 |  150  |  172.23.206.0 / 24  |  255.255.255.0  |
|    4     |   403   | B4-OUT-F0 |  120  |  172.23.207.0 / 25  | 255.255.255.128 |
|    4     |   404   |  B4-DMZ   |  40   | 172.23.207.128 / 26 | 255.255.255.192 |