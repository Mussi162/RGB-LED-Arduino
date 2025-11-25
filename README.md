# 🎨 RGB-LED-Arduino
Projeto Arduino que controla as cores de um LED RGB usando três fotoresistores (LDRs), criando um sistema interativo onde a intensidade da luz ambiente determina as cores exibidas.

🌐 Links do Projeto 🔗 https://www.tinkercad.com/things/3n8YN0YVdid-rgb-led

Este projeto utiliza três fotoresistores para capturar os níveis de luminosidade e traduzi-los em cores RGB em tempo real. Cada fotoresistor controla um canal de cor específico (Vermelho, Verde, Azul) do LED RGB, criando cores dinâmicas baseadas nas condições de iluminação do ambiente.
---

🛠 CFerramentário utilizado:

* Tinkercad 
* 1x Arduino Uno ou similar
* 1x LED RGB (cátodo comum)
* 3x Fotoresistores (LDRs)
* 3x Resistores de 10kΩ (para os LDRs)
* 3x Resistores de 220Ω (para o LED RGB)
* Protoboard e fios jumper
---

Lógica do Sistema: Cada LDR le os valore entre 0-1023, utilizando as entradas analógicas, baseado na luz do ambiente.
Os valores são convertidos para escala PWM(0-255).
Esses valores controlam a intensidade de cada cor no LED RGB
O loop contínuo repete o processo a cada 500ms.
