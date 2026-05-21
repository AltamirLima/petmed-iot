# 🚀 Implementação da Solução — PetMed IoT

## 📌 Sobre a Implementação

O projeto **PetMed IoT** foi desenvolvido com foco em monitoramento inteligente de pets utilizando conceitos de:

* Internet das Coisas (IoT)
* Visão Computacional
* API REST
* Automação
* Monitoramento em tempo real

A solução integra dispositivos ESP32 simulados no Wokwi, comunicação HTTP, processamento com Python/OpenCV e um Dashboard Flask centralizado.

---

# 🧠 Arquitetura da Solução

A solução é composta por quatro módulos principais:

## 1️⃣ Coleira Inteligente

Responsável pelo monitoramento do pet.

### Funcionalidades:

* Temperatura simulada
* Batimentos cardíacos
* Nível de estresse
* Envio de dados via HTTP

### Tecnologias:

* ESP32
* Wokwi
* Arduino C++

---

## 2️⃣ Dispenser Automático

Responsável pela automação da alimentação.

### Funcionalidades:

* Alimentação automática
* Controle de acionamento
* Integração com API Flask

### Tecnologias:

* ESP32
* Wokwi
* HTTP REST

---

## 3️⃣ Visão Computacional

Responsável pela análise comportamental do animal.

### Funcionalidades:

* Captura da webcam
* Detecção de movimento
* Monitoramento comportamental

### Tecnologias:

* Python
* OpenCV
* Background Subtraction MOG2

---

## 4️⃣ Dashboard/API

Responsável pela centralização das informações.

### Funcionalidades:

* Exibição dos dados
* Recebimento das informações IoT
* Endpoints REST
* Monitoramento em tempo real

### Tecnologias:

* Flask
* Flask-CORS
* Python

---

# 🌐 Fluxo do Sistema

```text
ESP32/Wokwi
      ↓
HTTP REST
      ↓
API Flask
      ↓
Dashboard
      ↓
Monitoramento em tempo real
```

---

# 📂 Estrutura do Projeto

```text
petmed_iot/
│
├── assets/
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
├── README.md
└── DESCRICAO_PROJETO.md
```

---

# ▶️ Como Executar o Projeto

## 1️⃣ Clonar o repositório

```bash
git clone https://github.com/AltamirLima/petmed-iot.git
```

---

## 2️⃣ Entrar na pasta

```bash
cd petmed-iot
```

---

## 3️⃣ Instalar dependências

```bash
pip install -r requirements.txt
```

---

# ▶️ Executando os módulos

## Dashboard/API

```bash
python python/dashboard.py
```

Abrir no navegador:

```text
http://localhost:5000
```

---

## Coleira Inteligente

```bash
python python/coleira_inteligente.py
```

---

## Dispenser Automático

```bash
python python/dispenser.py
```

---

## Visão Computacional

```bash
python python/visao_computacional.py
```

---

# 📡 Comunicação da Solução

Os módulos utilizam comunicação HTTP REST.

Exemplo de payload enviado:

```json
{
  "temperatura": 38.2,
  "batimentos": 92,
  "stress": "baixo"
}
```

---

# 📊 Tecnologias Utilizadas

| Tecnologia | Finalidade          |
| ---------- | ------------------- |
| Python     | Backend             |
| Flask      | API/Dashboard       |
| OpenCV     | Visão Computacional |
| ESP32      | IoT                 |
| Wokwi      | Simulação           |
| HTTP REST  | Comunicação         |

---

# ⭐ Diferenciais da Solução

* Integração completa entre IoT e IA
* Monitoramento em tempo real
* Dashboard centralizado
* Simulação funcional no Wokwi
* Uso de OpenCV
* Arquitetura modular
* API REST integrada

---

# 👥 Integrantes

| Nome                       | RM       |
| -------------------------- | -------- |
| Olavo Porto Neves          | RM563558 |
| Altamir Lima               | RM562906 |
| Felipe Conte               | RM562248 |
| Luiz Gustavo               | RM564495 |
| Pedro Henrique Dias França | RM561940 |

---

# 📌 Conclusão

O PetMed IoT demonstra como tecnologias modernas podem ser utilizadas para automatizar e monitorar o cuidado animal.

O projeto integra IoT, automação, API REST e Inteligência Artificial em uma única solução funcional e escalável.
