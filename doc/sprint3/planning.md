# Project 1 - Sprint 3 planning #

### 1. Scrum Master: ###
**Rui Moreira (1221696).**

### 2. Backlog: ###

| Task  |                                                                                                                      Task description                                                                                                                      |          Assignee          |
|:-----:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------:|
| T.3.1 |                                                  Update the building1.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 1.                                                  |  Beatriz Morais (1221401)  |
| T.3.2 | Update the building2.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 2.Final integration of each member’s Packet Tracer simulation into a single simulation (campus.pkt). |   Rui Moreira (1221696)    |
| T.3.3 |                                                  Update the building3.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 3.                                                  | Eduardo Carreiro (1211199) |
| T.3.4 |                                                  Update the building4.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 4.                                                  |  Diogo Correia (1212106)   |

### 3. Technical decisions ###


#### 3.2. OSPF dynamic routing ####

    Static routing will no longer be used, thus on every router, the existing static routing tables should be
    erased, the only exception is the default route established in the building 1 router.

    OSPF area ids to be used in each building must be settled on the planning meeting, each building is
    required to use a unique id.
    The team member in charge of building 1 must insert into the OSPF routing protocol the default route,
    pointing to the ISP router (default-information originate command).

#### 3.3. HTTP servers ####

    In addition to the already existing server, in each building, a new server must be added to the local DMZ
    network, as the former, it will have a manually set IPv4 address. On this server, the HTTP/HTTPS
    service is to be enabled, and a simple HTML page should be created, the page should at least identify the
    building it belongs to.

#### 3.4. DHCPv4 service ####

#### 3.5. VoIP service ####

#### 3.6. DNS ####

    DNS domain name: rcomp-23-24-dg-g3
    DNS local domain name: building-X.rcomp-23-24-dg-g3
    Unqualified DNS domain name: ns.rcomp-23-24-dg-g3
    Unqualified DNS local domain name: ns.building-X.rcomp-23-24-dg-g3

#### 3.7. NAT (Network Address Translation) ####

#### 3.8. Static Firewall (ACLs) ####




    