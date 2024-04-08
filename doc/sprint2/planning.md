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

- **Packet Tracer version:** 8.2.1


- **VLANIDs range:** 384 – 405


- **VTP domain name:** r2324dgg3


- **IPv4 address space:** 172.23.192.0/20


- **ISP router’s IPv4 node address:** 5.60.37.181/30


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
  - **Name:** Switch-B*nBuilding*-F*nFloor*-*HCC/ICC* (ex. Switch-B1-F1-HCC) and
Switch-B*nBuilding*-*MCC* (ex. Switch-B1-F1-HCC)
- **VoIP Phone:**
  - **Model:** 7960
  - **Name:** VoIP*number*-B*nBuilding*-F*nFloor* (ex. Phone1-B1-F1)

  
### 4. IPv4 networks ###
#### 4.1. Building 1 and Backbone ####

    End user outlets on the ground floor: 50 nodes
    End user outlets on floor one: 50 nodes
    Wi-Fi network: 80 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 100 nodes
    VoIP (IP-phones): 67 nodes

    Backbone: 200 nodes

#### 4.2. Building 2 ####

    End user outlets on the ground floor: 90 nodes  
    End user outlets on floor one: 120 nodes
    Wi-Fi network: 220 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 50 nodes
    VoIP (IP-phones): 110 nodes

#### 4.3. Building 3 ####

    End user outlets on the ground floor: 110 nodes
    End user outlets on floor one: 130 nodes
    Wi-Fi network: 200 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 45 nodes
    VoIP (IP-phones): 180 nodes

#### 4.4. Building 4 ####

    End user outlets on the ground floor: 120 nodes
    End user outlets on floor one: 150 nodes
    Wi-Fi network: 190 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 40 nodes
    VoIP (IP-phones): 170 nodes



