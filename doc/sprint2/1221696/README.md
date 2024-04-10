# Building 2 #

## Indice
### 1. Imagens do Layout do packet tracer
### 2. Defesa das estratégias usadas
### 3. Inventario



| Building | VLAN ID |   Name    |
|:--------:|:-------:|:---------:|
|    2     |   390   | B2-OUT-F0 |
|    2     |   391   | B2-OUT-F1 | 
|    2     |   392   |  B2-WIFI  |
|    2     |   393   |  B2-DMZ   |
|    2     |   394   |  B2-VOIP  |

    End user outlets on the ground floor: 90 nodes  
    End user outlets on floor one: 120 nodes
    Wi-Fi network: 220 nodes
    DMZ (Servers, administration workstations, and network infrastructure devices): 50 nodes
    VoIP (IP-phones): 110 nodes


    90 outlets0 - 172.23.195.0/25 mascara - 255.255.255.128
    120 outlets1 - 172.23.195.128/25 mascara - 255.255.255.128
    220 wifi - 172.23.196.0/24 mascara - 255.255.255.0
    50 DMZ - 172.23.197.0/26 mascara - 255.255.255.192
    110 VoIP - 172.23.197.64/25 mascara - 255.255.255.128