# TP Général CCNA 2 — Réseau d'entreprise multi-sites

## Topologie
- 2 routeurs : Router2 (Cisco 2911), Router1 (ISR4331)
- 7 switches Cisco 2960-24TT (Switch0–Switch6)
- 16 PCs, 2 serveurs
- Liaison série WAN entre Router2 et Router1

## Plan VLAN
| VLAN | Nom |
|------|-----|
| 10 | Schools |
| 20 | IT |
| 30 | RH |
| 40 | MRH |
| 50 | RMS |
| 101 | Native |

## Adressage IP
**Router2 (serveur DHCP)**
- Gi0/0.10 → 172.16.10.1/24
- Gi0/0.20 → 172.16.20.1/24
- Gi0/0.30 → 172.16.30.1/24
- Gi0/0.40 → 172.16.40.1/24
- Gi0/0.50 → 172.16.50.1/24
- Gi0/1 → 172.16.1.1/24
- Serial0/3/0 → 10.1.1.9/30

**Router1 (client)**
- Gi0/0/1 → 192.168.200.1/24
- Serial0/1/0 → 10.1.1.10/30

## Concepts couverts
- VLANs et liens trunk
- EtherChannel (Switch0/1/2/3)
- STP (Spanning Tree Protocol)
- Routage inter-VLAN (Router-on-a-stick)
- DHCP dynamique (Router2 = serveur)
- Routage statique IPv4/IPv6
- Liaison série WAN
- Port Security
