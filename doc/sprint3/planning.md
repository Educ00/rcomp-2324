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

    
#### 3.4. DHCPv4 service ####

    For the VoIP VLAN, the DHCP server configuration must include option 150, it represents the IP
    address of the TFTP (Trivial File Transfer Protocol) server to be used by Cisco IP phones model 7960
    to download the phone’s configuration file.

#### 3.5. VoIP service ####

    In the simulation, for VoIP local testing, in each building there should be at least two connected IP
    phones (please, use the 7960 model available in Packet Tracer).
    Ports of switches connecting to Cisco IP phones 7960, must have the voice VLAN enabled (switchport
    voice vlan VLANID) and the access VLAN disabled (no switchport access vlan).

#### 3.6. DNS ####

    DNS domain name: rcomp-23-24-dg-g3
    DNS local domain name: building-X.rcomp-23-24-dg-g3
    Unqualified DNS domain name: ns.rcomp-23-24-dg-g3
    Unqualified DNS local domain name: ns.building-X.rcomp-23-24-dg-g3

#### 3.7. NAT (Network Address Translation) ####
    HTTP and HTTPS requests received in the router’s backbone interface are redirected to the DNS server
    in the local DMZ. Both HTTP and HTTPS use TCP connections, assume the default service ports
    numbers are used, 80 and 443.

#### 3.8. Static Firewall (ACLs) ####

In higher-precedence-first order, traffic access policies to be enforced are:
* First 

      Block all spoofing, as far as possible. Internal spoofing from local networks, the DMZ may be
      excluded. External spoofing for traffic incoming from the backbone network.
* Second 

      All ICMP echo requests and echo replies are always allowed.

* Third
    
        All traffic to the DMZ is to be blocked, except for the DNS service and HTTP/HTTPS services
        to the corresponding servers. Every traffic incoming from the DMZ is allowed.
* Fourth 

      All traffic directed to the router itself (with a destination IPv4 node address belonging to the
      router) is to be blocked, except for the traffic required for the described features to work.
* Fifth
      
      Remaining traffic passing through the router should be allowed.


Regarding the fourth access policy exceptions, they will encompass several services that must be allowed
for networks where they are required, some not to be forgotten are:

 * The DHCPv4 service. Notice the first DHCPv4 request (DHCP discover) is sent from IPv4
source address 0.0.0.0 (unknown address) to the IPv4 destination address 255.255.255.255 (local
broadcast).
* The TFTP service (for IP phones).
* The ITS service (for IP phones and for other IST servers).
* OSPF traffic.
* Traffic encompassed by the enforced NAT static rules.
    