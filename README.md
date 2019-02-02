//Kevin Doench

//ECE 387

//Section A

//Dr. Jamieson

//February 24, 2019

//The following code is the prerequesite assignment to build an SOS blinker

//using a microprocessor (Arduino, in my case).

//An SOS signal in Morse Code is: ... (S) --- (O) ...(S)


int ledPin = 8;

void setup() {

pinMode(ledPin,OUTPUT);

}


void loop() {

// put your main code here, to run repeatedly:

//S

digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(750);



//O

digitalWrite(ledPin, HIGH);

delay(750);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(750);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(750);

digitalWrite(ledPin, LOW);

delay(750);



//S

digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(250);



digitalWrite(ledPin, HIGH);

delay(250);

digitalWrite(ledPin, LOW);

delay(1000);



//Repeat

}
