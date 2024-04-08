# Building 2 #

## Indice
### 1. Imagens do Edificio
### 2. Defesa das estrategias usadas
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


    90 nodes - 25 - 172.23.194.128 (next : 172.23.195.0)
    120 nodes - 25 - 172.23.195.0 (next : 172.23.195.128)
    220 nodes - 24 - 172.23.195.128 (next : 172.23.196.128)
    50 nodes - 26 - 172.23.196.128 (next : 172.23.196.192)
    110 nodes - 25 - 172.23.197.64