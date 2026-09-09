# Sistemas Distribuídos - Ambiente Virtualizado com Socket TCP/UDP

## 📹 Demonstração

<video width="100%" controls>
  <source src="Video.webm" type="video/webm">
  Seu navegador não suporta a tag de vídeo.
</video>

## 📋 Descrição do Trabalho

Implementação de um ambiente de rede virtualizado utilizando máquinas virtuais, com infraestrutura corporativa básica contendo:

- **3 Máquinas Virtuais** distribuídas em dois segmentos de rede distintos
- **Rede Interna Isolada** (Zona Protegida)
- **Rede Externa** com acesso à internet
- **Servidores Socket TCP/UDP Multithread**
- **Clientes TCP/UDP** para comunicação em rede

## 🏗️ Arquitetura

### Máquinas Virtuais

**VM1 - Roteador/DHCP/Servidor**
- Servidor DHCP
- Servidor Socket TCP (Multithread)
- Servidor Socket UDP (Multithread)
- 2 Interfaces de Rede:
  - R1: Rede Externa (Acesso Internet)
  - R2: Rede Interna Isolada

**VM2 - Cliente 1**
- Cliente Socket TCP
- Cliente Socket UDP
- 1 Interface de Rede: Rede Interna

**VM3 - Cliente 2**
- Cliente Socket TCP
- Cliente Socket UDP
- 1 Interface de Rede: Rede Interna

## 🎯 Objetivos

- ✅ Configurar ambiente virtualizado em hypervisor (VirtualBox/VMware/Proxmox/Hyper-V)
- ✅ Implementar comunicação TCP multithread entre servidor e clientes
- ✅ Implementar comunicação UDP multithread entre servidor e clientes
- ✅ Demonstrar funcionamento simultâneo de múltiplos clientes
- ✅ Documentar toda a infraestrutura e códigos
