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



https://user-images.githubusercontent.com/93513614/140762624-9f8e820e-07a0-4a50-9e31-8c7d9010bc56.mp4

