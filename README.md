# ECE387_Microprocessor_Prerequisite
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
  //S
  flash(250);
  flash(250);
  flash(250);
  delay(300);
  
  //O
  flash(600);
  flash(600);
  flash(600);
  delay(300);

  //S
  flash(250);
  flash(250);
  flash(250);
  delay(1000);
}

//this section of code defines the term "flash"
  void flash(int timex)
  {
    digitalWrite(ledPin, HIGH);
    delay(timex);
    digitalWrite(ledPin,LOW);
    delay(timex);
  }
