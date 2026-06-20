
---

## 🌐 Laboratório: Configuração de VLANs Corporativas (Cisco Packet Tracer)

Projeto prático focado em segmentação de rede, segurança lógica e performance utilizando switches e roteadores Cisco.

### 🗺️ Cenário da Rede
A rede foi dividida em 3 departamentos utilizando um único Switch Gerenciável, isolando o tráfego de broadcast e aumentando a segurança:

| Departamento / VLAN | ID da VLAN | Rede IP |
| :--- | :--- | :--- |
| **Admin (Diretoria)** | VLAN 10 | `192.168.10.0/24` |
| **Vendas (Comercial)** | VLAN 20 | `192.168.20.0/24` |
| **TI (Suporte)** | VLAN 30 | `192.168.30.0/24` |

*Para a comunicação entre as diferentes VLANs, foi aplicada a técnica **Router-on-a-Stick (Trunking)** conectando o Switch ao Roteador.*

### 🛠️ Principais Comandos Utilizados

**1. Criação das VLANs no Switch:**
```cisconet
Switch(config)# vlan 10
Switch(config-vlan)# name Admin
Switch(config-vlan)# vlan 20
Switch(config-vlan)# name Vendas
Switch(config-vlan)# vlan 30
Switch(config-vlan)# name TI
