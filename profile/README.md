
# Sistema Móvel de Purificação de Ar Baseado em VANT

Bem-vindo ao projeto **Sistema Móvel de Purificação de Ar Baseado em VANT – Drone Sugador de Fumaça**.

O projeto tem como objetivo desenvolver uma solução tecnológica inovadora capaz de auxiliar na redução da poluição do ar e no suporte a operações emergenciais em ambientes com alta concentração de fumaça, gases tóxicos e partículas poluentes.

A proposta consiste em um **VANT (Veículo Aéreo Não Tripulado)** equipado com sensores ambientais, sistema de sucção e filtragem de fumaça, monitoramento em tempo real e integração com aplicativo mobile para controle remoto e visualização de dados.

O sistema busca unir:

- Tecnologia;
- Sustentabilidade;
- Robótica aérea;
- Internet das Coisas (IoT);
- Monitoramento ambiental;
- Segurança operacional.

---

# Problema

Em ocorrências de incêndio, especialmente em ambientes confinados como edifícios residenciais, galpões e indústrias, a fumaça tóxica representa a principal causa de fatalidades, reduzindo drasticamente a visibilidade e dificultando o trabalho das equipes de resgate.

Atualmente, os métodos tradicionais de exaustão de fumaça dependem de equipamentos operados manualmente, exigindo a entrada prévia das equipes humanas em áreas de risco elevado.

O projeto busca solucionar essa lacuna através de uma primeira resposta aérea não tripulada, permitindo que o drone:

- Entre em áreas críticas antes das equipes humanas;
- Realize sucção emergencial de fumaça;
- Monitore a qualidade do ar;
- Auxilie no resgate e navegação em ambientes com baixa visibilidade;
- Gere corredores de ar respirável para evacuação.

---

# Objetivos

## Objetivo Geral

Desenvolver um sistema móvel de purificação de ar baseado em drone inteligente para monitoramento ambiental e sucção de fumaça tóxica em ambientes críticos.

## Objetivos Específicos

- Desenvolver um VANT com sistema de filtragem embarcado;
- Integrar sensores de qualidade do ar e gases;
- Monitorar dados ambientais em tempo real;
- Desenvolver aplicativo para controle remoto;
- Criar sistema de telemetria e comunicação IoT;
- Auxiliar operações de emergência e segurança.

---

# Alinhamento com os ODS da ONU

O projeto está alinhado aos seguintes Objetivos de Desenvolvimento Sustentável (ODS):

- **ODS 3 – Saúde e Bem-Estar**
- **ODS 9 – Indústria, Inovação e Infraestrutura**
- **ODS 11 – Cidades e Comunidades Sustentáveis**
- **ODS 13 – Ação Contra a Mudança Global do Clima**

---

# Tecnologias Utilizadas

| Camada | Tecnologia |
|---|---|
| Frontend Mobile | React Native |
| Linguagem Mobile | TypeScript |
| Backend | Node.js |
| Banco de Dados | Firebase Realtime Database |
| Comunicação | Wi-Fi / Bluetooth |
| Microcontrolador | ESP32 |
| Controladora de Voo | Pixhawk |
| Sensores | MQ, PM2.5, PM10, LiDAR |
| Navegação | GPS |
| Sistema Embarcado | C++ / Python |

---

# Arquitetura do Sistema

```txt
┌──────────────────────────────────────────────┐
│            Aplicativo Mobile                 │
│       React Native + TypeScript              │
└────────────────────┬─────────────────────────┘
                     │
┌────────────────────▼─────────────────────────┐
│         Backend e Comunicação IoT            │
│      Node.js + Firebase Realtime DB          │
└────────────────────┬─────────────────────────┘
                     │
┌────────────────────▼─────────────────────────┐
│           Sistema Embarcado VANT             │
│      ESP32 + Pixhawk + Sensores              │
└────────────────────┬─────────────────────────┘
                     │
┌────────────────────▼─────────────────────────┐
│       Sistema de Purificação de Ar           │
│     Sucção + HEPA + Umidificação             │
└──────────────────────────────────────────────┘
```

---

# Hardware

O drone será composto pelos seguintes componentes:

- Estrutura VANT;
- Motores Brushless;
- ESCs;
- Hélices;
- Controladora Pixhawk;
- ESP32;
- Sensores MQ para gases;
- Sensores PM2.5 e PM10;
- Sensor LiDAR;
- GPS;
- Sistema de sucção;
- Filtro HEPA;
- Umidificador ultrassônico;
- Bateria LiPo High-C.

---

# Aplicativo Mobile

O aplicativo será responsável pelo controle e monitoramento do drone em tempo real.

## Funcionalidades

- Controle de movimentação do drone;
- Visualização da localização em tempo real;
- Heatmap de dispersão de fumaça;
- Monitoramento de PM2.5 e PM10;
- Monitoramento de gases nocivos;
- Exibição de telemetria;
- Exibição do nível de bateria;
- Controle do sistema de sucção;
- Alertas de segurança;
- Controle manual e rotas automáticas.

---

# Backend

O backend será desenvolvido em **Node.js** e será responsável por:

- Comunicação em tempo real;
- Processamento de telemetria;
- Sincronização com Firebase;
- Gerenciamento de dados ambientais;
- Envio de alertas;
- Comunicação bidirecional com o drone.

---

# Funcionamento do Sistema

1. O drone realiza o monitoramento do ambiente;
2. Os sensores detectam fumaça e gases nocivos;
3. Os dados são enviados ao backend em tempo real;
4. O aplicativo exibe informações ambientais;
5. O sistema de sucção é ativado;
6. O ar passa pelo filtro HEPA;
7. O operador acompanha toda a operação remotamente.

---

# Casos de Uso

| Situação | Ação do Sistema |
|---|---|
| Incêndio em ambiente fechado | Sucção emergencial de fumaça |
| Alta concentração de gases | Alerta automático |
| Baixa visibilidade | Monitoramento remoto |
| Operação industrial | Purificação do ar |
| Queimadas | Monitoramento ambiental |

---

# Roadmap do Projeto

| Período | Atividade |
|---|---|
| Janeiro – Fevereiro | Pesquisa e planejamento |
| Março – Abril | Desenvolvimento do aplicativo |
| Maio – Junho | Integração de sensores |
| Julho – Agosto | Sistema de sucção e filtragem |
| Setembro – Outubro | Testes operacionais |
| Novembro – Dezembro | Refinamentos e documentação |

---

# Previsão Orçamentária

| Componente | Valor Estimado |
|---|---|
| Estrutura do VANT | R$ 1.100,00 |
| ESP32 + Pixhawk | R$ 450,00 |
| Sensores | R$ 350,00 |
| Sistema de Purificação | R$ 250,00 |
| Sistema de Alimentação | R$ 300,00 |
| **TOTAL** | **R$ 2.450,00** |

---

# Resultados Esperados

- Redução da concentração de fumaça em ambientes confinados;
- Monitoramento ambiental inteligente;
- Maior segurança em operações de resgate;
- Criação de corredores de ar respirável;
- Auxílio às equipes de bombeiros;
- Demonstração de viabilidade aerodinâmica do sistema.

---

# Futuras Implementações

- Inteligência Artificial para previsão de propagação de fumaça;
- Navegação autônoma avançada;
- Mapeamento 3D de ambientes;
- Comunicação 4G/5G;
- Sistema de múltiplos drones em rede;
- Dashboard web para monitoramento.

---

# Stakeholders

- Corpo de Bombeiros;
- Indústrias;
- Defesa Civil;
- Órgãos ambientais;
- Instituições de pesquisa;
- Equipe de desenvolvimento.

---

# Equipe de Desenvolvimento

Projeto desenvolvido como iniciativa acadêmica e tecnológica voltada à inovação sustentável, robótica aérea e monitoramento ambiental inteligente.

---

# Referências

- Organização Mundial da Saúde (OMS)
- ABNT NBR ISO/IEC 20924:2025
- Estudos sobre IoT e Robótica Aérea
- Sistemas embarcados com ESP32
- Monitoramento ambiental com sensores PM2.5 e PM10

---

# Contato

Em caso de dúvidas, sugestões ou contribuições, utilize as *Issues* deste repositório.
