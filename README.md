# Lab-virtualizacao
Este Repositório documenta a criação e configuração de um ambiente de virtualização utilizando servidores Dell PowerEdge R910, VMware ESXi 6.7, vSphere, TrueNAS, e infraestrutura de rede com switches Cisco e VPN PPTP.

## 📂 Estrutura do Repositório:
- [`docs/`](./docs/) - Documentação técnica detalhada
- [`scripts/`](./scripts/) - Scripts de automação para cluster e criação de VMs
- [`diagrams/`](./diagrams/) - Diagramas de topologia, infraestrutura e cabeamento

## 🖥️ Estrutura do Lab

### 🔧 Hardware

- **5x Servidores Dell PowerEdge R910**
  - Hypervisor: **VMware ESXi 6.7**
  - Todos os hosts adicionados a um cluster gerenciado via vCenter (vSphere)
  
- **1x Servidor dedicado para Storage**
  - Sistema: **TrueNAS**
  - Compartilhamento NFS/iSCSI configurado para uso com o cluster ESXi

- **Switch Gerenciável 3Com**
  - VLANs configuradas individualmente para cada host
  - Interligação entre rede dos hosts e storage

## 🛠️ Software

- **VMware ESXi 6.7** nos 5 servidores Dell
- **vCenter Server (vSphere Web Client)** para gerenciamento centralizado
- **TrueNAS** para compartilhamento de armazenamento em rede
- **VPN PPTP** para acesso remoto seguro ao ambiente de laboratório

## 🌐 Rede

- Cada host possui acesso às VLANs configuradas no switch 3Com
- Comunicação entre os hosts ESXi e o servidor TrueNAS via VLANs específicas
- PPTP configurado para acesso remoto à rede do laboratório

## 🔒 Acesso Remoto

- VPN PPTP ativa para conexão externa ao laboratório
- Acesso a vSphere Web Client e demais recursos via túnel VPN
