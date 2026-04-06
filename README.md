# Automatic-night-lamp
#code
int ldrPin=A0;
int ledPin=13;
int ldrValue=0;
void setup(){
  pinMode(ledPin,OUTPUT);
  Serial.begin(9600);
}
void loop(){
  ldrValue=analogRead(ldrPin);
  Serial.println(ldrValue);
  if(ldrValue<500){
    digitalWrite(ledPin,HIGH);
  }
  else{
    digitalWrite(ledPin,LOW);
  }
delay(200);
}
#Tinkercad Link
https://www.tinkercad.com/things/hnF4ykfZlR9/editel?returnTo=%2Fdashboard&sharecode=O5QAxmkUArLhoPX5dDmeUIkF0OLrNklHX3hRewu_NY4
#Working
1.The photoresistor detcts whether it is dark or light.
2.If it's dark, LED will glow.
3.Else LED won't glow.
