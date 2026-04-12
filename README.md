# 🔗 Nexus Dev - Sistema de Monitoramento de Luminosidade

## 📌 Descrição

Este projeto foi desenvolvido pela empresa (fictícia) **Nexus Dev** com o objetivo de monitorar a luminosidade do ambiente de armazenamento da (fictícia) Vinheria Agnello.

A exposição à luz, especialmente aos raios ultravioletas, pode comprometer a qualidade dos vinhos, causando alterações químicas indesejadas. Pensando nisso, criamos um sistema inteligente capaz de identificar e sinalizar níveis de luminosidade inadequados.

---

## ⚙️ Tecnologias e Componentes

- Arduino Uno (ATmega328P)
- Sensor LDR (Light Dependent Resistor)
- Resistores (10kΩ e 220Ω)
- LEDs (Verde, Amarelo e Vermelho)
- Buzzer
- Display LCD 16x2
- Protoboard
- Tinkercad

---

## 🧠 Funcionamento do Sistema

O sensor LDR capta a luminosidade do ambiente e envia um sinal analógico ao Arduino.

O microcontrolador utiliza o **ADC (Conversor Analógico-Digital)** para transformar esse sinal em valores digitais (0 a 1023). Em seguida, utilizamos a função `map()` para converter esses valores em uma escala de 0 a 100%, facilitando a interpretação.

---

## 🚦 Estados do Sistema

Com base na porcentagem de luminosidade, o sistema define três estados:

- 🟢 **0% a 30%** → Ambiente ideal (OK)  
- 🟡 **31% a 60%** → Nível de alerta (aciona buzzer)  
- 🔴 **61% a 100%** → Problema (excesso de luz)  

---

## 🔔 Sistema de Alerta

- LED Verde → Ambiente adequado  
- LED Amarelo → Alerta + buzzer por 3 segundos  
- LED Vermelho → Situação crítica  

---

## 🖥️ Interface do Usuário

O display LCD apresenta:

- Nome do grupo (Nexus Dev 🔗)
- Percentual de luminosidade
- Estado do ambiente
- Ícones visuais:
  - 🍷 Taça cheia → OK  
  - ⚠️ Taça rachada → ALERTA  
  - ❌ X → PROBLEMA  

---

## ▶️ Tinkercad

https://www.tinkercad.com/things/4SPotkq88u8-sensor-de-iluminacao-vinheira-agnello-cp1-edge-computing?sharecode=yNmauR47zf7lj8XgIcYD7ijipPQyV0DPyxfF5GH_uKo

---

## 🎥 Vídeo Explicativo

[(Adicionar link do vídeo aqui)](https://youtu.be/irMgv1CuT1U)

---

## ⚠️ Dificuldades Enfrentadas

- Problemas com a protoboard, pois utilizamos inicialmente uma unidade danificada sem saber, o que gerou falhas nas conexões e perda de tempo na identificação do erro.
- Calibração do sensor LDR, devido à variação dos valores e sensibilidade do componente, sendo necessário realizar diversos testes para ajustar o comportamento do sistema.

---

## 👨‍💻 Integrantes - Nexus Dev

- RM573282 - Isac Nilton Fernandes de Oliveira  
- RM570206 - João Benedito de Oliveira Simplicio  
- RM568732 - Thiago Souza de Lima  
- RM571340 - Julia Souza Matarazzo  
- RM572830 - Matheus Akira Aso  
