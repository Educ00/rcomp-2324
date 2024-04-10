# Project 1 - Sprint 2 planning #

### 1. Scrum Master: ###
**Beatriz Morais (1221401).**

### 2. Backlog: ###

| Task  |                                                                                             Task description                                                                                             |          Assignee          |
|:-----:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------:|
| T.2.1 | Development of a layer two and layer three Packet Tracer simulation for building 1 , encompassing the campus backbone.  Integration of every member’s Packet Tracer simulation into a single simulation. |  Beatriz Morais (1221401)  |
| T.2.2 |                                          Development of a layer two and layer three Packet Tracer simulation for building 2, encompassing the campus backbone.                                           |   Rui Moreira (1221696)    |
| T.2.3 |                                          Development of a layer two and layer three Packet Tracer simulation for building 3, encompassing the campus backbone.                                           | Eduardo Carreiro (1211199) |
| T.2.4 |                                          Development of a layer two and layer three Packet Tracer simulation for building 4, encompassing the campus backbone.                                           |  Diogo Correia (1212106)   |

### 3. Technical decisions ###
#### 3.1. Packet Tracer Version ####

- **Packet Tracer version:** 8.2.1

#### 3.2. IP's and VLAN's ####

- **IPv4 address space:** 172.23.192.0/20


- **ISP router’s IPv4 node address:** 5.60.37.181/30


- **VLANIDs range:** 384 – 405

| Building | VLANID range |    
|:--------:|:------------:|
|    1     |  384 - 389   | 
|    2     |  390 - 394   |   
|    3     |  395 - 399   |
|    4     |  400 - 404   |

| Building |    Subnet    |     Mask      |
|:--------:|:------------:|:-------------:|
|    1     | 172.23.192.0 | 255.255.252.0 |
|    2     | 172.23.196.0 | 255.255.252.0 |
|    3     | 172.23.200.0 | 255.255.252.0 |
|    4     | 172.23.204.0 | 255.255.252.0 |

| Building | Vlan Id |   Name    | Nodes |         Ip          |      Mask       |
|:--------:|:-------:|:---------:|:-----:|:-------------------:|:---------------:|
|    1     |   384   | Backbone  |  200  |  172.23.192.0 / 24  |  255.255.255.0  |
|    1     |   385   |  B1-DMZ   |  100  |  172.23.193.0 / 25  | 255.255.255.128 |
|    1     |   386   |  B1-WIFI  |  80   | 172.23.193.128 / 25 | 255.255.255.128 | 
|    1     |   387   |  B1-VOIP  |  67   |  172.23.194.0 / 25  | 255.255.255.128 |
|    1     |   388   | B1-OUT-F0 |  50   | 172.23.194.128 / 26 | 255.255.255.192 |
|    1     |   389   | B1-OUT-F1 |  50   | 172.23.194.192 / 26 | 255.255.255.192 |
|    2     |   390   |  B2-WIFI  |  220  |  172.23.196.0 / 24  |  255.255.255.0  |
|    2     |   391   | B2-OUT-F1 |  120  |  172.23.197.0 / 25  | 255.255.255.128 | 
|    2     |   392   |  B2-VOIP  |  110  | 172.23.197.128 / 25 | 255.255.255.128 |
|    2     |   393   | B2-OUT-F0 |  90   |  172.23.198.0 / 25  | 255.255.255.128 |
|    2     |   394   |  B2-DMZ   |  50   | 172.23.198.128 / 26 | 255.255.255.192 |
|    3     |   395   |  B3-WIFI  |  200  |  172.23.200.0 / 24  |  255.255.255.0  |
|    3     |   396   |  B3-VOIP  |  180  |  172.23.201.0 / 24  |  255.255.255.0  |
|    3     |   397   | B3-OUT-F1 |  130  |  172.23.202.0 / 24  |  255.255.255.0  |
|    3     |   398   | B3-OUT-F0 |  110  |  172.23.203.0 / 25  | 255.255.255.128 |
|    3     |   399   |  B3-DMZ   |  45   | 172.23.203.128 / 26 | 255.255.255.192 |
|    4     |   400   |  B4-WIFI  |  190  |  172.23.204.0 / 24  |  255.255.255.0  |
|    4     |   401   |  B4-VOIP  |  170  |  172.23.205.0 / 24  |  255.255.255.0  | 
|    4     |   402   | B4-OUT-F1 |  150  |  172.23.206.0 / 24  |  255.255.255.0  |
|    4     |   403   | B4-OUT-F0 |  120  |  172.23.207.0 / 25  | 255.255.255.128 |
|    4     |   404   |  B4-DMZ   |  40   | 172.23.207.128 / 26 | 255.255.255.192 |

#### 3.3. Naming Convention ####

- **VTP domain name:** r2324dgg3


- **Access Point:**
  - **Model:** AccessPoint-PT
  - **Name:** AP*number*-B*nBuilding*-F*nFloor* (ex. AP1-B1-F1)

  
- **Laptop:**
  - **Model:** Laptop-PT
  - **Name:** Laptop*number*-B*nBuilding*-F*nFloor* (ex. Laptop1-B1-F1)
  

- **PC:**
  - **Model:** PC-PT
  - **Name:** PC-B*nBuilding*-F*nFloor* (ex. PC-B1-F1)
  

- **Router:**
  - **Model:** 2811
  - **Name:** Router-B*nBuilding* (ex. Router-B1)


- **Server:**
  - **Model:** Server-PT
  - **Name:** Server*number*-B*nBuilding*-F*nFloor* (ex. Server1-B1-F1)


- **Switch:**
  - **Model:** Switch-PT-Empty
  - **Name:** Switch-B*nBuilding*-F*nFloor*-*HCC* (ex. Switch-B1-F1-HCC) and
Switch-B*nBuilding*-*ICC/MCC* (ex. Switch-B1-F1-HCC)


- **VoIP Phone:**
  - **Model:** 7960
  - **Name:** VoIP*number*-B*nBuilding*-F*nFloor* (ex. Phone1-B1-F1)
  
### 4. IPv4 networks ###
#### 4.1. Backbone ####
    Backbone: 200 nodes

#### 4.2. Building 1 ####
    End user outlets on the ground floor: 50 nodes
    End user outlets on floor one: 50 nodes
    Wi-Fi network: 80 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 100 nodes
    VoIP (IP-phones): 67 nodes

#### 4.3. Building 2 ####

    End user outlets on the ground floor: 90 nodes  
    End user outlets on floor one: 120 nodes
    Wi-Fi network: 220 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 50 nodes
    VoIP (IP-phones): 110 nodes

#### 4.4. Building 3 ####

    End user outlets on the ground floor: 110 nodes
    End user outlets on floor one: 130 nodes
    Wi-Fi network: 200 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 45 nodes
    VoIP (IP-phones): 180 nodes

#### 4.5. Building 4 ####

    End user outlets on the ground floor: 120 nodes
    End user outlets on floor one: 150 nodes
    Wi-Fi network: 190 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 40 nodes
    VoIP (IP-phones): 170 nodes



