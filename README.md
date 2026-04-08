# 🔗 Nexus Dev - Sistema de Monitoramento de Luminosidade

## 📌 Descrição

Este projeto foi desenvolvido para a Vinheria Agnello com o objetivo de monitorar a luminosidade do ambiente onde os vinhos são armazenados.

Sabemos que a exposição à luz pode comprometer a qualidade dos vinhos, especialmente devido à ação de raios ultravioletas, que causam alterações químicas indesejadas.

O sistema utiliza um sensor LDR para captar a luminosidade e, com base nesses dados, aciona diferentes alertas visuais e sonoros.

---

## ⚙️ Tecnologias e Componentes

- Arduino Uno (ATmega328P)
- Sensor LDR
- Resistores (10kΩ e 220Ω)
- LEDs (Verde, Amarelo e Vermelho)
- Buzzer
- Display LCD 16x2
- Protoboard
- Tinkercad

---

## 🧠 Funcionamento do Sistema

O LDR capta a luminosidade do ambiente e envia um sinal analógico ao Arduino.

O microcontrolador utiliza o conversor ADC (Analógico/Digital) para transformar esse sinal em valores digitais (0 a 1023), que são posteriormente convertidos em porcentagem utilizando a função `map()`.

Com base nesses valores, o sistema classifica o ambiente em três estados:

- 🟢 **0% a 30%** → Ambiente ideal (OK)
- 🟡 **31% a 70%** → Nível de alerta (aciona buzzer)
- 🔴 **71% a 100%** → Problema (excesso de luz)

---

## 🔔 Sistema de Alerta

- LED Verde: ambiente adequado
- LED Amarelo: nível de alerta + buzzer por 3 segundos
- LED Vermelho: nível crítico

---

## 🖥️ Interface

O display LCD apresenta:

- Mensagem inicial com o nome do grupo
- Percentual de luminosidade
- Estado atual do ambiente

---

## 💻Projeto no TinkerCad

https://www.tinkercad.com/things/4SPotkq88u8-sensor-de-iluminacao-vinheira-agnello-cp1-edge-computing?sharecode=yNmauR47zf7lj8XgIcYD7ijipPQyV0DPyxfF5GH_uKo

---

## 🎥 Vídeo Demonstrativo

(Colocar link aqui)

---

## 👨‍💻 Grupo
RM 573282 - Isac Nilton Fernandes de Oliveira
RM - João Benedito de Oliveira Simplicio
RM - Julia Matarazzo
RM - Matheus Akira
RM - Thiago

🔗 Nexus Dev
