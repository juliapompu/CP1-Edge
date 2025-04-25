# CP1 - Edge Computing 🍷💡  
**Projeto: Vinheria Agnello – Monitoramento de Luminosidade com Arduino**

Este repositório contém o projeto desenvolvido para o Checkpoint 01 da disciplina *Edge Computing & Computer Systems* (FIAP - 2025). Trata-se de um sistema físico e funcional montado com Arduino, focado no monitoramento da **luminosidade** do ambiente de armazenamento da Vinheria Agnello, com o objetivo de preservar a qualidade dos vinhos.

---

## 🧩 Descrição do Desafio

A Vinheria Agnello deseja expandir suas operações para o digital sem abrir mão da qualidade no atendimento e no cuidado com os produtos. Nosso desafio foi propor um sistema embarcado capaz de detectar condições ambientais inadequadas — neste caso, **luminosidade excessiva**.

### Funcionalidades implementadas:

- Leitura do nível de luminosidade com sensor LDR;
- LEDs sinalizadores:
  - ✅ **Verde:** ambiente adequado;
  - ⚠️ **Amarelo:** luminosidade em alerta;
  - ❌ **Vermelho:** luminosidade inaceitável;
- Acionamento de buzzer por 3 segundos quando houver alerta;
- Buzzer soa novamente se o alerta persistir.

---

## 💡 Solução Técnica

O sistema foi **montado fisicamente** e também **simulado no Tinkercad**.

### 🔗 Simulação no Tinkercad

[Acesse o projeto clicando aqui](https://www.tinkercad.com/things/35Ed8K8AP9W-cp1-edge-computing/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard)

### 🖼️ Imagem da simulação no Tinkercad

> [image](https://github.com/user-attachments/assets/cb7a0da0-6bf6-4799-8cf4-60dec95e4af5)

## 🔧 Componentes Utilizados

- 1 × **Arduino Uno R3** (`U1`)  
- 1 × **Fotorresistor (LDR)** (`Rluz`)  
- 1 × **Resistor de 220 Ω** (`R4`) – usado no divisor de tensão com o LDR  
- 3 × **LEDs**:
  - 1 × Vermelho (`Dled1`)
  - 1 × Verde (`Dled2`)
  - 1 × Amarelo (`Dled3`)
- 3 × **Resistores de 220 Ω** (`R1`, `R2`, `R3`,) – conectados aos LEDs  
- 1 × **Buzzer Piezoelétrico** (`PIEZO1`)  
- 1 × **Resistor de 500 Ω** (`R5`) – associado ao buzzer  
- Cabos Jumpers  
- 1 × Protoboard

---

## 🛠️ Montagem do Circuito (Resumo)

- **LDR + resistor de 220Ω**: leitura feita no pino analógico A0 (formando um divisor de tensão);
- **LEDs**: conectados aos pinos digitais:
  - Verde → pino 9
  - Amarelo → pino 8
  - Vermelho → pino 7
- **Buzzer**: conectado ao pino digital 6;
- Resistores de 220 Ω conectados em série com cada LED;
- Resistor de 500 Ω conectado ao buzzer para limitar corrente;
- GND e 5V do Arduino distribuídos nos trilhos laterais da protoboard.

---

## 💾 Execução do Projeto

1. Monte o circuito conforme o esquema elétrico;
2. Faça o upload do código na placa usando a IDE do Arduino;
3. Ajuste a luminosidade manualmente (ou use o controle do Tinkercad) para testar os diferentes comportamentos do sistema;
4. Observe os sinais visuais (LEDs) e sonoros (buzzer) em tempo real.

---

## 👥 Integrantes do Grupo

- **Julia Pompeu** – 561955  
- **Laura Tigre Amaral** – 565281  
- **Áurea Sardinha Carminato** – 563837  
- **Giovana Parreira** – 562275  
- **Ben-Hur Iung de Lima Ferreira** – 561564

---
