# multi-led-Glow-
int inpin1=4;
int outpin1=10;
int inpin2=5;
int outpin2=11;
int inpin3=6;
int outpin3=12;
int inpin4=7;
int outpin4=13;
int val=0;
void setup()
{
  pinMode(10, OUTPUT);
  pinMode(4, INPUT);
  pinMode(11, OUTPUT);
  pinMode(5, INPUT);
  pinMode(12, OUTPUT);
  pinMode(6, INPUT);
  pinMode(13, OUTPUT);
  pinMode(7, INPUT);
}
void loop(){
val=digitalRead(inpin1);
if(val==HIGH)
{
  digitalWrite(outpin1, HIGH);
}
val=digitalRead(inpin2);
if(val==HIGH)
{
  digitalWrite(outpin2, HIGH);
}
val=digitalRead(inpin3);
if(val==HIGH)
{
  digitalWrite(outpin3, HIGH);
}
val=digitalRead(inpin4);
if(val==HIGH)
{
  digitalWrite(outpin4, HIGH);
}
else
{
  digitalWrite(outpin1,LOW);
  digitalWrite(outpin2,LOW);
  digitalWrite(outpin3,LOW);
  digitalWrite(outpin4,LOW);
}
}
