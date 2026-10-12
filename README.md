# Arquitetura de Software e Protocolos de API

Este repositório é uma coletânea de exemplos práticos e didáticos sobre arquitetura de software, padrões de projeto, comunicação entre sistemas e diferentes estilos de implementação de APIs. Ele reúne materiais em Go e Python para abordar temas como:

- estilos arquiteturais fundamentais
- camadas, pipes-and-filters e microkernel
- APIs REST, gRPC, GraphQL, WebSocket e HTTP/3
- arquitetura de microsserviços
- gateways, mensageria e comunicação entre serviços

O objetivo é proporcionar uma visão prática e comparativa de como aplicações podem ser estruturadas e integradas em diferentes cenários.

---

## Visão geral

Este projeto foi organizado em três grandes blocos:

1. APIs e protocolos de comunicação
2. Estilos arquiteturais fundamentais
3. Microsserviços e integrações distribuídas

Cada módulo contém exemplos executáveis, pequenos estudos de caso e documentos explicativos que ajudam a entender o contexto e a implementação.

---

## Estrutura do repositório

```text
arquitetura-software/
├── apis/
│   ├── api-gateway-kong/
│   ├── protocolos-api-go/
│   └── protocolos-api-python/
├── estilos-fundamentais/
│   ├── 1.2-estilo-em-camadas/
│   ├── 1.3-pipes-and-filters/
│   └── 1.4-microkernel/
├── microsservicos/
│   ├── chassi-arquitetural/
│   ├── microsservicos-http/
│   └── microsservicos-rabbitmq/
└── README.md
```

---

## 1) APIs e protocolos

A pasta `apis/` reúne implementações didáticas de diferentes formas de comunicação entre sistemas.

### Inclui

- REST com HTTP/2 e HTTP/3
- GraphQL
- WebSocket
- gRPC
- API Gateway com Kong
- clientes e servidores em Go e Python

### Exemplos principais

- `apis/protocolos-api-go/`: implementações em Go com vários protocolos
- `apis/protocolos-api-python/`: versões equivalentes em Python
- `apis/api-gateway-kong/`: exemplo de API Gateway com Kong

Esses exemplos ajudam a comparar trade-offs entre os protocolos, como:

- simplicidade e conveniência de REST
- baixo acoplamento e streaming em gRPC
- flexibilidade de consulta em GraphQL
- comunicação em tempo real via WebSocket
- evolução e performance de HTTP/3

---

## 2) Estilos arquiteturais fundamentais

A pasta `estilos-fundamentais/` demonstra abordagens clássicas de arquitetura de software.

### Módulos

- `1.2-estilo-em-camadas`: arquitetura em camadas, com domínio, serviços e repositórios
- `1.3-pipes-and-filters`: processamento em fluxos encadeados por filtros
- `1.4-microkernel`: arquitetura com núcleo central e plugins extensíveis

Esses exemplos são excelentes para entender conceitos como:

- separação de responsabilidades
- acoplamento e coesão
- extensibilidade
- interface entre camadas e módulos

---

## 3) Microsserviços

A pasta `microsservicos/` mostra como separar sistemas em serviços independentes, com comunicação e gateway.

### Exemplos principais

- `microsservicos-http/`: comunicação entre microsserviços via HTTP
- `microsservicos-rabbitmq/`: integração com RabbitMQ para filas e mensagens assíncronas
- `chassi-arquitetural/`: estrutura base para uma aplicação distribuída

### Conceitos abordados

- API Gateway
- serviços independentes
- roteamento de requisições
- comunicação síncrona e assíncrona
- desacoplamento entre produtores e consumidores

---

## Tecnologias e linguagens

O repositório combina ferramentas e tecnologias comuns no ecossistema de software:

- Go
- Python
- Docker
- Kong API Gateway
- RabbitMQ
- gRPC
- GraphQL
- WebSocket
- HTTP/2 e HTTP/3

---

## Como navegar pelo repositório

Cada módulo possui seu próprio README e estrutura específica. Para executar um exemplo, recomenda-se entrar na pasta correspondente e seguir as instruções locais.

### Exemplos de execução

#### Python

```bash
cd estilos-fundamentais/1.2-estilo-em-camadas
python main.py
```

#### Go

```bash
cd microsservicos/microsservicos-http
go run .
```

> Em muitos casos, os subprojetos têm dependências próprias e README específicos para orientar a execução.

---

## objetivos didáticos

Este repositório foi pensado para:

- estudar arquitetura de software de forma prática
- comparar diferentes padrões e protocolos
- entender relações entre domínio, infraestrutura e comunicação
- servir como referência para projetos pessoais e estudos acadêmicos

---

## Contribuição

Este material é ideal para estudos, experimentação e aprendizado incremental. Se você quiser ampliar o repositório, pode:

- adicionar novos exemplos
- melhorar a documentação
- incluir comparativos entre protocolos
- expandir cenários de microsserviços

---

## Resumo

Este projeto funciona como uma base de estudos sobre arquitetura de software moderna, conectando teoria e prática com exemplos concretos. Ele é especialmente útil para quem quer entender:

- como sistemas são organizados em camadas
- como diferentes APIs se comunicam
- como microsserviços são implementados
- como a escolha de arquitetura impacta escalabilidade, manutenção e evolução do sistema

---

## Referências rápidas

- `estilos-fundamentais/` — fundamentos de arquitetura
- `apis/` — protocolos de API e integração
- `microsservicos/` — arquitetura distribuída e comunicação entre serviços

Se quiser explorar o repositório em ordem didática, comece pelos exemplos de arquitetura fundamental e depois avance para protocolos e microsserviços.
