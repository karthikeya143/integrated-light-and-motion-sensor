int data;
void setup() {
  pinMode(12, OUTPUT);
  pinMode(11, INPUT);
  Serial.begin(9600);
}

void loop() {
  data= digitalRead(11);
  Serial.print(data);
  if (data == 1){
  digitalWrite(12, HIGH);
  delay(1000);}
  else{
  digitalWrite(12, LOW);}
}