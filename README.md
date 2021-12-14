const int ledCount = 4;
const int ledPins[ledCount] = {16,17,22,23};

void setup() {
  for (int i = 0;i<ledCount; i++){
  pinMode(ledPins[i], OUTPUT);
}
}
void loop() {
   for (int i = 0;i < ledCount; i++){
   digitalWrite(ledPins[i],HIGH);
   delay(200);
}
   for (int i = ledCount - 1;i >= 0;i--){
   digitalWrite(ledPins[i],LOW);
   delay(200);
}
}
