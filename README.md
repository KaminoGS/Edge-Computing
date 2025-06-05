# 🌊 Sistema Inteligente de Monitoramento de Bueiros para Prevenção de Enchentes com Edge Computing 🚦

Este `README` descreve um sistema nosso projetado para **identificar bueiros obstruídos** e **priorizar sua manutenção**, com o objetivo principal de otimizar a drenagem urbana e prevenir inundações. A solução proposta utiliza sensoriamento de nível e fluxo de água em tempo real, fornecendo alertas visuais sobre o estado de cada bueiro.

## ✨ Visão Geral do Projeto
O projeto foca na criação de um dispositivo inteligente que atua na borda (Edge-Computing), analisando dados localmente para uma resposta rápida e eficiente. Ele monitora continuamente as condições dentro dos bueiros, permitindo uma gestão proativa da infraestrutura de drenagem.


## 🛠️ Como Funciona o Sistema
O sistema opera com base na coleta e análise de dados de dois parâmetros cruciais dentro do bueiro:

### 1. 📏 Monitoramento de Nível da Água
* Um **sensor de distância** (simulado por um **HC-SR04**) é responsável por receber valores sobre o **nível da água**.
* Essa medição é feita através da distância entre o sensor e a superfície da água.

### 2. 💧 Monitoramento de Fluxo da Água
* Outro sensor, um **Potenciômetro** (que irá simular um sensor de fluxo da água), irá receber valores sobre o **fluxo da água**.
* No simulador, esse valor é **alterável manualmente** através do potenciômetro.


## 🚦 Lógica de Operação e Identificação de Status
O dispositivo analisa as leituras dos sensores em tempo real e aciona indicadores luminosos para comunicar o estado do bueiro, de acordo com as seguintes condições:

### ✅ Drenagem Correta (LED Verde Ligado)
* **Condição:** Quando a água estiver em um fluxo maior que **(x)**, E o nível estiver abaixo de **(y)**.
* **Significado:** O bueiro está drenando a água corretamente.
* **Indicação:** Um **LED Verde** permanecerá ligado.

### ⚠️ Necessidade de Manutenção (LED Amarelo Ligado)
* **Condição:** Quando o fluxo de água permanecer maior que **(x)**, E o nível estiver acima de **(y)**.
* **Significado:** O bueiro não está drenando com a eficiência necessária e necessita de manutenção ou reforma.
* **Indicação:** Um **LED Amarelo** permanecerá ligado.

### ⛔ Obstrução Completa (LED Vermelho Piscando)
* **Condição:** Quando o fluxo de água for **0** E o nível estiver acima de **(y)**.
* **Significado:** O bueiro está completamente obstruído e necessita de reparo urgente.
* **Indicação:** Um **LED Vermelho** ficará piscando.
  
###Links
* **Vídeo:**
* **Simulação:** https://www.tinkercad.com/things/5bR5Phkhm9R-gs?sharecode=qurhPJYzqIoeAr7bV6eBquDAodL0CJqNTPAb8C7lMiE
