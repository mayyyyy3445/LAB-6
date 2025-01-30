# LAB-6

This circuit is a simple LED control setup using an Arduino Uno.

Components and Connections:
	1.	Arduino Uno – The microcontroller controlling the LED.
	2.	LED (Blue) – The output component that will light up when powered.
	3.	Resistor (likely 220Ω or 330Ω) – Limits current to prevent LED damage.
	4.	Wires:
	•	Blue wire connects an Arduino digital pin (pin 9 or 10) to the positive (anode) leg of the LED.
	•	Black wire connects the negative (cathode) leg of the LED to GND.
	•	The resistor is in series with the LED to limit current.

How It Works:
	•	The Arduino can turn the LED ON or OFF by setting the digital pin HIGH (5V) or LOW (0V).
	•	The resistor prevents excessive current from damaging the LED.

Arduino Code Example:

const int ledPin = 9;  // LED connected to pin 9

void setup() {
  pinMode(ledPin, OUTPUT);  // Set LED pin as output
}

void loop() {
  digitalWrite(ledPin, HIGH);  // Turn LED ON
  delay(1000);                 // Wait 1 second
  digitalWrite(ledPin, LOW);   // Turn LED OFF
  delay(1000);                 // Wait 1 second
}


