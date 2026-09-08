# Sistemas Distribuídos - Ambiente Virtualizado com Socket TCP/UDP

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

## 📁 Estrutura do Repositório

```
├── README.md                          # Este arquivo
├── video/                             # Vídeo explicativo do projeto
├── codigos/
│   ├── servidor_tcp.c                 # Servidor TCP Multithread
│   ├── cliente_tcp.c                  # Cliente TCP
│   ├── servidor_udp.c                 # Servidor UDP Multithread
│   ├── cliente_udp.c                  # Cliente UDP
│   └── Makefile                       # Compilação dos programas
├── docs/
│   ├── configuracao_rede.md           # Passo a passo da configuração de rede
│   ├── configuracao_vms.md            # Configuração das VMs
│   └── arquitetura.md                 # Detalhes da arquitetura
└── testes/
    └── relatorio_testes.md            # Resultados dos testes de conexão
```

## 🚀 Como Começar

1. Consulte a documentação em `docs/` para configurar o ambiente
2. Acesse `codigos/` para compilar e executar os programas
3. Assista ao vídeo em `video/` para demonstração completa

## 👥 Grupo

- Discente 1
- Discente 2

## 📅 Data de Entrega

**09 de setembro de 2026** - até às 20hrs

## 📊 Pontuação

**10,0 pontos** (Trabalhos da 1ª unidade = 30% da nota final)

---

**Status:** Em desenvolvimento 🔨
