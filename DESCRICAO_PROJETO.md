# 🐶 PetMed IoT — Descrição do Projeto

## 📌 Sobre o Projeto

O PetMed IoT é uma solução inteligente desenvolvida para monitoramento e automação de cuidados com animais domésticos utilizando Internet das Coisas (IoT), Inteligência Artificial e Visão Computacional.

O sistema foi criado com o objetivo de auxiliar tutores no acompanhamento remoto da saúde, comportamento e alimentação dos pets, centralizando as informações em um dashboard web integrado.

---

# 🎯 Objetivo

Desenvolver uma plataforma capaz de:

- Monitorar informações do pet em tempo real
- Automatizar alimentação
- Detectar movimentações e padrões comportamentais
- Centralizar os dados em uma API integrada
- Aplicar conceitos de IoT e Inteligência Artificial

---

# 🛠️ Tecnologias Utilizadas

## Backend
- Python
- Flask
- Flask-CORS

## IoT
- ESP32
- Wokwi
- Comunicação HTTP REST

## Inteligência Artificial
- OpenCV
- Background Subtraction (MOG2)

## Frontend
- Dashboard Flask

---

# 🧠 Funcionamento do Sistema

O sistema é composto por três módulos principais:

## 1️⃣ Coleira Inteligente

Responsável pelo monitoramento do animal através de sensores simulados no ESP32/Wokwi.

Dados coletados:
- Temperatura
- Batimentos cardíacos
- Estresse

---

## 2️⃣ Dispenser Automático

Responsável pela automação da alimentação do pet.

Funcionalidades:
- Alimentação automática
- Controle de horários
- Integração com API

---

## 3️⃣ Visão Computacional

Responsável pela análise comportamental utilizando OpenCV.

O sistema utiliza:
- Captura de webcam
- Detecção de movimento
- Identificação de movimentações anormais

---

# 🌐 Integração

Todos os módulos se comunicam com uma API Flask através de HTTP REST.

A API centraliza:
- Dados da coleira
- Dados do dispenser
- Dados da visão computacional

Essas informações são exibidas em um Dashboard Web.

---

# 📊 Diferenciais do Projeto

- Integração completa entre IoT e IA
- Monitoramento em tempo real
- Dashboard centralizado
- Simulação funcional com Wokwi
- Uso de Visão Computacional
- Estrutura modular e organizada

---

# 👥 Integrantes

| Nome | RM |
|---|---|
| Olavo Porto Neves | RM563558 |
| Altamir Lima | RM562906 |
| Felipe Conte | RM562248 |
| Luiz Gustavo | RM564495 |
| Pedro Henrique Dias França | RM561940 |

---

# 📌 Conclusão

O PetMed IoT demonstra a aplicação prática de tecnologias modernas para solução de problemas reais relacionados ao cuidado animal.

O projeto integra monitoramento, automação e inteligência artificial em uma única plataforma, proporcionando maior controle e acompanhamento do bem-estar dos pets.
