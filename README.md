int pinROJO=12;
int pinAMARILLO=7;
int pinVERDE=6;
int Pulsador=2;




void loop() {
  Serial.println(digitalRead(3));
  if (digitalRead(3) == 1) {
    digitalWrite(11, HIGH);
    digitalWrite(12, LOW);
    digitalWrite(13, LOW);
  }
    else {
    pinMode(pinVERDE,OUTPUT);
    digitalWrite(pinVERDE,HIGH);
    delay(4000);
    pinMode(pinVERDE,OUTPUT);
    digitalWrite(pinVERDE,LOW);
    pinMode(pinAMARILLO,OUTPUT);
    digitalWrite(pinAMARILLO,HIGH);
    delay(1000);
    pinMode(pinAMARILLO,OUTPUT);
    digitalWrite(pinAMARILLO,LOW);
    pinMode(pinROJO,OUTPUT);
    digitalWrite(pinROJO,HIGH);
    delay(6000);
    pinMode(pinROJO,OUTPUT);
    digitalWrite(pinROJO,LOW);
    }
}
