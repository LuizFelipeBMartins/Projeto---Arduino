# Sequencial de 3 Canais
No código disponibilizado pelo professor, é feito um sequencial de acender e apagar LEDs.
## Materiais
- Arduíno
- 3 LEDs
- 3 resistores(220Ω a 1kΩ)
- Jumpers e protoboard
### Código
O sketch foi disponibilizado pelo professor e colado na IDE do arduíno:

/*
  Controle Sequencial de Três LEDs
  Este exemplo demonstra como controlar três LEDs conectados aos pinos 4, 5 e 6 de um Arduino,
  acendendo cada um deles sequencialmente com um intervalo de um segundo.

  Elaborado/Adaptado por Epaminondas Lage
*/

// Definição dos pinos dos LEDs
const int ledPin1 = 4;
const int ledPin2 = 5;
const int ledPin3 = 6;

void setup() {
  // Define os pinos dos LEDs como saídas
  pinMode(ledPin1, OUTPUT);
  pinMode(ledPin2, OUTPUT);
  pinMode(ledPin3, OUTPUT);
}

void loop() {
  // Acende o primeiro LED e espera 1 segundo
  digitalWrite(ledPin1, HIGH);
  delay(1000);
  digitalWrite(ledPin1, LOW);
  
  // Acende o segundo LED e espera 1 segundo
  digitalWrite(ledPin2, HIGH);
  delay(1000);
  digitalWrite(ledPin2, LOW);
  
  // Acende o terceiro LED e espera 1 segundo
  digitalWrite(ledPin3, HIGH);
  delay(1000);
  digitalWrite(ledPin3, LOW);
}

#### Imagem real do projeto

![98769b2e-c433-40d5-b81a-02b6b9dc1d9a](https://github.com/user-attachments/assets/de195ea2-650a-4823-b734-c5a42ae94f5d)
