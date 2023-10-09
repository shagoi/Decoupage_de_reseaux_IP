# Decoupage_de_reseaux_IP

Le Pôle informatique (6 bureaux, environ **50 équipements** au total)  
Le Pôle développement (6 bureaux, environ **12 équipements** au total)  
Le Pôle Administratif (4 bureaux, environ **20 équipements** au total)   
Le Pôle Technicien (4 bureaux, environ **15 équipements** au total)

#### Découpage symétrique ####

|  | Adresse réseau | Adresse de broadcast | Adresse de début de plage | Adresse de fin de plage |
| --- | --- | --- | --- | --- |
| Le Pôle informatique | 172.16.1.0/58 | 172.16.0.63 | 172.16.0.1 | 172.16.0.62 |
| Le Pôle développement | 172.16.0.64/58 | 172.16.0.128 | 172.16.0.65 | 192.168.0.127 |
| Le Pôle Administratif | 172.16.0.129/58 | 172.16.0.193 | 172.1680.130 | 172.16.0.192 |
| Le Pôle Technicien | 172.16.0.194/58 | 172.16.0.255 | 172.16.0.195 | 172.16.0.254 |


#### Découpage asymétrique

| | Adresse réseau | Adresse de broadcast | Adresse de début de plage | Adresse de fin de plage |
| --- | --- | --- | --- | --- |
| Le Pôle informatique | 192.168.0.0/27 | 192.168.0.63 | 192.168.0.1 | 192.168.0.62 |
| Le Pôle développement | 192.168.0.64/27 | 192.168.0.93 | 192.168.0.65 | 192.168.0.92 |
| Le Pôle Administratif | 192.168.0.94/27 | 192.168.0.123 | 192.168.0.95 | 192.168.0.122 |
| Le Pôle Technicien | 192.168.0.124/27 | 192.168.0.153 | 192.168.0.125 | 192.168.0.152 |
