#include <Servo.h>
Servo myservo;  
int ledslot1 = 3;
int ledslot2 = 4; 
int gateled1 = 5;
int gateled2 = 6;
int slot1 = 8;
int slot2 = 9;
intgatesensor=10;   

void setup() {
myservo.attach(11);
pinMode(slot1,INPUT);
pinMode(slot2,INPUT); 
pinMode(gatesensor,INPUT);
pinMode(ledslot1,OUTPUT);
pinMode(ledslot2,OUTPUT);
pinMode(gateled1,OUTPUT);
pinMode(gateled2,OUTPUT);
}

void loop() {
  if (digitalRead(gatesensor)==LOW &&digitalRead(slot1)==HIGH &&digitalRead(slot2)==HIGH ){
myservo.write(90);
digitalWrite(ledslot1,HIGH);
digitalWrite(ledslot2,HIGH);
digitalWrite(gateled1,HIGH);
digitalWrite(gateled2,LOW);
    delay(5000);
  }

if (digitalRead(gatesensor)==LOW &&digitalRead(slot1)==LOW &&digitalRead(slot2)==HIGH ){
myservo.write(90);
digitalWrite(ledslot1,LOW);
digitalWrite(ledslot2,HIGH);
digitalWrite(gateled1,HIGH);
digitalWrite(gateled2,LOW);
  }
  if (digitalRead(gatesensor)==LOW &&digitalRead(slot1)==HIGH&&digitalRead(slot2)==LOW ){
myservo.write(90);
digitalWrite(ledslot1,HIGH);
}
