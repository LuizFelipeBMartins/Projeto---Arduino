# Projeto Final - Jogo GENIUS com arduíno
O projeto que será realizado é uma reprodução funcional do jogo de memória Genius, onde uma sequência é feita nos LEDs e o jogador deve apertar os botões de modo a respeitar essa sequência. A cada nova rodada a sequência fica maior.
## Materiais utilizados:
- 1x - Arduíno UNO
- 1x - Breadboard (placa de ensaio)
- 18x - Fios jumpers (macho-macho)
- 4x - Botões (bush buttom)
- 1x - Buzzer
- 4x - Resistores 220Ω
- 4x - LEDs(um de cada cor: vermelho, verde, azul e amarelo)
### Ligações:
- LEDs:
  - LED 1 (vermelho): anodo no pino 2 e catodo no GND com resistor de 220Ω
  - LED 2 (verde): anodo no pino 4 e catodo no GND com resistor de 220Ω
  - LED 3 (azul): anodo no pino 6 e catodo no GND com resistor de 220Ω
  - LED 4 (amarelo): anodo no pino 8 e catodo no GND com resistor de 220Ω
- Botões:
  - Botão 1: um lado no pino 3 e o outro no GND
  - Botão 2: um lado no pino 5 e o outro no GND
  - Botão 3: um lado no pino 7 e o outro no GND
  - Botão 4: um lado no pino 9 e o outro no GND
- Buzzer:
  - Anodo no pino 12 e catodo no GND

![Projeto no tinkercad](https://github.com/user-attachments/assets/505a42ad-a2af-4929-9902-31c1f99a8eb4)

#### Funcionamento:
Uma sequência é mostrada com os LEDs piscando enquanto o buzzer emite um som diferente para cada cor. O jogador deve pressionar os botões na sequência indicada. Se ele acertar, uma nova sequência é gerada em cima da sequência pré existente. Se errar, é emitido um som de erro, todos os LEDs piscam e recomeça uma nova sequência com apenas um LED piscando novamente.
##### 1. Início:
Com o começo do funcionamento, o arduíno executa a função setup():
  - Botões: pinos são configurados como entrada de informações
  - LEDs: pinos são configurados como saída (liga ou desliga os LEDs)
  - Buzzer: pino é configurado como saída para emissão de som
##### 2. Rodadas:
O código continua com a função loop(), que determina ações contínuas para que o jogo possa fluir sem parar. Os LEDs e o buzzer exibem a sequência que o jogador deve apertar, e os botões enviam informações para o arduíno.
##### 3. Desenvolvimento e progressão:
A cada nova rodada que o jogador acerta, mais uma "piscada" é executada, fazendo que seja mais difícil que a pessoa acerte. Caso o jogador erre, todos os LEDs piscam e uma sequência nova é gerada, de modo a recomeçar o jogo desde o início.

###### Imagem real do projeto:
![WhatsApp Image 2024-09-20 at 21 21 43](https://github.com/user-attachments/assets/823b36d9-764f-49e6-a1d4-c738027769cb)


