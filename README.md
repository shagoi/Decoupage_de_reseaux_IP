# Decoupage_de_reseaux_IP

Une société fictive a 4 pôles informatiques. Le réseau est en 172.16.1.0/24.
Découper ce réseau de 2 manières, symétrique et asymétrique, pour que chaque pôle ci-dessous puissent avoir assez d'adresse pour chaque équipement.

Le Pôle informatique (6 bureaux, environ **50 équipements** au total)  
Le Pôle développement (6 bureaux, environ **12 équipements** au total)  
Le Pôle Administratif (4 bureaux, environ **20 équipements** au total)   
Le Pôle Technicien (4 bureaux, environ **15 équipements** au total)

## Découpage symétrique
Nous sommes ici dans un découpage symétrique soit pour un maximum de 50 équipements donc un choix de 64 adresses.

|  | Adresse réseau | Adresse de broadcast | Adresse de début de plage | Adresse de fin de plage |
| --- | --- | --- | --- | --- |
| Le Pôle informatique | 172.16.1.0/26 | 172.16.0.63 | 172.16.0.1 | 172.16.0.62 |
| Le Pôle développement | 172.16.0.64/26 | 172.16.0.127 | 172.16.0.65 | 192.168.0.126 |
| Le Pôle Administratif | 172.16.0.128/26 | 172.16.0.191 | 172.16.0.129 | 172.16.0.190 |
| Le Pôle Technicien | 172.16.0.191/26 | 172.16.0.255 | 172.16.0.192 | 172.16.0.254 |


## Découpage asymétrique
Dans le cas d'un découpage asymétrique:

pour le pole informatique il nous faudra 64 adresses 2exp6.

Pour le Pôle développement il nous faudra 16 adresses 2exp4.

Pour le Pôle Administratif il nous faudra 32 adresses 2exp5.

Pour le Pôle Technicien il nous faudra 32 adresses 2exp5.

| | Adresse réseau | Adresse de broadcast | Adresse de début de plage | Adresse de fin de plage |
| --- | --- | --- | --- | --- |
| Le Pôle informatique | 172.16.0.0/26 | 172.16.0.63 | 172.16.0.1 | 172.16.0.62 |
| Le Pôle développement | 172.16.0.64/28 | 172.16.0.80 | 172.16.0.65 | 172.16.0.79 |
| Le Pôle Administratif | 172.16.0.81/27 | 172.16.0.113 | 172.16.0.82 | 172.16.0.112 |
| Le Pôle Technicien | 172.16.0.114/27 | 172.16.0.146 | 172.16.0.115 | 172.16.0.145 |
