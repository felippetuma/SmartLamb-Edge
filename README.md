# SmartLamp
💡 Smart Lamb

Sistema IoT desenvolvido para monitoramento e gerenciamento inteligente de lâmpadas utilizando ESP32, sensor de luminosidade, backend hospedado na Amazon AWS e Docker.

O projeto permite receber informações de luminosidade coletadas pelo ESP32, disponibilizá-las através de uma API e realizar operações de gerenciamento das lâmpadas, como cadastro, ativação, desativação e consulta de status.

📌 Sobre o projeto

O Smart Lamb é uma solução baseada em Internet das Coisas (IoT) desenvolvida para demonstrar a comunicação entre um dispositivo físico e uma infraestrutura de software hospedada em nuvem.

O ESP32 atua como o dispositivo IoT responsável pela coleta das informações provenientes do sensor de luminosidade. Esses dados são enviados para um backend hospedado na Amazon AWS, onde são processados e disponibilizados através de uma API.

Para facilitar os testes e a comunicação com o backend, utilizamos o Postman, permitindo visualizar os dados recebidos e realizar requisições para gerenciamento das lâmpadas.

Fluxo geral do sistema
┌──────────────────────┐
│   Sensor de          │
│   Luminosidade       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│        ESP32         │
│      Dispositivo     │
│         IoT          │
└──────────┬───────────┘
           │
           │ Dados de luminosidade
           ▼
┌──────────────────────┐
│     Amazon AWS       │
│                      │
│  ┌────────────────┐  │
│  │     Docker     │  │
│  │                │  │
│  │    Backend     │  │
│  └────────────────┘  │
└──────────┬───────────┘
           │
           │ API
           ▼
┌──────────────────────┐
│       Postman        │
│                      │
│ • Consultar dados    │
│ • Cadastrar lâmpada  │
│ • Ligar lâmpada      │
│ • Desligar lâmpada   │
│ • Consultar status   │
└──────────────────────┘
🎯 Objetivos

O projeto foi desenvolvido com os seguintes objetivos:

Aplicar conceitos de Internet das Coisas (IoT);
Utilizar o ESP32 para aquisição de dados de sensores;
Monitorar níveis de luminosidade;
Estabelecer comunicação entre um dispositivo físico e um servidor;
Hospedar o backend em infraestrutura de nuvem utilizando a Amazon AWS;
Utilizar Docker para execução e gerenciamento do backend;
Desenvolver uma API para comunicação entre os componentes;
Realizar testes e gerenciamento da aplicação através do Postman;
Permitir o gerenciamento do estado das lâmpadas;
Demonstrar uma arquitetura integrada entre hardware, software e cloud computing.
⚙️ Funcionalidades

💡 Gerenciamento de lâmpadas

O sistema permite realizar operações relacionadas às lâmpadas através da API:

Cadastrar uma nova lâmpada;
Consultar lâmpadas cadastradas;
Ativar uma lâmpada;
Desligar uma lâmpada;
Consultar o status atual da lâmpada.
🌞 Monitoramento de luminosidade

O sensor conectado ao ESP32 realiza a leitura da luminosidade do ambiente.

As informações coletadas são enviadas para o backend, permitindo:

Receber os dados do sensor;
Armazenar/processar as informações no backend;
Consultar os dados recebidos;
Verificar o nível de luminosidade do ambiente.
🧩 Tecnologias utilizadas
Tecnologia	Função
ESP32	Dispositivo IoT responsável pela comunicação e coleta dos dados
Sensor de luminosidade	Mede a luminosidade do ambiente
Backend	Processa as requisições e informações recebidas
Amazon AWS	Infraestrutura de hospedagem do sistema
Docker	Containerização e execução do backend
Postman	Testes e comunicação com a API
API REST	Comunicação entre o cliente e o backend
🏗️ Arquitetura

O Smart Lamb possui uma arquitetura baseada na integração entre hardware, API e infraestrutura em nuvem.

1. Dispositivo IoT

O ESP32 é responsável pela comunicação com o sensor de luminosidade.

O dispositivo coleta as informações do ambiente e realiza o envio desses dados para o backend.

2. Comunicação com o backend

Os dados coletados pelo ESP32 são enviados para uma API disponibilizada pelo backend.

O backend recebe as requisições, processa as informações e disponibiliza os dados para consulta.

3. Infraestrutura AWS

O backend é hospedado em uma infraestrutura da Amazon AWS.

A aplicação utiliza Docker para criar um ambiente isolado e padronizado para execução do backend.

4. Postman

O Postman é utilizado como ferramenta de testes da API.

Por meio dele é possível enviar diferentes requisições para verificar o funcionamento do sistema.

🔌 Comunicação do ESP32

O ESP32 funciona como o componente IoT responsável pela comunicação entre o sensor físico e o sistema online.

De forma simplificada:

Sensor
   ↓
ESP32
   ↓
Internet
   ↓
API
   ↓
Backend
   ↓
Dados do sistema

O ESP32 coleta o valor fornecido pelo sensor e envia essa informação para o servidor através da comunicação de rede configurada no projeto.


## Vídeo Demostrativo da Smart Lamp

[YouTube](https://youtube.com/shorts/bkxifsv-vls?feature=share)

## Integrantes

- Arthur Nepomuceno RM: 572626 
- Davi Yuu Santos Toyota RM: 569557 
- Felipe Santana Motta RM: 570550 
- Felippe Tuma Costa RM: 569459
- Renan Martins da Silva RM: 569549 
- Yan da Silva Lima RM: 572373
