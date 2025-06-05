# Edge-Computing
#Sistema Inteligente de Monitoramento de Bueiros para Prevenção de Enchentes

Este documento descreve um sistema inovador para identificar bueiros obstruídos e priorizar sua manutenção, visando otimizar a drenagem urbana e prevenir inundações. A solução proposta utiliza sensoriamento de nível e fluxo de água em tempo real, fornecendo alertas visuais claros sobre o estado de cada bueiro.

Dispositivo que identifica nível e o fluxo de água dentro de bueiros.
Assim, identificando quais bueiros estão obstruídos e necessitam de manutenção.

#O sistema funciona da seguinte forma:
-Um sensor (HCSR04 - sensor de distância que irá simular um sensor de nível da água) irá receber valores sobre o nível da água (distância entre o sensor e a água).
Outro sensor (Potenciômetro - irá simular um sensor de fluxo da água) irá receber valores sobre o fluxo da água (alterável manualmente pelo potenciômetro no simulador).

-Quando a água estiver em um fluxo maior que (x), e o nível estiver abaixo de (y), o bueiro está drenando a água corretamente, o que manterá um LED verde ligado.

-Quando o fluxo de água permanecer maior que (x), e o nível estiver acima de (y), o bueiro não está drenando com a eficiência necessária e necessita de manutenção ou reforma, o que manterá um LED amarelo ligado.

-Quando o fluxo de água for 0 e o nível estiver acima de (y), o bueiro está completamente obstruído e necessita de reparo, o que manterá um LED vermelho piscando.
