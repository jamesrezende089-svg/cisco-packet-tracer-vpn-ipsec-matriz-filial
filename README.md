
# Infraestrutura de Rede Corporativa — VPN IPsec Site-to-Site (Matriz e Filial) com DHCP Dedicado

Projeto prático desenvolvido no **Cisco Packet Tracer** simulando a interligação segura entre uma **Matriz** e uma **Filial** por meio de túnel **VPN IPsec Site-to-Site**, com distribuição automática de endereços IP via **servidor DHCP dedicado** e validação de conectividade ponta a ponta.

---

## Arquitetura e Endereçamento IP

* **Rede Matriz:** `192.168.0.0/24`
* **Rede Filial:** `192.168.2.0/24`
* **Segurança do enlace:** Túnel VPN IPsec Site-to-Site entre os roteadores da Matriz e da Filial
* **Atribuição de endereços:** Servidor DHCP dedicado para entrega automática de IP, máscara, gateway e demais parâmetros

---

## Evidências e Passo a Passo da Simulação

### 1. Topologia e Visão Geral da Rede
![Topologia e visão geral da rede](Captura%20de%20tela%202026-11-17%20221749.png)

### 2. Configuração do Roteador da Matriz (`Router 0`)
* Arquivo de configuração completo: [`Configuração_Router 0 - Matriz.txt`](Configura%C3%A7%C3%A3o_Router%200%20-%20Matriz.txt)

![Configuração do Router Matriz](Captura%20de%20tela%202_router_Matriz.png)

### 3. Configuração do Roteador da Filial (`Router 2`)
* Arquivo de configuração completo: [`Configuração_Router 2 - Filial.txt`](Configura%C3%A7%C3%A3o_Router%202%20-%20Filial.txt)

![Configuração do Router Filial](Captura%20de%20tela%20Routder%202_Filial.png)

### 4. Distribuição de IP via DHCP no Cliente (`PC2`)
![Recebimento de IP via DHCP no cliente PC2](Captura%20de%20tela%20_cliente_dhcp_pc2.png)

### 5. Configuração do Servidor DHCP Dedicado (serverPool)
![Detalhe adicional da simulação](Captura%20de%20tela%202026-11-17%20224117.png)

### 6. Validação de Conectividade e Rota (`ping` e `tracert`)
![Validação com ping e tracert](Captura%20da%20tela_valida%C3%A7%C3%A3o_ping_tracert.png)

---

## Autor

**James Rezende Coutinho** — Estudante de Tecnologia em Redes de Computadores
