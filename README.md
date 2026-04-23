# Sistema de Monitoramento de Temperatura com Display LED (Arduino)

## Descrição

Projeto e Implementação de renderização gráfica manual com fonte 8x8 personalizada e scroll de texto para leitura de temperatura utilizando sensor DHT11, com exibição em matriz de LEDs. 


## Funcionalidades

* Leitura de temperatura ambiente utilizando sensor DHT11
* Exibição da temperatura em matriz de LEDs 8x8
* Scroll de texto contínuo no display
* Renderização de caracteres com fonte personalizada (8x8)
* Manipulação de bits para controle direto da matriz LED
* Monitoramento e depuração via Serial Monitor

## Tecnologias Utilizadas

* Arduino (C/C++)
* Sensor DHT11
* Módulos de matriz LED 8x8 (MAX7219)
* Biblioteca LedControl

## Componentes Utilizados

* Arduino Uno
* Sensor de temperatura DHT11
* 4x módulos de matriz LED 8x8 (MAX7219)
* Resistores e jumpers

## Funcionamento do Sistema

1. O sensor DHT11 realiza a leitura da temperatura ambiente.
2. O valor da temperatura é processado e convertido em texto (ex: "TEMP:25C").
3. O sistema gera a representação gráfica dos caracteres utilizando uma fonte 8x8 personalizada.
4. Um buffer de exibição é criado para armazenar os pixels da mensagem.
5. A mensagem é exibida no display com efeito de scroll contínuo da esquerda para a direita.

## Diferenciais Técnicos

* Implementação manual de fonte de caracteres (bitmap 8x8)
* Criação de algoritmo próprio de scroll de texto
* Manipulação de bits para renderização gráfica em hardware
* Controle direto da matriz LED sem uso de bibliotecas de alto nível para texto

## ▶ Como Executar

1. Monte o circuito conforme os componentes listados
2. Abra o código na Arduino IDE
3. Instale a biblioteca necessária:

   * LedControl
4. Faça o upload do código para o Arduino
5. Abra o Serial Monitor para acompanhar a leitura da temperatura

