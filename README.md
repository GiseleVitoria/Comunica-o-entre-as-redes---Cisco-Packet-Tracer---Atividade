# Comunicação entre Três Redes Distintas – Cisco Packet Tracer

## Sobre o projeto

Projeto desenvolvido no **Cisco Packet Tracer** com o objetivo de implementar uma infraestrutura de rede capaz de estabelecer comunicação entre três redes locais distintas (A, B e C), utilizando um roteador para realizar o encaminhamento de pacotes.

A atividade envolve a montagem da topologia, configuração de endereços IPv4, gateways e testes de conectividade entre dispositivos.

## Tecnologias e dispositivos

- Cisco Packet Tracer
- 1 Roteador Cisco 2911
- 3 Switches Cisco 2960
- 6 computadores (PCs)
- Cabos Copper Straight-Through

## Topologia da rede

A infraestrutura foi organizada da seguinte maneira:

- **Rede A:** Switch A e dois computadores.
- **Rede B:** Switch B e dois computadores.
- **Rede C:** Switch C e dois computadores.

O roteador conecta os três switches por meio de suas interfaces GigabitEthernet, permitindo a comunicação entre as redes.

## Endereçamento IP

| Rede | Endereço de rede | Gateway | Máscara |
|---|---|---|---|
| A | 10.0.0.0 | 10.0.0.1 | 255.0.0.0 |
| B | 172.16.0.0 | 172.16.0.1 | 255.255.0.0 |
| C | 192.168.1.0 | 192.168.1.1 | 255.255.255.0 |

Os computadores receberam endereços IP estáticos:

| Computador | Endereço IP |
|---|---|
| PC A1 | 10.0.0.2 |
| PC A2 | 10.0.0.3 |
| PC B1 | 172.16.0.2 |
| PC B2 | 172.16.0.3 |
| PC C1 | 192.168.1.2 |
| PC C2 | 192.168.1.3 |

## Configuração do roteador

| Interface | Endereço IPv4 | Rede |
|---|---|---|
| GigabitEthernet 0/0 | 10.0.0.1 | A |
| GigabitEthernet 0/1 | 172.16.0.1 | B |
| GigabitEthernet 0/2 | 192.168.1.1 | C |

As três interfaces foram configuradas e ativadas para permitir o encaminhamento de pacotes entre as redes.

## Testes de conectividade

Foram realizados testes utilizando o modo de simulação do Packet Tracer para verificar a comunicação entre dispositivos de redes diferentes.

Exemplos de testes:
- PC A1 → PC B1
- PC A2 → PC C1
- PC B2 → PC A1
- PC C2 → PC B1

## Resultado esperado

Comunicação estabelecida entre os seis computadores, permitindo a troca de pacotes entre as três redes por meio do roteador.

## Conceitos aplicados

- Topologia de redes LAN.
- Endereçamento IPv4 e máscaras de sub-rede.
- Configuração de gateways.
- Funcionamento de switches e roteadores.
- Interfaces de rede.
- Roteamento entre redes distintas.
- Protocolo ARP.
- Simulação e testes de conectividade.
