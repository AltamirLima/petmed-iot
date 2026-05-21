# 🐾 PetMed IoT

Sistema inteligente para monitoramento de pets utilizando IoT, automação, visão computacional e dashboard web.

O objetivo do projeto é monitorar temperatura, atividade, alimentação e comportamento do pet em tempo real, utilizando dispositivos simulados no Wokwi, API Flask e análise comportamental via OpenCV.

---

## 👥 Integrantes

| Nome | RM |
|---|---|
| Olavo Porto Neves | RM563558 |
| Altamir Lima | RM562906 |
| Felipe Conte | RM562248 |
| Luiz Gustavo | RM564495 |
| Pedro Henrique Dias França | RM561940 |

---

## 🔗 Repositório GitHub


https://github.com/AltamirLima/petmed-iot

---

## 🎯 Problema Proposto

Muitos tutores possuem dificuldades em acompanhar a saúde e o comportamento do pet quando estão fora de casa.

Problemas comuns incluem:

- falta de monitoramento da temperatura corporal;
- ausência de controle alimentar;
- dificuldade para detectar comportamentos anormais;
- falta de informações sobre o bem-estar do animal.

O projeto **PetMed IoT** foi desenvolvido para resolver esse problema através de:

- IoT;
- Visão Computacional;
- Dashboard Web;
- Monitoramento remoto.

---

## 🚀 Tecnologias Utilizadas

### Backend
- Python
- Flask
- Flask-CORS

### Visão Computacional
- OpenCV
- Background Subtraction (MOG2)

### IoT
- ESP32 (simulado no Wokwi)
- HTTP REST API

### Dashboard
- Flask Dashboard

### Comunicação
- HTTP

---

## 🏗️ Arquitetura do Sistema

O sistema funciona através da integração entre dispositivos IoT, visão computacional e dashboard.

### Fluxo da aplicação

- Coleira Inteligente (ESP32) → API Flask
- Dispenser Automático (ESP32) → API Flask
- Webcam/OpenCV → API Flask
- API Flask → Dashboard Web

![Arquitetura](assets/arquitetura.png)

---

## 🤖 Inteligência Artificial

O projeto utiliza **Visão Computacional com OpenCV** para análise comportamental do pet.

Através da técnica de **Background Subtraction (MOG2)**, o sistema identifica movimentações e padrões comportamentais, permitindo detectar possíveis situações como:

- estresse;
- hiperatividade;
- movimentação intensa;
- ausência prolongada de atividade.

Esses dados são enviados para a API e podem ser visualizados no dashboard.

---

## ⚙️ Estrutura do Projeto

```txt
petmed_iot/
│
├── assets/
│   ├── arquitetura.png
│   ├── dashboard.png
│   ├── visao.png
│   ├── coleira.png
│   └── dispenser.png
│
├── python/
│   ├── dashboard.py
│   ├── coleira_inteligente.py
│   ├── dispenser.py
│   └── visao_computacional.py
│
├── wokwi/
│
├── requirements.txt
│
└── README.md
```

---

## ▶️ Como Executar o Projeto

### 1. Instalar dependências

```bash
pip install -r requirements.txt
```

---

### 2. Executar o Dashboard

```bash
python dashboard.py
```

---

### 3. Executar a Coleira Inteligente

```bash
python coleira_inteligente.py
```

---

### 4. Executar o Dispenser

```bash
python dispenser.py
```

---

### 5. Executar a Visão Computacional

```bash
python visao_computacional.py
```

---

### 6. Abrir no navegador

```text
http://localhost:5000
```

---

## 🌐 Endpoints da API

### Coleira

```http
GET /api/coleira
POST /api/coleira
```

---

### Dispenser

```http
GET /api/dispenser
POST /api/dispenser
```

---

### Visão Computacional

```http
GET /api/visao
POST /api/visao
```

---

### Status do Sistema

```http
GET /api/status
```

---

## 📦 Exemplo de Dados

### Coleira Inteligente

```json
{
  "temperatura": 38.2,
  "batimentos": 92,
  "stress": "baixo",
  "gps": {
    "lat": -23.5505,
    "lng": -46.6333
  }
}
```

---

### Dispenser

```json
{
  "status": "alimentado",
  "horario": "08:00"
}
```

---

### Visão Computacional

```json
{
  "movimento": 50233,
  "status": "movimento_intenso"
}
```

---

## 📈 Regras de Negócio

O sistema foi desenvolvido para:

- monitorar atividade do pet;
- identificar movimentações anormais;
- acompanhar alimentação;
- registrar temperatura e sinais vitais;
- fornecer monitoramento remoto via dashboard.

---

## 🔍 Monitoramento em Tempo Real

Os sensores simulados enviam dados continuamente para a API Flask, permitindo:

- atualização dinâmica;
- monitoramento remoto;
- visualização em tempo real;
- integração entre IoT e IA.

---

## ✅ Status do Projeto

Projeto funcional contendo:

- ✔️ IoT com ESP32 (Wokwi)
- ✔️ Dashboard Flask
- ✔️ API REST
- ✔️ OpenCV
- ✔️ Visão Computacional
- ✔️ Monitoramento remoto
- ✔️ Integração entre módulos

---

## 🎥 Demonstração em Vídeo

No vídeo serão apresentados:

- arquitetura do sistema;
- dispositivos IoT;
- dashboard;
- endpoints;
- visão computacional;
- comunicação entre módulos;
- funcionamento completo do sistema.

---

## 📄 Licença

Projeto acadêmico desenvolvido para fins educacionais.
